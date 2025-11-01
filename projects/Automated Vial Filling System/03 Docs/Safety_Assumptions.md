# Safety & Design Assumptions (Educational Project)

**Important:** This repository is an educational simulation and is NOT certified for real vaccine production or regulatory use.

## Main assumptions
1. Environmental ranges (temperature, humidity, microbe thresholds) are placeholders — real values must be provided by a qualified process engineer.  
2. All emergency-stop and interlock hardware are present and wired per plant safety standards. This project only models logic-level behavior.  
3. Robot, filler, and conveyor speeds are assumed safe for the devices used; physical integration requires mechanical validation.  
4. Vision system is simplified: camera outputs a pass/fail boolean. Real vision pipelines require exception handling and image storage.  
5. Electrical ratings, grounding, and PPE roles are out of scope.

## Safety recommendations
- Implement hardware interlocks and safety-rated PLC outputs for all actuators.
- Use a safety PLC or safety module for Emergency Stop and personnel protection.
- Perform FMEA before real deployment.
