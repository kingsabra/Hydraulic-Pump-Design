# Hydraulic Pump Design — Bilge Pump

Mechanical design and assembly package for a **hand-crank / mechatronic bilge pump** (piston pump). Created for **U.S. Coast Guard Academy — Introduction to Mechanical Design (IMED), Spring 2022**, Team 4.

The pump can be built in two configurations: **manual crank drive** or **motorized drive** controlled by an Arduino and a water-level sensor.

---

## Repository structure

| Folder | Contents |
|--------|----------|
| **`cad/`** | All SolidWorks files: main assembly, pump parts, fasteners, and drawings. Open `cad/Assem1.SLDASM` in SolidWorks to view the full assembly. |
| **`docs/`** | Reports (assembly instructions, BOM, drawing exports) in PDF and DOCX. |
| **`media/`** | Renders and animations (e.g. mechanism animation). |
| **`misc/`** | Other artifacts (e.g. SolidWorks add-in logs); safe to ignore for normal use. |

---

## What’s in each folder

### `cad/`
- **`Assem1.SLDASM`** — Main pump assembly.
- **Parts (`.SLDPRT`)** — Pump body, piston, connecting rod, axle, crank disk, crank handle, handle, support arm, piston screw, quick-disconnect coupling (male).
- **`screws/`** — Fastener and fitting library (set screws, bolts, brass fitting, etc.) used in the assembly.
- **`IMED_MS_001.SLDDRW`** — Multi-sheet drawing (BOM and part/detail views).
- **`CGA B Landscape.slddrt`** — Drawing template (title block, border).

### `docs/`
- **Assembly Report Team 4** (`.pdf`, `.docx`) — Full assembly process: pump body, handle, and mechatronics wiring. Primary reference for building the pump.
- **assembly report - Moustafa Mahmoud Sabra** (`.pdf`, `.docx`) — Separate OIR/interview report (not pump assembly steps).
- **`IMED_MS_drawings.PDF`** — Exported drawing set (BOM, dimensions, tolerances).

### `media/`
- **`Animation1.mp4`** — Short animation of the pump mechanism.

### `misc/`
- **`console.log`** — SolidWorks Marketplace add-in log; not part of the design. You can add `misc/console.log` to `.gitignore` if you don’t want it in the repo.

---

## Main parts (from BOM)

Pump body, support arm, axle, crank disk, crank handle, handle, connecting rod, piston, piston screw, quick-disconnect coupling, plus standard hardware (set screws, bolts, NPT barbed fitting, ball bearings) as listed in the assembly report and `IMED_MS_drawings.PDF`.

---

## How to use this repo

1. **View the assembly** — Open **SolidWorks** and open `cad/Assem1.SLDASM`. Keep all files under `cad/` (and `cad/screws/`) in place so references don’t break.
2. **Build the pump** — Follow **`docs/Assembly Report Team 4.pdf`** for step-by-step assembly (manual and mechatronics).
3. **Drawings and BOM** — Use **`docs/IMED_MS_drawings.PDF`** for dimensions and part list, or open `cad/IMED_MS_001.SLDDRW` in SolidWorks.

---

## Note on Arduino / firmware

The assembly report describes an **Arduino-based circuit** (C code in Arduino IDE) for motor control and water-level sensing. That **firmware is not included** in this repository; this repo contains only CAD and documentation. If you have the original sketch, you can add it in a folder such as `firmware/` and reference it in this README.

---

## License and use

SolidWorks files are marked as **Educational Product**. Use according to your institution’s and SolidWorks’ terms. Reports and drawings are from the referenced course and authors.
