# Test Plan

## Objective
Validate sequence correctness, I/O mapping, counters, reject logic and emergency handling.

## Tests
1. **Startup & Purge**
   - Simulate `Start_Button` pressed.
   - Verify HVAC_Coil turns ON for 10 minutes.
   - Verify microbe/temp/humidity sensors must report OK before continuing (simulate OK=true).

2. **Line Pressure**
   - Confirm `Pumps` start and reach line pressure (simulate pressure OK via a boolean flag).

3. **Robot Loading**
   - Simulate `Robot_Loader` performing load; verify dosing chamber full flag.

4. **Filling Batch (20)**
   - Simulate vials on conveyor (Vial_Present_Sensor triggers).
   - Start conveyor and stop at filling station.
   - Verify `Filler_Valves_Bank` triggers and fills exactly 20 vials (batch counter CT0 increments to 20).

5. **Capping & Sealing**
   - Simulate vacuum gripper and force sensor I0.1 for tightening.
   - If Force_Sensor_Cap fails, report error and mark vial for rework.

6. **Leakage Inspection**
   - Simulate Camera_Pass true/false.
   - If false, `Reject_Actuator` must remove vial.

7. **Drying & Labeling**
   - Verify `Air_Blower` and `Label_Applicator` triggers at correct timing.

8. **Counters**
   - Simulate continuous filling until `Daily_Counter` CT1 reaches configured threshold (e.g., 50,000) to test stop condition.

9. **Emergency Stop**
   - At random points, trigger `Emergency_Stop` and verify immediate cessation of outputs and safe state.

## Acceptance Criteria
- All process sequences occur in the correct order.
- Counters increment correctly and reset per batch rules.
- Safety stoppage works reliably.
