# Patient-Advocate-Research-Primer — TASKS.md

> Status: Draft · Version: 0.1.0 · Last updated: 2026-06-28 · Owner: TBD (maintainer) · Lane: donated

Backlog for **Patient-Advocate-Research-Primer** (slug: `patient-advocate-research-primer`), an
open-access educational primer + critical-appraisal toolkit that teaches cancer **patient advocates**
how to read research — study design and evidence quality — as **education, not medical advice**. See
`PLAN.md` for full context.

Two non-negotiables drive sequencing. (1) The **licence + provenance gate and the education-only
policy are the first build items**. (2) **All patient-facing content is high risk-tier** and ships
only with **dual sign-off (credentialed oncologist + experienced patient advocate)**. No advocacy
partner, oncologist reviewer, or advocate reviewer is yet secured, so every delivery-dependent task
carries `requestor: TO BE SECURED` and `verifiedNeed: false`.

## How these tasks map to Hee-Lee Oss

Each task below becomes a Hee-Lee Oss **Task JSON** validated against
`packages/schema/src/schemas.ts`. Field mapping:

- **id** — stable slug `patient-advocate-research-primer-<area>-NNN`
  (e.g. `patient-advocate-research-primer-licence-001`).
- **title** — the task title in the milestone table.
- **project** — `patient-advocate-research-primer`.
- **type** — one of `code | research | writing | data | design-spec | maintenance`.
- **lane** — `donated` (default; no funded tasks planned. Any `funded` task MUST add
  `fundedBudgetUsd` with a hard cap — see Open Q2 re: expert-review compensation).
- **priority** — `high | medium | low`.
- **domain** — string array, e.g. `["cancer","research-literacy","education","health"]`.
- **riskTier** — `low | medium | high`. **Patient-facing educational content = `high`** (oncologist +
  advocate sign-off). Methodology/curriculum without direct patient framing = `medium`. Pure
  tooling/infra/site = `low`.
- **urgent** — boolean (all `false` at cold-start; no time-critical work).
- **deliverable** — `pr | dataset | document | translation`.
- **tokenEstimate** — `small | medium | large` (maps to the Size column).
- **status** — `open | in-progress | review | delivered | done` (all start `open`).
- **context / objective / acceptanceCriteria[] / resources[] / output** — per task.
- **requestor** — partner/steward/expert; `TO BE SECURED` where unknown.
- **verifiedNeed** — `true` only once a specific partner confirms the need; currently **`false`
  everywhere** (no partner secured).
- **outputLicense** — content/docs: **CC-BY-4.0**; code: **MIT**.

Size legend: small ≈ `small`, med ≈ `medium`, large ≈ `large`.
Reviewer roles: **Maintainer**; **Methodology** (biostatistics/epidemiology/trials);
**Oncologist** (credentialed, high-tier); **Advocate** (experienced research advocate, high-tier);
**Licence steward**. High-tier sign-off (Oncologist + Advocate) is **TO BE SECURED**.

---

## Milestone M0 — Foundation, guardrails & one proven slice (cold-start)

| ID | Title | Type | Size | Risk | Deliverable | Depends on | Reviewer |
|---|---|---|---|---|---|---|---|
| patient-advocate-research-primer-licence-001 | Source-register schema + per-source licence/provenance model | design-spec | small | low | document | — | Maintainer + Licence steward |
| patient-advocate-research-primer-policy-002 | Education-only / no-medical-advice policy + refusal & advice-language checklist | design-spec | medium | high | document | — | Oncologist + Advocate |
| patient-advocate-research-primer-repo-003 | Repo + pnpm/TS/ESM + CI (build/test/lint) + static-site generator decision | code | small | low | pr | — | Maintainer |
| patient-advocate-research-primer-gate-004 | Licence + provenance build gate (fails CI on unverified/incompatible source or dangling citation) | code | medium | low | pr | 001, 003 | Maintainer + Licence steward |
| patient-advocate-research-primer-roles-005 | Partner + reviewer selection criteria & recruitment brief (all TO BE SECURED) | research | small | medium | document | — | Maintainer |
| patient-advocate-research-primer-module-006 | Module: "What kind of study is this?" (design/phase/arms/blinding) | writing | medium | high | document | 002, 004 | Oncologist + Advocate + Methodology |
| patient-advocate-research-primer-worksheet-007 | Original RCT critical-appraisal worksheet (CC-BY, not derived from CASP/JBI) | writing | medium | high | document | 002, 004 | Methodology + Advocate |
| patient-advocate-research-primer-walkthrough-008 | Annotated walkthrough of ONE licence-verified OA RCT paper | writing | medium | high | document | 006, 007 | Oncologist + Advocate + Methodology |

