# SageMic Prototype 1 — v1.5 (SolidWorks)

CAD for the SageMic field enclosure. Built in SOLIDWORKS 2026, so open it in SOLIDWORKS 2026 or newer.

**Open `Sgmc-Prototype1-v1.5-Assembly.SLDASM`.** It loads every other file in this folder through relative paths, so keep the folder structure as it is.

## Files

| File | Contents |
|---|---|
| `Sgmc-Prototype1-v1.5-Assembly.SLDASM` | Top-level assembly |
| `Sgmc-Prototype1-v1.5-Enclosure.SLDPRT` | Multibody part: **Body**, **Lid**, **Mic Holder**, **Solar Panel Holder**, plus reference bodies *Foam Windscreen (Ref)* and *Solar Panel (Ref)* |
| `Sgmc-Prototype1-v1.5-Cartridge-Assembly.SLDASM` | Electronics cartridge with the boards installed |
| `Sgmc-Prototype1-v1.5-Electronics-Cartridge.SLDPRT` | Printed electronics cartridge |
| `Sgmc-Prototype1-v1.5-Print-Profile.3mf` | Bambu Studio project (X1 Carbon, 0.4 mm nozzle). Plate 1: Lid, Plate 2: Body, Plate 3: Solar Panel Holder + Mic Holder (ASA-CF). Plate 4: Electronics Cartridge (PLA). |
| `Sliced-Files/` | Ready-to-print Bambu files (`.gcode.3mf`), one per plate, sliced for an X1 Carbon with a 0.4 mm nozzle on a textured PEI plate. |
| `Purchased-Parts/` | Off-the-shelf parts: McMaster-Carr hardware (draw latch, flat head screws, heat-set inserts), INMP441 microphone, Raspberry Pi 4 B, LTE base hat, solar charge controller, step-down converter. The `.step` files are the vendor originals. |

## Printed parts
Electronics Cartridge, Body, Lid, Mic Holder. "(Ref)" bodies are only for fit checks and aren't printed.

## Print settings
ASA-CF for the outdoor parts (0.16 mm layers, 4 walls, 15% gyroid, tree supports, 5 mm outer brim to stop ASA warping). Print with the X1C's enclosure door closed.

## Sliced files

| File | Part | Filament | Est. time | Filament used |
|---|---|---|---|---|
| `Plate1-Lid` | Lid | ASA-CF | 3 h 49 m | 68 g |
| `Plate2-Body` | Body | ASA-CF | 1 d 5 h 58 m | 534 g |
| `Plate3-SolarPanelHolder-MicHolder` | Solar Panel Holder, Mic Holder | ASA-CF | 1 h 10 m | 12 g |
| `Plate4-Electronics-Cartridge` | Electronics Cartridge | PLA | 11 h 57 m | 315 g |

Total: about 614 g ASA-CF and 315 g PLA. These files only work on a Bambu X1 Carbon. For another printer, re-slice from `Sgmc-Prototype1-v1.5-Print-Profile.3mf`.
