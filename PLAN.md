# Patient-Advocate-Research-Primer — PLAN.md

> Status: Draft · Version: 0.1.0 · Last updated: 2026-06-28 · Owner: TBD (maintainer) · Lane: donated · Risk tier: medium (project) / high (patient-facing content)

An open-access educational primer and critical-appraisal toolkit that teaches **cancer patient
advocates** — the lay members of research-review panels, advocacy organisations, patient and family
advisory councils, trial steering committees, and grant-review boards — how to *read the science*:
how a study is designed, what its evidence is actually worth, and where a claim is stronger or
weaker than it sounds. It is **education, not medical advice**, and it never tells anyone what to do
about their own or a loved one's cancer.

---

## Executive summary

Patient advocates are now embedded throughout cancer research. They sit on NIH/NCI study sections,
charity scientific advisory boards, IRBs/ethics committees, trial steering and data-safety
committees, and patient and family advisory councils; they co-author grant applications and review
lay summaries. The role asks them to weigh evidence — yet almost none receive structured training in
**research methodology or critical appraisal**, and the existing training that does exist
(GRADE, CASP, Cochrane) was written for clinicians and methodologists, sits behind non-commercial or
restrictive licences, or assumes statistical fluency advocates were never given.

The result is a quiet, consequential gap. An advocate who cannot tell a single-arm phase-I dose
study from a randomised phase-III trial, who reads a "73% responded" headline without asking *to
what, measured how, versus what, in whom*, or who treats progression-free survival as equivalent to
living longer, cannot fully discharge the duty the role places on them — and is vulnerable to being
steered by hype, by a press release, or by a sponsor's framing.

**Patient-Advocate-Research-Primer** closes that gap with a free, openly-licensed, source-cited
curriculum and toolkit: plain-language modules on study design and evidence quality; a methodology
glossary; original critical-appraisal worksheets; and **annotated walkthroughs of real, fully
open-access oncology papers** that show appraisal in action. Every factual and methodological
assertion carries a provenance citation to a primary or authoritative source. The deliverable is the
curriculum and toolkit themselves, delivered to a real advocacy partner and measured by whether
advocates can actually appraise a study better after using it.

Two design facts govern everything. **First, the licence and provenance discipline is the first
build item, not a footnote.** Worked examples may only use papers whose licence permits reuse and
adaptation, verified per-article; appraisal frameworks may only be *adapted* where their licence
allows redistribution under our open licence, and otherwise are linked, not copied. **Second, this
is education with a hard wall against medical advice.** The scope is *how to read research in
general*; it is never *what this evidence means for your cancer*. All patient-facing content is
**high risk-tier**: it ships only after sign-off by both a **credentialed oncologist** and an
**experienced patient advocate**, carries a persistent "not medical advice" frame, and the project
is engineered to refuse drift into individualised guidance.

No advocacy partner, oncologist reviewer, or advocate reviewer is yet secured. Those are recorded
throughout as **TO BE SECURED**, and every delivery-dependent task carries `verifiedNeed: false`
until a specific partner and need are confirmed.

---

## Problem & beneficiaries

**Who is helped (primary beneficiaries).** Cancer patient advocates and patient/family
representatives acting in a *research* capacity:

- Lay reviewers on grant study sections and charity scientific advisory boards.
- Patient/community members of IRBs, ethics committees, and data-safety monitoring boards.
- Patient and Family Advisory Council (PFAC) members and trial patient-partners / co-investigators.
- Advocacy-organisation staff and volunteers who summarise or respond to new evidence.
- By extension: the patients and families those advocates represent, who benefit from sharper,
  better-calibrated advocacy.

**Secondary beneficiaries.** Advocacy organisations and research institutions that want a free,
reusable onboarding curriculum for new patient reviewers; educators in patient-research-partnership
programmes; journalists and communicators who need the same appraisal literacy.

**The verified need.** *Not yet verified.* The need is strongly evidenced in the literature on
patient and public involvement (PPI) in research — repeated findings that involvement is
under-supported by training, that methodological/appraisal training is the most-requested and
least-met need, and that lay reviewers report low confidence appraising study quality. **But Hee-Lee Oss
requires a *named partner with a confirmed need*, and none is yet secured.** We will not assert
`verifiedNeed: true` on any task until a specific advocacy organisation (e.g. a cancer charity's
research-advocate programme, a cooperative-group patient-advocate committee, or a research-engagement
network) confirms the gap and commits to pilot the material. Partner status: **TO BE SECURED.**