**Acceptance criteria — key tasks**

- **…-policy-002 (education-only policy):**
  - Defines the hard boundary: teaches *how to read research in general*; never *what evidence means
    for an individual's cancer*; enumerates prohibited output (diagnosis, prognosis, treatment/trial
    recommendation, individualised guidance).
  - Provides an **advice-language checklist** (prescriptive second-person forms, "best treatment",
    reassurance/false-certainty patterns) usable by the linter (task 004 follow-on) and reviewers.
  - Mandates the persistent "not medical advice" frame and the dual high-tier sign-off rule.
  - Signed off by Oncologist + Advocate and recorded in the review ledger.
- **…-gate-004 (licence + provenance build gate):**
  - CI fails if any content citation has no matching `sources.yaml` entry (dangling reference).
  - CI fails if content `reproduce`/`adapt`s a source whose `allowedUse` forbids it.
  - CI fails if any referenced source lacks `licenceVerifiedDate`/`verifiedBy`.
  - Includes link-checking; documented in CONTRIBUTING.
- **…-worksheet-007 (RCT worksheet):**
  - Authored **in-house from methodological first principles**; cites EQUATOR/Cochrane/GRADE as
    provenance for concepts but copies no third-party checklist text; passes licence gate clean.
  - Covers randomisation, allocation concealment, blinding, endpoints, effect size + precision,
    attrition, COI/funding.
  - Printable + plain-language; usability-confirmed by Advocate.
- **…-walkthrough-008 (annotated OA paper walkthrough):**
  - Uses exactly one paper with a verified reuse-permitting licence (CC0/CC-BY/CC-BY-SA), recorded in
    `sources.yaml` with PMCID/DOI/licence; figures reproduced only if licence permits, else linked.
  - Applies worksheet 007 inline; carries dual high-tier sign-off.

**Definition of Done (M0):** repo + CI green incl. the licence/provenance gate; education-only policy
+ source-register schema published; partner/reviewer selection criteria published (all TO BE
SECURED); the module + worksheet + walkthrough slice passes CI and **dry-run** dual review (real
sign-off pending reviewer recruitment); nothing patient-facing marked `published` without real
sign-off.

---

## Milestone M1 — Core curriculum: design & evidence

| ID | Title | Type | Size | Risk | Deliverable | Depends on | Reviewer |
|---|---|---|---|---|---|---|---|
| patient-advocate-research-primer-module-101 | Module: evidence hierarchy & levels of evidence | writing | medium | high | document | M0 | Oncologist + Advocate + Methodology |
| patient-advocate-research-primer-module-102 | Module: clinical-trial phases (I–IV) & what each can/can't show | writing | medium | high | document | M0 | Oncologist + Advocate + Methodology |
| patient-advocate-research-primer-module-103 | Module: endpoints — OS vs PFS vs ORR vs surrogate/biomarker | writing | medium | high | document | M0 | Oncologist + Advocate + Methodology |
| patient-advocate-research-primer-module-104 | Module: statistics for appraisal — HR, CI, absolute vs relative risk, NNT, p-values & misuse | writing | large | high | document | M0 | Methodology + Oncologist + Advocate |
| patient-advocate-research-primer-glossary-105 | Methodology glossary seed (≥ 60 terms, original defs + provenance) | writing | medium | medium | document | M0 | Methodology + Advocate |

**Acceptance criteria — key tasks**

- **…-module-103 (endpoints):** distinguishes overall survival from PFS/ORR and surrogate endpoints;
  explains why a surrogate gain may not mean longer/better life; cites FDA/EMA endpoint guidance;
  dual high-tier sign-off.
- **…-module-104 (statistics):** explains hazard ratio + confidence interval reading, absolute vs
  relative risk framing traps, NNT, and p-value misinterpretation; every claim cited to an
  authoritative methods source; worked mini-examples use only licence-cleared/aggregate figures.

