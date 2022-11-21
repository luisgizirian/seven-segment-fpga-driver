# FPGA Driven Seven Segment Display
Trying to learn about FPGAs using *Arduino's MKR Vidor 4000*. Driving a 7 segment by using the *Cyclone 10 LP* that comes embedded into the board.

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
