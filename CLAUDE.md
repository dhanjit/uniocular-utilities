# CLAUDE.md

Guidance for working in this repository.

## What this project is

**uniocular-utilities** is a collection of software, manuals,
specifications, and guidelines that help **uniocular** (monocular) people —
those who see with only one eye, or have very limited vision in one eye.

Goals and the phased plan live in **[ROADMAP.md](ROADMAP.md)**. Contribution
process and principles live in **[CONTRIBUTING.md](CONTRIBUTING.md)**. Shared
terminology lives in **[GLOSSARY.md](GLOSSARY.md)**. Don't duplicate those
here — link to them.

## Directory structure

```
.
├── README.md            Human entry point: what's here + start-here links
├── ROADMAP.md           Goals, four pillars, phased plan, future directions
├── CONTRIBUTING.md      Repo layout, how to contribute, principles
├── GLOSSARY.md          Shared terminology (uniocular, stereopsis, etc.)
├── CLAUDE.md            This file
│
├── software/            Pillar 1 — runnable tools (phone, desktop, browser)
├── manuals/             Pillar 2 — task-oriented guides ("How to live with one eye")
├── specifications/      Pillar 3 — standards for builders
│   └── accessibility-guidelines.md   Draft; seed of the Uniocular Compatibility Standard
├── modules/             Pillar 4 — reusable, embeddable components
│
└── research/            Evidence base (knowledge base)
    ├── README.md                 Structure + methodology
    ├── literature-review.md      MASTER index — start here
    ├── deep-research-synthesis.md  External AI report (provisional, verification-tabled)
    ├── sources/<paper>/README.md   One note per strong paper
    └── topics/<topic>/README.md    One collated review per concept
```

Each pillar directory (`software/`, `manuals/`, `specifications/`,
`modules/`) has a `README.md` describing its purpose and candidate
deliverables.

## Research knowledge base conventions

- **Strong papers** get their own folder + note under `research/sources/`
  (citation, scope, key points, learnings, **verification status**, and the
  topics that cite them).
- **Concepts** get a collated review under `research/topics/` that cites the
  source notes plus minor references (web overviews, vendor pages) inline —
  minor references do **not** get their own folder.
- `research/literature-review.md` is the **master index**; keep its topic and
  source indexes in sync when adding material.
- Every source note carries a **verification status**: "verified" (checked
  against the source), "from search digest", or "from synthesis" (reproduced,
  still to confirm). Don't silently promote unverified figures.

## Working principles (enforced)

- **Evidence-based.** Claims trace to `research/` and from there to a primary
  source. Flag anecdotal advice. This project is **not medical advice**.
- **Scope.** Uniocular users typically retain normal acuity — they are
  distinct from low-vision/blind users. Don't import magnification/narration
  assumptions; focus on depth, blind side, fatigue, and eye protection.
- **No copyrighted PDFs** in the repo — cite and link (open-access mirrors
  where available).
- **Respectful, person-first language.** "Uniocular / monocular vision."
- **Markdown** for all docs. Plain language; specifications use MUST/SHOULD/MAY.

## Current sequencing

Per project direction: **research first, then the standard, then the
manuals.** The research knowledge base is the current focus; the Uniocular
Compatibility Standard and the "How to live with one eye" manual series come
after the evidence base is solid. See ROADMAP for the full plan.

## Git workflow

Active development branch: `claude/uniocular-utilities-uwvg9`. Open pull
requests as drafts against `main`.
