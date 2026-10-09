# Firefly Project

Recovery, configuration and calibration of a quadcopter for controlled flight, developed over three academic semesters. This document covers **Semester 1**.

> **Status:** Semester 1 objective achieved 07/10/2026 · **Deadline:** 01/12/2026

---

## Introduction

The project started with a pre-existing **F450 frame running ArduCopter**. It was discarded in the first weeks: the flight controller was damaged and oxidized. Serial monitor tests returned the following error, which prevented the controller from booting:

```
PANIC! Baro: internal sensor failed to respond
```

Development continued on a second airframe: a **DJI F330 frame with a DJI Naza-M Lite** flight controller. This is the platform documented in this repository.

---

## Semester 1 — Scope

| # | Task | Status |
|---|---|---|
| 1 | Component verification (motors, ESCs, battery, receiver) and replacement of faulty parts | Completed |
| 2 | Download and update of the Naza-M Lite driver and firmware | Completed |
| 3 | Configuration and calibration (receiver binding, ESC throttle range, Naza-M Lite Assistant setup) | Completed |

**Objective:** perform short, controlled flights.

**Result:** short, controlled untethered flights were performed successfully.

---

## Hardware

| Component | Specification | Qty. |
|---|---|---|
| Frame | DJI F330 (Quad X) | 1 |
| Flight controller | DJI Naza-M Lite | 1 |
| Motors | Brushless 2212 920KV | 4 |
| ESCs | EMAX SimonK 30A | 4 |
| Radio | HT-10A 2.4 GHz transmitter + receiver | 1 |
| Battery | LiPo | 1 |

---

## Software environment

| Item | Configuration |
|---|---|
| OS | Windows (required by DJI tools) |
| Configuration software | DJI Naza-M Lite Assistant |
| Driver | DJI WIN Driver (unsigned; requires driver signature enforcement to be disabled during installation) |

Download links: [`Firmware/readme.md`](Firmware/readme.md)

---

## Repository structure

| Path | Contents |
|---|---|
| [`Docs/Repair instructions.docx`](Docs/Repair%20instructions.docx) | Step-by-step repair, configuration and calibration procedure |
| [`Docs/Pictures/`](Docs/Pictures/) | Photos and videos of the process |
| [`Docs/DIP/`](Docs/DIP/) | Course (DIP) deliverable documents |
| [`Hardware/CAD/dji_f330/`](Hardware/CAD/dji_f330/) | F330 frame CAD model (SolidWorks), sourced from GrabCAD |
| [`Hardware/Datasheets/`](Hardware/Datasheets/) | Naza-M Lite manual, ESC manual and reference links |
| [`Hardware/Diagrams/`](Hardware/Diagrams/) | Naza-M Lite wiring diagram |
| [`Firmware/`](Firmware/) | Firmware and software download links |

---

## Future work

The Semester 1 platform is a working baseline. Upgrades and further additions will be defined in the following semesters.
