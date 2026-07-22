# Competitive & Improvement Analysis — `patient-advocate-research-primer`

*Analyst: Hee-Lee Oss research agent · Date: 2026-06-29 · Source plan: `scratchpad/plans/patient-advocate-research-primer/PLAN.md` (Draft v0.1.0)*

This is an unusually mature plan: the licence/provenance gate, the medium-vs-high split risk
tier, the dual oncologist+advocate sign-off, and the honest `verifiedNeed:false` / TO BE SECURED
discipline are all already in place. The findings below are therefore mostly *sharpening* a strong
draft, not rescuing a weak one. The single biggest substantive gap is that the plan reinvents an
evidence-literacy framework from scratch while a CC-BY, peer-reviewed, oncology-validated framework
(IHC Key Concepts) already exists and would both strengthen accuracy and slot cleanly under the
licence gate.

---

## 1. Correctness & completeness review of PLAN.md

**Evidence-evaluation content — accuracy of the substance.** The methodological spine is correct
and well-chosen: study classification (design/phase/arm/blinding/randomisation), placement on an
evidence hierarchy, endpoints (OS vs PFS vs ORR vs surrogate/biomarker), effect size and precision
(HR, CI, absolute vs relative risk, NNT), bias, confounding, COI, reproducibility, and "press
release vs paper." This is the right curriculum and it is pitched at the right targets. Specific
correctness notes and gaps:

- **The evidence hierarchy is the single most error-prone topic to teach, and the plan does not yet
  signal awareness of the nuance.** A naïve "pyramid" (RCT > cohort > case-control > case series)
  is exactly the over-simplification that modern EBM has spent 15 years correcting: GRADE rates the
  *body of evidence per outcome* and lets an RCT be rated *down* (risk of bias, imprecision,
  indirectness, inconsistency, publication bias) and observational evidence rated *up* (large
  effect, dose-response). An advocate taught "RCT = top, therefore trust it" has been mis-trained.
  **Recommendation:** teach the hierarchy as "a starting prior that GRADE then adjusts," not a fixed
  ranking. This is a correctness issue, not a polish issue.
- **The over-skepticism / credulity balance is named as a risk (good) but has no pedagogical
  mechanism.** The plan's worked-examples and worksheets teach *appraisal* (finding weaknesses),
  which structurally biases learners toward skepticism — the classic failure mode where a newly
  trained advocate dismisses *all* observational evidence or treats every limitation as fatal. There
  is no counterweight teaching *when evidence is good enough to act on*, *why we can't always have an
  RCT*, or *proportionality of critique*. Add an explicit "calibrated, not cynical" module and bake a
  "what would change your mind / what is this study legitimately good for" prompt into every
  worksheet.
- **Statistics module scope is right but high-risk for subtle error.** p-values "and their misuse,"
  absolute vs relative risk, and NNT are the correct priorities (these are where headlines mislead).
  Two common teaching errors to pre-empt in the style guide: (a) defining a 95% CI as "95% probability
  the true value lies in this range" (wrong frequentist interpretation — a recurring textbook error),
  and (b) conflating "not statistically significant" with "no effect." Flag both as named landmines
  for the methodology reviewer.
- **Surrogate-endpoint treatment is a genuine strength** and correctly placed — PFS/ORR vs OS is
  precisely where oncology hype and regulatory controversy live, and FDA/EMA endpoint guidance is the
  right authority to anchor it.

**The "not medical advice" boundary.** Well-engineered: persistent banner, advice-language linter
(D-5), dual high-tier sign-off, refusal scope, and "teaches method, renders no verdicts." Residual
risks the plan under-addresses:

- The boundary is hardest *inside a walkthrough*. The moment you appraise a real cancer drug's trial
  and conclude "the OS benefit is unproven," an advocate reading about that drug for a relative hears
  treatment guidance, regardless of the banner. **Mitigation:** prefer walkthrough papers that are
  methodologically instructive but *therapeutically low-salience* (older, settled, or
  non-decision-driving questions), and add an explicit "this is a method demonstration, not an
  assessment of whether this treatment works for anyone" unit-level frame.
- The linter is described as catching second-person prescriptive language. It will miss the subtler
  drift: *implied* prescription via selective emphasis (appraising only the harms of one option).
  This needs the advocate reviewer, not the linter — make that explicit in the review checklist.