**Why this is a good deed (against the 5 criteria).** (1) Tangible public benefit — better-trained
advocates improve research relevance and oversight for patients. (2) Freely available — CC-BY content,
MIT tooling, open access only. (3) No primary for-profit benefit — built for and handed to non-profit
advocacy; refuses sponsor/industry promotion. (4) No harm/discrimination/misinformation — the entire
project *teaches the detection of* misleading claims and is expert-reviewed. (5) Specific and
AI-executable with required human/expert review at the high-risk tier.

---

## Goals and non-goals

**Goals**

1. Teach advocates to **classify a study** (design, phase, arm structure, blinding, randomisation)
   and locate it on the evidence hierarchy.
2. Teach advocates to **interrogate evidence quality**: endpoints (overall survival vs progression-
   free survival vs response rate vs surrogate/biomarker endpoints), effect size and its precision
   (hazard ratio, confidence interval, absolute vs relative risk, number needed to treat), bias,
   confounding, conflicts of interest, and reproducibility.
3. Provide **original, openly-licensed critical-appraisal worksheets** advocates can use on a real
   paper or protocol.
4. Provide **annotated walkthroughs** of real fully-open-access oncology papers demonstrating
   appraisal end-to-end.
5. Deliver the material to a **real advocacy partner** and demonstrate a **measurable gain** in
   advocates' appraisal ability and confidence.
6. Maintain **provenance on every assertion** and a verifiable open-licence chain on every reused
   source.

**Non-goals**

- **Not medical advice, ever.** No guidance on diagnosis, prognosis, treatment selection, trial
  enrolment decisions, or "what this means for you / your patient."
- **Not a clinical-trial finder or matcher** (that is `ewing-trial-finder` / general trial-finder
  territory; this primer may *teach how to read* a trial record but does not recommend trials).
- **Not a systematic-review or meta-analysis service**, and not a tool that *renders verdicts* on
  specific drugs, studies, or controversies. It teaches the method; it does not adjudicate the science.
- **Not a data project.** It does not ingest, store, link, or analyse patient-level data of any kind.
- **Not a replacement** for formal biostatistics or epidemiology training, nor for an advocacy
  organisation's own governance and training.
- **Not a credential.** Completing the primer confers no certification or authority.

---

## Success metrics (outcomes)

Outcome-based and beneficiary-centric. Vanity metrics (page views, stars, downloads) are tracked
only as health indicators, never as success.

| # | Outcome metric | Baseline | Target | How measured |
|---|---|---|---|---|
| 1 | Advocate appraisal-skill gain | Pre-test score (pilot cohort) | **≥ 25-point median gain** on a 100-pt pre/post appraisal exercise | Same annotated-paper appraisal rubric scored pre and post, blinded |
| 2 | Self-rated confidence appraising a study | Pre-pilot survey | **≥ +2 on a 5-pt scale** (median) | Validated PPI confidence survey, pre/post |
| 3 | Real-world application | 0 | **≥ 60% of pilot advocates** report using a worksheet on an actual review within 8 weeks | Follow-up survey + partner attestation |
| 4 | Expert-review pass | n/a | **100%** of patient-facing modules carry dual sign-off (oncologist + advocate) before publish | Review ledger (each module has both sign-offs recorded) |
| 5 | Provenance integrity | n/a | **100%** of assertions cite a resolvable source; **0** dead/incorrect citations at release | Automated link-check + manual citation audit |
| 6 | Licence integrity | n/a | **0** reused sources without a verified, compatible licence record | Per-source licence register, audited in CI |
| 7 | Reach with retained quality | 0 | **≥ 3 advocacy orgs** adopt or fork the material within 12 months of v1.0 | Partner attestations / fork-with-attribution tracking |
| 8 | Accessibility | n/a | Plain-language target met (see §6); WCAG 2.1 AA for the web delivery | Readability scoring + automated + manual a11y audit |

Note metrics 1–3 require a secured pilot partner; until then they are **target-only** and the
project cannot claim "delivered" outcomes.

---

## Scope

**In scope**

- Plain-language educational **modules** on study design, evidence hierarchy, trial phases,
  endpoints, statistics-for-appraisal, bias/confounding, conflicts of interest, reproducibility,
  and reading the structure of a paper / protocol / registry record.
- An **original methodology glossary** (advocate-facing definitions with provenance).
- **Original critical-appraisal worksheets** (study-design-specific), authored in-house so they are
  cleanly CC-BY and not derivative of restrictively-licensed tools.
