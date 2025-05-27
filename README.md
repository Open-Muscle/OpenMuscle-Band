# OpenMuscle-Band

**Status:** Archived (Legacy Hardware)  
**License:** [CERN-OHL-S v2.0](https://github.com/Open-Muscle/OpenMuscle-Band/blob/main/LICENSE)

## Overview

The **OpenMuscle-Band** is the original prototype of the OpenMuscle project—a wearable forearm band equipped with 12 pressure sensors designed to detect muscle contractions and predict finger movements. This open-source hardware was developed to provide biometric data for machine learning applications in prosthetics and human-computer interaction.

## Hardware Specifications

- **Sensors:** 12 Hall Effect Sensors (49E) arranged in 6 dual-input sensor cells
- **Microcontrollers:** 3 × ESP32-C3 modules
- **Connectivity:** Wi-Fi (UDP transmission)
- **Sampling Rate:** Up to 1200 samples per second
- **Construction:** 3D-printed enclosures with integrated springs and magnets
- **Firmware:** MicroPython

## Repository Contents

- `BOM/`: Bill of Materials detailing all components used
- `KiCad/`: PCB design files for the sensor array
- `STLs/`: 3D-printable files for enclosures and mounts
- `Schematics/`: Electrical schematics of the system

## Legacy Information

This repository serves as an archive for the original OpenMuscle-Band design. Active development has moved to the [OpenMuscle GitHub Organization](https://github.com/Open-Muscle), where you'll find:

- [OpenMuscle-FlexGrid](https://github.com/Open-Muscle/OpenMuscle-FlexGrid): A modular 60-sensor wearable, successor to the OM12
- [OpenMuscle-LASK5](https://github.com/Open-Muscle/OpenMuscle-LASK5): Labeling device with joystick and buttons
- [OpenMuscle-Software](https://github.com/Open-Muscle/OpenMuscle-Software): MicroPython firmware, communication protocols, and ML hooks

For historical data and machine learning scripts, refer to the [legacy repository](https://github.com/turfptax/openmuscle).

## Accolades & Media Coverage

**Electromaker:**  
🏆 2nd Place — Electromaker of the Month, April 2024  
[Electromaker Winners – March 2024](https://www.electromaker.io/blog/article/electromaker-of-the-month-march-2024-winners-1)

**Hackaday Articles Featuring OpenMuscle:**  
- [Forearm Muscle Contraction Sensor Is Useful Component For Open Source Prosthetics](https://hackaday.com/?s=forearm+muscle+contraction+sensor)  
- [Hackaday Prize 2023: Finger Tracking Via Muscle Sensors](https://hackaday.com/?s=hackaday+prize+2023+finger+tracking)  
- [Hackaday Prize 2023: LASK4 Watches Those Finger Wiggles](https://hackaday.com/2023/06/02/hackaday-prize-2023-lask4-watches-those-finger-wiggles/)

## Getting Started

To replicate or study the OpenMuscle-Band:

1. **Hardware Assembly:**
   - Print the enclosures from the `STLs/` directory.
   - Assemble the sensor cells with Hall Effect Sensors, magnets, and springs.
   - Connect the sensors to the ESP32-C3 modules as per the schematics.

2. **Firmware Installation:**
   - Flash MicroPython onto each ESP32-C3 module.
   - Upload the appropriate `boot.py` and `main.py` scripts to handle data acquisition and transmission.

3. **Data Collection:**
   - Use the band to collect muscle contraction data.
   - Transmit data via UDP to a host machine for processing.

4. **Machine Learning (Optional):**
   - Utilize the scripts from the legacy repository to train models that predict finger movements based on sensor data.

## Contributing

As this is an archived repository, we are not accepting contributions. For ongoing development and contributions, please visit the [OpenMuscle GitHub Organization](https://github.com/Open-Muscle).

## License

This project is licensed under the CERN Open Hardware License v2.0. See the [LICENSE](https://github.com/Open-Muscle/OpenMuscle-Band/blob/main/LICENSE) file for details.
