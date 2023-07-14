# Overview: 
- A pool game programmed in C, running on the ARM processor in the DE1-SoC computer, and displayed on VGA

![media-4](https://github.com/dl423/DE1-SoC-Pool-Game/assets/81783344/f813b623-1abb-4148-94f6-45af011ae668)

# Quick Video Demo:

<iframe src="https://drive.google.com/file/d/1OBCACd7CLvhVe8dWXQFIKfmZnavOOpzh/preview" width="640" height="480" allow="autoplay"></iframe>

# Technical implementation:
- Programming language:  C
- The program runs on the ARM processor in the DE1-SoC computer, 
  - Note that the DE1-SoC board mainly consists of an FPGA and a Hard Processor System (HPS)
- Reads input from PS/2 keyboard connected to the computer
- Game interface is drawn on the VGA display by writing values into the pixel buffer
  - Wrote helper functions to draw lines, circles, etc. on the VGA display by calculating the appropriate pixel locations to draw on
  - Screen is constantly refreshed to create animation
- The code running on DE1-SoC computer and the PS/2 keyboard input can be simulated using CPUlator