- **Annotated walkthroughs** built *only* on individually licence-verified, fully open-access
  oncology papers.
- A lightweight **static web delivery** (accessible, offline-capable, printable) plus source in repo.
- A **pilot** with one advocacy partner and an outcome evaluation.

**Out of scope (explicit)**

- **Any controlled-access or identifiable patient data** (dbGaP, EGA, individual-level biobank,
  EHR, registry microdata) — categorically out of scope; this project uses *literature and
  authoritative methodology guidance only*.
- **Any patient-level or registry data store.** The project holds no health data about any person.
- Individualised medical, treatment, prognostic, or trial-enrolment advice or recommendations.
- Verdicts on specific drugs, trials, sponsors, institutions, or scientific controversies.
- Reproducing full text/figures of papers that are *not* under a reuse-and-adapt-permitting licence
  (those are linked and minimally quoted only).
- Adapting/redistributing third-party appraisal checklists whose licence forbids it (CASP, etc. —
  linked, not copied; see §7).
- Translation/localisation beyond *design hooks* in v1 (full translation is a future track and is
  itself high-risk for patient-facing health content).
- Certification, accreditation, or any authority-conferring function.

---

## Solution approach & architecture

This is primarily a **content + light-tooling** project: the durable good is the curriculum,
glossary, worksheets, and walkthroughs, plus the **provenance/licence discipline** that makes them
trustworthy and reusable.

**Components**

1. **Content corpus** (`/content`) — Markdown modules with structured front-matter (id, title,
   reading level, prerequisites, learning objectives, `riskTier`, review status, `lastReviewed`,
   `sources[]`). Single source of truth.
2. **Glossary** (`/content/glossary`) — one entry per term: advocate-facing definition, "why it
   matters for appraisal", common misreadings, and `source` provenance. Machine-readable (YAML/JSON).
3. **Worksheets** (`/content/worksheets`) — original critical-appraisal checklists per study type
   (RCT, single-arm/early-phase, observational/cohort, systematic review/meta-analysis, diagnostic/
   biomarker), as Markdown + printable PDF, CC-BY.
4. **Annotated walkthroughs** (`/content/walkthroughs`) — each pairs a licence-verified OA paper
   (linked, with its licence and PMCID/DOI) with an inline appraisal commentary keyed to a worksheet.
5. **Provenance layer** — every assertion references an entry in a central **source register**
   (`/data/sources.yaml`): id, citation, URL/DOI, access type (OA/authoritative-guidance), licence,
   licence-verified-date, allowed-use (link-only | quote | adapt | reproduce).
6. **Build/validation tooling** (`/packages/build`) — TypeScript/ESM scripts that (a) validate
   front-matter and that every assertion-citation resolves to a source-register entry; (b) run
   link-checking; (c) compute readability; (d) enforce the **licence gate** (fail build if any
   referenced source lacks a verified compatible licence record or if a non-adapt source is
   reproduced); (e) render the static site.
7. **Static site** (`/site`) — generated from content; accessible, printable, offline-capable;
   persistent "not medical advice" banner and per-page review/provenance footer.
8. **Review ledger** (`/governance/reviews`) — append-only record of expert sign-offs per content
   unit (reviewer role, date, version reviewed, decision).

**Tech stack.** TypeScript + ESM, pnpm workspaces; Markdown + YAML front-matter; a static-site
generator (e.g. Astro or Eleventy — TBD, decided in M0); Ajv for front-matter/source-register schema
validation; standard link-checker + readability library; MIT for code, CC-BY-4.0 for content.

**Key design decisions.**

- **Original worksheets over adapted ones** — authoring in-house avoids the licence trap of
  NC/SA appraisal tools and lets us publish cleanly under CC-BY (decision D-1).
- **Source register as a build gate, not a bibliography** — provenance and licence compatibility are
  *enforced in CI*; content cannot ship citing an unverified or incompatible source (D-2).
- **High-risk content is gated in the pipeline** — front-matter `riskTier: high` requires two
  recorded sign-offs in the review ledger before the build will mark a unit `published` (D-3).
- **No runtime, no accounts, no data collection** — a static site removes most security/privacy
  surface and makes offline/printable reuse trivial (D-4).
- **Education-only assertion linter** — a lightweight check + human-review checklist flags
  advice-shaped language ("you should", "the best treatment", second-person prescriptive forms) so
  drift toward advice is caught before review (D-5).

---

## Data, licensing & compliance

