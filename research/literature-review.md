# Literature review

An annotated bibliography of research relevant to uniocular people,
organized by topic. Each entry summarizes a key finding, links a source
(open-access where available), and notes how it informs the project
[roadmap](../ROADMAP.md).

See [README.md](README.md) for methodology and limitations. This is a
curated first pass — read the primary sources before relying on a finding.

---

## 1. Adaptation to monocular vision

How people adjust after losing vision in one eye, and how rehabilitation
helps.

- **Adaptation is slower after sudden loss than gradual loss.** Patients
  with sudden visual loss adapted more slowly than those with gradual
  loss (reported as ~8.8 vs. ~3.6 months). Main consequences are loss of
  depth perception and restricted peripheral field.
  - "Adaptation to monocular vision" — PubMed:
    <https://pubmed.ncbi.nlm.nih.gov/12131596/>
  - "Vision Rehabilitation Team Management of Acquired Monocular Vision":
    <https://www.researchgate.net/publication/235522108>
- **Structured rehabilitation programs exist.** The VA's Acquired
  Monocular Vision Rehabilitation program covers home adaptive skills and
  mobility training to compensate for reduced field and depth loss.
  - <https://www.rehab.research.va.gov/jour/07/44/4/ihrig.html>
- **Balance depends on vision as one of three systems.** Balance is
  controlled by the vestibular, somatosensory, and visual systems; losing
  visual input forces the body to lean on the other two. Visual-skills
  training (fixation, scanning, pursuit, saccades) helps compensate.
  - "Physical Therapy and Monocular Vision Loss":
    <https://tlc-pt.com/wp-content/uploads/sites/6/2024/06/Physical-Therapy-and-Monocular-Vision-Loss.pdf>
  - Patient-facing overview, Lighthouse Guild:
    <https://lighthouseguild.org/monocular-vision-etiology-symptoms-and-rehabilitation-2/>

**Informs:** the "first 90 days" manual (adaptation timeline, what to
expect); daily-living and mobility guides.

---

## 2. Depth perception and monocular cues

Uniocular people lose stereopsis but retain monocular depth cues. Motion
parallax — driven by head movement — is the most powerful.

- **Motion parallax needs translational head/body movement.** Depth
  information comes from side-to-side motion, not rotation. The visual
  system uses the smooth-pursuit eye-movement signal to resolve
  depth-sign (which way is nearer) from parallax.
  - "Modeling depth from motion parallax with the motion/pursuit ratio" —
    PMC: <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4186274/>
  - "Visual Depth from Motion Parallax and Eye Pursuit" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC3348271/>
  - "Motion parallax driven by head movements" — PubMed:
    <https://pubmed.ncbi.nlm.nih.gov/15943054/>
- **One-eyed people regain functional depth by keeping the head in
  motion** — often unconsciously, e.g. shifting the head when parking or
  pouring. But motion parallax does not fully replace binocular vision:
  in some visuomotor tasks head movement gave no measurable advantage
  despite generating comparable parallax.
- **Parallax can augment other depth cues.** In macular degeneration,
  motion parallax was found to augment disparity for depth perception —
  evidence that training cue-combination is worthwhile.
  - <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12849822/>
- **The monocular cue set** (relative size, occlusion/interposition,
  shadow and shading, texture gradient, aerial perspective, linear
  perspective) is well documented and teachable.
  - Hanover College interactive demos:
    <https://isle.hanover.edu/isle2/Ch07DepthSize/Ch07MonocDepthInv_evt.html>

**Informs:** the depth-cue trainer utility (motion parallax exercises,
head-movement habits); the depth-cue rendering module; the [accessibility
guidelines](../specifications/accessibility-guidelines.md) on reinforcing
depth with monocular cues.

---

## 3. Driving with monocular vision

Mixed evidence; the distinction between sudden monocularity and stable,
adapted monocular vision matters.

- **Sudden monocular condition sharply degrades performance.** In a
  racing-driver study, drivers under a sudden monocular condition were
  2.1–6.5x more likely to collide with target vehicles vs. their
  binocular baseline, with reaction-time increases of ~64–126 ms.
  Crucially, sudden monocular *reduction* in vision with the peripheral
  field preserved did **not** impair performance — it was the loss of the
  field/monocularity itself that mattered.
  - "Implications of monocular vision for racing drivers" — PLOS One
    (open access):
    <https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0226308>
  - PMC mirror: <https://pmc.ncbi.nlm.nih.gov/articles/PMC6913915/>
