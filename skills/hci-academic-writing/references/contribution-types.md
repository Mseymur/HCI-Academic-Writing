# HCI Contribution Types, Genres, and the Taxonomy-Word Glossary

Source basis: Wobbrock, "Seven Research Contributions in HCI" (2012 whitepaper, read in full; published in revised form as Wobbrock & Kientz, *Interactions* 23(3), 2016, pp. 38–44). Olsen, "Evaluating User Interface Systems Research," UIST 2007, pp. 251–258 (read in full). Zimmerman, Forlizzi & Evenson, "Research through Design as a Method for Interaction Design Research in HCI," CHI 2007, pp. 493–502 (verified via abstract and multiple academic sources quoting it with page references; full text paywalled — marked accordingly below).

## The seven contribution types (Wobbrock & Kientz)

For each type: what it is, the shape of its question, its deliverable, how it is judged, and a hallmark sentence.

### 1. Empirical
New findings from systematically gathered data — quantitative, qualitative, or mixed; lab experiments, field studies, interviews, surveys, diary studies, ethnography, logging.
- **Question shape:** answerable without mentioning any particular system. The system, if one exists, is the instrument.
- **Deliverable:** findings about human behavior in relation to technology or information.
- **Judged on:** rigor and precision of method. Confounds and biases must be identified and avoided; if methods are sound and findings important, the contribution is judged favorably. "The devil is in the details."
- **Hallmark sentence:** "This study provides the first controlled evidence of how [population] [behaves/performs] under [condition]."
- **Venue note:** when CHI adopted these types as optional submission keywords in 2016, the empirical type was split in two — empirical studies of *systems* and empirical studies of *people*. "Empirical systems study" (a functional system built as an instrument to answer a question about human behavior) is grounded in that CHI adaptation, not in the original seven. It is the correct default framing when the science is a controlled study and the system merely enables it.

### 2. Artifact
Inventions: new systems, architectures, tools, techniques, or designs. By definition dependent on never-before-seen inventions, instantiated as prototypes, mockups, demos, or envisionments.
- **Question shape:** what does this make possible that was not possible (or was impractical) before?
- **Deliverable:** the invention itself, usually at least partially functional.
- **Judged on:** systems and toolkits holistically, by what they make possible and how; interaction techniques almost always quantitatively, since human performance is central; designs by how compelling and well-informed their vision is.
- **Hallmark sentence:** "Before this, X was impractical; this system makes it possible."
- **Warning (load-bearing):** claiming artifact as the *primary* contribution invites the invention rubric. If the system assembles existing components, the examiner names the prior systems and scores novelty low. Assembly is engineering, not a research contribution.

### 3. Methodological
New or refined methods by which researchers or practitioners work — protocols, metrics, analysis procedures. Entirely new methods are rare; variations are common.
- **Question shape:** how should this be measured or studied?
- **Deliverable:** a method other researchers or practitioners adopt.
- **Judged on:** demonstrated utility, validity, and reliability for the intended purpose, usually via empirical validation (formal comparison or case study). Must be described well enough for others to employ, including warnings of pitfalls. The finding is about how to measure, not about the participants.
- **Hallmark sentence:** "This procedure lets researchers measure X reliably where previously they could not."

### 4. Theoretical
New or improved concepts, definitions, models, principles, or frameworks — qualitative or quantitative — structured to be useful in pursuing future knowledge.
- **Question shape:** why does this relationship hold, and what does it predict?
- **Deliverable:** a reusable thought-vehicle: descriptive (reveals what is) and predictive (foretells what will be), explanatory, and falsifiable.
- **Judged on:** novelty, importance, descriptive power, predictive power. Overfit theories don't generalize; underfit theories explain everything and therefore nothing. Validation is almost always accompanied by empirical work. (The additional criterion "generative for other designers" comes from the intermediate-level-knowledge tradition — Höök & Löwgren's strong concepts — not from Wobbrock & Kientz.)
- **Hallmark sentence:** "This model predicts when [effect] occurs, and explains why."
- This is where the word **"framework"** legitimately lives. Claiming it for a single-system study invites the demand for a validated structure spanning the design space.

### 5. Benchmark / Dataset
A new and useful corpus, usually with an analysis of its characteristics, released for the community; benchmarks come with standard tests enabling cross-project comparison.
- **Question shape:** what shared material does the community lack for testing future innovations?
- **Deliverable:** the released, documented corpus — the community's benchmark, not one's own findings.
- **Judged on:** how much the community needed it; documentation of how it was created, how representative it is, and how to use it. Often paired with tools (overlapping artifact or methodological contributions).
- **Hallmark sentence:** "This corpus enables comparable evaluation of [class of techniques] across projects."

