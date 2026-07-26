# Project-MSIS
Implemented the complete RTL-to-GDSII flow for an I²C Controller at 45nm

Complete digital implementation flow of an I²C Controller, taken from RTL to final 
GDSII layout at 45nm technology node.

## Overview
This project implements the full ASIC physical design flow for an I²C protocol 
controller using industry-standard Cadence EDA tools. The design was carried through 
synthesis, floorplanning, placement, clock tree synthesis, routing, and static timing 
analysis, achieving clean timing closure at sign-off.

## Flow Stages
- RTL Design – I²C Controller functional RTL (Verilog)
- Synthesis– RTL to gate-level netlist using Cadence Genus
- Floorplanning– Die/core area planning, power planning
- Placement– Standard cell placement and optimization
- Clock Tree Synthesis (CTS)– Clock network build and balancing
- Routing– Signal and power routing
- Static Timing Analysis (STA) – Sign-off timing verification using Cadence Tempus
- DFT– Scan insertion and testability using Cadence Modus
- Logic Equivalence Checking (LEC) – RTL-to-netlist and netlist-to-layout 
  verification using Cadence Conformal LEC

## Tools Used
Cadence Genus, Cadence Innovus, Cadence Tempus, Cadence Modus, Cadence Conformal LEC

## Results
- Achieved timing closure at 100 MHz
- Zero setup/hold violations across sign-off timing analysis
- Clean DRC/LVS-ready layout

## Repository Contents
- `rtl/` – I²C Controller RTL source files
- `synthesis/` – Synthesis scripts and reports
- `pnr/` – Floorplan, placement, CTS, and routing scripts
- `timing_reports/` – STA sign-off reports
- `screenshots/` – Layout and timing report screenshots

## VLSI Design intern
Manoj Kumar H L – M.E. VLSI Design, Manipal School of Information Sciences
