# Project SHIELD PCB

PCB design archive for Project SHIELD, a multi-sensor safety data-acquisition (DAQ) device. The design archives include KiCad schematic, PCB, footprint, and symbol assets for an IMU, microphone, photodiode, pressure sensor, temperature sensor, and vibration sensor.

## Contents

The repository stores its design files in four ZIP archives. `project shield.zip` and `project shield (4).zip` contain KiCad project files. `project shield (5).zip` and `project shield (10).zip` additionally contain fabrication artifacts, including Gerbers, drill files, a BOM, and a component-placement (CPL) CSV.

## Tools and use

Use [KiCad](https://www.kicad.org/) to inspect or modify the design:

1. Extract one of the committed archives, such as `project shield (5).zip`.
2. Open its `project shield.kicad_pro` file in KiCad.
3. Open the associated schematic (`.kicad_sch`) or board (`.kicad_pcb`) from the project.

This checkout does not contain firmware or Python source, so it cannot be run as a data logger. The included Gerber, drill, BOM, and CPL files are fabrication outputs rather than executable code.

## Credits and related work

Project SHIELD is a team project. My contributions were sensor-PCB design and Python paired-dataset logging pipelines; the Python pipeline source is not included in this PCB checkout.

Related project repositories:

- Firmware: [Houserz/Shield](https://github.com/Houserz/Shield)
- Binary-to-CSV conversion: [samkorostov/shield-data](https://github.com/samkorostov/shield-data)
- ML fault detection: [samkorostov/shield-model](https://github.com/samkorostov/shield-model)
- Telemetry dashboard: [samkorostov/shield-server](https://github.com/samkorostov/shield-server)

Supporting hardware-validation repositories of mine: `Faraday-Cage-design-` and `shaker-table-test`.
