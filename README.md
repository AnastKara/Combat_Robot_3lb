<!--
  RONIN — 3 lb Combat Robot README
  Placeholders marked [LIKE THIS] are details only you know; fill them in or
  reply and I'll update them.
-->

<div align="center">

# RONIN

### 3 lb (1.36 kg) Beetleweight Combat Robot — Belt-Driven Wedge

[![Class](https://img.shields.io/badge/Class-3%20lb%20%7C%201.36%20kg-blue)](#)
[![Config](https://img.shields.io/badge/Config-Belt--Driven%20Wedge-orange)](#)
[![Status](https://img.shields.io/badge/Status-Competition%20Ready-green)](#)
[![License](https://img.shields.io/badge/License-All%20rights%20reserved-lightgray)](#)

</div>

---

##  Overview

<img src="images/robot_hero.jpg" alt="RONIN — belt-driven 3 lb wedge robot" width="600"/>

> _A compact, belt-driven 3 lb combat robot engineered for durability, ease of
> maintenance, and consistent performance in high-impact matches. RONIN's
> architecture focuses on robust drive power, efficient energy distribution,
> and a reinforced front wedge built for pushing, deflecting, and controlling
> opponents._

Built for the **3 lb (1.36 kg) beetleweight class**, RONIN is designed to be
**serviceable between matches** — a modular two-piece frame with clean wiring
and a lightweight multi-material build (printed PETG / TPU 95A frame with a
7075 aluminum wedge) that keeps repair times short and combat performance
consistent.

---

##  Key Features

- **Reinforced front wedge** — aggressive pushing, deflection, and positional control
- **Belt-driven dual-wheel drivetrain** — smooth, high-traction torque delivery
- **Modular 2-piece chassis** — fast repairs between matches
- **Shock-resistant electronics mounting** — foam-damped ESCs and secure routing
- **Clean internal wiring** — reliable and quick to troubleshoot
- **Competition-ready layout** — compatible with most 3 lb rule sets

---

##  Technical Specifications

###  Chassis
| Item         | Specification                         |
| ------------ | ------------------------------------- |
| Material     | PETG + TPU 95A (3D printed)          |
| Manufacturing| Bambu Lab A1 Mini (FDM)              |
| Architecture | 2-piece modular frame                 |
| Fasteners    | M3 / M4 stainless steel               |
| Dimensions   | 220 × 160 × 91 mm (8.7 × 6.3 × 3.6 in) |
| Weight       | **1150 g (2.54 lb)** _(3.0 lb / 1.36 kg max)_ |

###  Drive System
| Item        | Specification                          |
| ----------- | -------------------------------------- |
| Drive type  | Belt-driven dual-wheel                 |
| Motor       | 2× DartBox V2 Drive gearmotors (VIPER model) |
| Drive ESC   | **WEKA 20A** Dual Brushed Motor Controller |
| Mainboard   | **Just 'Cuz Motherboard V4** (Just 'Cuz Robotics) |
| Receiver    | **FS2A** — AFHDS-2A protocol           |
| Wheels      | 43 mm (1.7 in) rubber / foam          |
| Belts       | **S3M timing belts** (74 teeth · 4 mm)  |
| Top speed   | **~3.5 m/s (12.6 km/h · 7.8 mph)** theoretical · ~2.6 m/s (9.4 km/h) realistic |

###  Power System
| Item              | Specification                     |
| ----------------- | --------------------------------- |
| Battery           | Tattu 3S LiPo · 11.1 V · 450 mAh · 75C |
| Connectors        | XT30                              |
| Power distribution| DartPCB (Just 'Cuz)                |
| Safety            | External power switch + removable link |

###  Electronics
| Item               | Specification                      |
| ------------------ | ---------------------------------- |
| Mainboard          | **Just 'Cuz Motherboard V4** (Just 'Cuz Robotics) |
| Drive ESC          | **WEKA 20A** Dual Brushed Motor Controller |
| Receiver           | **FS2A** — AFHDS-2A protocol       |
| Voltage regulation | 5 V BEC for receiver               |
| Telemetry          | LED status indicator               |
| Transmitter        | **FlySky FS-i6** — AFHDS-2A      |

---

##  Design & Engineering

### Design Philosophy
RONIN is a **pushing-and-control robot**. Instead of chasing high-energy
weapon hits, it wins through sustained aggression: getting its wedge under
opponents, driving them into hazards, and disrupting their weapon mounts and
drive chains. That philosophy drives three decisions:

- **Strength over speed** — a belt-driven, high-torque drivetrain delivers
  smooth, controllable pushing power in every match
- **Serviceability** — everything that commonly breaks (belts, wheels, wedge,
  ESC) is reachable within minutes between fights
- **Efficient weight budget** — the wedge, chassis, and drive get the weight;
  the electronics bay stays tight and clean

### Drivetrain
Two **DartBox V2 Drive gearmotors (VIPER model, 22 mm)** turn both wheels through
**S3M timing belts**, powered by the **WEKA 20A Dual Brushed Motor
Controller** and managed by the **Just 'Cuz Motherboard V4** mainboard. The
DartBox V2 motors are lightweight and ultra-powerful for their size, giving
RONIN a strong power-to-weight ratio. Belt drive reduces shock loading on
the motors and drivetrain during impacts — a key reliability win over direct
chain-drive setups — while the WEKA dual ESC delivers smooth, high-traction
torque for pushing matches.

> 📐 **Top-speed estimate:** Based on the DartBox V2 Drive output (1550 RPM @ 3S)
> and 43 mm wheels, RONIN reaches ~3.5 m/s (12.6 km/h · 7.8 mph) theoretical
> no-load top speed. Accounting for battery sag, friction, and belt losses, a
> realistic figure is ~2.6 m/s (9.4 km/h · 5.9 mph).

| Config      | Drive                                   | Electronics                          |
| ----------- | --------------------------------------- | ------------------------------------ |
| **Current** | 2× DartBox V2 Drive (VIPER) + S3M belts | WEKA 20A dual ESC · JCMB V4 · FS2A  |
| **Planned** | Brushless D3536 drivetrain              | 1200 kV motor + 40 A ESC            |

> 🔧 **Upgrade path:** For higher acceleration, RONIN can swap to a
> **brushless D3536** drivetrain (e.g., 1200 kV with a 40 A ESC) — trading some
> low-end simplicity for faster wheel speed and lighter electronics.

### Weapon
RONIN's "weapon" is its **reinforced 7075-T6 aluminum front wedge**: a
low-sweep, angled blade that gets under opponents and lifts their wheels for
positional control. The wedge geometry is optimized for **steel arena floors**,
and is re-torqued at every event to keep engagement angle consistent.

### Chassis & Manufacturing
RONIN's modular frame is **3D printed on a Bambu Lab A1 Mini** in **PETG** for
structural rigidity, with **TPU 95A** parts where flexibility and shock
absorption matter. This multi-material approach keeps the robot lightweight,
reduces part count, and makes it fast to reprint spare parts between events.

---

##  Assembly Guide

### 1. Chassis Preparation
1. Install the front wedge using **M4 bolts**.
2. Mount side panels and check alignment.
3. Add the top plate **last** for easy internal access.

### 2. Drivetrain Installation
1. Mount the drive motors securely; apply **thread-locker**.
2. Align pulleys and tension the S3M belts.
3. Install wheels and verify free rotation.

### 3. Electronics Setup
1. Mount ESCs with **foam tape** for shock absorption.
2. Route motor wires cleanly along chassis walls.
3. Keep the receiver away from high-current lines.
4. Connect: **battery → PD board → ESCs → motors**.

### 4. Final Checks
- [ ] Verify belt tension
- [ ] Confirm correct motor direction
- [ ] Test radio failsafe
- [ ] Inspect all fasteners

---

##  Testing & Calibration

1. **No-load spin-up** — confirm smooth motor ramp with wheels off the ground.
2. **Steering response** — check left/right trim center and full-lock turns.
3. **Wedge engagement** — test on a flat surface; wedge should lift, not bounce.
4. **Thermal soak** — 1–2 minute drive test to confirm ESC and motor
   temperatures stay within limits.

---

##  Maintenance

- **Inspect belts** after every match — replace at the first sign of fraying
- **Re-tighten all screws**, especially the wedge bolts
- **Check motor bearings** for debris and re-grease as needed
- **Replace wheels** when worn to maintain consistent traction
- **Battery care** — keep Tattu 3S LiPos balanced and store them safely (450 mAh nominal)

---

## 📦 Bill of Materials (BOM)

| Component      | Specification                            | Source / Link                                   |
| -------------- | ---------------------------------------- | ----------------------------------------------- |
| Drive motor    | 2× DartBox V2 Drive · VIPER 22 mm        | [🔗 DartBox Drive](https://justcuzrobotics.com/products/dartbox-squared-drive) |
| Drive ESC      | WEKA 20A Dual Brushed Motor Controller   | [🔗 WEKA 20A](https://justcuzrobotics.com/products/weka-dual-20-esc-for-brushed-drive) |
| Mainboard      | Just 'Cuz Motherboard V4                 | [🔗 Motherboard V4](https://justcuzrobotics.com/products/motherboard) |
| Power dist.    | DartPCB (Just 'Cuz)                      | [🔗 DartPCB](https://justcuzrobotics.com/products/dartpcb) |
| Receiver       | FS2A (AFHDS-2A protocol)                 | [🔗 Buy / info](https://your-link.example/fs2a) |
| Battery        | Tattu 3S LiPo · 450 mAh · 75C            | [🔗 Buy / info](https://your-link.example/tattu-3s) |
| Wheels         | 43 mm rubber / foam                      | [🔗 Buy / info](https://your-link.example/wheels-43mm) |
| Belts          | S3M timing belt · 74 teeth · 4 mm        | [🔗 S3M 74T Belt](https://justcuzrobotics.com/products/s3m-timing-belt-74t-4mm-wide-used-in-ssp-kits) |
| Weapon (wedge) | 7075-T6 aluminum                         | [🔗 Buy / info](https://your-link.example/7075-wedge) |
| Chassis        | PETG + TPU 95A (Bambu Lab A1 Mini print) | [🔗 Print settings](https://your-link.example/print-file) |
| Connectors     | XT30                                     | [🔗 Buy / info](https://your-link.example/xt30) |
| Transmitter    | FlySky FS-i6 (AFHDS-2A)                  | [🔗 Buy / info](https://your-link.example/fs-i6) |
| Fasteners      | M3 / M4 stainless steel                  | [🔗 Buy / info](https://your-link.example/fasteners) |

> 🔗 **Sources:** The drive motor, ESC, mainboard, power-distribution board, and
> belt rows have live links to Just 'Cuz Robotics. The remaining
> `your-link.example` entries are placeholders — swap in the real store / CAD /
> print-files URLs when you have them.

> Full BOM with part numbers and links: **[add file: bom.xlsx / parts/]**.

---

##  Battle Record

| Date        | Event                    | Opponent          | Result | Notes       |
| ----------- | ------------------------ | ----------------- | ------ | ----------- |
| [YYYY-MM-DD] | [Event name / location] | [Opponent]        | [W/L]  | [Highlight] |
| [YYYY-MM-DD] | [Event name / location] | [Opponent]        | [W/L]  | [Highlight] |

---

##  Competition Notes

- Designed for the **3 lb (1.36 kg) beetleweight** class
- Complies with standard safety rules: **removable link** and **LiPo protection**
- Wedge geometry optimized for **steel arena floors**
- Drive tuned for **high-traction pushing matches**

---

##  Upgrade Roadmap

- [x] Belt-driven dual-wheel drivetrain
- [x] Brushed drive + WEKA 20A dual ESC (JCMB V4 / FS2A)
- [ ] **Brushless drive upgrade** — D3536 · 1200 kV + 40 A ESC for higher acceleration
- [ ] **Hardened AR500 steel wedge** — more bite and durability
- [ ] **Gyro-assisted driving** — stability under self-righting hits
- [ ] **Quick-swap battery bay** — faster pit stops

---

##  Build Files

| Path        | Description                                |
| ----------- | ------------------------------------------ |
| `cad/`      | [CAD source (Fusion 360 / Onshape / STEP)] |
| `drawings/` | [Dimensioned drawings, DXF cut files]      |
| `parts/`    | [BOM spreadsheet / order links]            |
| `images/`   | Build & media photos                       |

---

##  Safety & Rules Compliance

- **Removable link** — power can be broken instantly from outside the arena
- **Hard-cased / secured LiPo** — battery strapped or pocketed securely
- **E-stop** — external power switch for immediate power-down
- Always verify against the **current SPARC / NHRL / event ruleset** before
  competing.

---

##  Credits

RONIN was designed, built, and driven by **Anastasis Karaivazoglou** as part
of the **IRONBRICK | Fibran** team.

Special thanks to our sponsors **Fibran** and **JLC** for their support of the build.

##  License

**All rights reserved.** © [2026] Anastasis Karaivazoglou / IRONBRICK | Fibran.

This project is provided for reference and personal use only. No part of the
design, documentation, or media may be reproduced, distributed, or used in
commercial or competitive projects without prior written permission.
Sponsors: **Fibran** and **JLC**.

---

_README maintained with the RONIN build. Last updated: September 2026._