**This is the critical section. Posture is conservative by default; when uncertain, link rather than
copy, and exclude rather than assume.**

### Cancer-domain guardrails (binding, inherited from the portfolio)

- **Open-access / aggregate / de-identified ONLY.** This project consumes *published literature and
  authoritative methodology guidance*. **Controlled-access data (dbGaP, EGA, individual-level
  biobanks) and any identifiable patient data are categorically out of scope** and require authorised
  access + IRB that this project will never seek, because it has no need for them.
- **No data store.** The project holds **no** patient-level, registry, or health data about any
  individual. There is nothing to consent, de-identify, or breach. (The portfolio's consent-first,
  deceased/aggregate-only registry rules are noted for completeness but **do not apply** — this
  project is not a registry and stores no such data.)
- **No medical advice.** Patient-facing content is **education only**, sourced, carries a persistent
  "not medical advice" notice, and is **oncologist- and advocate-reviewed** (`riskTier: high`).
- **Provenance on every assertion** — non-negotiable; enforced by the build (§ above).
- **Per-source licence verification** — every reused source's licence is verified and recorded
  *before* use; non-commercial / no-derivatives sources are linked and minimally quoted, never
  republished or adapted.

### Source classes and their handling

| Source class | Examples | Licence reality | Our handling |
|---|---|---|---|
| Worked-example papers | PMC **Open Access Subset** oncology articles | Per-article: CC0 / CC-BY / CC-BY-NC / CC-BY-NC-ND / custom "non-commercial" | **Verify per article via the PMC OA licence metadata.** Reproduce/adapt text+figures **only** for CC0 / CC-BY / CC-BY-SA. For NC/ND: **link + minimal quotation** for commentary only; never republish or re-host the figure. Record PMCID, DOI, licence, verified-date in source register. |
| Methodology authority | Cochrane Handbook, EQUATOR Network (CONSORT, PRISMA, STROBE, SPIRIT), GRADE Handbook, FDA/EMA endpoint guidance, NCI Dictionaries | Mixed; many are copyrighted with limited reuse | **Cite and link as authority for our original prose.** Do **not** reproduce checklists/text verbatim unless the specific item's licence permits. Our worksheets are *original*, citing these as provenance. |
| Critical-appraisal checklists | **CASP** (CC BY-NC-SA 4.0), JBI, SIGN, AMSTAR/AMSTAR-2 | Non-commercial / share-alike → **incompatible** with our CC-BY output | **Do NOT copy or adapt into CC-BY material.** Link to them as further reading; build our own worksheets from first principles, citing the methodological *concepts* (which are not copyrightable) not the *expression*. |
| Statistics/aggregate references | SEER/GLOBOCAN aggregate stats (for illustrative examples only) | Generally public / open with attribution | Use aggregate figures with attribution; never any sub-aggregate or identifiable cut. |
| Glossary anchors | NCI Dictionary of Cancer Terms, NCI Dictionary of Genetics Terms | US-Gov work / public-domain-leaning but verify | Write **original** definitions; cite NCI as the authoritative anchor. Verify reuse terms before any quotation. |

### Provenance model

- Central **source register** (`/data/sources.yaml`): `id, citation, doiOrUrl, accessType
  (oa|authoritative|aggregate), licence, licenceVerifiedDate, verifiedBy, allowedUse
  (link|quote|adapt|reproduce)`.
- Every assertion in content references a source `id`; the build fails on any dangling reference,
  any `reproduce`/`adapt` use against a source whose `allowedUse` forbids it, or any source missing
  `licenceVerifiedDate`.
- A human **licence steward** owns the register and re-verifies on a schedule (licences change).

### Privacy / PII stance

- **No personal data is collected or stored** — static site, no accounts, no analytics that profile
  individuals (privacy-respecting, cookieless aggregate counts at most, opt-in).
- No patient stories, case reports with identifiers, or quotes naming individuals without documented
  consent and licence — and none are needed; examples come from published, licence-cleared papers.

### Attribution

- Each walkthrough names the paper, authors, DOI/PMCID, and its licence. Each worksheet/module lists
  its provenance sources. Output ships under **CC-BY-4.0** (content) / **MIT** (code) with a NOTICE
  file preserving upstream attributions and licences.

---

## Quality, review & risk gates

**Risk tier.** Project-level **medium**; **all patient-facing educational content is high** and
requires credentialed expert sign-off before publish, per the cancer guardrails and the good-deed
definition (health = high tier).

**Required review before a unit is "done":**

