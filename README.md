# FPGA Driven Seven Segment Display
Learning about FPGAs using *Arduino's MKR Vidor 4000*. Driving a 7 segment by using the *Cyclone 10 LP* that comes embedded into the board.

> Source https://github.com/luisgizirian/seven-segment-fpga-driver

## What's our plan?
To learn about FPGA's, their Toolset, digital circuits design process, by using what we have at hand:

* Laptop
* Raspberry Pi
* Arduino MKR Vidor 4000
* 7-segment display
* Switch
* Breadboard
* Wires

### A Laptop + a Pi?

We're planning to use them both to achieve building the project in-tandem. The Laptop will be in charge of VSCode and running a VM loaded with Intel's Quartus II instance. The Raspberry Pi hosts, the source code, the final building & running process, and it is hooked to both the laptop though *VSCode Remote SSH Extension* capabilities in one end and to the Vidor 4000 through the USB cable on the other, tying the whole solution together.

## Inspiration

* Nandland Go Board Project 5 - Seven Segment Display https://youtube.com/watch?v=iT9MVuIZFJ8&feature=share
* Remote Development on Raspberry and Arduino with VS Code https://joachimweise.github.io/post/2020-04-07-vscode-remote/

## Status

(**Nov 23**) Combining FPGA newbieness + undeveloped *Vidor 4000* tooling ecosystem, we've reached a frozen status, filled with **pains (*Vidor 4000* context)**...

* FPGA dev flow & Quartus
 * Input and Output Pins, assignments
 * VHDL & Verilog learning curve
 * Quartus text editor capabilities look '90s
 * Obtaining a .TTL (bit stream) file and turning it *Vidor 4000* friendly

### To test next...

* VHDPlus IDE [https://vhdplus.com/]
* VHDL + *Vidor 4000* + breadboard sample [https://forum.arduino.cc/t/how-to-code-and-run-vhdl-examples/561115/12]

### Conclusion (current state of affairs)

Still can't figure out if *Vidor 4000* was a good choice as Development Board for newcomers into the FPGA world.

Relevant links
- https://maker.pro/arduino/tutorial/how-to-program-the-arduino-mkr-vidor-4000s-fpga-with-intel-quartus-ide
- https://www.youtube.com/watch?v=R8NmKzZAufE
- https://nandland.com/project-5-seven-segment-display/
- https://github.com/nandland/nandland/tree/master/7_Segment
- https://forum.arduino.cc/t/how-to-code-and-run-vhdl-examples/561115/7
- https://docs.arduino.cc/tutorials/mkr-vidor-4000/vidor-gsvhdl
- https://github.com/vidor-libraries/VidorBitstream/tree/release/TOOLS/makeCompositeBinary
- https://github.com/vidor-libraries/VidorFPGA

---

Until next update!
