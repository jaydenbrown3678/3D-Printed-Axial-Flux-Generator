# 3D-Printed-Axial-Flux-Generator

# 3D-Printed Three-Phase Axial Flux Generator

![Generator Status](https://img.shields.io/badge/status-prototype-yellow)
![License](https://img.shields.io/badge/license-MIT-blue)
![3D Printing](https://img.shields.io/badge/3D-printed-orange)
![Phase](https://img.shields.io/badge/phase-3--phase-green)

A hand-cranked, 12V electricity generator built almost entirely from 3D-printed parts and recycled components. This project demonstrates electromagnetic induction principles and is designed to be assembled without a drill press, lathe, or other heavy machinery.

![Generator Image]
<img width="5712" height="4284" alt="IMG_0718" src="https://github.com/user-attachments/assets/826dd2ac-7cc5-4a99-a205-3f01cdf51649" />
<img width="5712" height="4284" alt="IMG_0717" src="https://github.com/user-attachments/assets/10d07400-4818-41a9-87c5-a447e9e2696a" />
<img width="5712" height="4284" alt="IMG_0716" src="https://github.com/user-attachments/assets/07e79b41-ab4c-4c2d-a678-3185e54bc33e" />
<img width="5712" height="4284" alt="IMG_0719" src="https://github.com/user-attachments/assets/5e8aea8b-c242-43a8-82a3-4a75a6101475" />


---

##  Table of Contents

- [Overview](#overview)
- [Features](#features)
- [How It Works](#how-it-works)
- [Bill of Materials (BOM)](#bill-of-materials-bom)
- [3D Printing Instructions](#3d-printing-instructions)
- [Assembly Guide](#assembly-guide)
- [Wiring Instructions](#wiring-instructions)
- [Testing](#testing)
- [Troubleshooting](#troubleshooting)
- [Performance](#performance)
- [Future Improvements](#future-improvements)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

##  Overview

This generator converts mechanical energy (from a hand crank, wind turbine, or water wheel) into electrical energy. With a built-in 64:1 gearbox, the rotor spins 64 times for every single turn of the input crank, generating usable voltage even at moderate cranking speeds.

**Why build this?**
- Learn electromagnetic induction hands-on
- Generate electricity from recycled materials
- Understand three-phase power systems
- Power small devices like LEDs or charge phones (with a rectifier)

---

##  Features

| Feature | Specification |
|---------|---------------|
| **Phase type** | 3-phase AC output |
| **Target voltage** | 12V DC (after rectification) |
| **Gear ratio** | 64:1 (integrated) |
| **Magnets** | 8 x N52 neodymium (20x3mm) |
| **Coils** | 6 x ~400 turns of 0.1mm magnet wire |
| **Bearings** | 608zz (salvaged from rollerblades) |
| **Frame** | Fully 3D-printed (PLA/PETG) |
| **Drive method** | Hand crank, wind, or water |

---

##  How It Works

This generator operates on **Faraday's Law of Electromagnetic Induction**:

> A changing magnetic field induces voltage in a conductor.

- **Rotor:** Holds 8 neodymium magnets arranged with alternating polarity (N-S-N-S...)
- **Stator:** Holds 6 copper coils arranged in three opposing pairs
- **Gear train:** 64:1 ratio increases rotor speed relative to crank input
- **Rectifier (external):** Converts 3-phase AC to DC for practical use

When you turn the crank, the gears accelerate the rotor. The spinning magnets create a changing magnetic field across the stationary coils, pushing electrons through the wire and generating electricity.

---

##  Bill of Materials (BOM)

### 3D-Printed Parts (PLA or PETG)

| Part | Quantity | Notes |
|------|----------|-------|
| End plates (with bearing slots) | 2 | |
| Compound gears | 5 | Each needs 2 bearings |
| Single spur gear | 1 | Press-fit M8 hex nut |
| Rotor body | 1 | Holds 8 magnets |
| Stator body | 1 | Holds 6 coils |
| Coil sockets | 6 | Snaps into stator |
| Coil cores | 6 | Metal preferred (or 3D-printed) |
| Washers/spacers | ~30 | Various thicknesses |

### Standard Hardware

| Component | Specification | Quantity | Source |
|-----------|---------------|----------|--------|
| Aluminum rod | 8mm diameter | 1 | Hardware store |
| Bolts | M8 x 130mm (quarter-threaded) | 5 | Hardware store |
| Hex nuts | M8 | ~15 | Hardware store |
| Neodymium magnets | N52, 20x3mm | 8 | Online (Amazon/eBay) |
| Bearings | 608zz (22mm OD) | 15+ | Salvaged from rollerblades |
| Magnet wire | 0.1mm diameter (enameled copper) | 1 spool | Online or recycled (microwave) |
| Crazy glue/Superglue | | 1 tube | Hardware store |
| 3-Phase bridge rectifier | 10A 1000V | 1 | Amazon/eBay |

### Optional / Testing

| Component | Specification |
|-----------|---------------|
| Multimeter | With AC/DC voltage |
| Resistor | 220Ω - 1kΩ |
| LED | Standard 5mm |
| Socket wrench or pliers | For cranking |

---

##  3D Printing Instructions

- **Download the design:** [Tinkercad Link](https://www.tinkercad.com/things/6l8Wafbcfa4)
- **Printer:** Any desktop FDM printer (6.5" x 6.5" build area minimum)
- **Nozzle:** 0.4mm - 0.8mm
- **Layer height:** 0.2mm - 0.5mm
- **Infill:** 20-40%
- **Material:** PLA or PETG (PETG recommended for gears for better durability)

**Estimated print times (0.8mm nozzle, 0.5mm layer height):**

| Part | Time |
|------|------|
| End plate | ~47 minutes |
| Compound gear | ~30 minutes |
| Rotor/Stator | ~1-2 hours each |
| Coil sockets | ~15 minutes each |

### Important Tolerances

- Bearing press-fit: Bearings should require force to insert (use vice or hammer with wood block)
- Magnet slots: Magnets should click firmly into place (no glue required)
- Gear teeth: Ensure no stringing or warping for smooth meshing

---

##  Assembly Guide

### 1. Prepare Bearings and Hardware
Press all bearings into their designated slots. Press an M8 hex nut into the single spur gear.

### 2. Wind the Coils (Most Tedious Step)

For each of the 6 coils:
1. Insert a coil core into a coil socket
2. Leave a 10-15cm wire tail
3. Wind ~400 turns of 0.1mm magnet wire
4. Apply superglue every 50 turns to secure windings
5. Leave another tail and glue the final winding
6. Repeat 5 more times

**Tip:** Use a vice and a washer with tape to guide the wire.

### 3. Connect the Coils (3-Phase Wye Configuration)
