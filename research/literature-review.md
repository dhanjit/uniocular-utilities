# Literature review

A deep-dive annotated bibliography of research relevant to uniocular
people, organized by topic. Each entry summarizes a key finding, links a
source (open-access where available), and notes how it informs the project
[roadmap](../ROADMAP.md).

See [README.md](README.md) for methodology and limitations. This is a
curated review — read the primary sources before relying on a finding.
Findings are summarized in good faith from abstracts and open-access text;
figures are approximate unless quoted.

A longer external AI-generated synthesis (with a proposed Uniocular
Compatibility Standard and a task-difficulty matrix) is kept separately in
[deep-research-synthesis.md](deep-research-synthesis.md); only its
spot-verified findings have been folded into this review.

## Contents

1. [Epidemiology and causes](#1-epidemiology-and-causes)
2. [Adaptation to monocular vision](#2-adaptation-to-monocular-vision)
3. [Depth perception and monocular cues](#3-depth-perception-and-monocular-cues)
4. [Functional impact of stereopsis loss](#4-functional-impact-of-stereopsis-loss)
5. [Driving with monocular vision](#5-driving-with-monocular-vision)
6. [Field-of-view loss and the blind side](#6-field-of-view-loss-and-the-blind-side)
7. [Protecting the remaining eye](#7-protecting-the-remaining-eye)
8. [Eye strain, fatigue, and screen ergonomics](#8-eye-strain-fatigue-and-screen-ergonomics)
9. [Sports and physical activity](#9-sports-and-physical-activity)
10. [Children, amblyopia, and accommodations](#10-children-amblyopia-and-accommodations)
11. [Psychological and social impact](#11-psychological-and-social-impact)
12. [Enucleation and prosthetic rehabilitation](#12-enucleation-and-prosthetic-rehabilitation)
13. [Assistive technology: AR, smart glasses, and AI](#13-assistive-technology-ar-smart-glasses-and-ai)
14. [Standards and accessibility frameworks](#14-standards-and-accessibility-frameworks)
15. [Research gaps](#15-research-gaps)

---

## 1. Epidemiology and causes

Who is uniocular, and why.

- **Trauma is a leading cause of unilateral blindness.** Roughly 30–40% of
  monocular blindness is attributed to ocular trauma, which is the leading
  cause of monocular best-corrected blindness in working-age people, and
  disproportionately affects males.
  - "Ocular Trauma: An Overview" — PMC:
    <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4139697/>
  - "Monocular Precautions" — EyeWiki:
    <https://eyewiki.org/Monocular_Precautions>
- **Disease causes (worse than 20/40 in the better eye)** were reported as
  macular degeneration (~33%), glaucoma (~18%), retinal disease (~15%), and
  diabetic retinopathy (~9%).
- **Global context.** An estimated ~43 million people were blind in 2020
  (Global Burden of Disease analysis); these figures count bilateral
  blindness, but the same disease and injury causes drive unilateral loss.
  - GBD analysis — Lancet Global Health (PMC):
    <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7820390/>

**Informs:** scoping (trauma, age-related disease, and congenital/childhood
causes are all in scope); the "first 90 days" and protection guides.

---

## 2. Adaptation to monocular vision

How people adjust after losing vision in one eye, and how rehabilitation
helps.

- **Adaptation is slower after sudden loss than gradual loss** (reported
  ~8.8 vs. ~3.6 months). In a 65-patient retrospective survey, sequelae
  included depth-perception difficulty, reading strain, and serious
  psychosocial harm — yet ~91% received no formal rehabilitation.
  - Kraut & Lopez-Fernandez, *International Ophthalmology Clinics*, 2002 —
    PubMed: <https://pubmed.ncbi.nlm.nih.gov/12131596/>
  - "Vision Rehabilitation Team Management of Acquired Monocular Vision":
    <https://www.researchgate.net/publication/235522108>
- **Structured rehabilitation programs exist** (e.g. the VA Acquired
  Monocular Vision Rehabilitation program): home adaptive skills and
  mobility training to compensate for reduced field and depth loss.
  - <https://www.rehab.research.va.gov/jour/07/44/4/ihrig.html>
- **Balance leans on the remaining two systems.** Balance is controlled by
  vestibular, somatosensory, and visual systems; losing visual input
  forces compensation. Visual-skills training (fixation, scanning,
  pursuit, saccades) helps.
  - "Physical Therapy and Monocular Vision Loss":
    <https://tlc-pt.com/wp-content/uploads/sites/6/2024/06/Physical-Therapy-and-Monocular-Vision-Loss.pdf>
  - Lighthouse Guild overview:
    <https://lighthouseguild.org/monocular-vision-etiology-symptoms-and-rehabilitation-2/>

**Informs:** the "first 90 days" / "how to live with one eye" manuals
(adaptation timeline, expectations); daily-living and mobility guides.

---

## 3. Depth perception and monocular cues

Uniocular people lose stereopsis but retain monocular depth cues. Motion
parallax — driven by head movement — is the most powerful.

- **Motion parallax needs translational head/body movement.** Depth comes
  from side-to-side motion, not rotation; the visual system uses the
  smooth-pursuit eye-movement signal to resolve depth-sign.
  - "Modeling depth from motion parallax with the motion/pursuit ratio" —
    PMC: <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4186274/>
  - "Visual Depth from Motion Parallax and Eye Pursuit" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC3348271/>
  - "Motion parallax driven by head movements" — PubMed:
    <https://pubmed.ncbi.nlm.nih.gov/15943054/>
- **One-eyed people regain functional depth by keeping the head in motion**
  — often unconsciously (shifting the head when parking or pouring). But
  parallax does not fully replace binocular vision: in some visuomotor
  tasks head movement gave no measurable advantage.
- **Parallax can augment other cues.** In macular degeneration, motion
  parallax augmented disparity for depth perception — evidence that
  training cue-combination is worthwhile.
  - <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12849822/>
- **The Pulfrich effect is a hazard for some monocular-ish conditions.**
  When the two eyes differ in brightness/contrast (e.g. monovision, a
  dim/blurred eye), the brain processes the darker image more slowly,
  creating a false sense of motion in depth — relevant to driving. Studies
  found little neural adaptation to small-aperture monovision Pulfrich.
  - "Small-Aperture Monovision and the Pulfrich Experience" — PMC:
    <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3796532/>
  - Reverse Pulfrich after cataract surgery — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC10290313/>
- **The monocular cue set** (relative size, occlusion, shadow/shading,
  texture gradient, aerial perspective, linear perspective) is teachable.
  - Hanover College interactive demos:
    <https://isle.hanover.edu/isle2/Ch07DepthSize/Ch07MonocDepthInv_evt.html>

**Informs:** the depth-cue trainer utility (motion-parallax exercises,
head-movement habits); the depth-cue rendering module; accessibility
guidance on reinforcing depth with monocular cues. Note the Pulfrich
caveat for anyone with *partial* vision in the second eye, not full
monocularity.

---

## 4. Functional impact of stereopsis loss

How much does losing stereo vision actually cost, and at what tasks?

- **Stereopsis helps most for fine motor tasks under direct vision.**
  Stereo-normal participants outperformed stereo-absent ones on a fine
  motor task viewed directly; depth-related errors were significantly
  higher without stereo, while *lateral* errors did not differ.
  - "Drilling into the functional significance of stereopsis" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC5519940/>
- **2D viewing neutralizes the stereo advantage.** Under video-assisted /
  2D conditions (e.g. laparoscopic surgery on a monitor), stereopsis
  confers little advantage — a key insight: tasks mediated by a 2D screen
  are relatively fair for uniocular people.
  - "Effects of absence of stereopsis on a simulated surgical task" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC4316921/>
- **Compensation is possible but costs cognitive effort.** Adaptations
  relying on monocular cues are typically less precise and require more
  processing, potentially slowing reaction times.

**Informs:** realistic framing in manuals (which tasks are genuinely
harder vs. which are unaffected); the case for routing depth-critical work
through 2D representations where possible.

---

## 5. Driving with monocular vision

Mixed evidence; the distinction between sudden monocularity and stable,
adapted monocular vision matters.

- **Sudden monocular condition sharply degrades performance.** Racing-
  driver study: under a sudden monocular condition drivers were 2.1–6.5x
  more likely to collide, with reaction-time increases of ~64–126 ms. A
  sudden monocular *reduction* in vision with the peripheral field
  preserved did **not** impair performance — the field loss/monocularity
  itself is the issue.
  - PLOS One (open access):
    <https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0226308>
  - PMC mirror: <https://pmc.ncbi.nlm.nih.gov/articles/PMC6913915/>
- **Population studies conflict.** Commercial-driver research reports mixed
  results — some find more crashes/convictions among monocular drivers,
  others find equivalent rates. Many jurisdictions screen with both eyes
  or the better-seeing eye.
  - "Vision and Driving" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC2975746/>
- **Takeaway:** adaptation time matters. The Pulfrich effect (§3) is an
  additional, specific driving hazard for people with unequal eyes.

**Informs:** the driving guide (adaptation period, mirror setup, scanning,
"check local law" framing). The project must avoid blanket
fitness-to-drive or legal advice.

---

## 6. Field-of-view loss and the blind side

Uniocular vision and hemianopic field loss share a problem: a region where
hazards go undetected. Hemianopia research transfers usefully.

- **Compensatory scanning is the core behavioral strategy.** Training a
  large blind-side scan helps detect hazards; a minimum scan magnitude can
  serve as a training criterion or assistive-technology target.
  - "Driving With Hemianopia VII" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC7804568/>
- **Prism-based optical aids expand blind-side awareness.** Peripheral
  prisms (e.g. Peli Lens) shift images from the blind region into the
  seeing field. Peli's **multiplexing prism** superimposes a shifted view
  to expand the field by ~20–43° (design-dependent) *without* an apical
  scotoma, and is being trialled specifically for monocular vision.
  - Peli, "Multiplexing Prisms for Field Expansion", *Optometry and Vision
    Science*, 2017 — PMC: <https://pmc.ncbi.nlm.nih.gov/articles/PMC5542858/>
  - Multiplexing-prism field-expansion trial for **monocular** vision:
    <https://clinicaltrials.gov/study/NCT06027216>
  - Peripheral prism trial: <https://clinicaltrials.gov/study/NCT00494676>
  - Multi-periscopic prism trial: <https://clinicaltrials.gov/study/NCT04827147>
- **Electronic collision-warning devices** warn of mid/high obstacles a
  long cane would miss.
  - <https://clinicaltrials.gov/study/NCT03057496>
- **Overlay/AR approaches** can integrate information to increase the
  effective field of view.
  - "Visual Field Loss: Integrating Overlayed Information" — MDPI Vision:
    <https://www.mdpi.com/2411-5150/6/4/67>

**Informs:** the blind-side-assist utility (collision warning, scan
prompts); the alerting module; scanning-habit manuals. Prism optics are
reference material, not something the project builds.

---

## 7. Protecting the remaining eye

The single most consequential safety topic: a uniocular person's remaining
eye is irreplaceable, so injury prevention is paramount.

- **Polycarbonate lenses, worn at all times.** Clinicians counsel monocular
  patients to wear polycarbonate glasses at all times, even at home;
  polycarbonate resists shattering and adds UV protection. Prescriptions
  should specify polycarbonate; non-prescription clear polycarbonate is an
  option for those who don't need correction. Keep a spare pair.
  - "Monocular Precautions" — EyeWiki:
    <https://eyewiki.org/Monocular_Precautions>
  - OcularPro overview: <https://ocularpro.com/protection-for-remaining-vision/>
  - AAO, protective eyewear:
    <https://www.aao.org/eye-health/symptoms/injuries-protective-eyewear>
- **Sports and high-risk activities require rated protection.** Functionally
  one-eyed athletes (best-corrected acuity worse than 20/40 in the poorer
  eye) should always wear sports-rated polycarbonate eye protection, avoid
  boxing and full-contact martial arts, and may need to avoid the highest-
  risk sports.
  - AAO clinical statement, "Protective Eyewear for Young Athletes":
    <https://www.aao.org/education/clinical-statement/protective-eyewear-young-athletes>
- **Compliance is a real problem, and the barriers are psychosocial.** In a
  132-patient anophthalmic study, prior glasses-wearers complied ~79.7% of
  the time, while ~67.1% of prior non-wearers did not comply; reasons for
  non-compliance were "lack of concern" (43%), aesthetics (26%), and feeling
  it unnecessary because acuity was already sharp (17%). Compliance
  correlated significantly with the number of clinical encounters —
  repeated structured counseling is the main proven lever.
  - Neimkin & Custer, *Ophthalmic Plastic & Reconstructive Surgery*, 2017 —
    PMC: <https://pmc.ncbi.nlm.nih.gov/articles/PMC4980283/>
- **Pediatric compliance is higher but still imperfect.** In one study of
  functionally one-eyed children, only ~35% wore safety glasses ≥90% of the
  day while ~34% rarely or never did; barriers were discomfort, appearance,
  and lens-induced vision reduction.
  - "Protective eyewear in children with one eye vision loss" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC12238169/>
  - Childhood Eye Cancer Trust guidance:
    <https://chect.org.uk/protective-eyewear-for-children-with-monocular-vision/>

**Informs:** a high-priority protection guide (likely the most impactful
manual); design of any reminder/habit tooling; tone that takes compliance
barriers seriously rather than just prescribing.

---

## 8. Eye strain, fatigue, and screen ergonomics

The single working eye does all the visual work; managing fatigue and
screen setup matters.

- **Asthenopia is highly prevalent and tied to sustained near work.**
  Symptoms: eye tiredness, strain, blurred vision, headache, occasional
  double vision. A systematic review reported pooled prevalence of eye
  tiredness ~65% and strain/fatigue ~47%. Unequal refractive error between
  the eyes is itself a contributor.
  - Systematic review & meta-analysis — JOGH:
    <https://jogh.org/2026/jogh-16-04053/>
  - EyeWiki: <https://eyewiki.org/Asthenopia>
- **The 20–20–20 rule** (every 20 min, look ~20 ft away for 20 s) is a
  research-supported, low-cost mitigation; structured breaks reduce strain.
- **Monitor ergonomics.** Screen at roughly arm's length (~20–30 in), top
  of screen at or slightly below eye level. For multi-monitor setups,
  center the primary monitor directly ahead. Lower brightness, larger
  fonts, and higher contrast reduce strain.
  - OHCOW office-ergonomics guide:
    <https://www.ohcow.on.ca/office-ergonomics-reference-guide/computer-screens-monitors/>
  - Ergonomics Plus monitor checklist:
    <https://ergo-plus.com/office-ergonomics-position-computer-monitor/>

**Informs:** the eye-strain-manager utility (20-20-20 timer, contrast/
reading presets); a screens-and-computing guide within "how to live with
one eye"; accessibility guideline 4.x (break reminders, contrast, text
size).

---

## 9. Sports and physical activity

Fast-moving-ball sports are hardest, but participation is achievable with
adaptation and protection.

- **Tracking fast objects is the core challenge.** Loss of binocular vision
  makes judging a moving ball's position harder; tennis, squash, baseball,
  and cricket are demanding. Yet competitive play is documented (e.g. A-
  grade squash players with one eye).
  - "Sport with an Artificial Eye":
    <https://artificialeyes.net/adjusting-to-eye-loss-mind-map/eye-loss-sports/>
  - AAO "Sports & Vision":
    <https://www.aao.org/museum/exhibition-detail/sports-vision>
- **Elite ball-sport performance does not require perfect stereo vision.**
  A 59-athlete study (cricketers, rugby-league players) found ~27% had
  sub-optimal habitual on-field vision (mostly uncorrected refractive
  error); only elite cricketers exceeded stereoacuity norms. Compensation
  likely leans on *looming* (retinal-image expansion) and relative size
  more than stereopsis. Notable elite athletes have adapted (e.g. cricketer
  Hanif Mohammad with a squint).
  - Barrett et al., *Sports Medicine - Open*, 2017 (open access) — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC5681452/>
- **Protection is non-negotiable** for functionally one-eyed athletes (see
  §7).

**Informs:** a sports-and-hobbies guide; cross-links to the protection
guide; realistic, encouraging framing.

---

## 10. Children, amblyopia, and accommodations

Amblyopia is the most common cause of functional monocular vision and has
measurable effects on everyday function.

- **Prevalence and impact.** Amblyopia affects up to ~4% of children and
  often persists into adulthood, interfering with contrast sensitivity,
  attention, reading, eye–hand coordination, physical activity, and HRQoL.
  - "Amblyopia and the whole child" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC9998377/>
  - "Functional consequences of amblyopia and its impact on HRQoL" —
    PubMed: <https://pubmed.ncbi.nlm.nih.gov/40319624/>
  - StatPearls: <https://www.ncbi.nlm.nih.gov/books/NBK430890/>
- **Reading is measurably slower** (~28–32% slower than peers; ~148 vs.
  ~204 wpm in one report).
- **Treatment outcome is age-dependent.** Spectacles alone yield full
  acuity recovery in ~32% under age 7, ~14% at 7–12, ~11% at 13–17;
  occlusion therapy improves ≥~75% of treated children, though recurrence
  is possible. Patching affects children's quality of life during
  treatment.
  - <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8951718/>
- **Long-term social outcomes may be reassuring** (a 1958 British cohort
  found no mid-adulthood differences in education/health/social outcomes).
- **School and sports accommodations.** Functionally one-eyed children need
  sports-rated polycarbonate protection at all times and should avoid the
  highest-risk sports; compliance is a known challenge (§7).

**Informs:** a children/families manual; reading-aid features; supportive,
non-deficit design tone.

---

## 11. Psychological and social impact

Vision loss is not only a sensory event; adjustment is psychological.

- **Elevated depression and anxiety.** Adults with visual impairment are
  roughly twice as likely to experience depression; ~1 in 4 adults with
  vision loss report anxiety or depression (CDC). Sight loss is linked to
  increased suicide risk.
  - "Visual Impairment and Mental Health: Unmet Needs" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC7721280/>
  - "Psychiatric disorders linked to visual impairment" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC12836230/>
- **The relationship is bidirectional** — stress/anxiety can worsen
  perceived vision, creating a negative spiral.
- **Acceptance and social support improve adjustment** to irreversible
  vision loss; identity and self-concept are affected.

**Informs:** the "first 90 days" manual (a frank, supportive section on
emotional adjustment and when to seek help); tone across all content;
signposting to mental-health resources. Not a substitute for clinical
care.

---

## 12. Enucleation and prosthetic rehabilitation

For people who have lost an eye entirely, rehabilitation is partly
prosthetic and strongly psychosocial.

- **Early prosthesis fitting improves quality of life** (reported timing:
  conformer ~2 months post-enucleation/implant; prosthesis within ~3
  months of the conformer).
  - Case series — PMC: <https://pmc.ncbi.nlm.nih.gov/articles/PMC5379827/>
- **Psychosocial impact is significant.** Prostheses improve confidence and
  social acceptance; a longitudinal trial measured quality of life,
  perceived stress, and clinical adaptation in anophthalmic patients.
  - Makrakis 2021, J. Prosthodontics:
    <https://onlinelibrary.wiley.com/doi/abs/10.1111/jopr.13332>
  - "Quality of life living with ocular prosthesis":
    <https://www.tandfonline.com/doi/full/10.1080/17469899.2018.1503534>

**Informs:** the "first 90 days" manual (what prosthetic rehab involves,
psychosocial support); reinforces person-first language.

---

## 13. Assistive technology: AR, smart glasses, and AI

Camera-based AR and AI wearables are advancing fast and are central to the
"AI-future" direction for this project.

- **AR depth-mapping overlays improve obstacle avoidance.** A depth-to-
  pseudocolor overlay on a HoloLens helped retinitis pigmentosa patients
  navigate and avoid obstacles ~50% better. A color-mesh overlay preserves
  true color/texture (unlike full-VR replacement).
  - "Enhanced Depth Navigation Through AR Depth Mapping" — Scientific
    Reports: <https://www.nature.com/articles/s41598-019-47397-w>
  - PMC mirror: <https://pmc.ncbi.nlm.nih.gov/articles/PMC6677879/>
- **Mainstream AI smart glasses are now consumer reality (2025).** Meta
  Ray-Ban (Gen 2, ~8 hr battery; Display variant with in-lens screen) were
  *not* designed for low-vision users but provide useful hands-free AI
  description tasks at a ~$300 entry point.
  - AFB AccessWorld review:
    <https://afb.org/aw/fall2025/meta-glasses-review>
  - Meta accessibility page:
    <https://www.meta.com/ai-glasses/blind-visually-impaired/>
- **Purpose-built assistive glasses exist.** Envision Glasses (~$800+)
  offer text reading, scene/image description, document scanning, and face
  recognition; the Ally Solos glasses (Envision, launched Oct 2025) bring
  real-time AI description.
  - SpecialNeeds comparison:
    <https://www.specialneeds.com/articles/assistive-tech/vision/smart-glasses-for-vision-impairment-in-2025-meta-ray-ban-vs-envision-vs-specialized-options/>
  - "Meta smart glasses—LLMs and the future for assistive glasses" — PMC:
    <https://pmc.ncbi.nlm.nih.gov/articles/PMC11009354/>
- **Caveat:** most assistive-tech evidence targets *low-vision/blind*
  users (RP, macular degeneration), not uniocular users specifically.
  Uniocular users keep good acuity but lack stereopsis and blind-side
  coverage — so the high-value AI/AR features for them are *depth
  rendering, distance cues, and blind-side coverage*, not magnification or
  full scene narration. This is a clear design opening.

**Informs:** the blind-side-assist and distance-estimator utilities; the
depth-cue rendering module; the "smart glasses & AI" chapter of "how to
live with one eye". Flags a research/product gap (uniocular-specific AI
aids).

---

## 14. Standards and accessibility frameworks

Existing frameworks to build on for a Uniocular Compatibility Standard
(see [roadmap](../ROADMAP.md)).

- **W3C XR Accessibility User Requirements (XAUR, 2020)** — ~18–19 user
  needs for accessible XR/VR, published by the W3C APA Working Group. A
  natural anchor for requirements about monoscopic modes and depth.
  - <https://w3c.github.io/xaur/>
- **Game Accessibility Guidelines** and **Virtual Environments
  Accessibility Guidelines** — community standards for 3D worlds.
  - VR-games accessibility synthesis — Frontiers:
    <https://www.frontiersin.org/journals/virtual-reality/articles/10.3389/frvir.2021.697504/full>
- **Adoption is hard.** Research notes no systematic study of how XR
  practitioners interpret these guidelines, which hinders adoption — an
  argument for a *concise, testable, certifiable* standard rather than a
  long advisory document.
  - "How Well Can 3D Accessibility Guidelines Support XR Development?" —
    arXiv: <https://arxiv.org/abs/2602.17939>
- **WCAG** remains the baseline for non-immersive UI; the project's
  [accessibility guidelines](../specifications/accessibility-guidelines.md)
  reference WCAG AA for contrast and text.

**Informs:** the Uniocular Compatibility Standard — borrow XAUR's
user-needs framing and WCAG's testable-criteria + conformance-levels
model; keep it short and certifiable to maximize adoption.

---

## 15. Research gaps

Where evidence is thin and the project may need to commission research,
rely on weaker evidence, or fund primary work:

1. **Uniocular-specific AI/AR aids.** Almost all assistive-tech evidence
   comes from low-vision/blind populations with different needs. No strong
   evidence base for AI/AR aids tuned to uniocular users (good acuity, no
   stereopsis, blind side).
2. **Effectiveness of depth-cue training** for adults adapting to new
   monocular vision — widely recommended, but rigorous outcome data is
   thin.
3. **Long-term ergonomics of single-eye screen use** — asthenopia research
   rarely isolates uniocular users.
4. **Quantified daily-living task data** (pouring, stairs, thresholds) —
   much guidance is anecdotal.
5. **Protective-eyewear compliance interventions** — the problem is well
   documented (§7) but effective behavior-change strategies are not.
6. **A conformance methodology for uniocular compatibility** — no existing
   standard certifies products as uniocular-compatible (§14).