### 6. Survey
A review and synthesis of a matured research area, exposing trends, themes, and gaps.
- **Question shape:** what is currently known about this area, and what does it mean?
- **Deliverable:** a structured synthesis and gap map others cite — explicitly *not* a laundry list of prior work.
- **Judged on:** completeness, depth, organization, maturity, synthesis, and fairness; also on how well it uncovers promising areas for future work.
- **Hallmark sentence:** "Across N studies, three themes emerge, and [context] remains almost unstudied."

### 7. Opinion
Persuasive argument intended to change the field's mind, compel discussion, or force a change of course. Draws on the other contribution types (especially empirical results) as evidence; separate as a type because its goal is persuasion, not information.
- **Judged on:** credibility of supporting evidence, fair treatment of alternative perspectives, strength of the articulated position, breadth of relevance.
- **Never a Master's thesis** (skill guidance, not Wobbrock & Kientz). Olsen's UIST 2007 paper is itself classified by Wobbrock as an opinion contribution.

## Two genres that are ways of working, not taxonomy slots

### Research through Design (RtD) — Zimmerman, Forlizzi & Evenson, CHI 2007
Asks what a preferred future *should* be like; designers produce novel integrations of HCI research "to make the right thing." Suited to under-constrained problems.
- **Deliverable:** the artifact plus its annotated design process and rationale.
- **Judged through four lenses:** **process** (rigor and documentation of the design process so it can be examined and repeated as an approach), **invention** (a novel integration of subject matters, demonstrated against the literature, with articulation of what is new), **relevance** (why the preferred state matters — why anyone should care), **extensibility** (the work is documented so the community can build on it). No effect sizes required; the argument is made through the annotated artifact.
- *Verification status: four lenses confirmed via multiple academic secondary sources citing the paper with page references (e.g., extensibility defined at p. 500); full text not read in this compilation.*

### Olsen-style systems research — Olsen, UIST 2007 (read in full)
Asks whether a new UI system, toolkit, or architecture makes real progress — and argues that simple usability testing is the wrong instrument for judging it.
- **Three evaluation errors to avoid (as author and as self-critic):**
  - **The usability trap:** usability testing assumes walk-up-and-use users, a standardized low-variability task, and a 1–2 hour scale. Toolkit and architecture work violates all three, so demanding a usability score for a systems contribution measures the wrong thing.
  - **The fatal flaw fallacy:** a small team building a new systems approach is guaranteed to omit something; if evaluation focuses on "what does it not do," no research system ever passes. (Turned inward, this is the over-demolished limitations section — see Rule R2.)
  - **The legacy code argument:** "it breaks existing applications" is a barrier to progress, not a valid criticism.
- **Legitimate systems claims, each with its own demonstration:** situate the work in an **STU context** (situations, tasks, users) and establish **importance** first — populations matter by size, criticality, or need, and people change tools only for large improvements; then claim some of: **problem not previously solved**, **generality** (demonstrated through diverse solved examples), **reduced solution viscosity** (flexibility, expressive leverage — accomplishing more by expressing less — and expressive match — the form of expression fits the problem), **empowering new design participants**, **power in combination** (inductive combination of primitives; N-to-1 interconnection like the web's browser/site architecture; ease of combination), and **scale** (show the model survives a realistically large problem).
- Deployment is not among Olsen's criteria; the demonstration is diverse worked solutions and scale, not field release.

## The taxonomy-word glossary (frequently confused)

- **Taxonomy:** sorts existing things into categories. Wobbrock & Kientz's seven types is itself a taxonomy.
- **Design space:** spans dimensions and their values so every possible design is a point in the space. Its power move: empty cells are future papers — and an unoccupied cell is a legitimate novelty claim (see novelty-and-positioning reference).
- **Model:** describes how something works or predicts when something happens, often with variables (e.g., moderators predicting *when* an effect occurs). Falsifiable and usually validated empirically.
- **Theory:** the biggest word; explains *why*. In HCI usually imported from psychology rather than invented in a thesis. Do not use it for a set of observations or guidelines.
- Practical ladder for a thesis: observations → guidelines → model → design space → taxonomy → framework/theory. Claim the lowest rung the evidence fully supports.
