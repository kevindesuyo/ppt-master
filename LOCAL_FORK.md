# ローカル fork の運用

このチェックアウトは、上流 `hugohe3/ppt-master` に少数のローカル変更を載せた疑似 fork です。ppt-master スキルの実体はここだけに置き、各エージェントからは symlink で参照します。

## ブランチ

| ブランチ | 中身 | 追跡先 |
|---|---|---|
| `main` | 上流そのまま。fast-forward だけで更新し、上流への PR の起点にする | `origin/main` |
| `local` | `main` + ローカル変更。普段チェックアウトしておくのはこちら | `origin/main` |

`local` は公開 fork（`kevindesuyo/ppt-master`）の `main` に push します。fork の `main` は上流のミラーではないので、上流への PR ブランチは `origin/main` から切ります。公開リポジトリなので、会社名・案件名・会社の素材はコミットにもメッセージにも入れません。

## ローカル変更

- `mbb-consulting` スタイル：社用プロファイルで作ったコンサル資料の作法のうち、会社固有でない部分を移植（2026-09-14 作成、会社の色・フォント・ロゴ・素材は含めない）

ローカル変更は 1 つの目的ごとに 1 コミットにまとめ、`git log origin/main..local` で一覧できる状態を保ちます。

## 参照元

- `~/.agents/skills/ppt-master` → `../../Documents/workfolder/ppt-master/skills/ppt-master`（Codex など）
- `~/.claude/skills/ppt-master` → `../../.agents/skills/ppt-master`（Claude Code）
- `workfolder/skills/.agents/skills/ppt-master`：skills リポジトリ単体で取得できるようにするための複製。更新後に下記の手順で同期する

## 上流の取り込み

```sh
git fetch origin
git switch main && git merge --ff-only origin/main
git switch local && git rebase origin/main
uv run --no-project --with 'tiktoken>=0.7.0' python skills/ppt-master/scripts/prompt_audit.py
git push --force-with-lease fork local:main
```

rebase でコミットが作り直されるため、fork への push は毎回 `--force-with-lease` になります。rebase で `mbb-consulting` が競合したら、上流の変更を取り込んだうえでローカルの作法を残します。`prompt_audit.py` が重複許可エントリの不整合を報告したら、`scripts/prompt_audit_manifest.json` の該当エントリを直します。

## skills リポジトリへの同期

```sh
rsync -a --delete --exclude .DS_Store --exclude __pycache__ --exclude .pytest_cache \
  skills/ppt-master/ ../skills/.agents/skills/ppt-master/
```

同期後、skills リポジトリの README にある収録元コミットを `git rev-parse --short local` の値に更新して commit・push します。
