# FIFO Memory Controller - RTL to GDSII

This project implements a FIFO memory controller from RTL to a physical GDSII layout.
The design was synthesized, placed, and routed using the OpenLane/OpenROAD flow targeting the SkyWater 130nm (sky130A) process node.

 **Total Cell Count** - 309 
 **Die Area** - 3733.58 µm² 
 **D-Flip-Flops (Storage)** - 80 
 **Multiplexers** - 96 

## Flow Methodology
1. **Synthesis:** Yosys used to convert RTL to a gate-level netlist.
2. **Floorplanning:** Defined die area and power distribution network (PDN).
3. **Placement:** Standard cells placed using OpenROAD.
4. **Routing:** Global and detailed routing performed to ensure zero DRC violations.
5. **Sign-off:** Verified via LVS (Layout vs. Schematic) and DRC (Design Rule Check).
