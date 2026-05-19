# Contributing

Thanks for helping build tools for uniocular people. This guide covers how
the repository is organized and the principles every contribution follows.

## Repository layout

| Directory          | Holds                                              |
| ------------------ | -------------------------------------------------- |
| `software/`        | Runnable tools (phone, desktop, browser)           |
| `manuals/`         | Plain-language, task-oriented guides               |
| `specifications/`  | Standards and guidelines for builders              |
| `modules/`         | Reusable, embeddable components                    |

See [ROADMAP.md](ROADMAP.md) for direction and [GLOSSARY.md](GLOSSARY.md)
for shared terminology.

## How to contribute

1. Open an issue to propose a utility, claim a roadmap item, or suggest a
   new direction. This avoids duplicated effort.
2. Work on a feature branch and open a pull request.
3. Keep pull requests focused — one utility, guide, or specification at a
   time.
4. New tools and modules go in their own subdirectory with a README that
   states what it does, how to run it, and which roadmap item it serves.

## Principles

Every contribution follows the project's [guiding
principles](ROADMAP.md#guiding-principles):

- **Evidence-based.** Cite optometry/ophthalmology sources. Clearly flag
  advice that is anecdotal or based on lived experience rather than
  research. This project does not provide medical advice and never
  replaces a clinician.
- **Low barrier.** Prefer tools that need no install and work offline.
- **Accessible by construction.** Software must follow the project
  [accessibility guidelines](specifications/accessibility-guidelines.md) —
  never require stereo vision, depth gestures, or 3D-only cues.
- **Respectful language.** Use "uniocular" or "monocular vision". Describe
  people first, not deficits. See the glossary for preferred terms.

## Writing style

- Plain language. Short sentences. Define jargon on first use.
- Markdown for all documentation.
- Manuals are task-oriented: tell the reader what to do, in order.
- Specifications are testable: use MUST / SHOULD / MAY for requirements.
