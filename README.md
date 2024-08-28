This repository contains only the changed files from the original v1.14.0 PX4 autopilot firmware to support the following:
- custom parameters (handled within the battery_status module yaml file)
- modified common.xml, showing how to convert existing mavlink messages (DebugVect in this case) into your own message
- multiple DebugArray message instances with custom names (change as desired)
- disabled internal px4fmu files to enable MATLAB/Simulink -- PX4 safety support through QGroundControl
- reduced firmware build size (on fixedwing build target) with 11 modules disabled

Simply drop this file into your existing PX4 autopilot folder and it will automatically overwrite the necessary files. After performing a re-build of the firmware, Simulink will recognize the new DebugArray instances.
