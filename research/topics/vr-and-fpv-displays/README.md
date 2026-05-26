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

**From search digest.** Drawn from vendor/support docs, community forums, and
general explainers, not peer-reviewed studies. The monoscopic nature of FPV
feeds and Apple Vision Pro's single-eye setting are well-corroborated; the
finer hardware details should be confirmed against current manufacturer
manuals before being relied on.
