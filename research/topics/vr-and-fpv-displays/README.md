# Topic: VR headsets and drone FPV goggles

Whether near-eye displays — VR/mixed-reality headsets and first-person-view
(FPV) drone goggles — work for uniocular users, and what makes a headset
uniocular-compatible.

## Summary

- **VR/MR headsets** (Oculus Rift, Meta Quest, PlayStation VR/VR2, Apple
  Vision Pro) are **stereoscopic**: they render a separate image per eye for
  binocular disparity. A uniocular user sees only one of the two images, so
  the stereo-3D effect is lost — but the experience still works on monocular
  cues, above all the **head-tracked motion parallax** these devices excel at.
  Usability turns on IPD fit and on eye-tracking-dependent features. **Apple
  Vision Pro is the only major device with an explicit single-eye
  accessibility setting.**
- **FPV drone goggles** are almost all **monoscopic** — a drone carries one
  camera, so the *same* 2D feed is sent to both eyes. There is no stereo depth
  to lose, which makes them inherently uniocular-friendly. Single-lens "box"
  goggles are ideal; dual-display goggles work fine once IPD is aligned.

## Key findings

### VR / mixed-reality headsets

- Headsets render one image per eye to create binocular disparity; with one
  working eye there is **no stereoscopic 3D**, but **motion parallax** (from
  6-DoF head tracking), perspective, occlusion, relative size, texture, and
  lighting remain — and these carry most of the usable depth. Motion parallax
  is the strongest recoverable cue (see
  [depth-perception](../depth-perception/)).
  (<https://www.vrs.org.uk/can-you-use-vr-with-just-one-eye/>;
  <https://www.howtogeek.com/844048/can-you-use-vr-with-one-eye/>)
- **IPD (interpupillary distance)** adjustment assumes two eyes; it should be
  set so the **working eye is centered on its lens**. A wrong IPD causes blur,
  edge distortion, and strain. Quest 2 offers 58–68 mm in three steps; many
  headsets use a continuous dial.
  (<https://www.howtogeek.com/758896/how-to-measure-your-ipd-and-why-it-matters-for-vr/>;
  <https://zybervr.com/blogs/news/a-complete-guide-of-pd-what-is-pd-ipd-why-important-and-how-to-adjust-the-pd-of-oculus-quest-2>)
- The blank or duplicated image at the non-seeing eye can be distracting or
  admit stray light; **occluding that lens** is a common comfort fix.
  (<https://www.vrs.org.uk/can-you-use-vr-with-just-one-eye/>)
- **Eye tracking is the real compatibility variable:**
  - **Apple Vision Pro** uses gaze as the primary input and during setup, but
    explicitly supports monocular use: **Settings > Accessibility > Eye Input
    > Both Eyes / Left Eye Only / Right Eye Only**, plus a dedicated
    "help with eye setup" path and prescription/vision-condition guidance. The
    best-supported device for uniocular users.
    (<https://support.apple.com/en-us/118513>;
    <https://support.apple.com/guide/apple-vision-pro/eye-input-tan88016cfa4/visionos>;
    <https://support.apple.com/en-by/120052>)
  - **PSVR2 / Quest Pro** use eye tracking for **foveated rendering**;
    single-eye calibration may degrade or need the working eye selected. Not a
    hard blocker for most content, but eye-tracked titles can misbehave.
    (<https://www.dexerto.com/tech/what-is-foveated-rendering-on-psvr2-2069522/>)
    Reported workarounds (provisional, forum-sourced, see synthesis note
    below): skip automated IPD/eye calibration and set IPD manually by
    sharpening text in the working eye; calibrate one eye at a time by closing
    the other; or disable eye tracking entirely (PSVR2 then falls back to fixed
    foveated rendering). The Quest Pro's gaze-averaging ("cyclopean") logic can
    misbehave with a prosthetic or amblyopic eye, but eye tracking can be paused
    or revoked per-app.

### Physiology: VR sickness and the vergence–accommodation conflict

- A clinical study found monocular viewing produced **lower** VR-sickness
  scores than binocular viewing (dizziness and eye discomfort significantly
  lower), not higher — see
  [monocular-vr-sickness-2018](../../sources/monocular-vr-sickness-2018/). So a
  uniocular user is **not at a sickness disadvantage** in VR.
- Mechanistically, much VR sickness stems from the **vergence–accommodation
  conflict** (eyes converge on a simulated near object while the lens stays
  focused on the headset's fixed focal plane). A uniocular user has **no
  vergence demand**, so they largely bypass this conflict — a genuine
  physiological advantage (rationale carried from the project
  [synthesis](../../deep-research-synthesis.md), Part B).

### Drone FPV goggles

- A drone carries a **single camera**, so FPV goggles are **monoscopic**: the
  same 2D feed goes to both eyes, with no binocular disparity. There is **no
  stereo depth to lose** — a uniocular pilot sees the complete picture with one
  eye. (<https://oscarliang.com/fpv-goggles/>;
  <https://fpvlab.com/forums/archive/index.php/t-32964.html>)
- Two designs: **single-lens "box" goggles** (one screen + one large lens —
  naturally fine for one eye, full screen at full resolution); and
  **dual-display binocular goggles** (DJI, Fat Shark, Skyzone — each display
  shows the same feed). Dual-display models need **IPD alignment** so the
  working eye registers cleanly — DJI Goggles 3 slide 56–72 mm, older models
  use an IPD knob.
  (<https://oscarliang.com/fpv-goggles/>;
  <https://blog.uavmodel.com/dji-goggles-3-setup-complete-pairing-firmware-and-display-calibration-guide-2026/>)
- Some one-eyed pilots report discomfort seeing two screens; **covering the
  unused side** or tuning IPD resolves it.
  (<https://fpvdronepilots.com/threads/fpv-goggles-uncomfortable-seeing-2-individual-displays-skyzone-04x.4318/>)
- **True stereoscopic 3D FPV** (dual-lens 3D camera → two offset feeds, e.g.
  the discontinued Skyzone 3D goggles) did once exist and *would* disadvantage
  a uniocular pilot — but that market collapsed (cost, drone weight, no way to
  share 3D on 2D platforms) and is effectively extinct, so it is moot for
  today's pilots. (provisional, from the synthesis note below)

### Regulatory angle: a single-eye HUD can aid line-of-sight compliance

- Under **FAA Part 107.31**, the remote pilot must keep the aircraft in
  **visual line of sight with vision unaided by any device other than
  corrective lenses** — enclosed FPV/box goggles do not satisfy this unless a
  separate visual observer is present.
  (<https://www.ecfr.gov/current/title-14/chapter-I/subchapter-F/part-107/subpart-B/section-107.31>)
- A **monocular FPV display** (a single micro-display/HUD over one eye, the
  other eye left unobstructed) lets a solo pilot watch the onboard feed *and*
  keep the physical aircraft in unaided line of sight with the other eye —
  useful for uniocular *and* binocular pilots, though it imposes a
  split-attention cognitive load.

## Implications for the project

- FPV goggles are a clean example of the project principle that **a 2D feed
  neutralizes the stereopsis disadvantage** (see
  [stereopsis-functional-impact](../stereopsis-functional-impact/)): monoscopic
  by design, so uniocular-compatible by default. **Single-lens goggles** are
  the recommended form factor.
- For VR, the uniocular-compatibility levers are: **continuous IPD
  adjustment**, an explicit **single-eye accessibility mode** (Apple Vision Pro
  is the model to copy), **graceful degradation** of eye-tracking/foveated
  features when only one eye calibrates, and content that leans on
  **motion-parallax** depth rather than stereo. These are candidate clauses for
  the Uniocular Compatibility Standard (see
  [accessibility-standards](../accessibility-standards/)).

## Open questions

- Measured comfort/fatigue of prolonged single-eye VR use (one working eye
  doing all the work behind a near-eye display) — see
  [eye-strain-and-ergonomics](../eye-strain-and-ergonomics/).
- How much, quantitatively, stereo-dependent VR content (depth-based gameplay,
  reach-and-grab 3D UI) actually disadvantages a uniocular user versus the
  monocular cues available.
- Robustness of eye-tracking calibration for monocular users across Quest Pro,
  PSVR2, and Vision Pro.

## Verification status

**Mixed.** This note draws on (a) direct web sources — vendor/support docs,
community forums, general explainers — and (b) an external **Gemini Deep
Research** report commissioned for this project (the same kind of provisional
synthesis as the project-wide
[deep-research-synthesis.md](../../deep-research-synthesis.md); treat its
unverified detail as provisional).

Spot-verified against primary sources:

- **Monocular VR sickness is not worse than binocular** — verified; the IOVS
  study is real and figures match, see
  [monocular-vr-sickness-2018](../../sources/monocular-vr-sickness-2018/)
  (conference abstract).
- **FAA Part 107.31** unaided-VLOS requirement — verified against the eCFR
  text.
- **Apple Vision Pro single-eye Eye Input** setting — verified against Apple
  Support.

Still provisional (reproduced as reported / forum-sourced): the PSVR2/Quest
eye-tracking workarounds, OpenXR-Toolkit single-eye render culling, specific
monocular-HUD product specs, and the "3D FPV is extinct" market claim. The
Gemini report mis-attributed several citations (its footnotes pointed to a
single explainer page); the underlying facts above were re-checked
independently. Confirm finer hardware details against current manufacturer
manuals before relying on them.