1. **Methodology accuracy** — every module/worksheet reviewed for methodological correctness
   (study-design, statistics, evidence-grading claims) by a reviewer with biostatistics/epidemiology
   or clinical-trials competence.
2. **Oncology accuracy + safety (high-tier)** — a **credentialed oncologist** confirms clinical
   framing is correct and nothing reads as treatment guidance.
3. **Advocate usability + safety (high-tier)** — an **experienced patient advocate** confirms the
   material is usable, non-condescending, and does not stray into advice or false reassurance.
4. **Licence + provenance audit** — licence steward confirms every source is verified and compatible
   and every assertion is cited.
5. **Education-only / refusal audit** — content is screened (linter + checklist) for advice-shaped
   language and individualised-guidance drift.

Items 2 and 3 are the **hard high-tier gate**: no patient-facing unit publishes without *both*
recorded in the review ledger. CI green (build/test/lint, link-check, licence gate, readability) is
necessary but not sufficient.

**Definition of Shipped.** A content unit is *delivered* when: acceptance criteria met; CI green
(incl. licence + provenance + readability gates); dual high-tier sign-off recorded (oncologist +
advocate) for patient-facing units; licence/provenance audit passed; **and** the unit is published
to the partner and in the advocates' hands (last-mile handoff by the steward). "Delivered, not
merged."

---

## Roadmap & milestones

Realistic, dependency-ordered. M0 is a thin cold-start that stands up the guardrails and proves one
vertical slice end-to-end before scaling content.

**M0 — Foundation, guardrails & one proven slice (cold-start).**
*Goal:* stand up the non-negotiables and prove the pipeline on a single module + worksheet +
walkthrough. *Exit criteria:* repo + CI skeleton green; education-only policy + content style guide
written; source-register schema + licence gate enforced in CI; advisory roles scoped (partner,
oncologist, advocate — all TO BE SECURED, with selection criteria published); **one** module
("What kind of study is this?") + **one** worksheet (RCT) + **one** annotated walkthrough on a
licence-verified OA paper, all passing CI and *dry-run* dual review (real sign-off pending reviewer
recruitment).

**M1 — Core curriculum: design & evidence.**
*Goal:* the heart of the primer. *Exit criteria:* modules on evidence hierarchy, trial phases,
endpoints (OS/PFS/ORR/surrogate), and statistics-for-appraisal (HR/CI/absolute-vs-relative
risk/NNT/p-values & their misuse) authored, cited, CI-green, and **high-tier-reviewed**; glossary
seeded (≥ 60 terms). Depends on M0.

**M2 — Critical-appraisal toolkit & walkthroughs.**
*Goal:* turn knowledge into practice. *Exit criteria:* full worksheet set (RCT, early-phase/single-
arm, observational, systematic-review/meta-analysis, diagnostic/biomarker); bias/confounding and
conflicts-of-interest modules; "press release vs paper / spotting hype" module; ≥ 4 annotated
walkthroughs across study types, all licence-verified and high-tier-reviewed. Depends on M1.

**M3 — Delivery, accessibility & pilot readiness.**
*Goal:* make it usable and ready to hand over. *Exit criteria:* accessible static site (WCAG 2.1 AA),
printable/offline worksheets, readability targets met, persistent "not medical advice" + provenance
footers; pre/post evaluation instrument built and method-reviewed; localisation hooks in place.
Depends on M1–M2.

**M4 — Pilot, evaluation & sustainability.**
*Goal:* deliver to real advocates and measure. *Exit criteria* (**requires secured partner**): pilot
run with ≥ 1 advocacy org; outcome metrics 1–3 measured; findings published; maintenance owner and
re-review cadence committed; v1.0 tagged. Depends on M3 **and** partner secured.

---

## Work breakdown

The itemised, schema-mapped backlog lives in **`TASKS.md`**, organised by the milestones above with a
task table, per-task acceptance criteria for the most important items, and a Definition of Done per
milestone. Highlights: M0 establishes the licence gate, education-only policy, and one proven slice;
M1–M2 are the bulk of authored, expert-reviewed content; M3 delivery/accessibility; M4 pilot +
outcome measurement. A schema-valid example Task JSON for the first M0 task is included in `TASKS.md`.

---

## Governance, roles & stakeholders

- **Maintainer (Owner) — TBD.** Owns the repo, build/CI, source register schema, releases, and this
  plan. Accountable for the licence and provenance gates.
- **Methodology reviewer — TO BE SECURED.** Biostatistics/epidemiology/clinical-trials competence;
  reviews accuracy of design/statistics/grading content.
