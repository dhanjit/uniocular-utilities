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

- Daily-living guides: pouring, cooking, stairs, crowds, doorways.
- Driving with monocular vision: mirror setup, scanning habits, legality
  notes by region.
- Sports and hobbies: catching, cycling, swimming adaptations.
- Returning to work and school: workspace setup, requesting adjustments.

### 3. Specifications and guidelines (`/specifications`)

Standards for builders so their products work for uniocular users.

- **Accessible UI guidelines** — never require stereo vision, depth
  gestures, or 3D-only cues; provide 2D fallbacks.
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
  that is anecdotal. This project does not replace medical guidance.
- **Low barrier.** Prefer tools that need no install and run offline.
- **Accessible by construction.** Everything here meets the accessibility
  guidelines we publish.
- **Respectful language.** "Uniocular/monocular vision"; describe people
  first, not deficits.

## How to contribute

This roadmap is a starting point, not a contract. Open an issue to propose
a utility, claim a roadmap item, or suggest a new pillar. Early priorities
are the Phase 1 deliverables.