**Definition of Done (M1):** modules 101–104 + glossary seed authored, cited, CI-green (licence +
provenance + readability), and dual high-tier sign-off recorded for all patient-facing units.

---

## Milestone M2 — Critical-appraisal toolkit & walkthroughs

| ID | Title | Type | Size | Risk | Deliverable | Depends on | Reviewer |
|---|---|---|---|---|---|---|---|
| patient-advocate-research-primer-worksheet-201 | Worksheet: early-phase / single-arm studies | writing | medium | high | document | M1 | Methodology + Oncologist + Advocate |
| patient-advocate-research-primer-worksheet-202 | Worksheet: observational / cohort studies (confounding focus) | writing | medium | high | document | M1 | Methodology + Advocate |
| patient-advocate-research-primer-worksheet-203 | Worksheet: systematic reviews & meta-analyses | writing | medium | high | document | M1 | Methodology + Advocate |
| patient-advocate-research-primer-module-204 | Module: bias, confounding & conflicts of interest | writing | medium | high | document | M1 | Methodology + Oncologist + Advocate |
| patient-advocate-research-primer-module-205 | Module: press release vs paper — spotting hype | writing | medium | high | document | M1 | Oncologist + Advocate + Methodology |
| patient-advocate-research-primer-walkthrough-206 | ≥ 3 annotated walkthroughs across study types (licence-verified OA) | writing | large | high | document | 201–205 | Oncologist + Advocate + Methodology |

**Acceptance criteria — key tasks**

- **…-module-205 (hype-spotting):** maps common overclaim patterns (surrogate-as-cure, relative-risk
  headlines, single-arm "response" framing, sponsor spin) to the worksheet questions that defuse
  them; renders **no verdicts** on real products; dual high-tier sign-off.
- **…-walkthrough-206:** each walkthrough uses a distinct, licence-verified OA paper recorded in
  `sources.yaml`, applies the matching worksheet inline, and passes the licence gate; reviewers with
  a COI on a given paper recuse.

**Definition of Done (M2):** full worksheet set + bias/COI + hype modules + ≥ 3 walkthroughs, all
licence-verified, CI-green, dual high-tier sign-off recorded.

---

## Milestone M3 — Delivery, accessibility & pilot readiness

| ID | Title | Type | Size | Risk | Deliverable | Depends on | Reviewer |
|---|---|---|---|---|---|---|---|
| patient-advocate-research-primer-site-301 | Accessible static site (WCAG 2.1 AA) + persistent "not medical advice"/provenance footers | code | medium | low | pr | M1, M2 | Maintainer |
| patient-advocate-research-primer-print-302 | Printable/offline worksheet pack (PDF) | code | small | low | pr | M2 | Maintainer + Advocate |
| patient-advocate-research-primer-eval-303 | Pre/post evaluation instrument (appraisal rubric + confidence survey) | research | medium | medium | document | M1, M2 | Methodology + Advocate |
| patient-advocate-research-primer-a11y-304 | Accessibility + readability audit (automated + manual) | maintenance | small | low | document | 301 | Maintainer |
| patient-advocate-research-primer-i18n-305 | Localisation hooks (content extraction, no translation yet) | code | small | low | pr | 301 | Maintainer |

**Definition of Done (M3):** site live and accessible (AA), printable pack shipped, evaluation
instrument method-reviewed, readability targets met, localisation hooks in place.

---

## Milestone M4 — Pilot, evaluation & sustainability (requires secured partner)

| ID | Title | Type | Size | Risk | Deliverable | Depends on | Reviewer |
|---|---|---|---|---|---|---|---|
| patient-advocate-research-primer-pilot-401 | Pilot with ≥ 1 advocacy org + measure outcome metrics 1–3 | research | medium | medium | document | M3 + partner | Maintainer + Steward + Advocate |
| patient-advocate-research-primer-report-402 | Publish pilot findings + corrections incorporated | writing | medium | medium | document | 401 | Maintainer + Methodology |
| patient-advocate-research-primer-maint-403 | Maintenance + re-review cadence + licence re-verification plan; tag v1.0 | maintenance | small | low | document | 402 | Maintainer + Licence steward |

**Definition of Done (M4):** pilot run; metrics 1–3 measured and published; maintenance owner + cadence
committed; v1.0 tagged. **Blocked until a partner is secured (`verifiedNeed` → true).**

---

## Backlog / future (sized, unscheduled)

