# Accessibility guidelines for uniocular users

**Status:** Draft
**Audience:** Designers and developers building software, content, or
hardware that uniocular people will use.

This specification defines how to build products that work well for people
who see with one eye. It complements general accessibility standards (such
as WCAG); it does not replace them.

The keywords MUST, SHOULD, and MAY are used as defined in RFC 2119.

## 1. Background

Uniocular vision lacks *stereopsis* — the depth perception that comes from
combining two eyes' images. Uniocular people judge depth using monocular
cues (motion parallax, relative size, occlusion, shadow; see the
[glossary](../GLOSSARY.md)). They also have a narrower field of view, with
a "blind side" toward the non-seeing eye, and the single working eye
fatigues faster.

Products that assume two working eyes can become difficult or unusable.
These guidelines remove that assumption.

## 2. Depth and 3D

- **2.1** A product MUST NOT require stereopsis to be used. Any
  information conveyed by stereoscopic depth MUST also be available
  through a monocular cue or a non-visual channel.
- **2.2** Stereoscopic or autostereoscopic 3D (VR, 3D displays, parallax
  barriers) MUST offer a 2D / monoscopic mode that exposes the same
  functionality.
- **2.3** Where depth is meaningful, products SHOULD reinforce it with
  monocular cues: shadow, occlusion, relative size, and motion parallax.
- **2.4** Depth-based input (e.g. hand-distance gestures, gaze-depth
  selection) MUST have an equivalent input that does not depend on the
  user judging distance.

## 3. Field of view and layout

- **3.1** Critical content and controls MUST NOT depend on the user
  noticing something at the far edge of a wide field. Important alerts
  SHOULD appear near the center or be repeated centrally.
- **3.2** Time-limited prompts that can appear anywhere on screen SHOULD
  give enough time for a user scanning with one eye, or be dismissible
  later.
- **3.3** Layouts SHOULD NOT assume the user can attend to both far-left
  and far-right regions simultaneously.

## 4. Eye comfort and fatigue

- **4.1** Text MUST be resizable and reflow without loss of function.
- **4.2** Products SHOULD support high-contrast and adjustable-contrast
  modes; default contrast MUST meet WCAG AA at minimum.
- **4.3** Products with sustained reading or close work SHOULD offer
  break reminders and MUST NOT penalize the user for pausing.
- **4.4** Essential motion and flashing MUST respect the user's
  reduced-motion setting; rapid flashing MUST NOT be required.

## 5. Multi-channel feedback

- **5.1** Important state changes SHOULD be conveyed through at least two
  channels (e.g. visual plus audio or haptic), so a missed visual cue is
  recoverable.
- **5.2** Proximity, collision, or distance alerts SHOULD support audio
  and/or haptic output, not visual-only.

## 6. Hardware

- **6.1** Wearables and cameras intended as monocular aids SHOULD position
  capture and feedback to cover the user's blind side.
- **6.2** Devices SHOULD let the user configure which side is the blind
  side; this MUST NOT be assumed.

## 7. Testing

- **7.1** Products SHOULD be tested by covering one eye, or with uniocular
  testers, before release.
- **7.2** Any feature that conveys depth or spatial relationships MUST be
  verified to work with a single eye.

## 8. Open questions

This is a draft. Feedback is welcome via issues. Areas still to settle:

- Concrete contrast and text-size minimums beyond WCAG AA.
- Guidance for games where depth judgment is core gameplay.
- A conformance checklist contributors can run against.
