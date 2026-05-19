# Glossary

Shared terminology for the uniocular-utilities project. Use these terms
consistently across code, documentation, and issues.

## Vision terms

**Uniocular / monocular vision** — seeing with one eye, or having usable
sight in only one eye. The preferred terms in this project. Avoid
"one-eyed" in user-facing text.

**Binocular vision** — seeing with both eyes together.

**Stereopsis** — depth perception that comes from the brain combining the
slightly different images from two eyes. Not available with one eye.

**Monocular depth cues** — depth information available to a single eye.
The basis for most of this project's tools:

- *Motion parallax* — nearer objects sweep across vision faster than
  farther ones when the head moves.
- *Relative size* — a known object looks smaller when farther away.
- *Occlusion (interposition)* — a nearer object overlaps a farther one.
- *Shadow and shading* — light direction reveals shape and distance.
- *Texture gradient* — surface detail gets finer with distance.
- *Aerial perspective* — distant objects look hazier and lower-contrast.
- *Linear perspective* — parallel lines converge with distance.

**Field of view** — the area a person can see at one moment. Uniocular
vision reduces the horizontal field, creating a "blind side".

**Blind side** — the side toward the non-seeing (or absent) eye, where
obstacles and hazards are easily missed.

**Amblyopia** — reduced vision in one eye that did not develop normally,
sometimes called "lazy eye".

**Enucleation** — surgical removal of an eye.

**Diplopia** — double vision.

## Project terms

**Pillar** — one of the four categories of deliverable: software
utilities, manuals, specifications, helping modules.

**Utility** — a runnable tool in `software/`.

**Module** — a reusable, embeddable component in `modules/`.

**Guide / manual** — a task-oriented document in `manuals/`.

**Specification** — a standard for builders in `specifications/`.
