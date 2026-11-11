# Breadboard-Power-Supply
A custom 2 layer pcb , power supply board which fits directly onto breadboard 
# Breadboard Power Supply PCB

A 2-layer breadboard power supply board designed in KiCad.


<img width="790" height="765" alt="image" src="https://github.com/user-attachments/assets/618f80b5-3a92-43ef-b311-f3f26fc30280" />

## Specs
- Input: 12 V DC via barrel jack, with on/off switch
- Outputs: two independent output headers, each jumper-selectable between 3.3 V and 5 V
- 3.3 V rail: LM317 adjustable regulator (R1 = 240 ohm, R2 = 390 ohm, about 3.28 V)
- 5 V rail: LM7805 fixed regulator
- Power-on indicator LED
- Output connectors: 2-pin headers and screw terminals for the breadboard
- Current: regulators are rated 1.5 A, but at 12 V input each one dissipates 7-8.7 W per amp, so a heatsink is needed above roughly 100-150 mA

## Known limitations
- No reverse-polarity protection or fuse
- Not yet fabricated or tested
  
## Status
Schematic, 2-layer board layout and 3D model are complete. Final DRC cleanup is in progress.

## Files
- `kicad/` : KiCad project (schematic and PCB)
- `docs/schematic.pdf` : schematic
- `docs/pcb_3d.png` : 3D render

Built with KiCad.
