# 🧪 Automated Vial Filling System — PLC Project

**Author:** Girish Thammadahlli Maruthi  
**Course:** PLC Programming Training (Internshala)  
**Status:** ✅ Completed  

---

## ⚠️ Disclaimer  
This project is an **educational PLC simulation** created for training purposes only.  
It is **not certified for industrial or medical production use**.  
Do **not** apply this logic or design in live vaccine filling lines without qualified engineering validation and regulatory approval.

---

## 📘 Overview  
This project simulates an **Automated Vial Filling System** designed for bulk vaccine production.  
It covers critical steps from **sterile environment monitoring** to **packaging**, representing a compact industrial automation model using **PLC ladder logic**.

### 🔹 System Workflow Includes:
- Sterile environment monitoring (microbe sensors, temperature, humidity)
- Automated **HVAC purge (10 minutes)** and **line pressurization**
- **Robot-assisted vial loading** into a 20-station filling system
- **Automated capping, tightening**, and **vision-based leakage detection**
- **Reject actuator** for faulty vials
- **Batch & production counters** (20-vial batches; 50,000/day target)

---

## 🧩 File Structure
| File | Address | Description |
- `00 README.md` | projects/Automated Vial Filling System/00_README.md | This documentation file |
- `01 Safety_Assumptions` | projects/Automated Vial Filling System/01_Safety_Assumptions.md | Contains system-level safety assumptions and conditions |
- `02 Test_Plan` | projects/Automated Vial Filling System/02_Test_Plan.md | Detailed plan for testing each PLC logic stage |
- `03_Flowchart.png` | projects/Automated Vial Filling System/03_Flowchart.png | Process flowchart showing each automation stage |
- `04_Ladder_Diagram.pdf` | projects/Automated Vial Filling System/04_Ladder_Diagram.pdf | Ladder logic screenshots and tag references |
- `05_Simulation.md` | projects/Automated Vial Filling System/05_Simulation.md | Screen recording of simulation in PLC simulator |
- `06_Simulation_Explanation.md` | projects/Automated Vial Filling System/06_Simulation_Explanation.md | Step-by-step explanation of simulation sequence |

---

## 🧰 Tools Used
- **PLC Simulator:** Online PLC Ladder Logic Simulator  
- **PLC Software:** Ladder Logic (IEC 61131-3 Standard)  
- **Diagram Tools:** Draw.io / Lucidchart  
- **Documentation:** Markdown, PDF, and PNG assets

---

## ▶️ Ladder Logic Simulation
[Watch the Simulation Video](https://github.com/user-attachments/assets/35695e7e-1995-48d9-b08f-4eba1eb3d663)

This video demonstrates the real-time logic sequence in the PLC simulator:
1. **Startup & System Purge**
2. **Sterile Environment Checks**
3. **Line Pressurization & Valve Control**
4. **Vial Loading & Filling**
5. **Capping & Sealing**
6. **Leak Inspection & Reject Handling**
7. **Batch Completion & Counter Increment**

---

## 🧠 Design Assumptions & Safety
Refer to:  
- `01 Safety_Assumptions.md` → Operator and hardware safety measures  
- `02 Test_Plan.md` → Verification steps for each ladder segment  

---

## 📫 Contact
**Author:** Girish Thammadahlli Maruthi  
📧 Email: [girishtm44@gmail.com](mailto:girishtm44@gmail.com)  
📂 Repository: [PLC-Learning](https://github.com/girishtm/PLC-Learning)

---

> _“Automation is not just about control — it’s about precision, safety, and consistency.”_  
> — *Girish Thammadahlli Maruthi*
