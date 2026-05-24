# Topic: Assistive technology — AR, smart glasses, and AI

Camera-based AR and AI wearables are advancing fast and are central to the
project's "AI-future" direction.

## Summary

AR depth overlays improve mobility for low-vision users; mainstream AI smart
glasses (2025) and purpose-built assistive glasses exist. But almost all of
it targets low-vision/blind users — a uniocular-specific design gap remains.

## Key findings

- AR depth-mapping overlay improved obstacle avoidance ~50% (RP patients) —
  see [ar-depth-mapping-2019](../../sources/ar-depth-mapping-2019/).
- Mainstream AI smart glasses are now consumer reality (Meta Ray-Ban, ~$300,
  not designed for low vision) and purpose-built ones exist (Envision ~$800+,
  Ally Solos, 2025). (AFB review: <https://afb.org/aw/fall2025/meta-glasses-review>;
  comparison: <https://www.specialneeds.com/articles/assistive-tech/vision/smart-glasses-for-vision-impairment-in-2025-meta-ray-ban-vs-envision-vs-specialized-options/>;
  LLM assistive glasses review: <https://pmc.ncbi.nlm.nih.gov/articles/PMC11009354/>)
- Optical state of the art for the blind side is the multiplexing prism — see
  [peli-2017-multiplexing-prism](../../sources/peli-2017-multiplexing-prism/).
- AI **monocular depth estimation** (2D→3D) is mature (ARKit/ARCore), but
  consumer software translating it into alternative feedback (haptic,
  color-mapping) for users lacking stereopsis is essentially missing
  (provisional, from the [synthesis](../../deep-research-synthesis.md)).

## Implications for the project

- The high-value features for uniocular users are **depth/distance cues and
  blind-side coverage**, not magnification or scene narration.
- Directly informs the blind-side-assist, distance-estimator, and depth-cue
  rendering work.

## Open questions

- Uniocular-specific AI/AR aids are an open opportunity with little existing
  evidence.
