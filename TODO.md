# TODO / next steps

A running backlog of concrete next actions. Big-picture goals and phases
live in [ROADMAP.md](ROADMAP.md); this is the actionable shortlist. Check
items off or move them into issues as work starts.

## Incoming next session — user-provided PDFs

The maintainer has downloaded PDFs of several research papers to share next
session. Plan for handling them:

- [ ] Read each PDF and use it to **verify provisional figures** currently
      flagged in the source notes and the
      [deep-research synthesis](research/deep-research-synthesis.md).
- [ ] Update the **verification status** line in the relevant
      `research/sources/<paper>/README.md` from "from synthesis" /
      "from search digest" to "verified" once confirmed (or correct the
      figure if it doesn't match).
- [ ] **Do NOT commit the PDFs** to the repo. This violates the project's
      "no copyrighted PDFs" principle (see [CLAUDE.md](CLAUDE.md)) and risks
      copyright infringement. Read them in-session, extract findings, cite
      and link the source — keep PDFs out of version control (a
      `.gitignore` entry can enforce this if they're placed in the working
      tree).

## Research — finish firming up the evidence base

- [ ] Verify still-provisional items: the prevalence table (Lancet GH 2017
      corneal figure; Australian National Eye Health Survey; Andhra Pradesh
      Eye Disease Study), the single-eye accommodation-fatigue claims, and
      the Ferris (1972) / Dorethy parallax-training citations.
- [ ] Add source notes currently cited only inline: GBD blindness 2020,
      the smart-glasses LLM review (PMC11009354), children's protective-
      eyewear compliance (PMC12238169), macular-degeneration parallax
      (PMC12849822).
- [ ] Confirm the Ono & Ujike (2005) journal of record (Perception vs.
      Vision Research) and the Kraut vs. Coday/Warner attribution of the
      n=65 / 91%-untrained survey specifics.
- [ ] Close or downgrade the seven research gaps in
      [research/literature-review.md](research/literature-review.md) as
      evidence is found.

## Then — the standard (after research is solid)

- [ ] Promote the draft Uniocular Compatibility Standard (Levels A/AA/AAA in
      the synthesis doc) into a real `specifications/` document, modelled on
      WCAG (testable criteria + conformance levels + self-certification
      checklist).
- [ ] Fold the existing
      [accessibility-guidelines.md](specifications/accessibility-guidelines.md)
      into / align it with the standard.

## Then — the manuals

- [ ] Write the flagship "How to live with one eye — first 90 days" guide
      (draws on the adaptation, psychological-impact, and prosthetics
      topics).
- [ ] Write the eye-protection guide (highest-impact safety content).

## Housekeeping

- [ ] Add per-pillar candidate deliverables as GitHub issues so contributors
      can claim them.
