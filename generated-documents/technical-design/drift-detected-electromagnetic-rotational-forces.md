# DRIFT DETECTED — Electromagnetic & Rotational Forces Harvesting (Railway and Domestic Appliances)

Status: drift detected — moved out of core SCEV scope for separate tracking and analysis.

## Summary
During literature review and ideation, several harvesting opportunities were identified that rely on rotational forces but are not directly aligned with the SCEV product scope. Notable examples include railway axle/track-side harvesting concepts and harvesting from domestic laundry equipment (washing machines and tumble dryers). These ideas are recorded here to capture the drift, assess risk/benefit, and recommend whether to pursue them in a separate R&D stream.

## Why this is scope drift
- Different operational environment: railway systems are governed by rail safety, infrastructure owners, and long asset lifecycles.
- Different product constraints: domestic appliances present distinct maintenance, regulatory, and user-safety profiles versus road vehicles.
- Divergent business models and customers: infrastructure operators and appliance OEMs are different buyers than vehicle OEMs or fleet operators.

## Items observed
- Railway rotational-harvesting concepts
  - Target: axle-mounted or wayside devices that harvest energy from wheel rotation, vibrations, or regenerative braking.
  - Considerations: high mechanical loads, harsh environment, certification for trackside equipment, integration with signalling and telecom systems.
  - SCEV relevance: low — engineering and certification paths differ substantially from road vehicle electrical subsystems.

- Washing machine / tumble dryer rotational harvesting
  - Target: capture energy from drum rotation, imbalanced-load vibrations, or clutch/drive components.
  - Considerations: low absolute power per device, user-safety and ingress concerns, economics dominated by appliance lifecycle and retrofit complexity.
  - SCEV relevance: peripheral — technically interesting but not directly transferable to vehicle platforms without significant rework.

## High-level assessment
- Feasibility: medium (railway) / low (domestic appliances) for meaningful, repeatable power delivery compared to vehicle-scale needs.
- Impact on SCEV objectives: limited — these areas are unlikely to deliver repeatable, vehicle-grade self-charging improvements in the near term.
- Resource risk: high if pursued within the same R&D track (diverts focus, requires different domain expertise and certifications).

## Recommendation
1. Track these as a separate R&D thread labelled `drift:rotational-harvest` with a lightweight intake card per idea (owner, expected power, environment, certification needs). Do not allocate core SCEV sprint capacity to these items.
2. For each candidate (railway, appliance), capture a one-page technical feasibility note and estimated effort (person-weeks) before any prototyping.
3. If compelling cross-over opportunities are identified (for example, technologies or materials that can be shared with vehicle systems), create a clear transfer plan and gate decisions on technical metrics relevant to SCEV (power density per kg, reliability, environmental robustness).

## Suggested triage fields (for PMO register)
- id, title, owner, proposed start, expected deliverables, estimated effort (pw), regulatory risk, SCEV-transfer-score (0-10), status

## Next steps
- Create intake cards in the PMO tracker for: (a) Railway axle/wayside harvesting, (b) Washing machine drum harvesting, (c) Tumble dryer vibration harvest.
- Assign a technical reviewer to each card and require a 2-week desktop feasibility review before committing to prototypes.

---

File created to record the drift and prevent scope creep. If you want me to convert the intake lines to CSV/JSON and add them to the `pmo-ip-register.csv`, I can do that next.