- **Population studies are conflicting.** Research on commercial drivers
  (truck, bus, taxi) reports mixed results — some find more crashes and
  convictions among monocular drivers, others find equivalent rates. Many
  jurisdictions screen using both eyes or the better-seeing eye.
  - "Vision and Driving" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC2975746/>
- **Takeaway:** adaptation time matters. Newly monocular drivers should
  not assume their pre-loss performance; established monocular drivers
  can perform comparably. Regional licensing rules vary.

**Informs:** the driving manual (adaptation period, mirror setup and
scanning habits, "check local law" framing). The project must avoid
giving blanket legal or fitness-to-drive advice.

---

## 4. Field-of-view loss and the blind side

Uniocular vision and hemianopic field loss share a problem: a region
where hazards go undetected. Hemianopia research transfers usefully.

- **Compensatory scanning is the core behavioral strategy.** Training
  individuals to make a large blind-side scan helps them detect hazards;
  a minimum scan magnitude can serve as a training criterion or a target
  for assistive technology.
  - "Driving With Hemianopia VII" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC7804568/>
- **Prism-based optical aids expand awareness of the blind side.**
  Peripheral prisms (e.g. the Peli Lens) shift images from the blind
  region into the seeing field, expanding blind-side awareness by ~30°+.
  Clinical trials of peripheral and multi-periscopic prism glasses exist.
  - Peli peripheral prism trial: <https://clinicaltrials.gov/study/NCT00494676>
  - Multi-periscopic prism trial: <https://clinicaltrials.gov/study/NCT04827147>
- **Electronic collision-warning devices** are being studied to warn of
  mid/high obstacles a long cane would miss.
  - <https://clinicaltrials.gov/study/NCT03057496>
- **Overlay/AR approaches** can integrate information to increase the
  effective field of view.
  - "Visual Field Loss: Integrating Overlayed Information" — MDPI Vision:
    <https://www.mdpi.com/2411-5150/6/4/67>

**Informs:** the blind-side-assist utility (collision warning, scan
prompts); the alerting module; manuals on scanning habits. Note: prism
optics are a hardware domain, useful as reference rather than something
the project builds.

---

## 5. Eye strain and fatigue (asthenopia)

The single working eye does all the visual work; managing fatigue
matters. General asthenopia research applies.

- **Asthenopia is highly prevalent and tied to sustained near work.**
  Symptoms include eye tiredness, strain, blurred vision, headache, and
  occasional double vision, arising after prolonged screen use, reading,
  or fine close work. A systematic review/meta-analysis reports pooled
  prevalence of eye tiredness ~65% and strain/fatigue ~47%.
  - Systematic review & meta-analysis — JOGH:
    <https://jogh.org/2026/jogh-16-04053/>
  - PMC mirror: <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12879263/>
- **Cause** is largely the sustained effort of accommodation/convergence;
  unequal refractive error between the eyes is itself a contributor.
- **The 20–20–20 rule** (every 20 minutes, look ~20 feet away for 20
  seconds) is a research-supported, low-cost mitigation; structured break
  scheduling reduces strain.
  - EyeWiki overview: <https://eyewiki.org/Asthenopia>

**Informs:** the eye-strain-manager utility (break reminders, 20-20-20
timer, contrast/reading presets); accessibility guideline 4.3 (break
reminders, no penalty for pausing).

---

## 6. Amblyopia and children

Amblyopia ("lazy eye") is the most common cause of functional monocular
vision and has measurable effects on everyday function.

- **Prevalence and impact.** Amblyopia affects up to ~4% of children and
  often persists into adulthood. It can interfere with contrast
  sensitivity, attention, reading, eye–hand coordination, physical
  activity, and health-related quality of life.
  - "Amblyopia and the whole child" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC9998377/>
  - "Functional consequences of amblyopia and its impact on HRQoL" —
    PubMed: <https://pubmed.ncbi.nlm.nih.gov/40319624/>
  - StatPearls overview: <https://www.ncbi.nlm.nih.gov/books/NBK430890/>