- **Oncologist reviewer (high-tier) — TO BE SECURED.** Credentialed oncologist; clinical-accuracy +
  no-advice sign-off on patient-facing content.
- **Patient-advocate reviewer (high-tier) — TO BE SECURED.** Experienced research advocate; usability
  + safety + tone sign-off; ideally co-designs the curriculum.
- **Licence/provenance steward — TBD.** Owns `sources.yaml`, per-source verification, re-verification
  cadence, NOTICE/attribution.
- **Steward (last-mile owner) — TO BE SECURED.** Owns delivery to the partner and tracking of
  real-world use (outcome metrics 3, 7).
- **Partner / requestor — TO BE SECURED.** Advocacy organisation that confirms the need and pilots
  the material; flips `verifiedNeed` to true.
- **Reviewer rotation & COI.** Reviewers declare conflicts (industry funding, sponsor ties);
  a reviewer with a material COI on a paper used in a walkthrough recuses. Sign-offs are recorded in
  the append-only review ledger. High-tier units require two distinct reviewers (oncologist +
  advocate); one person cannot hold both roles.

All roles are currently unfilled; selection criteria are published in M0 so recruitment is concrete,
not vague.

---

## Dependencies & integrations

- **PMC Open Access Subset** + its per-article licence metadata (worked-example papers).
- **EQUATOR Network** reporting guidelines (CONSORT, PRISMA, STROBE, SPIRIT) — cited as authority.
- **Cochrane Handbook**, **GRADE Handbook** — cited as authority for evidence-grading concepts.
- **FDA/EMA** oncology-endpoint guidance — cited as authority on endpoints/surrogates.
- **NCI Dictionaries** (Cancer Terms, Genetics Terms) — glossary anchors.
- **SEER / GLOBOCAN** aggregate statistics — illustrative aggregate examples only.
- **Hee-Lee Oss pieces:** task schema (`packages/schema`), the donated-lane CLI workflow (workspace prep +
  PR), good-deed-definition risk tiers, and portfolio cancer guardrails.
- **Tooling:** static-site generator (TBD M0), Ajv, link-checker, readability scorer, a11y auditor.

No paid services, no API keys, no runtime backend.

---

## Risks & mitigations

| Risk | Likelihood | Impact | Mitigation | Owner |
|---|---|---|---|---|
| Content drifts into medical advice | Medium | High | Education-only policy as first build item; advice-language linter + review checklist; dual high-tier sign-off; persistent "not medical advice" frame; refusal scope in CLAUDE-derived agent instructions | Oncologist + advocate reviewers |
| Reusing a paper/figure under an incompatible (NC/ND) licence | Medium | High | Per-article licence verification in source register; build gate blocks `reproduce`/`adapt` against forbidding licences; default to link+quote | Licence steward |
| Adapting CASP/JBI/etc. into CC-BY output (licence breach) | Medium | High | Policy D-1: author original worksheets; link (not copy) third-party tools; documented in §7 | Licence steward + Maintainer |
| Methodological error teaches advocates wrong appraisal | Medium | High | Methodology reviewer + provenance to authoritative sources on every claim; worked examples cross-checked | Methodology reviewer |
| No advocacy partner secured → can't measure outcomes / no verified need | High | Medium | `verifiedNeed:false` everywhere; published partner-selection criteria; M0–M3 deliver standalone value; M4 gated on partner | Maintainer + Steward |
| No credentialed reviewers recruited → high-tier content stuck unpublished | Medium | High | Recruit early (M0 task); "dry-run review" in M0 to derisk; nothing patient-facing publishes without real sign-off | Maintainer |
| Outdated science/licence over time | Medium | Medium | `lastReviewed` front-matter; scheduled re-review + licence re-verification; issue templates for corrections | Maintainer + stewards |
| Tone alienates or patronises advocates | Medium | Medium | Advocate co-design + usability sign-off; plain-language + reading-level targets | Advocate reviewer |
| Over-scope into trial-finding / verdicts on specific science | Medium | Medium | Explicit non-goals; scope review at each milestone gate | Maintainer |
| Misuse: material cited to lend false authority to a claim | Low | Medium | "Not medical advice" + "teaches method, renders no verdicts" framing; no endorsements | Maintainer |

---

## Security & privacy

- **Threat surface is small by design:** static site, no accounts, no backend, no PII, no health
  data. Primary surfaces are (a) supply chain (dependencies) and (b) content integrity.
