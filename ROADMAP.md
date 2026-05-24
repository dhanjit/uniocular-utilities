# Project Roadmap

A planning document for **uniocular-utilities** — a collection of software,
manuals, specifications, and guidelines that help people who see with only
one eye (or have very limited vision in one eye).

## Who this is for

"Uniocular" (also called monocular) vision means relying on a single eye.
Causes include enucleation, amblyopia, injury, retinal disease, or being
born with sight in one eye only. The lived challenges this project aims to
address include:

- **Depth perception** — no stereopsis, so judging distance relies on
  monocular cues (motion parallax, relative size, occlusion, shadow).
- **Reduced field of view** — a blind side that hides obstacles, people,
  and hazards.
- **Eye strain and fatigue** — the working eye does all the work.
- **Daily tasks** — pouring, threading, parking, catching, stairs, doorways.
- **Protecting the remaining eye** — the one working eye is irreplaceable.
- **Emotional adjustment** — vision loss carries a real psychological toll.
- **Software that assumes two eyes** — 3D/stereo UIs, depth-based gestures.

## Project pillars

The repository is organized around four kinds of deliverables.

### 1. Software utilities (`/software`)

Practical tools, runnable on common devices (phone, desktop, browser).

- **Blind-side assist** — use a phone or webcam to surface what is on the
  non-seeing side, with audible/haptic alerts for approaching objects.
- **Distance estimator** — AR/camera tool that estimates distance to a
  target using monocular cues and known reference sizes.
- **Depth-cue trainer** — exercises and games that strengthen the use of
  monocular depth cues (parallax, motion, size gradients).
- **Stereo-to-mono converter** — strips 3D/stereoscopic content (images,
  video, VR) into a comfortable single-eye view.
- **Eye-strain manager** — break reminders, contrast/zoom presets, and
  reading-pace tools tuned for a single working eye.

### 2. Manuals and guides (`/manuals`)

Plain-language, task-oriented documentation.

The flagship is **"How to live with one eye"** — an umbrella series that
starts with the newly-monocular reader and branches into every part of
life. Planned chapters:

- **First 90 days** — adaptation timeline, what to expect, emotional
  adjustment, and when to seek help.
- **Protecting your remaining eye** — polycarbonate eyewear, when to wear
  it, sport/activity protection. (High priority; see research §7.)
- **Daily tasks** — pouring, cooking, stairs, crowds, doorways, threading.
- **Driving** — mirror setup, scanning habits, the Pulfrich caveat,
  regional legality notes.
- **Screens and computing** — monitor setup, eye-strain management, the
  20-20-20 rule.
- **Sports and hobbies** — catching, cycling, swimming, protective gear.
- **Work and school** — workspace setup, requesting adjustments,
  accommodations for children.
- **Smart glasses and AI** — how current AI wearables (and near-future
  ones) can help with depth, distance, and the blind side, and their
  limits for uniocular users specifically.

### 3. Specifications and guidelines (`/specifications`)

Standards for builders so their products work for uniocular users.

The headline goal is a **Uniocular Compatibility Standard (UCS)** — a
concise, testable, *certifiable* standard. If a product (software or
hardware) meets it, anyone can be confident it works for uniocular people,
and the maker can display a "uniocular-compatible" mark. Planned shape:

- **Conformance levels** (e.g. A / AA) and **testable success criteria**,
  modelled on WCAG's structure rather than a long advisory document
  (research §14 notes that long guidelines see poor adoption).
- **Self-certification checklist** a builder can run against a product.
- **Scope across software, content, and hardware** — covering stereo/3D
  fallbacks, depth-input alternatives, blind-side/field considerations,
  contrast/text, and multi-channel feedback.
- The existing **[accessible UI guidelines](../specifications/accessibility-guidelines.md)**
  are the seed; UCS formalizes them into a certifiable standard.

Supporting specifications:

- **Content guidelines** — caption depth, avoid autostereoscopic-only media.
- **Hardware notes** — recommendations for cameras, mounts, and wearables.

### 4. Helping modules (`/modules`)

Reusable, embeddable components other projects can drop in.

- A depth-cue rendering library (shadows, parallax, size scaling).
- An alerting module (audio + haptic) for proximity events.
- A reference-size dataset for distance estimation.

## Phased plan

### Phase 1 — Foundation
- Repository structure (the four directories above).
- Contribution guidelines and a glossary of terms.
- One flagship written guide: "Living with one eye — first 90 days".
- An accessibility-guidelines draft (specification pillar).

### Phase 2 — First utilities
- Browser-based **depth-cue trainer** (no install, works on any device).
- **Eye-strain manager** as a browser extension or small desktop app.
- Expand manuals: driving, daily living.

### Phase 3 — Camera-based tools
- **Blind-side assist** mobile prototype.
- **Distance estimator** with the reference-size dataset.
- Reusable alerting and depth-cue **helping modules**.

### Phase 4 — Polish and reach
- Localization of manuals and UI.
- Accessibility audit of the project's own tools.
- Outreach: partner with low-vision organizations and clinicians.

## Guiding principles

- **Evidence-based.** Cite optometry/ophthalmology sources; flag advice
  that is anecdotal. The shared evidence base lives in
  [`research/`](research/). This project does not replace medical
  guidance.
- **Low barrier.** Prefer tools that need no install and run offline.
- **Accessible by construction.** Everything here meets the accessibility
  guidelines we publish.
- **Respectful language.** "Uniocular/monocular vision"; describe people
  first, not deficits.

## Future directions and ideas

Captured from project discussion — not yet scheduled, but worth recording:

- **"How to live with one eye" as the manuals centrepiece** — see pillar 2.
  The intent is breadth: anything from driving and daily tasks to screens
  and an AI-future chapter on smart glasses and AI assistants.
- **A certifiable Uniocular Compatibility Standard** — see pillar 3. The
  ambition is that "uniocular-compatible" becomes a claim a product can
  make and a buyer can trust, the way WCAG conformance works for the web.
- **Uniocular-specific AI/AR aids** — the research review (§13) finds that
  almost all assistive tech targets low-vision/blind users; aids tuned to
  uniocular needs (depth, distance, blind-side coverage, with good acuity)
  are an open opportunity.
- **Deepening the research base** — the [research/](research/) review is a
  living document; topics with thin evidence are listed in its research-
  gaps section.

## How to contribute

This roadmap is a starting point, not a contract. Open an issue to propose
a utility, claim a roadmap item, or suggest a new pillar. Early priorities
are the Phase 1 deliverables.
