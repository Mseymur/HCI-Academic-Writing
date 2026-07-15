---
name: hci-academic-writing
description: Academic writing discipline for HCI and adjacent fields — covers both sentence-level register AND framing/positioning (contribution vocabulary, novelty claims, gap statements, proposal shaping). Load BEFORE drafting or revising ANY scholarly text an examiner, reviewer, or admissions committee will read — thesis chapters, PhD proposals, paper drafts, abstracts, related-work sections, methods sections, contributions lists, rebuttals, gap statements, expressions of interest to professors. Fires on revision requests as much as drafting ("tighten this section", "make this sound academic", "review my proposal", "fix my contributions list"), and on framing questions ("is this a framework?", "how do I claim novelty?", "what's my contribution?"). Supersedes and replaces the academic-writing-style skill.
---

# HCI Academic Writing

Two layers. **Register** governs the sentence: plainly declarative, confident without protesting its own rigor. **Framing** governs the claim: which contribution noun, in what order, with what novelty argument. Reviewers attack framing errors first and register errors second; both hand them the weapon.

Apply while writing, not as a cleanup pass. Reference files (read when the task touches them):

- `references/contribution-types.md` — the seven HCI contribution types, the RtD and systems-research genres, and the taxonomy / design-space / model / theory glossary. Read when choosing or checking a contribution noun, writing a contributions list, or classifying what a piece of work *is*.
- `references/novelty-and-positioning.md` — how gap statements are built (Swales' CARS moves), what counts as a legitimate novelty claim, and related-work positioning. Read when writing an introduction, related work, or a novelty argument.
- `references/proposal-writing.md` — the full HCI proposal anatomy: grading rubric, CHI Doctoral Consortium section structure, the operational-goals criterion, the evaluation plan, publication plan and success criteria for structured European doctorates, length norms. Read whenever the document is a proposal of any kind — PhD admission, proficiency evaluation, doctoral consortium, funding.
- `references/level-calibration.md` — how Master's-level criteria and judging differ from doctoral (EQF 7 vs 8, Dublin Descriptors, the MPhil/PhD licenses), and Master's proposal norms. Read whenever the document is Master's-level work, or when calibrating how strong a claim or how ambitious an originality form the degree level requires.
- `references/originality-forms.md` — Phillips & Pugh's fifteen recognized forms of originality. Read when the writer doubts their work is "original enough" or needs to name which kind of originality a contribution has.

---

## Layer 1 — Register

### Rule R1 — Do not argue with an invisible reviewer (the load-bearing rule)

The failure mode: a sentence does not just *state* a choice, it *defends the choice against an objection nobody has raised yet*. The writing imagines a skeptic and rebuts in advance.

**Tells** (grep the draft for these — each is usually a defense in disguise):
- "stated as a deliberate boundary, **not hidden**"
- "this is **deliberately not** a packaging claim"
- "reported as the finding, **not spun as** X"
- "a **deliberate** choice", "in two **honest** ways", "**deliberately** between the poles"
- "to be clear", "admittedly", "it should be noted that", "we do not claim"
- any clause of the shape *"X, not Y"* where Y is an accusation no one made

**Why it fails:** protesting "this isn't hidden" makes the reader hunt for what is hidden. Defending an ordinary choice signals the author expects attack, which invites the attack. The defense is addressed to a reviewer while the reader is trying to understand the work — the arguing-back is noise between them and the science.

**The fix — state the property, drop the defense.** Same content, no fight.
- BEFORE: "This scope is stated as a deliberate boundary, not hidden."
- AFTER: "The study is scoped to task performance with novice users in a laboratory setting; longitudinal adoption is out of scope."
- BEFORE: "The mixed result is reported as the finding, not spun as superiority of the new technique."
- AFTER: "The comparison is dimensional: the finding is which measures favor the new technique and which favor the baseline."

### Rule R2 — Concede real limitations plainly; do not defend ordinary choices at all

The line R1 must not cross: owning a genuine limitation is good practice and stays. The skill is telling the two apart.
- KEEP (real limitation, stated once, plainly): "The evaluation uses a simulated environment, not a live deployment; ecological validity is future work."
- CUT (defending a normal choice against an unraised objection): "We deliberately and transparently chose a simulated environment, which is not a weakness but a considered trade-off..."
- Concede once. Do not re-defend the same limitation every time it is adjacent to a claim. Exhaustively demolishing one's own work in the limitations section is the fatal-flaw fallacy turned inward (see Olsen in the contribution-types reference): every research system has omissions by construction; state the boundary, not an inventory of everything the work is not.

### Rule R3 — Register and word choice

- Plain declarative sentences, one idea each, connected in sequence. Methods-section register, not chat.
- No editorializing adverbs about one's own rigor: *deliberately, carefully, honestly, transparently, rigorously* applied to one's own choices are almost always deletable.
- No field cliché or value-judgment shorthand (workhorse, vanilla, unsexy, quick-and-dirty). Name the concrete property instead (more established, higher-resolution, faster but less accurate).
- No emoji, no decorative headers in the prose itself.
- Hedge only where the evidence is genuinely uncertain; do not hedge as a reflex. Conversely, do not overclaim where the evidence is one study.

### Rule R4 — Every empirical claim is traceable

Each empirical statement traces to a source (corpus paper, primary data, or a flagged out-of-corpus reference). Do not attribute a claim, a quote, or a finding to a paper whose full text has not been read — a search snippet or abstract is a lead, not a source. Flag out-of-corpus citations explicitly. If a claim cannot be sourced, delete it rather than soften it.

---

## Layer 2 — Framing

### Rule F1 — Pick the contribution noun before writing, and pick it by rubric, not by flattery

Each contribution noun hands the examiner a grading rubric. Using the wrong noun means being graded against the wrong standard:
- **"Framework"** invites the demand for a validated conceptual structure covering a design space — a theoretical contribution judged on descriptive and predictive power. A single-system study cannot survive that rubric.
- **"System" / "artifact" as the primary claim** invites the invention rubric: the examiner names the prior systems holding each component and scores novelty low, because assembling existing parts is engineering, not a research contribution.
- **"Empirical study"** (with the system as instrument) invites the rigor rubric: methods, confounds, analysis. This is the correct default when the science is a controlled study and the system exists to enable it.

**Decision cue:** if the research question can be stated without mentioning the system, the contribution is empirical and the system is the instrument. (Heuristic derived from Wobbrock & Kientz's typology, not stated in it.) When unsure which noun fits, read `references/contribution-types.md` before committing.

### Rule F2 — Order contributions by what the work actually proves

Reviewers grade top-down from item #1 of a contributions list; the first item sets the rubric for the whole work. For empirical work: (1) the empirical evidence from the study, (2) the designed artifact as the instrument that enabled it, (3) transferable design guidelines derived from the data. Putting the artifact first causes the work to be graded on invention — and to fail on it.

### Rule F3 — Novelty is a question, never a combination

"Nobody has combined X + Y + Z" is a packaging claim; examiners treat it as an automatic fail — combining existing parts is engineering, not science. Frame the contribution as an **open empirical question the field has not answered**, and concede occupied territory openly by naming the prior systems that hold each component. The question, not the component count, is what makes the work new. Legitimate shapes for a novelty claim: an unanswered question, an unmeasured comparison, an unoccupied cell in a design space, an established finding tested in an untested population or context. For the full anatomy of a defensible gap statement, read `references/novelty-and-positioning.md`; for the range of things that legitimately count as original, read `references/originality-forms.md`.

### Rule F4 — Framing-level defensive patterns (R1's big siblings)

- **Arguing with ghosts:** explaining to the examiner why a criticism would be wrong before anyone made it. Delete; state the actual scope in one declarative sentence.
- **Over-justifying standard methodology:** citing seven prior papers' sample sizes to justify one's own N reads as begging for permission. State the design requirement and the power analysis; let the math speak. One sentence of precedent is context; a paragraph is a plea.
- **Courtroom limitations:** "this is a concession, not a mitigation" and similar legal framing. State the boundary neutrally: "Scope boundary: the hardware form factor prevents in-the-wild social-acceptability testing; evaluation is scoped to interaction mechanics."

### Rule F5 — A thesis argues one position

A thesis (document) must contain a thesis (position): one storyline, a coherent argument every chapter advances. Relevance to that argument is the pruning criterion — data or sections that do not push the storyline are cut, however costly they were to produce. If a chapter cannot say what the argument gains from it, it does not belong. (Phillips & Pugh: "not having a thesis" is one of the canonical ways of failing a PhD.)

### Rule F6 — Related work positions; it never lists

A related-work section is an argument that a specific gap exists, not an inventory. Organize by theme around the research question, not by paper. Each subsection closes on what the reviewed work leaves unanswered — that sentence is a load-bearing joint in the gap argument. A section an examiner can read as "here are papers I found" fails even if every summary is accurate. Concede occupied territory inside related work (per F3): naming the closest prior systems and stating precisely what they did and did not answer is what makes the remaining gap credible.

### Rule F7 — Establish importance before novelty

A gap can be real and not worth filling. Before any novelty claim, establish the context — which users, which tasks, which situations — and why that context matters (Olsen's importance criterion). An examiner persuaded of importance forgives an incremental contribution; an examiner unpersuaded of importance rejects even a genuine first.

### Rule F8 — A proposal is graded prospectively; a thesis retrospectively

A thesis defends delivered contributions; a proposal argues that a question deserves years of work and that this candidate at this institution can answer it. The rubric shifts to: originality of the question, feasibility within the funded period, methodological awareness, coherence, and fit with the supervisor's expertise. Consequences for the prose: contributions are stated as expected outcomes, specific rather than grandiose; the timeline and required resources are part of the argument, not paperwork; scope boundaries demonstrate feasibility rather than apologize; and the proposal is a rigorous starting point, not a contract — but it must read as viable exactly as written. A proposal is not a begging letter: the register is that of a researcher bringing the department a question worth its resources. Two proposal-specific tests worth applying to every draft: research questions are questions about what will be *known*, never design goals in disguise; and every goal is *operational* — the finished work must be checkable against the goal statement. Full section-by-section guidance, including the evaluation plan, publication plan, and success criteria, is in `references/proposal-writing.md` — read it for any proposal of any kind.

---

## Self-check before saving prose

1. Grep for R1 tells (`not hidden`, `deliberate`, `not spun`, `not a ... claim`, `to be clear`, `X, not Y`). Each hit: defending against an unraised objection? Rewrite to plain declaration.
2. Every limitation conceded exactly once, plainly (R2). No fatal-flaw inventory.
3. No rigor-adverbs about one's own choices; no cliché; hedges only where evidence is uncertain (R3).
4. Every empirical claim has a real, read source (R4).
5. Contribution noun matches the rubric the work can survive; contributions list ordered evidence → instrument → guidelines (F1, F2).
6. No novelty-by-combination sentence anywhere; occupied territory named (F3).
7. No ghost-arguments, no methodology pleading, no courtroom limitations (F4).
8. One storyline; every section earns its place in it (F5).
9. Each related-work subsection ends on an open question (F6).
10. Importance established before novelty claimed (F7).
11. If a proposal: prospective framing, feasibility argued, fit stated (F8).
12. Claim strength and originality form calibrated to the degree level — Master's work graded on the demonstrated process, doctoral on the contribution (see `references/level-calibration.md`).

## Fallback rule

If a framing or vocabulary question arises that this skill and its reference files do not settle, check primary sources or official venue/university guidance on the web before answering. Do not improvise contribution-type definitions from memory.
