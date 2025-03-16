# Sky-Water-RTL-TO-GDS-
This repository documents the RTL-to-GDSII flow for a Not Gate using the SkyWater 130nm PDK on Ubuntu. It covers RTL design (Verilog), synthesis (Yosys), floorplanning &amp; placement, routing, and signoff, followed by the final GDS export

📂 RTL/
This folder contains the RTL (Register Transfer Level) design of the inverter in Verilog. It includes the initial design files and testbenches used for functional verification.

📂 Synthesis/
Here, the RTL code is converted into a gate-level netlist using Yosys. The output shows how the design is mapped to standard cells available in the SkyWater 130nm PDK.

📂 Floorplanning/
This stage defines chip layout constraints such as die area, power grid, and macro placements. The floorplan ensures the circuit is arranged efficiently before placement and routing.

📂 Placement/
Placement involves positioning standard cells in the defined floorplan without overlaps, using tools like OpenROAD. This folder contains the placed netlist and visualization of cell locations.

📂 Routing/
The routing stage connects the placed cells using metal layers while following Design Rule Constraints (DRC). Outputs from TritonRoute are stored here, showing properly wired connections.

📂 Signoff/
Signoff includes essential Design Rule Checks (DRC) and Layout vs. Schematic (LVS) verification to ensure correctness. It ensures that the final design is manufacturable.

📂 Final_GDS/
This folder contains the final GDSII layout, which is the standard format used for fabrication. It includes the generated mask layout ready for chip manufacturing.
