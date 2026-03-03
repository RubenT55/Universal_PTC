# Universal PTC Board

A PCB project designed in **KiCad 9.0** that implements an external, universal PTC (Positive Temperature Coefficient) circuit for CRT monitors.

## Description
Many modern generic replacement chassis for CRT monitors (commonly known as "universal Chinese chassis") do not include an integrated PTC circuit to perform the automatic degaussing function of the screen. 

This board provides a compact, external solution, allowing you to add the degaussing feature cleanly and safely. It is designed to be compatible with most CRT picture tubes and generic arcade/TV chassis on the market.

## Repository Contents
- `UniversalPTC.kicad_pro` — Main KiCad project file
- `UniversalPTC.kicad_sch` — Schematic design
- `UniversalPTC.kicad_pcb` — PCB layout
- `local_libs/` — Directory containing project-specific assets
  - `3dmodels/` — 3D component models (e.g., MZ73 connectors) in `.step` format
  - `footprints/` — Custom footprint libraries (`.pretty`)
  - `symbols/` — Custom schematic symbols (`.kicad_sym`)

## Requirements
- [KiCad 9.0](https://www.kicad.org/) or higher.

## How to open the project
1. Clone the repository to your local machine:
   `git clone https://github.com/RubenT55/Universal_PTC.git`
2. Open KiCad, go to **File > Open Project**, and select the `UniversalPTC.kicad_pro` file.

> **Technical note:** This project is 100% *portable*. All custom footprints, symbols, and 3D models (like the PTC connector) are isolated inside the `local_libs/` folder using relative paths (`${KIPRJMOD}`). There is no need to install external libraries or configure global environment variables to view the complete project, including the 3D viewer.

## License
This project is open source. Feel free to modify, manufacture, and adapt the board for your arcade and CRT restoration needs.