- **Secrets:** none required; CI uses no API keys or tokens for content. No secret may ever be
  written to logs, content, or the source register (CLAUDE.md rule).
- **PII:** none collected or stored; no patient-level or identifiable data anywhere in scope.
  Privacy-respecting, opt-in, aggregate-only usage counts at most.
- **Supply chain:** pinned/lockfiled dependencies, CI audit, minimal dependency footprint.
- **Content integrity / abuse:** provenance + licence gates prevent unsourced or mis-licensed claims;
  append-only review ledger; PRs require review; corrections process. Refusal guardrails (no advice,
  no harm, no for-profit steering) are encoded in the agent instructions and the review checklist.
- **Abuse/misuse prevention:** explicit "renders no verdicts / not medical advice" framing limits
  weaponisation of the material to lend false authority; no individual or institution is endorsed.

---

## Sustainability & maintenance

- **Maintenance owner — TBD** commits to a re-review cadence: patient-facing content re-reviewed at
  least annually or on material guidance change; **licence steward** re-verifies sources on a
  schedule (licences and OA status change).
- **Outcome tracking** continues past delivery: the steward tracks real-world use (metrics 3, 7) via
  partner attestations and fork-with-attribution signals.
- **Low ongoing cost:** static content, no runtime, no paid services → cheap to host and fork.
- **Forkability is the durability plan:** CC-BY content + MIT tooling + a documented source register
  mean any advocacy org can adopt, translate, or extend the material if the original maintainer steps
  away. A CONTRIBUTING guide + corrections issue templates lower the contribution barrier.

---

## Open questions

1. **Partner.** Which advocacy organisation pilots this, and does it confirm the need? (Gates M4 and
   all `verifiedNeed`.)
2. **Reviewers.** How do we recruit and (if needed) compensate the oncologist + advocate reviewers in
   a donated-lane project? Is a small funded-lane carve-out for expert review justified?
3. **Static-site generator** choice (Astro vs Eleventy vs plain) — decided in M0.
4. **Code licence** MIT vs Apache-2.0 — default MIT per conventions; confirm with governance.
5. **Disease scope.** General oncology examples vs a specific cancer (e.g. align with the Ewing track
   for shared walkthroughs)? Generality aids reach; specificity aids a partner.
6. **Worksheet originality bar.** Confirm with counsel/steward that concept-level (not expression-
   level) reuse of established appraisal frameworks is sufficiently clean to publish under CC-BY.
7. **Localisation.** Is translated patient-facing content in-scope later, given it is itself high-risk?

---

## References

- `C:\code\hee-lee-oss\CLAUDE.md` — Hee-Lee Oss work rules, lanes, quality bar, refusal guardrails.
- `C:\code\hee-lee-oss\docs\good-deed-definition.md` — good-deed criteria + risk tiers.
- `C:\code\hee-lee-oss\packages\schema\src\schemas.ts` — Task JSON schema (TASKS.md maps to it).
- `C:\code\hee-lee-oss\planning\ROADMAP.md` — portfolio + Track 8 cancer guardrails.
- EQUATOR Network (CONSORT, PRISMA, STROBE, SPIRIT) — reporting guidelines.
- Cochrane Handbook for Systematic Reviews of Interventions; GRADE Handbook.
- US FDA / EMA oncology clinical-endpoint guidance (OS, PFS, ORR, surrogate endpoints).
- NCI Dictionary of Cancer Terms; NCI Dictionary of Genetics Terms.
- PMC Open Access Subset and its licence metadata.
- CASP / JBI / SIGN appraisal checklists — *linked as further reading; not adapted* (licence).

---

## Appendix A — Improvements applied

Twenty-five specific improvements were identified during drafting and are **already applied** in the
plan above (and the companion `TASKS.md`).

1. **Split risk tiers explicitly** — project medium, patient-facing content high — rather than a
   single ambiguous "medium"; encoded in the header, §8, and per-task `riskTier`.
2. **Made the licence gate a CI build step (D-2)**, not a guideline, so content cannot ship citing an
   unverified/incompatible source.
3. **Authored original worksheets (D-1)** to dodge the CASP/JBI non-commercial/share-alike licence
   trap, with the reasoning documented in §7 and a dedicated risk row.
4. **Per-article (not per-corpus) OA licence verification** for worked-example papers, with an
   `allowedUse` field distinguishing link/quote/adapt/reproduce.
5. **Added an education-only advice linter (D-5)** plus a human refusal-audit checklist to catch
   drift toward medical advice before review.