| ID | Title | Type | Size | Risk | Deliverable | Notes |
|---|---|---|---|---|---|---|
| patient-advocate-research-primer-module-501 | Module: reading a trial registry record / protocol | writing | medium | high | document | Extends M1; teaches structure, not trial selection |
| patient-advocate-research-primer-module-502 | Module: diagnostic & biomarker test appraisal (sens/spec/PPV) | writing | medium | high | document | Pairs with a biomarker worksheet |
| patient-advocate-research-primer-i18n-503 | Full translation of vetted content (high-risk; needs translation review) | translation | large | high | translation | Each language re-reviewed; gated like patient-facing content |
| patient-advocate-research-primer-walkthrough-504 | Disease-specific walkthrough set (e.g. align with Ewing track) | writing | large | high | document | Depends on disease-scope decision (Open Q5) |
| patient-advocate-research-primer-facilitator-505 | Facilitator/workshop guide for advocacy orgs | writing | medium | medium | document | Supports reuse/adoption |

---

## Example task JSON

Schema-valid Task JSON for the first M0 task (`patient-advocate-research-primer-licence-001`),
validated field-by-field against `taskSchema` in `packages/schema/src/schemas.ts`. Donated lane, so
no `fundedBudgetUsd`; `verifiedNeed: false` (no partner secured).

```json
{
  "id": "patient-advocate-research-primer-licence-001",
  "title": "Source-register schema + per-source licence/provenance model",
  "project": "patient-advocate-research-primer",
  "type": "design-spec",
  "lane": "donated",
  "priority": "high",
  "domain": ["cancer", "research-literacy", "open-access", "licensing", "provenance"],
  "riskTier": "low",
  "urgent": false,
  "deliverable": "document",
  "tokenEstimate": "small",
  "status": "open",
  "context": "Patient-Advocate-Research-Primer teaches cancer patient advocates to read research as education, not medical advice. Per Hee-Lee Oss cancer guardrails it may reuse ONLY open-access / aggregate / de-identified sources, each with a verified licence, and must carry provenance on every assertion. Before any content is authored, the project needs a machine-readable source register that records each source's licence and the uses it permits, so the CI licence gate (task 004) can enforce it.",
  "objective": "Design the source-register schema and per-source licence/provenance model that every reused paper, guideline, or statistic must have an entry in before content may cite it.",
  "acceptanceCriteria": [
    "Defines a sources.yaml schema with fields: id, citation, doiOrUrl, accessType (oa|authoritative|aggregate), licence, licenceVerifiedDate, verifiedBy, allowedUse (link|quote|adapt|reproduce).",
    "Specifies that controlled-access and identifiable patient data are out of scope and MUST NOT appear in the register.",
    "Documents the conservative default: non-commercial / no-derivatives sources get allowedUse 'link' or 'quote' only, never 'adapt'/'reproduce'.",
    "Provides a worked example entry for one open-access (CC-BY) oncology paper and one authoritative guideline (EQUATOR/Cochrane).",
    "Specifies a scheduled re-verification cadence and the licence steward as owner.",
    "Is consumable by the CI licence + provenance gate (task 004) without further interpretation."
  ],
  "resources": [
    "PLAN.md (Data, licensing & compliance section)",
    "https://www.ncbi.nlm.nih.gov/pmc/tools/openftlist/ (PMC Open Access Subset + licence metadata)",
    "https://www.equator-network.org/ (reporting guidelines, cited as authority)",
    "packages/schema/src/schemas.ts (Hee-Lee Oss task schema conventions)"
  ],
  "output": "A design-spec document defining sources.yaml schema, the per-source licence/provenance model, allowed-use rules, worked example entries, and re-verification cadence — committed to the repo as the basis for the CI licence gate.",
  "requestor": "TO BE SECURED",
  "verifiedNeed": false,
  "outputLicense": "CC-BY-4.0"
}
```

---

## Generated task index

Generated by Hee-Lee Oss task-decomposition on 2026-06-29. All 32 files are schema-valid (validated against
`packages/schema/dist/index.js`). No fan-out dimensions were enumerated in TASKS.md; each row maps
to exactly one task file. The seed file (`licence-001`) was retained unchanged.

