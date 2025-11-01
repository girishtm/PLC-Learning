# Automated Vial Filling System — PLC Project
**Author:** Girish Thammadahlli Maruthi  
**Course:** PLC Programming Training (Internshala)  
**Status:** Completed

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
- `flowchart.svg` — vertical process flowchart
- `ladder_logic/` — ladder screenshots & tag lists
- `io_list.csv` — I/O mapping
- `docs/` — test plan and safety notes
- `simulation/demo.mp4` — optional process demo

## I/O examples
`I0.0` — Start Button  
`Q0.1` — Conveyor Motor  
(See `io_list.csv` for complete mapping)

## How to view
- Flowchart: open `flowchart.svg`
- Ladder logic: view `ladder_logic/ladder_screenshots/`

## Design assumptions & safety
See `docs/safety_assumptions.md`. Important: real vaccine production requires regulatory specs which are **not** provided here — this is a training simulation only.

## License
MIT License — see `LICENSE`

## Contact
Author: Girish Thammadahalli Maruhti. 
girishtm44@gmail.com
This folder will contain my PLC project files..
