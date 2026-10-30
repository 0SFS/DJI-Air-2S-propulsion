# DJI Air 2S propulsion

Declarative engine mod `0sfs/dji-air2s-propulsion`. The `DJI-Air-2S` airframe depends on this mod and selects engine `dji-air2s-propulsion` through `quad.propulsionId`.

This repository owns the physical motor speed response and propeller specification consumed by `multirotor`, plus the acoustic calibration passed to `0SFS/electric-sound`. Rotor count, hub positions, directions and installation belong to the airframe. The sound host combines physical geometry and acoustic calibration without copying the physical values into another profile.

The electric source uses each rotor's simulated speed, thrust, shaft torque and inflow. Motor electromagnetic parameters and recordings are not supplied; the sound is an uncalibrated procedural approximation.

The engine has no native JSBSim combustion engine, start property or fuel telemetry.

Topics: `0sfs-mod` and `0sfs-engine-mod`. [Modding guide](https://github.com/0SFS/docs/blob/main/modding.md) describes discovery and installation.
