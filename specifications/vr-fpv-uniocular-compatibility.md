# Uniocular compatibility profile for VR and FPV displays

**Status:** Draft
**Last updated:** 2026-05
**Audience:** Manufacturers and platform developers of VR/AR/MR headsets and
first-person-view (FPV) drone goggles, and the SDK/engine vendors who serve
them.

This is a **device-class profile** of the general
[accessibility guidelines for uniocular users](accessibility-guidelines.md):
it keeps those rules and adds normative requirements specific to near-eye
stereoscopic displays. It is a seed of the project's proposed **Uniocular
Compatibility Standard (UCS)** and is intended for voluntary adoption and,
eventually, self-certification by manufacturers.

The keywords MUST, SHOULD, MAY, MUST NOT, and SHOULD NOT are used as defined
in RFC 2119. A product **conforms at a level** when it meets every MUST/MUST
NOT at that level and all lower levels.

> **This profile dates.** VR/FPV hardware evolves fast. Requirements are
> written against device *capabilities*, not specific models; re-check the
> evidence base ([research topic](../research/topics/vr-and-fpv-displays/),
> last reviewed 2026-05) when revising.

## 1. Scope and rationale

Uniocular users have one working eye: no stereopsis, a blind side, and faster
single-eye fatigue, but typically **normal acuity** (so magnification and
narration are *not* the relevant accommodations — see the
[research](../research/topics/vr-and-fpv-displays/)). Two facts drive this
profile:

- Stereoscopic 3D is **one depth cue among many**. Motion parallax (from head
  tracking), occlusion, relative size, shading, and perspective remain fully
  available to a uniocular user and carry most usable depth.
- FPV drone feeds are **monoscopic by origin** (one camera), so they are
  already uniocular-compatible in content; the constraints are purely in the
  goggle hardware and its calibration.

A uniocular user is **not** at a VR-sickness disadvantage and in fact bypasses
the vergence–accommodation conflict
([evidence](../research/sources/monocular-vr-sickness-2018/)). The barriers are
therefore design and calibration choices, not biology.

## 2. Stereo independence (Level A)

- **2.1** A product MUST NOT require stereopsis (binocular disparity) to
  complete any task, navigate any menu, or perceive any safety-critical
  information.
- **2.2** Any information a product conveys *only* through stereoscopic depth
  MUST also be available through a monocular cue (occlusion, size, shadow,
  parallax) or a non-visual channel.
- **2.3** A headset/platform MUST be fully operable when output is presented to
  **one eye only** (see §4), and MUST NOT gate launch, setup, or core features
  on detecting two eyes.

## 3. Interpupillary distance and optical fit (Level A)

- **3.1** The product MUST allow the working eye to be optically centered on
  its lens. Hardware with mechanical IPD adjustment MUST expose its full range;
  software MUST allow a **manual IPD/lens-offset override** that does not depend
  on detecting both pupils.
- **3.2** IPD/optical calibration MUST offer a path that succeeds with one eye
  (e.g. focus-by-sharpness on a target), and MUST NOT require the user to align
  two on-screen eye markers to proceed.
- **3.3** The product SHOULD document its IPD range and per-eye adjustment so a
  uniocular user can assess fit before purchase.

## 4. Single-eye output and eye selection (Level A → AA)

- **4.1 (A)** The product MUST provide an explicit **single-eye mode** that
  designates the working eye (left/right) for input and, where applicable,
  rendering and UI placement. (Apple Vision Pro's *Settings > Accessibility >
  Eye Input > Left/Right Eye Only* is the reference implementation.)
- **4.2 (A)** If the product uses **eye tracking** for input or calibration, it
  MUST allow that tracking to target a single eye, and MUST allow eye tracking
  to be **disabled** with a graceful fallback (head pointer, controller, fixed
  foveated rendering) that preserves full functionality.
- **4.3 (A)** Eye-tracking logic MUST NOT average a working eye with a
  non-tracking, prosthetic, or misaligned eye in a way that degrades the
  pointer. When only one eye is reliably detected, the product MUST use it
  rather than failing.
