This repository contains only the changed files from the original v1.14.0 PX4 autopilot firmware to support the following:
- custom parameters (handled within the battery_status module yaml file)
- modified common.xml, showing how to convert existing mavlink messages (debug_vect in this case) into your own message
- multiple debug_array message instances with custom names (change as desired)

Simply drop this file into your existing PX4 autopilot folder and it will automatically overwrite the necessary files.
