# Topic: Accessibility standards and frameworks

Existing standards to build on for a Uniocular Compatibility Standard.

## Summary

Current accessibility frameworks treat vision impairment as an
acuity-reduction scale and do not codify the needs of users with good acuity
but no stereopsis. No certification for "uniocular-compatible" exists.

## Key findings

- **W3C XAUR** (XR Accessibility User Requirements, 2021): ~18–19 immersive
  user needs; does not isolate stereopsis loss, but its routing of alerts to
  secondary text/haptic channels is adaptable to blind-side alerts.
  (<https://www.w3.org/TR/xaur/>)
- **Game Accessibility Guidelines**: mono/stereo audio toggle (note:
  same-side hearing loss often accompanies trauma eye loss), adjustable FOV,
  off-screen/blind-side indicators.
  (<https://gameaccessibilityguidelines.com/full-list/>)
- **WCAG 2.2**: 2D-DOM focused; no guidance for 3D/z-axis/stereoscopic
  dependencies.
- Long advisory guidelines see poor adoption — argues for a **concise,
  testable, certifiable** standard. (arXiv: <https://arxiv.org/abs/2602.17939>)
- 2D representations largely neutralize the stereo disadvantage — see
  [stereopsis-2d-3d-2014](../../sources/stereopsis-2d-3d-2014/).

## Implications for the project

- Borrow XAUR's user-needs framing and WCAG's testable-criteria +
  conformance-levels model for a **Uniocular Compatibility Standard (UCS)**.
- A concrete UCS Level A/AA/AAA draft already exists in the
  [deep-research synthesis](../../deep-research-synthesis.md) — the starting
  point when we move from research to the standard.
- A first device-class profile has been drafted: the
  [VR/FPV uniocular compatibility profile](../../../specifications/vr-fpv-uniocular-compatibility.md),
  grounded in the [VR/FPV research](../vr-and-fpv-displays/).

## Open questions

- No existing scheme certifies products as uniocular-compatible — the gap
  this project's standard would fill.