6. **Required dual high-tier sign-off (oncologist + advocate)** with a one-person-can't-hold-both-
   roles rule, recorded in an append-only review ledger.
7. **Recast all success metrics as beneficiary outcomes** (skill gain, confidence, real-world use)
   with baselines/targets, demoting page-views to non-success health indicators.
8. **Marked outcome metrics 1–3 as target-only until a partner is secured**, so we never claim
   delivered outcomes we can't measure.
9. **Honest `verifiedNeed: false` everywhere** and partner/reviewers marked **TO BE SECURED**, per
   the spec's anti-fabrication rule.
10. **Published reviewer/partner *selection criteria* in M0** so recruitment is concrete.
11. **Added a "dry-run review" in M0** to derisk the pipeline before real reviewers are recruited.
12. **Source register schema** (`id, licence, licenceVerifiedDate, verifiedBy, allowedUse`) with
    scheduled re-verification, acknowledging licences change.
13. **Clarified the project stores no patient/registry data**, so consent/de-id/registry rules are
    explicitly noted as *not applicable* rather than vaguely gestured at.
14. **Sharpened non-goals** to fence off trial-finding, verdict-rendering, and meta-analysis (avoids
    scope creep into adjacent high-risk projects).
15. **Chose a static, account-less, analytics-light architecture (D-4)** to shrink the security/
    privacy surface to near zero and enable offline/printable reuse.
16. **Added an aggregate-only constraint** even for illustrative SEER/GLOBOCAN statistics (no
    sub-aggregate cuts), consistent with the data guardrail.
17. **Added COI/recusal rules** for reviewers, especially on papers used in walkthroughs.
18. **Added accessibility as a first-class outcome** (WCAG 2.1 AA + readability targets), not an
    afterthought.
19. **Provenance-on-every-assertion enforced by build**, with link-checking and a citation audit in
    the Definition of Shipped.
20. **NOTICE/attribution file** to preserve upstream paper attributions and licences in the CC-BY
    output.
21. **Mapped the project against all five good-deed criteria** explicitly in §2.
22. **Added a misuse risk** (material cited to lend false authority) with a "renders no verdicts"
    mitigation — beyond the usual inaccuracy risk.
23. **Made M4 hard-gated on a secured partner** and listed it as a dependency, so the roadmap is
    honest about what cannot proceed yet.
24. **Forkability named as the sustainability plan** (CC-BY + MIT + documented register), reducing
    single-maintainer risk.
25. **Raised the expert-compensation question** (open Q2) — a real, unresolved tension between a
    donated-lane project and the need to fairly engage credentialed reviewers.

---

## Review sign-off

A completeness and correctness review was performed against PLAN_SPEC.md, the good-deed definition,
the cancer guardrails, and the Task schema. Findings and resolutions:

- **All 17 required H2 sections present and in order**, with `Data, licensing & compliance` leading
  on the cancer guardrails. ✔
- **Risk gates correct:** health content = high tier requiring credentialed expert sign-off, matching
  the good-deed definition; project medium. ✔
- **Cancer guardrails honoured:** open-access/aggregate/de-identified only; controlled-access and
  identifiable data explicitly out of scope; per-source licence verification; no medical advice +
  "not medical advice" + dual review; provenance on every assertion; registry/consent rules noted as
  not-applicable because no data is stored. ✔
- **Honesty:** no partner/need/reviewers invented; all marked TO BE SECURED; `verifiedNeed:false`
  throughout (verified against TASKS.md and the example Task JSON). ✔
- **Licence correctness check:** confirmed the plan does **not** adapt CASP (CC BY-NC-SA) or other
  NC/SA tools into CC-BY output — corrected the approach to original worksheets + link-out, and added
  a dedicated risk row and §7 register handling. ✔
- **Outcome metrics** are beneficiary-centric with baselines/targets; vanity metrics demoted. ✔
- **Schema mapping:** TASKS.md maps every field; the example Task JSON was validated field-by-field
  against `taskSchema` (all required fields present; enums valid; donated lane so no
  `fundedBudgetUsd`; `verifiedNeed:false`). ✔
- **One gap fixed during review:** added the expert-compensation open question (Q2), since a
  donated-lane project still needs to fairly engage high-tier reviewers — previously implicit.

Reviewer: drafting agent (senior staff engineer + TPM). Status: **ready for maintainer review**;
blocking items for v1.0 are partner + reviewer recruitment (TO BE SECURED), not document gaps.