**Advocate co-design.** Named (advocate reviewer "ideally co-designs") but weak as specified —
co-design is listed as a *review* role at the *end*, which is review, not co-design. Genuine
co-design means advocates shape scope, examples, and sequencing *before* authoring. This is also the
plan's strongest differentiator (see §4) and is currently underbuilt. Elevate at least one advocate
from reviewer to co-author from M0.

**Sourcing / provenance.** Excellent and arguably best-in-class for this space: source register as
a CI gate, per-assertion citation, per-article OA licence verification with an `allowedUse` field,
re-verification cadence. One gap: the plan cites authorities (Cochrane, GRADE, EQUATOR, FDA) but does
not yet adopt the one *open-licensed, learner-facing* framework purpose-built for this audience —
**IHC Key Concepts (CC-BY)** — which would reduce original-authoring risk *and* give the curriculum
an externally-validated backbone. This is the headline §1 finding.

**Assessment.** The pre/post appraisal rubric and validated confidence survey are good, but the plan
asserts a "validated PPI confidence survey" without naming an instrument, and proposes a bespoke
100-pt appraisal rubric whose own validity is unestablished. A bespoke rubric measuring a bespoke
curriculum risks construct-circularity. Anchor to an existing validated instrument where one exists
(e.g. adapt items from the "Claim Evaluation Tools" database from the IHC project, which is built and
validated for exactly this) and have the methodology reviewer sign off the rubric itself.

**Accessibility.** Strong — WCAG 2.1 AA, readability scoring, printable/offline, plain-language as a
first-class outcome metric. Suggest naming a concrete readability target band and acknowledging the
tension that some terms (hazard ratio, confidence interval) cannot be made simple, only *explained*
simply — a glossary-anchored "plain explanation, not dumbing down" standard.

**Scope vs siblings.** The non-goals fence off trial-finding and verdict-rendering cleanly. The
boundary with the sibling projects (`oncology-data-literacy`, `stats-for-clinicians`) is the main
ambiguity. "Statistics-for-appraisal (HR/CI/absolute-vs-relative/NNT/p-values)" overlaps heavily
with what a `stats-for-clinicians` project and an `oncology-data-literacy` project would teach. The
plan should state the dividing line explicitly: this primer teaches the *consumer's* appraisal
statistics (interpreting a reported HR), `stats-for-clinicians` teaches the *producer's* statistics
(choosing/computing it), and `oncology-data-literacy` teaches *data/registry* literacy (not
literature appraisal). Add a one-paragraph "relationship to sibling projects" subsection and a shared
glossary to avoid divergence and duplicated review burden.

**Completeness — present and correct:** all 17 H2 sections; risk tiers; cancer guardrails; honest
unsecured-partner discipline; beneficiary-centric metrics; COI/recusal; sustainability/forkability.
**Missing/thin:** (a) IHC framework adoption; (b) a "calibration vs cynicism" pedagogical mechanism;
(c) GRADE-nuanced hierarchy framing; (d) named assessment instrument; (e) sibling-boundary
subsection; (f) co-design depth.

---

## 2. Competitive landscape

This is a *crowded* space for cohort-based, application-gated training and a *near-empty* space for
open, self-serve, source-cited primers. That asymmetry is the whole opportunity.

**Cancer research-advocacy training (cohort/institutional):**

- **NBCC Project LEAD — the gold standard.** Six-day intensive; cancer biology, genetics,
  epidemiology, research design, advocacy; renowned faculty; competitive selection; no tuition;
  2,500+ graduates. *Strengths:* depth, rigor, reputation, alumni network, real influence on study
  sections and policy. *Weaknesses for our purposes:* breast-cancer-centric; in-person, cohort-gated,
  capacity-limited (you must be selected and travel); not a self-serve reusable artifact; curriculum
  not openly licensed/forkable; no public critical-appraisal worksheet set you can pick up tonight.
  https://www.stopbreastcancer.org/what-we-do/education/project-lead/ ;
  https://pmc.ncbi.nlm.nih.gov/articles/PMC2794400/
- **AACR Scientist↔Survivor Program.** 28+ years; plain-language lectures + mentor pairing +
  capstone at the Annual Meeting. *Strengths:* scientist-advocate relationships, mentorship, prestige,
  cross-cancer. *Weaknesses:* event-bound, selective, relationship-driven rather than a durable
  open curriculum; nothing to self-study or fork.
  https://www.aacr.org/patients-caregivers/patient-advocacy/scientist-survivor-program/
