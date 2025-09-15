# Needs & Requirements — Causes, Signals and Derived Program Needs

Purpose
- Capture the observable signals and root causes that justify the SCEV program and define high‑level needs and requirements for prioritisation, scoping and acceptance.

1. Signals (what we observe)
- Market signals: rising energy prices, fleet demand for lower operating cost, OEM interest in differentiation.
- Customer signals: range anxiety, desire for resilience (backup power), preference for lower total cost of ownership.
- Regulatory signals: emissions targets, incentives for distributed energy resources, evolving grid interop standards.
- Technical signals: maturity of PV, hub‑integrated harvesters, advanced BMS and bidirectional charging prototypes.
- Operational signals: depot charging constraints, demand charges, high vehicle utilization patterns.
- Internal signals: IP opportunities, partner interest, available in‑house expertise (ML, power electronics).

2. Root Causes (why the signals exist)
- Electricity cost volatility and higher peak tariffs.
- Limitations of current vehicle range and charging infrastructure.
- Grid and market transitions emphasizing distributed flexibility.
- Technological fragmentation: components mature independently but lack integrated systems.
- Business model gaps: fleet economics sensitive to downtime and demand charges.
- Regulatory complexity requiring coordinated certification and standards engagement.

3. Derived Needs (what the program must deliver)
- Technical needs: validated energy harvesting subsystems (Solari, Kinetix), robust BMS (Guardian), and bidirectional hardware (Nexus).
- Systems needs: integrated IPMS (Synapse) for orchestration and energy optimisation.
- Safety & compliance: certification pathways, EMC, functional safety evidence.
- Commercial needs: demonstrable ROI for target segments, clear GTM for fleets and OEMs.
- Data & governance: telemetry schema, data privacy controls, model lifecycle management.
- Operational needs: depot integration patterns, maintenance processes, supply chain readiness.

4. High‑Level Requirements
- Functional
  - R1: Vehicle shall support bidirectional charging to enable V2H (Nexus).
  - R2: System shall harvest and record kWh generated per subsystem with ±10% accuracy.
  - R3: IPMS shall optimise energy flows based on telemetry, driver intent and grid signals.
- Non‑Functional
  - N1: Safety: No autonomous actuator commands from unvalidated models; human/independent safety controller required.
  - N2: Reliability: Prototype system MTBF target > X hours (define per subsystem).
  - N3: Performance: Bidirectional round‑trip efficiency target ≥ A% (pilot goal).
  - N4: Privacy: Telemetry anonymisation and consent controls by design.

5. Stakeholders & Owners
- Program Sponsor / Board — strategic decisions
- Program Director / PMO — prioritisation, funding
- Project Leads (Solari, Kinetix, Guardian, Synapse, Nexus) — delivery of technical requirements
- Regulatory & Legal — certification and data/IP governance
- Commercial / Sales — GTM and pilots
- Simulation Lead & Lead Systems Engineer — validation tasks (ENERGY‑001, SPIKEs)

6. Acceptance Criteria & KPIs (examples)
- Measured kWh/day per vehicle consistent with lab simulations within ±15%.
- Demonstrated V2H discharge to a household load for X minutes without safety trip.
- Pilot ROI within target profile for fleet customers (scenario‑based).
- Evidence packs (model cards, test reports, ICDs) submitted for phase‑gate entry.

7. Prioritisation & Roadmap guidance
- Phase 1: Validate core subsystems (bench + sim SPIKEs), establish telemetry & safety baselines.
- Phase 2: Depot/fleet pilots to prove economics and operational procedures.
- Phase 3: Certification & scaled pilots (Nexus V2H/V2G).

8. Traceability & Artifacts
- Link each high‑level requirement to: project story, acceptance test (SPIKE/ENERGY), evidence pack, and RTM entry.
- Maintain change log for requirements and record owners and dates.

9. Recommended Next Steps (immediate)
- Create ENERGY‑001 parametric model if not complete; owner = Simulation Lead; ETA = 1 week.
- Prioritise SPIKE-001..003 for bench validation; owners = Lead Systems Engineer; Priority = High.
- Author acceptance criteria templates and attach to phase‑gate checklists in PMO.
- Rotate sensitive keys (security reminder) and ensure telemetry privacy controls before pilot data ingestion.

Appendix: terminology mapping (quick)
- Signal → Root cause → Derived need → Requirement → Acceptance test → Evidence pack
