# Wearable Device

This repository contains the development of a **wearable glove system** for a wearable–drone interaction based mobility assistance system.

The wearable glove serves as a bidirectional Human–Drone Interface by sensing hand and finger motion and providing haptic feedback for navigation guidance and hazard alerts.

---

## System Overview

The wearable device provides the following functions:

- IMU-based hand and finger joint motion sensing
- Motion capture data generation
- Transmission of hand motion data to the drone system
- Haptic navigation feedback
- Haptic hazard alert feedback
- Integrated wearable firmware operation

In the later development stage, hand motion data acquired from the wearable glove will be combined with full-body motion information obtained from the drone camera for multimodal user intent recognition.

---

## Hardware

### Main Components

| Component | Purpose |
|---|---|
| ESP32 | Main wearable controller and wireless communication |
| MPU6500 | Hand and finger motion sensing |
| TCA9548A | Multi-IMU I2C multiplexing |
| Vibration Motor | Haptic navigation and hazard feedback |
| Power Circuit | Power supply and voltage regulation |

For detailed hardware components, see:

- [Bill of Materials](docs/bom.md)
- [Hardware Documentation](docs/hardware.md)

---

## Repository Structure

```text
wearable-device/
├── firmware/
│   ├── imu_test/
│   ├── multi_imu/
│   ├── motion_capture/
│   ├── haptic_navigation/
│   ├── haptic_hazard_alert/
│   └── wearable_main/
│
├── hardware/
│   ├── cad/
│   └── circuit/
│
├── docs/
│   ├── images/
│   ├── bom.md
│   ├── hardware.md
│   └── protocol.md
│
└── README.md