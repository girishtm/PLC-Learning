# 🧩 Automated Vial Filling System – Simulation Explanation

This simulation demonstrates the complete automated vial filling process for bulk vaccine production, controlled by a PLC ladder logic program.

---

## 🟢 Step 1 – System Initialization
- The operator presses the **Start push button** to begin the process.  
- The **HVAC system** activates to purify and pressurize the air in the sterile environment.  
- It runs for 10 minutes (simulated with a timer).  
- After completion, the **microbe detection**, **temperature**, and **humidity sensors** check the air quality.  
- Only when all sensors confirm safe conditions does the process continue.

---

## 🟢 Step 2 – Line Preparation
- The filling lines are automatically purged to remove any contamination.  
- The **pumps** are turned ON to build line pressure.  
- Once stable, the **robot arm** moves into position to load the bulk vaccine into the dosing chamber.

---

## 🟢 Step 3 – Vial Filling Cycle Begins
- The operator starts the cycle, and the **conveyor** begins moving empty vials toward the washing station.  
- At the washing station, **high-pressure sprinklers** clean the vials before filling.

---

## 🟢 Step 4 – Vaccine Filling Station
- The conveyor stops when a batch of 20 vials reaches the filling station.  
- **Dispensing valves and pumps** fill each vial with the required quantity of vaccine.  
- A timer ensures consistent filling time across all vials.  
- Once filling completes, the conveyor restarts automatically.

---

## 🟢 Step 5 – Capping and Tightening Station
- The filled vials reach the **capping station**, where the conveyor stops.  
- A **vacuum gripper** picks up caps and places them on the vials.  
- The vials then move to the **tightening station**, where a **load actuator** applies pressure to tighten the caps.  
- A **force sensor** ensures proper sealing before continuing.

---

## 🟢 Step 6 – Leakage Test and Rejection
- **Camera sensors** inspect each vial for leakage or defects.  
- If a defect is found, a **reject actuator** diverts the vial away.  
- Only defect-free vials continue in the line.

---

## 🟢 Step 7 – Drying and Labeling
- The vials move through **air blowers** to remove moisture and ensure complete drying.  
- The conveyor rotates the vials by 180° for uniform drying.  
- At the labeling station, **label applicators** apply labels to each vial.

---

## 🟢 Step 8 – Counting and Packaging
- A **batch counter** keeps track of every 20-vial group completed.  
- Once 100 vials are processed, they move to the **packaging system**.  
- A **production counter** maintains the total daily output, targeting 50,000 vials per day.

---

## ⚙️ Automation Logic Overview
- The ladder logic uses **timers**, **counters**, and **conditional control** to manage sequence flow.  
- Each phase is interlocked with sensor feedback to ensure safe and consistent operation.  
- The process runs continuously in batches, maintaining automation, hygiene, and production efficiency.

---

## 🧠 Simulation Outcome
The simulation successfully demonstrates:
- End-to-end automation of vial filling, capping, and sealing.  
- Use of interlocks for safety and sequencing.  
- Parallel batch processing of 20 vials at multiple stages.  
- Continuous operation aimed at high-volume vaccine production.

---

## ✅ Conclusion
This PLC simulation showcases a realistic automation scenario combining mechanical motion, robotic handling, and process control—ensuring efficiency, safety, and scalability in vaccine production.

---
