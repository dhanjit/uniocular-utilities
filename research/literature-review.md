# Literature review (master)

The top-level overview of the project's research knowledge base. It
summarizes what we know about functional uniocular vision and indexes the
per-topic collated reviews and per-source notes.

See [README.md](README.md) for how this knowledge base is organized and its
methodology/limitations. This is a curated review — read the primary sources
(linked from each source note) before relying on a finding.

## How the knowledge base is structured

- **`topics/<topic>/`** — a collated review per concept, summarizing the
  learnings and citing both source notes and minor references.
- **`sources/<paper>/`** — one note per strong paper: citation, scope, key
  points, learnings, verification status, and which topics cite it.
- **[deep-research-synthesis.md](deep-research-synthesis.md)** — an external
  AI-generated report kept separately; only its verified findings are folded
  into the topics.

## Scope distinction

Functionally uniocular people typically retain **normal acuity** in the
working eye. They are distinct from low-vision/blind populations, so
magnification, contrast filters, and scene narration are largely misaligned.
Their four core challenges: loss of stereopsis; a reduced field / blind side;
fatigue of the single working eye; and protecting the one irreplaceable eye.

## Topics

| Topic | Focus |
| --- | --- |
| [epidemiology-and-causes](topics/epidemiology-and-causes/) | Who is uniocular and why |
| [adaptation](topics/adaptation/) | Adjustment timeline and rehabilitation |
| [depth-perception](topics/depth-perception/) | Monocular cues, motion parallax, Pulfrich |
| [stereopsis-functional-impact](topics/stereopsis-functional-impact/) | Which tasks stereo loss actually costs |
| [driving](topics/driving/) | Safety evidence and adaptation |
| [field-of-view-and-blind-side](topics/field-of-view-and-blind-side/) | Scanning, prisms, electronic aids |
| [eye-protection](topics/eye-protection/) | Protecting the remaining eye; compliance |
| [eye-strain-and-ergonomics](topics/eye-strain-and-ergonomics/) | Asthenopia, screen setup |
| [sports](topics/sports/) | Performance and protection |
| [children-and-amblyopia](topics/children-and-amblyopia/) | Pediatric impact and accommodations |
| [psychological-impact](topics/psychological-impact/) | Mental-health adjustment |
| [prosthetics-and-rehabilitation](topics/prosthetics-and-rehabilitation/) | Ocular prosthesis, rehab programs |
| [assistive-technology](topics/assistive-technology/) | AR, smart glasses, AI |
| [vr-and-fpv-displays](topics/vr-and-fpv-displays/) | VR headsets and drone FPV goggles for uniocular users |
| [accessibility-standards](topics/accessibility-standards/) | Frameworks for a compatibility standard |

## Cross-cutting takeaways

- **Adaptation takes months** and is faster after gradual loss; formal
  rehabilitation is rarely provided — the project's central unmet need.
- **Motion parallax** (head movement) is the most powerful recoverable depth
  cue and is trainable in principle.
- **2D screens largely neutralize** the stereopsis disadvantage — a key
  design lever and standard principle. The same holds for **immersive
  displays**: FPV drone goggles are monoscopic by design, and monocular VR use
  is not worse for sickness (it bypasses the vergence–accommodation conflict).
- **Protecting the remaining eye** is the highest-impact safety message, and
  the barrier to compliance is behavioral, not informational.
- **Assistive tech is biased to low-vision/blind users**; uniocular-specific
  aids (depth, distance, blind side) are an open opportunity.
- **No standard certifies "uniocular-compatible"** — a gap the project's
  proposed UCS would fill.

## Source index

Strong papers with their own notes (see `sources/`):

- [kraut-2002-adaptation](sources/kraut-2002-adaptation/) · [ihrig-amvr](sources/ihrig-amvr/)
- [ono-ujike-2005-motion-parallax](sources/ono-ujike-2005-motion-parallax/) · [motion-parallax-pursuit-2014](sources/motion-parallax-pursuit-2014/) · [pulfrich-monovision-2013](sources/pulfrich-monovision-2013/)
- [stereopsis-surgical-performance-2017](sources/stereopsis-surgical-performance-2017/) · [stereopsis-2d-3d-2014](sources/stereopsis-2d-3d-2014/)
- [racing-drivers-2019](sources/racing-drivers-2019/) · [driving-hemianopia-vii-2021](sources/driving-hemianopia-vii-2021/)
- [peli-2017-multiplexing-prism](sources/peli-2017-multiplexing-prism/) · [ar-depth-mapping-2019](sources/ar-depth-mapping-2019/) · [monocular-vr-sickness-2018](sources/monocular-vr-sickness-2018/)
- [neimkin-custer-2017-eyewear-compliance](sources/neimkin-custer-2017-eyewear-compliance/)
- [asthenopia-meta-analysis-2026](sources/asthenopia-meta-analysis-2026/)
- [barrett-2017-elite-athletes](sources/barrett-2017-elite-athletes/)
- [amblyopia-whole-child-2023](sources/amblyopia-whole-child-2023/) · [kelly-2025-amblyopia-hrqol](sources/kelly-2025-amblyopia-hrqol/)
- [visual-impairment-mental-health](sources/visual-impairment-mental-health/) · [makrakis-2021-prosthesis-qol](sources/makrakis-2021-prosthesis-qol/)

## Research gaps

1. Uniocular-specific AI/AR aids (vs. low-vision/blind tools).
2. Effectiveness of depth-cue / motion-parallax training in newly monocular
   adults.
3. Biometric models of single-eye screen/accommodation fatigue.
4. Quantified daily-living task data (pouring, stairs, thresholds).
5. Protective-eyewear compliance interventions for adults.
6. A conformance methodology certifying uniocular compatibility.
7. A clean global prevalence estimate of functional uniocularity.
