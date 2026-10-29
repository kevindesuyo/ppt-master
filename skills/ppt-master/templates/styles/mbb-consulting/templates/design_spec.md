---
style_id: mbb-consulting
kind: style
summary: Strategy-document method in the MBB consulting convention — answer-first reasoning, on-page proof, argument-led composition, readable document density, and verifiable editability.
keywords: [consulting, strategy-document, MBB-style, document-density, exhibits]
---

# MBB Consulting — Style Specification

> Method and design defaults only. No project communication contract, brand identity, page structure, or SVG prototypes.

## I. Style Overview

| Property | Value |
|---|---|
| Style Name | MBB Consulting |
| Best Fit | Strategy documents read at desk distance in the top-tier strategy-consulting convention: market and portfolio diagnoses, priority recommendations, board and management decision papers |
| Reusable Intent | Make each substantive page deliver a decision-relevant answer with visible, traceable proof at readable document density; choose exhibits and composition from the argument while leaving identity and the current communication contract open to the project |
| Sources | Method inherited from `consulting-decision` ([GitHub Issue #241](https://github.com/hugohe3/ppt-master/issues/241)); document-density conventions from the EV market-priority deck (example `ppt169_ev_market_priorities`, 2026-09-05). Local fork change (2026-09-14): generalizes the user-authored consulting craft from a company profile kept outside this repository — reasoning, composition selection, capacity, editable evidence, and acceptance. Company identity, assets, fixed values, native-source routing, and automatic review activation are excluded; this specification is self-contained. |

## II. Communication Method

- **Preferred Mode**: pyramid
- **Argument Flow**: Establish audience, decision, requested action, and scope before outlining. Define the overall answer, its key supporting arguments, the evidence required for each, and unresolved assumptions or evidence gaps. Maintain the trace `overall answer → key support → page message → evidence`; combine layers in a short deck while retaining that connection. Remove duplicate or decision-irrelevant pages, then rehearse the explanation end to end and repair missing links in the plan.
- **Page Message Discipline**: Give each substantive page one primary role and the chain `governing question → answer → on-page proof → audience move`. State the answer in an assertion title or equally dominant message; the proof must establish that actual answer, not merely describe a related topic. Explain what the evidence means. A citation or a reference to unseen evidence on another page cannot replace visible proof. Cover and navigation pages establish context or sequence; substantive claims on them still need support.
- **Claim Discipline**: Keep facts, assumptions, implications, and recommendations semantically distinct. Cite facts, name uncertainty in assumptions, derive implications from visible evidence, and pair recommendations with their rationale and action. Keep recommendation and implication wording consistent across the deck; never promote an unsupported claim to a conclusion.
- **Reference Hygiene**: Borrow a reference's composition only after identifying the feature that serves the current argument. Example companies, figures, claims, speaker notes, and embedded workbook data are not evidence for the current deck.

## III. Page Role Vocabulary

| Role | Communication Job | Evidence Obligation | Composition Tendency |
|---|---|---|---|
| Executive synthesis | State the governing decision and overall answer | Show the strongest supports, their evidence paths, and any material gap | One dominant answer with a small set of aligned keyword-and-explanation blocks or numbered findings; add basis numbers or a decision-ask column when they support the answer |
| Recommendation | Specify the action and why it is preferable | Connect the action to diagnosis, expected effect, dependencies, and trade-offs | Pair each action label with its rationale or concrete change; use a priority table when explicit criteria distinguish tiers |
| Situation / complication / resolution | Establish context, surface the tension, and resolve the governing question | Distinguish observed conditions from the interpretation that creates the tension | Let the contrast between current reality and the answer carry the page |
| Driver decomposition | Explain what determines an outcome or decision | Use distinct supported branches; preserve real overlap or acknowledged gaps | Make the governing relationship primary and branches easy to compare |
| Current-state diagnosis | Identify the condition that matters and its causes | Separate observation from interpretation and tie each diagnosis to evidence | Related exhibits with aligned comparisons and a nearby implication; add a compact table or KPI strip only when it supplies further proof |
| Comparison / benchmark | Clarify a decision through alternatives, peers, periods, or standards | State basis, units, period, and comparability; never invent a benchmark | Align comparable evidence and emphasize only decision-relevant differences |
| Process / operating model | Explain how work, ownership, or decisions flow | Show actors, handoffs, dependencies, controls, and failure points that the source supports | Prioritize causal or operational flow over decorative process art |
| Roadmap | Translate the recommendation into sequenced action | Connect phases to outcomes, dependencies, milestones, and decision gates | Distinct time and workstream lanes with owners, milestones, and dependency links; use stage chevrons only for real sequence |
| Risk / mitigation | Expose uncertainty and the response it requires | Pair each risk with likelihood or trigger evidence, impact, mitigation, and owner when known | A risk register aligns triggers, impact, response, and monitoring data; status color maps to a stated condition and next response |
| Decision request | Ask for the decisions and name what happens without them | Show each ask with its rationale, action, owner, due date, immediate dependency, and consequence of not deciding; label unknown owners and dates unresolved | Aligned ask, action, owner, timing, and consequence fields; numbering expresses real priority or sequence |
| Open discussion | Frame a decision still open | Show options, evaluation criteria, trade-offs, and the judgment requested | Comparable alternatives with the unresolved choice visibly distinguished from established findings |
| Appendix / evidence | Preserve detail needed to audit or deepen the argument | Retain source, period, method, definitions, and limitations | Full data tables as numbered exhibits, a calculation-method block, and a source-and-licence block with links |

**Composition Selection**

Choose one dominant pattern from the question and proof; the role examples above are starting points, not a roster or fixed arrangement. A supporting inset belongs on the same reading path.

| When the argument depends on | Pattern and realization test |
|---|---|
| One answer supported by several reasons | Answer above supports; aligned keywords and concise explanations; numbers only for real priority or sequence |
| Issues and responses, alternatives, or change | Match each issue to its response; align identical criteria, units, periods, and scope across comparisons |
| Two dimensions of classification or priority | Matrix with both axes labeled and a stated basis for each placement; color alone is not a criterion |
| Components, ownership, or handoffs | System map or process flow in which every connection encodes a supported relationship; distinguish sequence from ownership |
| Decomposition or layered support | Logic tree with a stated split rule, or pyramid for genuine hierarchy; disclose real overlap or gaps rather than forcing exhaustive, disjoint branches |
| Change across phases | Roadmap separating time, workstreams, ownership, milestones, and dependencies |
| Quantitative change | Chart with a nearby conclusion and direct annotation of the decisive delta |
| A compact model of the whole answer | One-page synthesis with one organizing frame and reading path; move audit detail to the appendix before sacrificing readability |

## IV. Evidence & Data Expression

- **Argument Trace**: Every page message must trace back to one key support for the overall answer and forward to visible proof. Keep missing evidence or unresolved assumptions explicit instead of concealing the gap with confident wording.
- **Charts**: Choose the chart from the decision question and comparison logic. Identify exhibits consistently (A, B, C), with a descriptive title and unit line. Prefer direct labels for decisive values, deltas, and multiples; retain axes, scales, uncertainty, and reference lines needed to interpret quantities, and remove only non-evidentiary furniture. Keep labels readable rather than labeling every point in a dense series. Annotate the decision-relevant change in the accent colour and footnote calculations. Use a consistent time direction; never reverse, truncate, or change a quantitative scale merely to imply improvement. Separate observation from interpretation and never invent a baseline, peer, target, or trend.
- **Tables**: Derive columns and row groups from the comparison or decision logic. Align criteria, units, periods, and scope, preserve hierarchy, distinguish facts from assumptions, and emphasize only differences that affect the answer. Add tier, judgment, or evidence-page columns when the decision requires them. Meaningful headers, status cells, and structural regions may use fill; declare each status or risk color's meaning and required response.
- **Sources**: Number footnotes at the bottom-left of every page with the source line beneath them, and reference footnote numbers from titles, unit lines, and labels. Retain source, period, scope, and measurement basis; label estimates, proxies, scenario values, and computed values as such. Do not present unattributed or unsupported statements as facts.
- **Native Editability**: Prefer native charts for supported quantitative evidence and editable tables and business shapes. Identify required editing behavior before authoring and use the selected route's supported representation. Editable bars are not a native PowerPoint chart; typed bullet glyphs are not paragraph bullets; a visible line is not a connector that follows moved endpoints. When the required behavior is unsupported, disclose that limitation before choosing a fallback; appearance alone does not establish compliance.
- **Notation**: Set numeral width, punctuation, dates, units, and terminology consistently across the deck; preserve the same measurement and calculation basis across related exhibits.

## V. Visual System Defaults

- **Preferred Visual Style**: custom
- **Visual Style References**: swiss-minimal
- **Visual Style Behavior**: Analytical document pages with an assertion title, a clear exhibit hierarchy, nearby implications, and traceable footnotes. Use consistent section cues and page numbering; add a draft marker only when applicable. A key-message column, exhibit badges, or a dark cover may serve the argument but are not compulsory. Let emphasis and alignment establish hierarchy; prefer unboxed conclusions and a clean title area over decorative underlines or filled conclusion callouts.
- **Composition**: Organize the page around a small number of primary evidence regions and one dominant pattern from section III. A table, matrix, or system map may contain many internal cells while remaining one organizing region. Add exhibits, comparisons, or summary strips when each supplies distinct proof. Keep semantic peers equal in size and treatment unless a supported data comparison encodes the difference. Align frames and spacing geometrically; preserve whitespace around the answer and decisive evidence rather than filling a module quota.
- **Density**: Preserve document-level analytical depth while varying density with the page role. At the intended reading size, the answer, proof, labels, and sources must remain legible. Resolve overload by shortening copy, deferring audit detail, splitting the argument, or choosing a better-fitting composition before reducing type. Keep bullets to a few rendered lines by default. Use stable role sizes, readable paragraph spacing, and aligned numerals; do not enlarge a small chart solely to occupy unused width.
- **Decoration**: Use restrained rules where they separate meaningful rows or regions, and fill where it encodes grouping, comparison, or status. Emphasize the decisive phrase or value through weight or focus color. Decorative treatments should not compete with the answer or its proof.
- **Color Behavior**: One deep dominant carries titles, badges, primary series, and axes; one saturated accent marks the point of each exhibit (the emphasized bar, the priority tier, the highlighted figure, the implication bar); a light tint of the accent carries the secondary series; a grey ramp carries context, category labels, unit lines, and footnotes; one negative colour is reserved for declines and risk triggers. Tints of one family order series; never rainbow-code. Any confirmed Brand or Deck identity replaces these tendencies; never imply a consultancy-specific or trademarked palette.
- **Typography Character**: One compact sans-serif family for all editable text, with a lining-figure companion for numerals in charts, tables, KPI strips, and badges. Hierarchy comes from weight, size steps, letter-spaced small labels for trackers and column headers, and alignment — never from containers. Exact families and locale coverage remain current-project or resolved identity decisions.
- **Typography and Alignment**: Resolve language coverage for body text, Latin runs, numbers, units, chart labels, table cells, and sources. Assess physical point sizes using the actual slide-to-canvas scale; a point value is not a canvas pixel value. Distinguish declared fonts from fonts available to the renderer. Use text frames, paragraph indentation, and paragraph spacing for alignment rather than repeated spaces or forced line breaks; keep connected labels and their shapes editable together where supported.

### Fallback Color Scheme

| Role | HEX | Purpose |
|---|---|---|
| Field | #FFFFFF | Page field on every page except the cover |
| Dominant | #051C2C | Titles, badges, primary series, axes, and the cover field |
| Accent | #2251FF | The point of each exhibit: emphasized bar, priority tier, highlighted figure, implication bar |
| Accent tint | #8FB8FF | Secondary series and secondary text on the cover |
| Body | #333333 | Body copy, key messages, and table text |
| Muted | #7F7F7F | Category labels, unit lines, trackers, and footnotes |
| Hairline | #B7B7B7 | Axes and dividers |
| Grid | #E3E3E3 | Table row separators and dashed connectors |
| Surface | #F7F7F7 | Meaningful table headers, status cells, and grouped lanes |
| Negative | #B3261E | Declines, negative deltas, and risk triggers |

### Fallback Typography

| Role | Primary | Fallback Tail | Character |
|---|---|---|---|
| Titles and body | Microsoft YaHei | Arial | Compact neutral sans; bold for action titles, exhibit titles, and badges |
| Numerals and data | Arial | Helvetica | Lining figures for chart labels, tables, KPI strips, page numbers |

## VI. Image & Icon Direction

- **Preferred Image Rendering**: minimalist-swiss
- **Image Usage**: Use images only when they provide evidence, necessary context, or a causal explanation that shapes the decision. Default to sparse imagery; keep data and business structures editable instead of replacing them with decorative illustrations.
- **Image Treatment**: Crop for the evidentiary subject, use restrained framing or a functional scrim, and retain a nearby caption or source when the image supports a claim. Avoid gratuitous full bleed, synthetic text inside images, and atmospheric imagery that weakens the argument.
- **Icon Treatment**: Use one coherent icon family with consistent stroke or fill treatment, only when an icon clarifies a role, state, or relationship. Avoid logos, consultancy-specific marks, decorative icon grids, and mixed visual languages; actual icon selection remains a project decision.

## VII. Review Focus
<!-- visual-review-trigger: explicit-user-only -->
> Apply this section only after the user explicitly activates visual review. It never triggers that stage.

- The intended answer is identifiable quickly at the rendered slide size.
- The governing question is actually answered rather than repeated as a topic.
- Visible evidence supports the message and is spatially connected to it.
- Facts, assumptions, implications, and recommendations remain distinguishable and semantically consistent.
- Direct labels, sources, hierarchy, and annotations remain legible at the rendered slide size.
- The dominant pattern passes its section III realization test; each exhibit adds distinct proof, and hierarchy or connectors express real relationships rather than decoration.
- Dense pages retain one clear scan path and do not hide overflow or structural ambiguity.
- No unsupported claim is presented as established evidence; unresolved gaps remain visible.
- Summary supports connect to the detailed argument; execution asks include known owners, timing, and dependencies, with unknown commitments marked unresolved.
- Comparable evidence retains consistent criteria, units, periods, scales, and notation; status colors have stated meanings and responses.
- Inspect every final PPTX page with a PowerPoint-compatible renderer when assessing delivery quality, not only intermediate SVGs. Record renderer and actual font availability, and distinguish technical validity from visual approval.
- Verify promised editing behavior in the exported file: native chart parts and workbook values, paragraph bullet/indent properties, shape text, and connector bindings where required. Check that slide text, notes, caches, and embedded workbooks contain current approved content rather than reference examples.
- Record page-level findings, evidence, reviewer, and verdict as pass, fail, or not-verified. Missing rendering or fonts remains not-verified; when independent review is required, name the reviewer and do not relabel self-review as independent approval. Do not claim checks that were not performed.
- Repair missing proof in the plan and visual realization faults in the affected page through the selected route; re-export and recheck changed pages and any shared-style effects. These checks refine an explicitly requested review without creating a new route or confirmation gate.