- **Research Advocacy Network (Advocate Institute).** Closest analogue: free publications/tutorials
  explaining the research system and scientific concepts for advocates; 2,500+ trained; partners with
  Mayo, ECOG-ACRIN, Conquer Cancer/ASCO. *Strengths:* free, advocate-specific, established partners,
  print+download resources. *Weaknesses:* materials are explanatory/orientation-oriented rather than a
  structured *critical-appraisal skills* curriculum with worksheets + worked OA-paper walkthroughs;
  not openly licensed for fork/translation as far as published; appears lightly maintained.
  https://www.researchadvocacy.org/ ; https://www.researchadvocacy.org/organizations
- **ASCO / NCI CCCT Patient Advocate Steering Committee (PASC) / NCI CARRA.** Institutional pipelines
  defining advocate competencies and integrating advocates into trial design. *Strengths:* authority,
  real seats at the table, defined competency frameworks (the PASC's four competency domains are a
  useful external reference for our learning objectives). *Weaknesses:* internal, role-specific, not a
  public open curriculum; explicitly flagged (2017 NCTN evaluation) as *needing more advocate
  training* — i.e. an admitted gap we can help fill.
  https://www.cancer.gov/about-nci/organization/ccct/steering-committees/patient-advocate ;
  https://pmc.ncbi.nlm.nih.gov/articles/PMC9360467/ ; https://ascopubs.org/doi/10.1200/EDBK_100035

**General evidence-literacy / critical-appraisal (open, cross-disease):**

- **Testing Treatments interactive / James Lind Library.** Free full-text book + essays on "fair
  tests of treatments" for lay audiences; multi-format (PDF/audio/hypertext), multilingual.
  *Strengths:* superb plain-language pedagogy, public-facing, free, trusted lineage (Chalmers et al.),
  some reuse-friendly. *Weaknesses:* general medicine not oncology; book/essay form, not worksheets
  or appraisal toolkits; not tied to advocate research-panel roles; no oncology worked examples.
  https://en.testingtreatments.org/ ; https://www.jameslindlibrary.org/
- **Informed Health Choices (IHC) Key Concepts + Claim Evaluation Tools.** A peer-reviewed,
  **CC-BY**, 49-concept framework for judging treatment claims, *plus* a validated item bank for
  measuring those skills; there is even a published protocol prioritising IHC Key Concepts
  *specifically for people impacted by cancer*. *Strengths:* the only openly-licensed, validated,
  learner-facing backbone in this space; directly adoptable under our licence gate; comes with
  assessment instruments. *Weaknesses:* abstract/general, not oncology-contextualised, not
  advocate-role-shaped, no worked oncology papers — exactly the contextualisation layer we would add.
  https://f1000research.com/articles/7-1784 ; https://hrbopenresearch.org/articles/5-55 ;
  https://pmc.ncbi.nlm.nih.gov/articles/PMC7670481/
- **Students 4 Best Evidence (Cochrane).** Free blog/tutorial network; "how to do critical
  appraisal," 20-question checklist, the 34 key-concepts series. *Strengths:* free, approachable,
  Cochrane-backed. *Weaknesses:* student/clinician audience, blog-fragmented (not a sequenced
  curriculum), general not oncology, not advocate-role-oriented.
  https://s4be.cochrane.org/
- **Cochrane Consumer Network + Evidence Essentials.** Five interactive modules (EBM, RCTs,
  systematic reviews, using reviews, consumer involvement), co-created with patients; CCNet ~1,500+
  consumers; new critical-appraisal module. *Strengths:* consumer-written, free, authoritative,
  co-designed with patients — a model for our co-design claim. *Weaknesses:* systematic-review-centric,
  general medicine, oriented to involvement-in-Cochrane rather than appraising oncology trials;
  licensing for fork/adaptation not clearly open.
  https://consumers.cochrane.org/resources ; training.cochrane.org/online-learning/consumer-involvement
