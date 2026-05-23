# Research

The project's knowledge base on functional uniocular vision — what is known,
with citations and links to sources.

## Structure

```
research/
  literature-review.md        # master overview + index (start here)
  deep-research-synthesis.md  # external AI-generated report (provisional)
  topics/<topic>/README.md    # collated learnings per concept; minor cites inline
  sources/<paper>/README.md   # one note per strong paper
```

- **[literature-review.md](literature-review.md)** — the master document:
  scope, cross-cutting takeaways, the topic index, the source index, and the
  consolidated research gaps. **Start here.**
- **[topics/](topics/)** — a collated review per concept (adaptation, depth
  perception, driving, eye protection, etc.). Each cites the relevant source
  notes plus minor references that don't warrant their own note.
- **[sources/](sources/)** — one folder + note per strong paper: full
  citation, scope, key points, learnings, verification status, and the
  topics that cite it.
- **[deep-research-synthesis.md](deep-research-synthesis.md)** — an external
  Gemini Deep Research report, reproduced with a verification table. Treated
  as provisional; only spot-verified findings are folded into the topics.

## Why this is here

The project's [guiding principles](../ROADMAP.md#guiding-principles) require
evidence-based work. This knowledge base is the evidence: before a manual
gives guidance or a utility makes a design choice, it should trace to a
topic doc and, through it, to a source.

## Methodology and limitations

- A **curated** knowledge base, not a systematic review. Findings are
  summarized in good faith from abstracts and open-access text.
- Many primary sources are **paywalled**; notes link open-access mirrors
  where they exist. We do **not** redistribute copyrighted PDFs — we link.
- Each source note carries a **verification status**. "Verified" means the
  citation/figures were checked against the source; "from search digest" or
  "from synthesis" means they are reproduced and still need confirmation.
- Informational only — **not medical advice**.

## Contributing

- New strong paper → add `sources/<slug>/README.md` (use an existing note as
  a template) and cite it from the relevant topic doc.
- New finding for an existing topic → update `topics/<topic>/README.md`; add
  a minor reference inline, or a source note if it's a strong paper.
- Keep the master [literature-review.md](literature-review.md) index in sync.
- See [CONTRIBUTING.md](../CONTRIBUTING.md).
