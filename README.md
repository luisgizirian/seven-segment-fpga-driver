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

(**Dec 8**) VHDPlus plays well with Intel's Quartus II and as well as their own hardware and standards they appply to (i.e. CRUVI, PMOD). *Vidor 4000* is under the Arduino umbrella, so it out scopes VHDPlus support (as I read over their Discord [Get an invite at https://vhdplus.com/]).

---

(**Nov 29**) Managed to upload and run a design into the embedded FPGA by following this post (https://nerdhut.de/2020/08/17/arduino-mkr-vidor-4000-verilog-fpga-and-mcu-hello-world-tutorial/). We need to run some fixes now (either into design or physical wiring) to make our test smoothly work.

Relevant links:
- https://forum.arduino.cc/t/how-to-code-and-run-vhdl-examples/561115/8
- https://forum.arduino.cc/t/how-do-i-upload-verilog-directly-to-my-vidor-4000-board/1013022/3
- https://forum.arduino.cc/t/next-chapter-of-mkr-vidor-4000-fpga-upload-live-data-exchange/1023945
- (duplicated) (https://nerdhut.de/2020/08/17/arduino-mkr-vidor-4000-verilog-fpga-and-mcu-hello-world-tutorial/

### To test next...

* VHDPlus IDE [https://vhdplus.com/]

### Conclusion (current state of affairs)
Having a custom design uploaded into the Arduino's FPGA is encouraging. Tooling is still a bit cumbersome so we'll chech if something can be improved in that space. 

---

(**Nov 23**) Combining FPGA newbieness + undeveloped *Vidor 4000* tooling ecosystem, we've reached a frozen status, filled with **pains (*Vidor 4000* context)**...

* FPGA dev flow & Quartus
 * Input and Output Pins, assignments
 * VHDL & Verilog learning curve
 * Quartus text editor capabilities look '90s
 * Obtaining a .TTL (bit stream) file and turning it *Vidor 4000* friendly

### To test next...

* VHDPlus IDE [https://vhdplus.com/]
* VHDL + *Vidor 4000* + breadboard sample [https://forum.arduino.cc/t/how-to-code-and-run-vhdl-examples/561115/12]

### Conclusion

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
