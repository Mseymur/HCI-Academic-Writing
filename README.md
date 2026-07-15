# HCI-Academic-Writing — a Claude Skill for HCI students who write for examiners

## The story

This skill exists because of red ink.

I built it as a Master's student in Interaction Design, in the middle of a thesis that came back from review with conditional approval and a long list of required revisions. Reading that feedback carefully, a pattern emerged: most of what reviewers attacked was not the research. It was the *writing around* the research — sentences that defended choices nobody had questioned, a contributions list that led with the wrong item, a novelty claim built on "nobody has combined X, Y, and Z," a related-work section that listed papers instead of arguing a gap.

None of this is taught. HCI has a hidden curriculum: which word ("framework," "system," "empirical study") triggers which grading rubric, in what order examiners read a contributions list, what counts as a legitimate gap and what counts as a packaging claim. You usually learn it one painful review at a time.

So I turned the reviewer feedback into rules, verified the rules against the primary literature, and packaged the result as a Claude Skill — so the AI that helps you draft and revise carries the hidden curriculum with it, instead of cheerfully reproducing the mistakes that got me the red ink in the first place.

I made it for myself. It helped. Now it's yours.

## What this skill is — and is not

**It is** a discipline layer for Claude when it writes or revises scholarly text: thesis chapters, PhD and Master's proposals, paper drafts, abstracts, related-work sections, contributions lists, rebuttals — anything an examiner, reviewer, or admissions committee will read.

**It is not** a thesis-writing machine. It will not do your research, invent your argument, or produce a finished document from nothing. Its job is to make the writing you do *with* Claude survive contact with an examiner: catching the failure patterns, correcting the framing, calibrating the claims, and explaining *why* each fix matters so you learn the rules yourself.

## What it actually does

The skill works in two layers:

**Register (sentence level).** It kills defensive writing — the habit of arguing with an imaginary reviewer ("this is a deliberate boundary, not hidden"), re-defending the same limitation five times, or decorating your own choices with rigor-adverbs ("carefully," "transparently"). It enforces plain declarative prose, honest one-time concession of real limitations, and traceability: no empirical claim without a source actually read.

**Framing (claim level).** It checks which contribution noun your work can survive ("framework" invites a demand your single-system study cannot meet), orders your contributions list the way reviewers actually grade it (evidence first, artifact as instrument second, guidelines third), converts novelty-by-combination claims into open research questions, makes your related-work section argue a gap instead of listing papers, and requires importance to be established before novelty is claimed.

On top of that sit two specialized layers:

- **Proposal writing** — the full HCI proposal anatomy, built from the CHI Doctoral Consortium content requirements and European doctoral-school guidance: the operational-goals criterion (a goal you can check the finished work against), the research-question-vs-design-goal distinction, the evaluation plan, and — for structured European doctorates — publication plans and success criteria.
- **Level calibration** — Master's and doctoral work are graded on *different licenses*, not one rubric with a lower passing score. The skill knows what is permitted at Master's level (replication, attributed secondary sources, humbler originality forms) and what only a doctorate requires — so it stops Master's drafts from overclaiming and PhD drafts from underdelivering.

## What to expect from Claude with this skill installed

- It will push back on your framing before it polishes your sentences — and tell you which rule fired and why.
- It will ask (or decide) what level the document is: a Master's chapter and a PhD proposal get different calibration.
- It will grep your draft for a specific list of "tells" ("to be clear," "not hidden," "we do not claim," "X, not Y") and rewrite each into a plain declaration.
- It will refuse to let "nobody has combined..." stand as a novelty claim, and will help you restate it as a question the field has not answered.
- It will not invent citations: the traceability rule treats abstracts and search snippets as leads, not sources.
- When a question falls outside the skill's knowledge, it is instructed to check primary sources or official venue guidance rather than improvise.

## What's inside

```
hci-academic-writing/
├── SKILL.md                              # the rules (register + framing) and a self-check checklist
└── references/
    ├── contribution-types.md             # the 7 HCI contribution types, RtD, Olsen-style systems research, glossary
    ├── novelty-and-positioning.md        # gap statements (Swales' CARS), legitimate vs rejected novelty, related work
    ├── proposal-writing.md               # HCI proposal anatomy: CHI DC structure, evaluation plans, success criteria
    ├── originality-forms.md              # Phillips & Pugh's 15 recognized forms of doctoral originality
    └── level-calibration.md              # Master's vs doctoral criteria (EQF 7/8, Dublin Descriptors, MPhil/PhD licenses)
```

Claude loads the small SKILL.md whenever the skill triggers and reads the reference files only when the task needs them — so the skill stays cheap in normal use and deep when it matters.

## Scholarly basis

The rules are grounded in the literature, not vibes: Wobbrock & Kientz's contribution-types taxonomy (*Interactions*, 2016), Olsen's "Evaluating User Interface Systems Research" (UIST 2007), Zimmerman, Forlizzi & Evenson on Research through Design (CHI 2007), Swales' CARS model of research introductions (*Genre Analysis*, 1990), Phillips & Pugh's *How to Get a PhD*, the CHI Doctoral Consortium content requirements, and the EQF / Dublin Descriptors that govern European degree levels. Where a claim could only be triangulated rather than read from the primary source, the reference files say so explicitly — the skill practices the traceability it preaches.

## How to install

**Claude.ai (web/desktop/mobile):** download the `.skill` file from the Releases page (or package the folder yourself), then go to **Settings → Capabilities → Skills → Upload skill**. Alternatively, send the `.skill` file to Claude in a chat and use the **Save skill** button on the file card.

**Claude Code:** copy the `hci-academic-writing/` folder into `~/.claude/skills/` (personal) or `.claude/skills/` inside your project.

/plugin marketplace add Mseymur/HCI-Academic-Writing
/plugin install hci-academic-writing@hci-academic-writing-marketplace

Then just write: "review my proposal draft," "is this a framework?", "tighten my related work" — the skill triggers on revision requests and framing questions, not only on drafting.

## Who this is for

HCI and interaction-design students first — the contribution taxonomy, the venue conventions, and the examples are HCI-native. The register layer (defensive writing, limitation handling, traceability) applies to academic writing in any empirical field, so students in adjacent disciplines will still get most of the value.

## A caveat, in the skill's own register

This skill encodes one set of validated reviewer feedback plus the primary literature; it does not encode your supervisor, your program's template, or your field's local dialect. Where your institution's guidance conflicts with the skill, the institution wins — the skill itself says so. Scope boundary, stated once.

## License
MIT
