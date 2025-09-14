# Acceptance Tests — Requirements (anchors)

This document lists acceptance-test anchors for each requirement in `rtm-requirements-to-epics.csv`. Use these anchors for linking from the RTM.

## REQ-001
- Test: Dashboard shows live status for a sample fleet of 10 vehicles; updates within 5 seconds on simulated events.
- Pass criteria: All 10 vehicles update within 5s; scheduled charge adherence > 95% during test window.

## REQ-002
- Test: Scheduler creates charging windows and applies a simulated off-peak tariff; scheduling applies to 30 vehicles.
- Pass criteria: >90% of scheduled chargers start in off-peak window and recorded energy cost reduction > 5%.

## REQ-003
- Test: Field app records 20 jobs offline and syncs when connectivity restored; offline navigation routes correctly.
- Pass criteria: Sync success rate 100%; no data loss; navigation waypoints accurate within 100m.

## REQ-004
- Test: V2H supplies 2kW to a resistive load with safe isolation; disconnect under fault conditions.
- Pass criteria: Delivered power meets expected kW with safe disconnect within spec.

## REQ-005
- Test: Executive dashboard generates automated sustainability report; metrics align with source data.
- Pass criteria: Report available within 5 minutes; metrics reconcile with raw data within 0.5%.

## REQ-006
- Test: API returns historical and real-time data for a 24-hour period; schema matches documentation.
- Pass criteria: All endpoints return expected fields and data completeness > 99%.

## REQ-007
- Test: User profile changes persist across sessions and devices for 50 test accounts.
- Pass criteria: 98% persistence and correct preferences applied on login.

## REQ-008
- Test: OTA deployment to 5 test vehicles succeeds with rollback exercised.
- Pass criteria: 100% successful updates; rollback recovers pre-update state.

## REQ-009
- Test: Predictive alerts issued for 100 vehicles with simulated faults; recommendations provided.
- Pass criteria: Alert precision > 80% and lead time meets SLA.

## REQ-010
- Test: Automated emissions report for 10 vehicles generated and exported in CSV and PDF.
- Pass criteria: Values match source telemetry; export completes within expected timeframe.

## REQ-011
- Test: Create and process a bulk purchase order; digital warranties generated.
- Pass criteria: Order processed and warranty documents issued within expected processing time.

## REQ-012
- Test: Compliance pack prepared and reviewed for a procurement RFP simulation.
- Pass criteria: All required documents present and pass checklist review.

(These test anchors are intentionally concise; convert to formal test cases in your QA system.)

## POLICY-001
- Test: Weekly policy-watch brief produced for the 2025/2026 EU review; stakeholder positions collated and recommended program triggers identified.
- Pass criteria: Brief issued weekly for 4 consecutive weeks; at least 3 stakeholder positions tracked and a set of 3 program trigger recommendations provided.