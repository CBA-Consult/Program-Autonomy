# First-principles Energy-Balance — Sensitivity Summary

Purpose
- Provide quick, reproducible sensitivity calculations showing the mechanical force (torque equivalent) induced by harvesting power from a rolling wheel and the immediate propulsion power increase required to sustain speed.

Key formula
- F_gen (N) = P_gen (W) / v (m/s)
- Additional propulsion power required ≈ P_gen (ignoring conversion inefficiencies)

Assumptions
- Baseline example propulsion power for percent calculations: 20 kW (user-adjustable).
- Speeds: 30, 60, 100 km/h (converted to m/s in the CSV).
- P_gen sample values: 2.5, 5, 10, 20 kW.

How to use
- See energy-balance-sensitivity.csv for numeric table.
- Interpretation: additional propulsion power equals the harvested power (P_gen). Percent impact depends on vehicle baseline propulsion. Example: 5 kW harvested on a vehicle requiring 20 kW cruise power = 25% increase in propulsion demand.

Next steps (recommended)
1. Run SPIKE-001 (bench + simulation) to measure torque vs generated power and confirm conversion losses (Owner: Lead Systems Engineer; Priority: High).
2. Run SPIKE-002 and SPIKE-003 per existing spike definitions (Priority: High; Owner: Lead Systems Engineer).
3. Complete ENERGY-001 "First-principles energy-balance" task to produce a full parametric model and updated percent impacts across baseline propulsion profiles (Owner: Simulation Lead; ETA: 1 week).

Link to tests & tasks
- SPIKE-001 .. SPIKE-003 (see acceptance-tests.md anchors)
- ENERGY-001: First-principles energy-balance (created in RTM / Jira import)
- Note: Until SPIKE and ENERGY-001 are complete, do not publish payback or net-positive claims.