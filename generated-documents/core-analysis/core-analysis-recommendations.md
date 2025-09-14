# Core Analysis — Recommendations and Prioritized Actions

Status: draft — generated after review of core-analysis documents.

## Executive summary
The `generated-documents/core-analysis` collection is thorough and aligns well with PMBOK processes, personas, and requirement collection for the SCEV (Self-Charging Electric Vehicle) Program Autonomy initiative. To increase delivery velocity and investor-readiness, focus on a small set of high-impact changes: strengthen traceability, operationalize requirements into epics and measurable KPIs, create a prioritized roadmap with acceptance gates, and centralize the PMO intake and triage process.

## Summary of suggested improvements (prioritized)

### 1) Strengthen requirements traceability and measurable acceptance

## Implementation plan — prioritized actions

1) Stabilize traceability (High priority)
- Action: Finalize Epic mappings for all REQs in `rtm-requirements-to-epics.csv` and add acceptance-test links. Owner: PMO / Business Analyst. ETA: 5 working days.
- Outcome: Every requirement row contains a valid `epic_id` and `acceptance_test_link` that references `generated-documents/core-analysis/acceptance-tests.md` anchors.

2) Create implementation backlog (High priority)
- Action: Convert high-priority REQs (priority=High) into user stories and sub-tasks in the backlog; produce a compact Jira import CSV for sprint 0. Owner: Product Owner. ETA: 7 working days.
- Outcome: `generated-documents/core-analysis/jira-import-userstories.csv` reviewed and finalized; import-ready with Epic links.

3) Technical validation spikes (Medium priority)
- Action: Open 2–3 timeboxed technical spike tickets to validate assumptions in `electromagnetic-induction-energy-generation.md` and hardware integration notes (duration 5–10 days each). Owner: Lead Systems Engineer. ETA: 2 weeks.
- Outcome: Spike reports with measurable pass/fail criteria and recommended next steps.

4) Compliance & EMC plan (High priority)
- Action: Draft a minimum-compliance plan (safety, EMC, functional safety alignment) and map required lab tests and standards. Owner: Compliance Engineer. ETA: 10 working days.
- Outcome: Compliance matrix and lab booking plan; list of required certificates and test criteria.

5) Pilot preparation and APQP inputs (Medium priority)
- Action: Prepare pilot BOM, mechanical interface pack, and APQP checklist entries for early supplier engagement. Owner: Program Engineering Lead. ETA: 3 weeks.
- Outcome: Pilot integration package and APQP checklist itemized for the pilot scope.

6) Data & telemetry readiness (Medium priority)
- Action: Define telemetry schema, ingestion pipeline, and privacy rules for pilot telemetry. Owner: Data Engineer. ETA: 10 working days.
- Outcome: Telemetry spec and minimal cloud ingestion demo-ready service.

7) IP & FTO actions (High priority)
- Action: Produce a short IP/FTO action list (who to contact, what searches remain, cost estimate). Owner: Legal / IP Lead. ETA: 7 working days.
- Outcome: IP risk register and recommended next steps for freedom-to-operate.

## Progress tracking
- Add the prioritized actions to `generated-documents/core-analysis/core-analysis-prioritized-actions.md` (created alongside this file) and update `rtm-requirements-to-epics.csv` with owners and ETAs where appropriate.

## Acceptance criteria for this implementation plan
- All high-priority items have owners and clear ETAs.
- RTM contains Epic IDs for all requirements marked high or medium priority.
- Pilot integration package and APQP checklist exist as living documents in `generated-documents/basic-docs/appendices/`.

## Next steps
- Create `core-analysis-prioritized-actions.md` with per-REQ actions, owners, ETAs, priority, and acceptance criteria.
- Run a 2-hour mapping workshop to convert top 20 requirements into epics and acceptance criteria (deliverable: `requirements-to-epics.csv`).
- Create a lightweight roadmap draft and milestone gates (`roadmap-gates.md`).
- Add the PMO intake rows for top recommendations into `pmo-ip-register.csv` and schedule triage.

---

If you want, I can now:
- create `requirements-to-epics.csv` draft from the existing `collect-requirements.md` (auto-generate IDs and a first-pass mapping),
- or convert the top recommendations into PMO CSV rows and append them to the PMO register.

Which should I do next? (I suggest starting with the requirements-to-epics mapping.)
