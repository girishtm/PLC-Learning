# Automated Vial Filling System — PLC Project
**Author:** Girish Thammadahlli Maruthi  
**Course:** PLC Programming Training (Internshala)  
**Status:** Completed

## Disclaimer: 
This project is an educational simulation for PLC training only. It is not certified for production or regulatory use. Do not use this design in a live vaccine line without qualified engineering and regulatory approval.

## Overview
This project implements ladder logic and system documentation for an automated vial filling system for bulk vaccine production. The system covers sterile-environment monitoring, HVAC purge, automated filling (20-vial batches), capping, sealing, leakage inspection, washing, drying, labeling and packaging counters.

## Key features
- Sterile environment monitoring (microbe sensors, temperature, humidity)
- Automated HVAC purge (10 minutes) and pumps for line pressurization
- Robot-assisted loading and 20-station parallel filling/capping/sealing
- Vision-based leakage detection & reject actuator
- Batch & production counters (20-batch counter; 50,000/day target)
- I/O mapping, ladder logic screenshots, flowchart, and test plan included

## File structure
See repository root for:
- `flowchart.png` — vertical process flowchart
- `ladder_logic/` — ladder screenshots & tag lists
- `docs/` — test plan and safety notes
- `simulation/demo.mp4` — optional process demo

## How to view
- Flowchart: open `flowchart.svg`
- Ladder logic: view `ladder_logic/ladder_screenshots/`

## Design assumptions & safety
See `safety_assumptions.md`.

## Ladder Logic Simulation
https://github.com/user-attachments/assets/35695e7e-1995-48d9-b08f-4eba1eb3d663

## Contact
Author: Girish Thammadahalli Maruhti. 
girishtm44@gmail.com
This folder will contain my PLC project files..