- **Sense About Science.** Public campaigns and guides (e.g. "Making Sense of …", "Ask for
  Evidence") promoting evidence literacy. *Strengths:* communication craft, public trust, plain
  language. *Weaknesses:* campaign/guide form, not a skills curriculum, general not oncology, not
  advocate-role-specific.
- **PCORI Research Fundamentals / engagement resources.** Free, plain-language, self-paced training
  on patient-centered outcomes research; engagement rubric; data-interpretation guide. *Strengths:*
  free, self-serve, plain language, partner-respected, US-funded credibility. *Weaknesses:* about
  *engaging in* PCOR and partnership process, not about *appraising the literature*; methods-standards
  curriculum is academic; not oncology-specific.
  https://www.pcori.org/engagement-research/engagement-resources

**Landscape verdict.** The cancer-specific players (LEAD, SSP, RAN, NCI/ASCO) own *cohort and
institutional* training but offer no open, self-serve, forkable critical-appraisal toolkit. The open
players (Testing Treatments, IHC, S4BE, Cochrane Consumer, PCORI) own *general* evidence literacy but
none is *oncology-contextualised with worked OA cancer papers and advocate-role framing*. No single
incumbent occupies the intersection this project targets.

---

## 3. Gaps we can fill

1. **The self-serve gap.** Every cancer-specific competitor is application-gated, cohort-based, or
   event-bound. An advocate appointed to a study section *next week* cannot get into Project LEAD in
   time. A free, open, do-it-tonight primer fills a real timing/access gap.
2. **The "worked oncology paper" gap.** No open resource walks an advocate through appraising a *real
   open-access oncology trial* end-to-end, keyed to a reusable worksheet. Testing Treatments is
   general; IHC is abstract; LEAD's materials are not public. This is the project's most defensible,
   hardest-to-copy asset.
3. **The forkable/translatable gap.** None of the cancer-specific curricula are openly licensed for
   adaptation, translation, or reuse by other disease communities. CC-BY content + a documented source
   register makes ours the one a sarcoma, leukemia, or rare-disease group can fork.
4. **The oncology-endpoint-literacy gap.** OS vs PFS vs ORR vs surrogate is *the* oncology-specific
   appraisal skill and the one most exploited by hype; general resources barely touch it.
5. **The provenance-transparency gap.** A learner-facing resource where *every claim resolves to a
   cited, licence-verified source* is rare. That transparency is itself a teaching artifact (it models
   the behaviour it teaches) and a trust differentiator.
6. **The "calibration" gap.** Most appraisal training teaches fault-finding; few teach *when evidence
   is good enough to act on*. A primer that explicitly trains calibrated confidence (not reflexive
   skepticism) fills a pedagogical gap the incumbents leave open.
7. **The role-contextualised gap.** "You are on a study section / DSMB / PFAC — here is what to ask"
   framing connects appraisal skills to the advocate's *actual seat*, which general EBM resources
   never do.

---

## 4. Differentiators to win (incl. vs NBCC Project LEAD)

- **Open, free, self-serve, and forkable** vs LEAD/SSP's selective, in-person, capacity-limited
  cohorts. We don't compete with LEAD's depth or network — we complement it by reaching the ~99% of
  advocates who will never get a LEAD seat, and by being available the day an advocate is appointed.
  Position explicitly as "the open on-ramp and reference companion to LEAD/SSP," not a rival. (A LEAD
  alumnus or RAN as a partner would be a credibility coup, not a conflict.)
- **Oncology-contextualised worked examples on real OA papers** — the asset none of the open
  competitors (Testing Treatments, IHC, S4BE, Cochrane Consumer, PCORI) have and none of the
  cancer-specific players publish openly. This is the strongest single differentiator.
- **Provenance-as-a-feature.** Every assertion source-cited and licence-verified, enforced in CI. No
  competitor ships this; it doubles as a trust signal and a worked example of the appraisal mindset.
- **Calibrated-not-cynical pedagogy.** An explicit stance against the over-skepticism failure mode
  that fault-finding curricula induce — a teachable, differentiated philosophy.
- **Standards-anchored, not invented.** Building the spine on the CC-BY IHC Key Concepts framework
  (validated, oncology-prioritisation already published) lets us claim external validity LEAD's
  bespoke curriculum cannot, while remaining fully open.
- **Genuine advocate co-design + dual expert sign-off** as a published, auditable process (review
  ledger) — matches Cochrane Consumer's co-design credibility while exceeding its transparency.
- **Role-aware framing** (study section / DSMB / IRB / PFAC) that maps skills to the seat — neither
  the general nor the cancer-specific incumbents do this in an open artifact.

---

## 5. Claude API leverage

**Where Claude adds real leverage (all human-/expert-gated):**

- **Drafting plain-language modules from authoritative sources.** Claude can turn Cochrane/GRADE/
  EQUATOR/FDA-endpoint guidance and the IHC Key Concepts into advocate-pitched first drafts at a
  target readability band, with per-claim source placeholders the author/steward then verifies. Big
  time-saver on the bulk authoring in M1–M2.
- **Generating worked-example critique drafts on licence-verified OA papers.** Given an
  OA-licence-cleared paper, Claude can draft a structured first-pass appraisal (design, endpoints,
  effect size + precision, bias, COI, spin) keyed to a worksheet — the most labor-intensive
  deliverable. Human methodology + oncology review is mandatory before publish.
- **Authoring original critical-appraisal worksheets from first principles** (concept-level, not
  copying CASP/JBI expression) — Claude is well-suited to drafting question sets per study type that
  the licence steward confirms are clean-room original.
- **Practice critiques / formative feedback generator.** Claude can produce *practice* appraisal
  scenarios and model answers, and (carefully, non-authoritatively) give learners feedback on their
  worksheet attempts — high pedagogical value, framed as practice not assessment.
- **Plain-language glossary drafting + readability passes + "spot the spin" exercise generation** from
  real (cleared) abstracts vs their press releases.
- **The advice-language linter itself** can be Claude-backed: flag prescriptive/second-person/
  individualised-guidance drift in PRs more flexibly than regex (D-5), surfacing to human reviewers.
- **Assessment-item drafting** adapted from the IHC Claim Evaluation Tools bank (validated), for the
  methodology reviewer to approve.

**Where Claude must NOT decide (hard boundaries):**

- **No medical advice, ever** — Claude must never assess what evidence means for an individual's
  cancer; the linter/refusal scope applies to Claude's own output first.
- **Accuracy and clinical framing are decided by humans** — the credentialed oncologist and the
  methodology reviewer hold final say; Claude drafts, experts adjudicate. Methodological subtleties
  (GRADE up/down-rating, CI interpretation, surrogate validity) are exactly where LLMs err
  plausibly-but-wrongly.
- **No fabricated or hallucinated studies, statistics, citations, or licences.** Every paper, PMCID/
  DOI, figure, statistic, and licence string must be human-verified against the source register; the
  CI provenance + licence gate exists precisely to catch model invention. Claude must never assert a
  source is OA/compatible — the licence steward verifies.
- **No verdicts on specific drugs/trials/controversies** — Claude drafts *method demonstrations*, not
  adjudications.
- **Tone/usability and "does this patronise advocates" are decided by the advocate co-designer,** not
  the model.
- **Funded-lane note:** any metered Claude use stays within the donated-lane posture / hard budget cap
  per the Hee-Lee Oss rules; this project needs no runtime API and should keep authoring use offline/batch.

---

## 6. Ten concrete optimizations

1. **Adopt the IHC Key Concepts (CC-BY) framework as the curriculum spine,** mapping every module/
   worksheet question to a Key Concept ID. Gains external validity, reduces clean-room authoring
   risk, and slots under the licence gate. Cite the cancer-prioritisation protocol (HRB Open).
2. **Teach the evidence hierarchy GRADE-style** ("starting prior, then rate up/down per outcome"),
   not as a fixed pyramid — fixes the most consequential teaching error in the domain.
3. **Add a dedicated "calibrated, not cynical" module** and bake a "what is this study legitimately
   good for / what would change your mind" prompt into every worksheet to counter induced
   over-skepticism.
4. **Promote at least one advocate from reviewer to co-author from M0** (true co-design on scope,
   examples, sequencing) — converts a claimed differentiator into a real one and de-risks tone.
5. **Name validated assessment instruments** (adapt IHC Claim Evaluation Tools for the appraisal
   rubric; name a specific PPI confidence scale) and have the methodology reviewer sign off the rubric
   itself, removing construct-circularity from metrics 1–2.
6. **Add a "relationship to sibling projects" subsection** drawing the consumer-vs-producer-vs-data
   statistics line against `stats-for-clinicians` and `oncology-data-literacy`, plus a *shared
   glossary* to prevent divergence and duplicate review.
7. **Choose therapeutically low-salience walkthrough papers** (settled/older/non-decision-driving
   questions) and add a unit-level "method demo, not a treatment assessment" frame to harden the
   not-advice wall inside walkthroughs.
8. **Position explicitly as the open on-ramp/companion to LEAD/SSP/RAN,** and pursue one of them (or a
   LEAD alumni network) as the named pilot partner — turns the strongest incumbents into distribution
   channels and credibility, not competitors.
9. **Add named statistics "landmines" to the style guide** (95% CI misinterpretation; "non-significant
   ≠ no effect"; relative-risk inflation; PFS≠OS) as mandatory methodology-reviewer checkpoints.
10. **Publish the source register + review ledger as a public, browsable artifact** ("see every claim's
    source and every sign-off") — turns provenance discipline into a visible trust differentiator and a
    teaching exhibit, and models the appraisal behaviour the primer teaches.

---

## 7. Parallel & perpendicular spin-offs

- **Shared glossary + Key-Concept taxonomy as a portfolio primitive.** A single CC-BY methodology
  glossary and IHC-mapped concept index, consumed by this primer, `oncology-data-literacy`,
  `stats-for-clinicians`, and `systematic-review-assist`. Build once, reuse across the cancer track;
  prevents four projects defining "hazard ratio" four ways.
- **`oncology-data-literacy` tie.** This primer = *literature/claim* appraisal; that sibling = *data/
  registry/statistics* literacy. Co-design the boundary and share the glossary; a learner graduates
  from "read the paper" (here) to "read the dataset" (there).
- **`stats-for-clinicians` tie.** Consumer-side stats here (interpret a reported HR/CI/NNT) vs
  producer-side there (choose/compute). Shared worked examples could serve both audiences at different
  depths from the same OA paper.
- **`systematic-review-assist` tie.** The "appraise a systematic review / meta-analysis" worksheet and
  the spotting-spin module are direct feedstock; conversely that project's outputs become walkthrough
  material here. Strong reuse loop.
- **`ewing-research-landscape` tie.** Use the Ewing track to source disease-specific OA walkthrough
  papers, giving a rare-sarcoma community a concrete, role-relevant example set — and demonstrating the
  fork-for-your-disease pattern (open Q5: generality vs specificity → answer "general core + per-disease
  example packs").
- **Reusable cross-disease research-literacy curriculum for advocates.** The flagship perpendicular
  spin-off: a *disease-agnostic core* (study design, hierarchy, endpoints, stats, bias, spotting hype)
  plus *swappable per-disease example packs* (breast, sarcoma, leukemia, rare disease). CC-BY +
  documented register makes this the forkable artifact no incumbent offers — the path to "≥3 orgs adopt/
  fork" (metric 7) across diseases, not just cancer.
- **An MCP server: "appraisal-companion."** A read-only, offline-friendly MCP server exposing the
  glossary, worksheets, Key-Concept index, and the licence-verified walkthrough corpus as structured
  tools, so an advocate (or their own agent) can pull "the RCT appraisal worksheet" or "the plain-
  language definition of progression-free survival, with source" in context. *Strictly retrieval +
  education* — it surfaces sourced curriculum, renders no verdicts, gives no medical advice, and
  inherits the not-advice frame. Could ship the same content the static site serves, reusing the
  source register as the trust layer.
- **Reviewer-facing "spot the spin" trainer.** A standalone micro-tool/dataset pairing OA abstracts
  with their press releases for spin-detection drills — useful to journalists and communicators
  (secondary beneficiaries) and forkable.

---

## 8. Open questions

1. **IHC adoption:** Should the curriculum spine *be* the IHC Key Concepts (CC-BY, validated, cancer-
   prioritisation published), or remain independently structured citing IHC as one authority? (Strong
   recommendation: adopt and map to it — affects M0/M1 architecture.)
2. **Partner = competitor-as-channel?** Is RAN, a Project LEAD alumni network, an NCI/ASCO advocate
   committee, or a single-disease charity the right pilot partner — and does approaching an incumbent
   create a perceived-overlap problem or a credibility win? (Recommendation: companion-not-rival
   framing; pursue actively.)
3. **Disease scope (plan Q5):** General core + per-disease example packs (recommended) vs single
   disease for partner alignment — resolve before M1 example authoring.
4. **Assessment validity:** Which validated instruments anchor metrics 1–2, and can IHC Claim
   Evaluation Tools be adapted under their licence for the appraisal rubric?
5. **Calibration measurement:** How do we *measure* whether we produced calibrated (not merely more
   skeptical) appraisers? Does the rubric reward proportionate critique and "good-enough-to-act"
   judgements, not just fault-finding?
6. **Walkthrough paper selection criteria:** What objective bar makes a paper "therapeutically low-
   salience" enough to appraise safely while still pedagogically rich?
7. **Sibling-boundary governance:** Who owns the shared glossary/Key-Concept taxonomy across the four
   cancer-track projects, and how are changes coordinated?
8. **Expert compensation (plan Q2):** Unresolved donated-lane tension — is a small funded-lane
   carve-out for credentialed oncologist/methodology review justified to secure quality reviewers?
9. **MCP/tooling scope creep:** Does an appraisal-companion MCP server stay safely on the education
   side of the not-advice wall, or does interactive retrieval invite individualised-guidance drift that
   the static site avoids?