- **Reading is measurably slower.** Children with amblyopia have been
  reported reading ~28–32% slower than peers during binocular viewing
  (~148 vs. ~204 words/min).
- **Treatment outcome is age-dependent.** Spectacles alone achieve full
  acuity recovery in ~32% of children under 7, but only ~14% at ages
  7–12 and ~11% at 13–17; occlusion therapy yields favorable improvement
  in at least ~75% of treated children, though recurrence is possible.
- **Long-term social outcomes may be reassuring.** A 1958 British birth
  cohort found no differences in educational, health, or social outcomes
  in mid-adulthood between adults with amblyopia and those with normal
  vision.
- **Occlusion (patching) therapy affects children's quality of life**
  during treatment — relevant to designing supportive, non-punishing
  tools.
  - <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8951718/>

**Informs:** a potential children/families manual; reading-aid features
in the eye-strain manager; design tone (supportive, not deficit-framed).

---

## 7. Enucleation and prosthetic-eye rehabilitation

For people who have lost an eye entirely, rehabilitation is partly
prosthetic and strongly psychosocial.

- **Early prosthesis fitting improves quality of life.** Reported
  best-practice timing: conformer ~2 months after enucleation/implant,
  ocular prosthesis within ~3 months of the conformer.
  - Case series — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC5379827/>
- **Psychosocial impact is significant.** Prostheses improve confidence
  and social acceptance; eye loss has documented emotional and social
  effects. A longitudinal trial measured quality of life, perceived
  stress, and clinical adaptation in anophthalmic patients.
  - Makrakis 2021, J. Prosthodontics:
    <https://onlinelibrary.wiley.com/doi/abs/10.1111/jopr.13332>
  - "Quality of life living with ocular prosthesis":
    <https://www.tandfonline.com/doi/full/10.1080/17469899.2018.1503534>

**Informs:** the "first 90 days" manual (psychosocial support, what
prosthetic rehabilitation involves); reinforces respectful, person-first
language in [CONTRIBUTING.md](../CONTRIBUTING.md).

---

## 8. Augmented reality and wearable depth aids

Camera-based AR aids are an active research area and directly relevant to
the project's camera-based utilities.

- **AR depth-mapping overlays improve obstacle avoidance.** A depth-to-
  pseudocolor overlay on a HoloLens helped retinitis pigmentosa patients
  navigate a maze and avoid obstacles ~50% better than without the aid. A
  color-mesh overlay preserves true color/texture through gaps (unlike
  full-VR replacement).
  - "Enhanced Depth Navigation Through AR Depth Mapping" — Scientific
    Reports: <https://www.nature.com/articles/s41598-019-47397-w>
  - PMC mirror: <https://pmc.ncbi.nlm.nih.gov/articles/PMC6677879/>
  - USC Ginsburg Institute summary:
    <https://ibt.usc.edu/researchers-usc-ginsburg-institute-biomedical-therapeutics-develop-augmented-reality-glasses-help-low-vision-patients-navigate-environments/>
- **Randomized trials of AR mobility/grasp aids** have been run
  (double-blinded design), signalling the field is maturing past
  proof-of-concept.
- **Caveat:** most studies target low-vision conditions (RP, macular
  degeneration), not uniocular vision specifically. Findings transfer
  partially — uniocular users keep good acuity but lack stereopsis and
  blind-side coverage — so AR aids for them should focus on depth
  rendering and blind-side coverage rather than magnification.

**Informs:** the blind-side-assist and distance-estimator utilities; the
depth-cue rendering module. Highlights a research gap: AR aids designed
specifically for uniocular (vs. low-vision) users.

---

## Identified research gaps

Topics where the project may need to commission, request, or rely on
weaker evidence:

1. **AR/software aids designed for uniocular users specifically** — most
   evidence comes from low-vision populations with different needs.
2. **Effectiveness of depth-cue training** for adults adapting to new
   monocular vision — exercises are widely recommended but rigorous
   outcome data is thin.
3. **Long-term ergonomics of single-eye screen use** — asthenopia
   research rarely isolates uniocular users.
4. **Daily-living task data** (pouring, stairs, thresholds) — much
   guidance is anecdotal; quantified studies are scarce.