| File | Title | Milestone |
|---|---|---|
| `tasks/patient-advocate-research-primer-licence-001.json` | Source-register schema + per-source licence/provenance model | M0 (seed) |
| `tasks/patient-advocate-research-primer-policy-002.json` | Education-only / no-medical-advice policy + refusal & advice-language checklist | M0 |
| `tasks/patient-advocate-research-primer-repo-003.json` | Repo + pnpm/TS/ESM + CI (build/test/lint) + static-site generator decision | M0 |
| `tasks/patient-advocate-research-primer-gate-004.json` | Licence + provenance build gate | M0 |
| `tasks/patient-advocate-research-primer-roles-005.json` | Partner + reviewer selection criteria & recruitment brief | M0 |
| `tasks/patient-advocate-research-primer-module-006.json` | Module: "What kind of study is this?" (design/phase/arms/blinding) | M0 |
| `tasks/patient-advocate-research-primer-worksheet-007.json` | Original RCT critical-appraisal worksheet | M0 |
| `tasks/patient-advocate-research-primer-walkthrough-008.json` | Annotated walkthrough of ONE licence-verified OA RCT paper | M0 |
| `tasks/patient-advocate-research-primer-module-101.json` | Module: evidence hierarchy & levels of evidence | M1 |
| `tasks/patient-advocate-research-primer-module-102.json` | Module: clinical-trial phases (I-IV) & what each can/can't show | M1 |
| `tasks/patient-advocate-research-primer-module-103.json` | Module: endpoints — OS vs PFS vs ORR vs surrogate/biomarker | M1 |
| `tasks/patient-advocate-research-primer-module-104.json` | Module: statistics for appraisal — HR, CI, absolute vs relative risk, NNT, p-values & misuse | M1 |
| `tasks/patient-advocate-research-primer-glossary-105.json` | Methodology glossary seed (>= 60 terms, original defs + provenance) | M1 |
| `tasks/patient-advocate-research-primer-worksheet-201.json` | Worksheet: early-phase / single-arm studies | M2 |
| `tasks/patient-advocate-research-primer-worksheet-202.json` | Worksheet: observational / cohort studies (confounding focus) | M2 |
| `tasks/patient-advocate-research-primer-worksheet-203.json` | Worksheet: systematic reviews & meta-analyses | M2 |
| `tasks/patient-advocate-research-primer-module-204.json` | Module: bias, confounding & conflicts of interest | M2 |
| `tasks/patient-advocate-research-primer-module-205.json` | Module: press release vs paper — spotting hype | M2 |
| `tasks/patient-advocate-research-primer-walkthrough-206.json` | >= 3 annotated walkthroughs across study types (licence-verified OA) | M2 |
| `tasks/patient-advocate-research-primer-site-301.json` | Accessible static site (WCAG 2.1 AA) + persistent footers | M3 |
| `tasks/patient-advocate-research-primer-print-302.json` | Printable/offline worksheet pack (PDF) | M3 |
| `tasks/patient-advocate-research-primer-eval-303.json` | Pre/post evaluation instrument (appraisal rubric + confidence survey) | M3 |
| `tasks/patient-advocate-research-primer-a11y-304.json` | Accessibility + readability audit (automated + manual) | M3 |
| `tasks/patient-advocate-research-primer-i18n-305.json` | Localisation hooks (content extraction, no translation yet) | M3 |
| `tasks/patient-advocate-research-primer-pilot-401.json` | Pilot with >= 1 advocacy org + measure outcome metrics 1-3 | M4 |
| `tasks/patient-advocate-research-primer-report-402.json` | Publish pilot findings + corrections incorporated | M4 |
| `tasks/patient-advocate-research-primer-maint-403.json` | Maintenance + re-review cadence + licence re-verification plan; tag v1.0 | M4 |
| `tasks/patient-advocate-research-primer-module-501.json` | Module: reading a trial registry record / protocol | Backlog |
| `tasks/patient-advocate-research-primer-module-502.json` | Module: diagnostic & biomarker test appraisal (sensitivity/specificity/PPV) | Backlog |
| `tasks/patient-advocate-research-primer-i18n-503.json` | Full translation of vetted content (high-risk; needs translation review) | Backlog |
| `tasks/patient-advocate-research-primer-walkthrough-504.json` | Disease-specific walkthrough set | Backlog |
| `tasks/patient-advocate-research-primer-facilitator-505.json` | Facilitator/workshop guide for advocacy orgs | Backlog |
