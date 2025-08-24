# pico_drone_pcb
[![KiCad](https://img.shields.io/badge/KiCad-8/9-blue?logo=kicad)](https://www.kicad.org/)
![Status](https://img.shields.io/badge/status-in_development-orange)
![License](https://img.shields.io/badge/license-TBD-lightgrey)
![PCB](https://img.shields.io/badge/board-drone_controller-green)

Custom PCB for a Raspberry Pi Pico–powered drone.  

This board integrates the core electronics needed to run a quadcopter, with power regulation, sensor connectors, and interfaces for ESCs and other peripherals.

The corresponding code, written in c can be found [here](https://github.com/Torbjorn-Lund/pico_drone_project)

## Features
- Designed for **Raspberry Pi Pico 2**  
- Power regulation:
  - Buck converter supporting up to **18 V input**
  - **TVS diode protection** limiting input voltage to ~10 V  
  - Optimized for **2S LiPo batteries (≈7.4 V nominal, 8.4 V fully charged)**  
- Breakouts for:
  - ESCs (dshot)
  - IMU (ICM-20948)  
  - Barometer (BMP280)  
  - GPS (NEO-M8N)  
  - Time-of-flight sensor (VL53L1X)  

## Images
![PCB image](/images/pcb_side.png "Optional Title")
![PCB image](/images/pcb_front.png "Optional Title")
![PCB image](/images/pcb_back.png "Optional Title")

## Notes / Limitations
- TVS diode limits voltage, so this board is not suitable for 3S+ LiPo packs.  
- Board is still under development.
