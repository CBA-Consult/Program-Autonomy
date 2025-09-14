# Core Analysis — Prioritized Actions

This file converts recommendations into prioritized, timeboxed actions that can be imported into the RTM and executed by the program team.

Format: REQ ID | Short action | Owner | ETA | Priority | Acceptance criteria

REQ-001 | Create Epic & user story, wire into backlog | Product Owner | 3d | High | Story exists in backlog and links to EPIC-XXX; acceptance-tests.md anchor referenced.

REQ-002 | Draft technical spike for energy-harvest model validation | Lead Systems Engineer | 7d | High | Spike report with data and go/no-go recommendation.

REQ-003 | Define telemetry schema & PII rules | Data Engineer | 10d | Medium | Telemetry spec published; demo ingestion receiving synthetic data.

REQ-004 | EMC compliance scoping & lab bookings | Compliance Engineer | 10d | High | Compliance plan with test list and booked lab slots.

REQ-005 | Pilot BOM and mechanical interface pack | Program Engineering Lead | 14d | Medium | Integration package created and reviewed by OEM/vehicle engineering.

REQ-006 | IP/FTO short-run search and risk register | Legal / IP Lead | 7d | High | Preliminary FTO findings and risk register submitted.

REQ-007 | Create acceptance-test artifacts (anchors) | QA Lead | 4d | High | Acceptance-tests.md contains anchors and test steps for REQ-007.

REQ-008 | Build sprint-0 Jira import CSV for high-priority stories | Product Owner | 5d | High | `jira-import-userstories.csv` validated and ready for import.

REQ-009 | Spike: mechanical vibration/durability test plan | Test Engineer | 10d | Medium | Vibration test plan and sample schedule with pass/fail criteria.

REQ-010 | Define software update and security patch process | DevOps Lead | 7d | Medium | Documented update process and initial CI/CD pipeline sketch.

REQ-011 | Supplier readiness checklist (APQP intro) | Procurement / Program Engineering | 14d | Medium | APQP checklist draft stored in `generated-documents/basic-docs/appendices/`.

REQ-012 | Pilot data privacy & consent flow | Data / Legal | 7d | Medium | Privacy flow documented and consent templates created.

Cross-cutting tasks
- Add owners and ETA columns to `rtm-requirements-to-epics.csv`. Owner: PMO. ETA: 3d.
- Review and finalize `jira-import-userstories.csv` by mapping Epic IDs or placeholders. Owner: Product Owner. ETA: 3d.

How to use
- Convert each row above into a sprint backlog item; assign to the named owner and set the ETA as the target sprint.
- For high-risk spikes, treat them as blocking tasks; do not schedule dependent work until the spike outcome is recorded.

Contact & escalation
- PMO: Menno Drescher (Project Manager)
- Product Owner: (provide)

---
This artifact is intended as a practical handoff from analysis to delivery. After you confirm owners and ETAs I can update the RTM CSV and generate an updated Jira import file.
