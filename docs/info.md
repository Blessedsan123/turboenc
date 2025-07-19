<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

How it works

The Turbo Encoder (turboenc) project implements a parallel concatenated convolutional encoder architecture using two Recursive Systematic Convolutional (RSC) encoders and an interleaver. The input data is first passed to the first RSC encoder. Then, an interleaved version of the same data is passed to the second RSC encoder. The final encoded output consists of the original input (systematic bits) and the parity bits from both encoders, enhancing error correction performance in noisy communication channels.
How to test

  Prepare Input: Provide an input binary stream (e.g., 8-bit or 16-bit).
    Simulation: Use any Verilog simulator like ModelSim, Vivado Simulator, or Icarus Verilog to run the testbench.
    Check Outputs: The testbench will display the encoded output stream (systematic and parity bits).

  Verification: Compare the encoded output with expected values from theoretical turbo encoding or MATLAB reference.

External hardware

   None.
   This project is fully simulation-based and does not require any external hardware for testing or implementation.
