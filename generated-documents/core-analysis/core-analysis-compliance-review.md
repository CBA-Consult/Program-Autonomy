# Core Analysis — Compliance Review (PMBOK / DMBOK / BABOK)

Status: draft — generated on 2025-09-13 after review of core-analysis documents.

## Overview
This review assesses the `generated-documents/core-analysis` documents for alignment with three industry guidance sets:
- PMBOK (Project Management Body of Knowledge) — focus on project lifecycle, processes, inputs/outputs, change control, scope, and closure.
- DMBOK (Data Management Body of Knowledge) — focus on data governance, data quality, metadata, data architecture, and operational data management.
- BABOK (Business Analysis Body of Knowledge) — focus on requirements elicitation, traceability, stakeholder analysis, and solution evaluation.

For each core-analysis document we provide: a short compliance assessment, gaps, and recommended remediation steps prioritized by effort and impact.

---

## Files reviewed
- `collect-requirements.md`
- `develop-project-charter.md`
- `close-project-phase-process.md`
- `control-scope-process.md`
- `validate-scope-process.md`
- `perform-integration-change-control-process.md`
- `monitor-and-control-project-work.md`
- `key-roles-and-needs.md`
- `personas-assess-motivations.md`
- `user-personas.md`
- `program-autonomy-purpose.md`
- `strategic-business-case.md`

---

## High-level findings
- PMBOK alignment: Core PMBOK processes are present (charter, scope control, validate/close, integrated change control, monitoring). However, several documents are high-level and lack explicit artifacts, templates, and traceable IDs that PMBOK recommends for rigorous execution (e.g., a RACI, a change log template, baseline scope statement, and formal acceptance checklists).
- DMBOK alignment: Data requirements and governance are mentioned (APIs, exports, analytics) but lack formal DMBOK artifacts: no data glossary, no data quality rules, no metadata management plan, and no data stewardship assignments.
- BABOK alignment: Requirements elicitation is thorough in collection, but requirements aren't consistently expressed with unique IDs, prioritization, or formal acceptance criteria mapped to testable conditions. Persona usage is strong but could connect more tightly to job stories and acceptance tests.

---

## Per-file findings & remediation

### collect-requirements.md
- PMBOK: Good coverage of elicitation approaches. Gap: missing a requirements traceability matrix (RTM) and formal prioritization method (MoSCoW or WSJF) as an output.
- DMBOK: Mentions API and data exports but lacks data stewardship assignments, data quality rules, and glossary.
- BABOK: Good stakeholder mapping. Gap: missing explicit requirement IDs, acceptance criteria, and mapping to test cases.

Remediation (priority):
1. Create a Requirements Traceability Matrix (REQ-ID → Persona → Epic → Acceptance Criteria → KPI).
2. Add a prioritization policy (MoSCoW or WSJF) and record prioritization results.
3. Add data stewardship and a short data glossary section.

Estimated effort: 2-4 person-days.

### develop-project-charter.md
- PMBOK: Satisfies charter basics. Gap: missing RACI for key deliverables and a high-level milestone acceptance criteria table.
- DMBOK/BABOK: N/A (minimal data/business analysis content).

Remediation (priority):
1. Add a RACI matrix for project governance.
2. Include a milestone acceptance criteria table for gates.

Estimated effort: 1 person-day.

### close-project-phase-process.md
- PMBOK: Captures key activities. Gap: missing formal 'Lessons Learned' template and a post-implementation review checklist.
- DMBOK: Ensure data archiving and retention policies are referenced.

Remediation:
1. Add a Lessons Learned template and archive checklist referencing data retention policy.

Estimated effort: 0.5-1 person-day.

### control-scope-process.md
- PMBOK: Good high-level activities. Gap: missing baseline scope statement, variance thresholds, and scope-change decision criteria.

Remediation:
1. Add scope baseline excerpt and variance thresholds (e.g., >5% schedule variance triggers steering committee).
2. Add decision authority table for scope changes.

Estimated effort: 1-2 person-days.

### validate-scope-process.md
- PMBOK: Describes acceptance but lacks formal acceptance checklists and sign-off templates.
- BABOK: Suggest mapping deliverables to requirements and including test pass-fail criteria.

Remediation:
1. Add deliverable acceptance checklist template and sign-off record.
2. Add mapping of deliverables → requirement IDs used in acceptance testing.

Estimated effort: 1 person-day.

### perform-integration-change-control-process.md
- PMBOK: Process present. Gap: missing a change log template and explicit change evaluation criteria (cost/time/impact matrix).

Remediation:
1. Add change log template and change impact scoring matrix.
2. Define approval thresholds (e.g., PM, PMO, Steering Committee) based on impact.

Estimated effort: 1-2 person-days.

### monitor-and-control-project-work.md
- PMBOK: Good list of activities. Gap: lack of explicit metrics to monitor (KPIs) and no sample report templates.
- DMBOK: Include data quality monitoring if analytics are in scope.

Remediation:
1. Include a set of recommended KPIs (Schedule performance index, Cost performance index, Feature throughput, Mean time to restore) and dashboard mockup.
2. Add data quality KPIs and monitoring frequency.

Estimated effort: 1-2 person-days.

### key-roles-and-needs.md
- BABOK: Strong stakeholder coverage. Gap: missing formal stakeholder engagement plan and RACI mapping.

Remediation:
1. Add stakeholder engagement plan (communication frequency, channels, escalation paths).
2. Add RACI for key deliverables.

Estimated effort: 1 person-day.

### personas-assess-motivations.md & user-personas.md
- BABOK: Personas are well-developed. Gap: need job stories and acceptance tests per persona, and mapping to requirements.

Remediation:
1. Create 2-3 prioritized job stories per key persona and attach acceptance tests.
2. Cross-link personas to requirements in the RTM.

Estimated effort: 2-4 person-days.

### program-autonomy-purpose.md & strategic-business-case.md
- PMBOK: Strategic alignment is present. Gap: missing measurable benefit metrics, financial assumptions, and sensitivity analysis.
- DMBOK: Financial/market data sources should be documented and governed.

Remediation:
1. Add measurable benefit metrics (e.g., TCO reduction %, energy savings kWh/year per vehicle) with assumptions.
2. Add sensitivity/what-if analysis and data source citations.

Estimated effort: 2-3 person-days.

---

## Consolidated remediation plan (30/60/90-day)
- 0-30 days (quick wins)
  - Add RTM template and start mapping top 20 requirements. (REQ-ID convention)
  - Add RACI to project charter and key roles doc.
  - Add acceptance checklist templates to validate/close docs.
- 30-60 days (medium)
  - Define KPIs and dashboard templates for monitoring and reporting.
  - Build PMO intake templates and add triage rules.
  - Draft data glossary and assign data stewards for critical datasets.
- 60-90 days (deeper)
  - Complete requirements-to-epics mapping and backlog integration.
  - Run stakeholder workshops to validate job stories and acceptance tests.
  - Implement change log and impact scoring into the PMO process.

---

## Annex: Suggested templates to include (file names)
- `core-analysis/rtm-requirements-to-epics.csv`
- `core-analysis/project-charter-raci.md`
- `core-analysis/acceptance-checklist-template.md`
- `core-analysis/change-log-template.md`
- `core-analysis/pmo-intake-template.md`
- `core-analysis/data-glossary.md`

---

If you want, I can now generate the first artifact: `rtm-requirements-to-epics.csv` drafted from `collect-requirements.md` with auto-generated IDs and a first-pass mapping. Or I can append the top recommendations to the PMO register CSV. Tell me which you'd like next.