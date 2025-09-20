# Week0_VSDIAT

Summary of the Video:
The video had a basic introducion of the RTL to GDSII flow. 
In the first stage, chip modelling, the architecture is captured in C or C++. RISC-V this could be a simple C model or a simulator like Spike, where the instruction set, toolchain, and any custom extensions are tested. Programs compiled with the RISC-V GCC toolchain act as the testbench to check if the specification works as intended.

In the second stage, RTL architecture, the design is implemented in Verilog or SystemVerilog. This includes building the RISC-V processor core along with peripherals such as UART, GPIO, and accelerators. Verification is done using RISC-V ISA tests and real binaries. Once verified, the RTL is synthesized into a gate-level netlist, and additional blocks like SRAM macros and analog IPs such as PLLs are added.

The third stage is SoC integration. At this point, all of the components : CPU, memories, peripherals, and analog IPs are brought together to form a complete RISC-V SoC. The physical design flow is carried out, which includes floorplanning, placement, clock tree synthesis, routing, and sign-off checks. The final product of this stage is the GDSII file, which is the physical layout that gets sent for chip fabrication.