- **4.4 (AA)** The product SHOULD let the non-working eye's display be blanked
  or its render culled (to reduce distraction, stray light, fatigue, and — on
  capable hardware — power/GPU load), without affecting the working-eye view.

## 5. Depth, motion parallax, and latency (Level AA)

- **5.1** Where depth matters, the product SHOULD reinforce it with monocular
  cues (high-contrast shadows, occlusion, atmospheric perspective) and SHOULD
  offer a toggle to **strengthen** these cues.
- **5.2** Head-tracked **motion parallax** is the primary recoverable depth cue
  for uniocular users; 6-DoF head tracking MUST remain low-latency in
  single-eye mode (no parallax penalty for disabling the second eye).
- **5.3** Depth-based input (hand-distance gestures, gaze-depth selection) MUST
  have an equivalent that does not require the user to judge absolute distance.

## 6. Field of view and blind-side awareness (Level AA)

- **6.1** Safety- or task-critical events MUST NOT rely on the user noticing
  something at the far edge of a wide FOV; such events SHOULD be surfaced near
  center or repeated centrally.
- **6.2** The product SHOULD let the user declare which side is the blind side
  (this MUST NOT be assumed) and SHOULD route blind-side hazards to a central
  visual, audio, or haptic indicator.

## 7. Comfort and fatigue (Level AA)

- **7.1** Sustained-reading or close-work surfaces SHOULD be lockable to a
  fixed, comfortable focal distance to limit continuous accommodation by the
  single working eye.
- **7.2** The product MUST honor the platform reduced-motion setting; rapid
  flashing MUST NOT be required, and break reminders for long sessions SHOULD
  be available.

## 8. FPV-goggle–specific requirements (Level A → AA)

- **8.1 (A)** Goggles MUST present the (monoscopic) camera feed fully to the
  working eye — dual-display goggles MUST route the complete image to each
  display (not split halves) so a single-eye pilot loses no telemetry or frame.
- **8.2 (A)** Goggles MUST provide IPD/lens adjustment sufficient to center one
  display on the working eye, OR offer a **single-lens / box** form factor that
  is inherently single-eye-compatible.
- **8.3 (AA)** Manufacturers SHOULD offer or document a **single-eye HUD**
  option (one display over one eye, the other eye unobstructed). Beyond
  uniocular access, this helps any pilot keep the aircraft in **unaided visual
  line of sight** where regulators require it (e.g. FAA 14 CFR 107.31), and the
  product documentation SHOULD note this rather than implying enclosed goggles
  alone satisfy line-of-sight rules.
- **8.4 (AA)** Goggles SHOULD allow one display to be powered down or dimmed in
  single-eye use to save battery and reduce stray light.

## 9. Multi-channel feedback (Level AA)

- **9.1** Proximity, collision, altitude, and distance warnings SHOULD be
  available through audio and/or haptic channels, not visual-only.
- **9.2** Important state changes SHOULD use at least two channels so a missed
  visual cue is recoverable.

## 10. Conformance and testing (Level A)

- **10.1** Before release, the product MUST be tested in single-eye mode (by
  uniocular testers or with one eye occluded), and every feature that conveys
  depth or spatial relationships MUST be verified to work with one eye.
- **10.2** A conforming product SHOULD publish which level (A/AA/AAA) it meets
  and against which version/date of this profile, so the claim is checkable.

## 11. Level AAA (optimal)

- **11.1** Exaggerated/adjustable motion parallax on lateral head movement as
  an opt-in depth aid.
- **11.2** Per-eye render culling exposed as a documented power/performance
  optimization for single-eye users.
- **11.3** Built-in single-eye onboarding that calibrates fit and input without
  ever requiring two eyes.

## 12. Open questions

This is a draft seeking implementer feedback (via issues):

- A machine-checkable conformance checklist and a self-certification mark.
- Quantitative latency/parallax thresholds for single-eye depth comfort.
- Alignment with W3C XAUR and the Game Accessibility Guidelines so this profile
  extends rather than competes (see the
  [accessibility-standards research](../research/topics/accessibility-standards/)).
