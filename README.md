# 62DAC Signal Integrity Study

Read it here: **https://cozycactus.github.io/62dac-si-study/**

A simulation study of the 62DAC, a stereo non-oversampling DAC built on two Analog Devices AD1862 chips and driven by a Raspberry Pi Pico. It asks what on the PCB limits the AD1862, and what to change to get its full 20-bit performance.

The study covers:

- clock and latch edge integrity at the DAC pins
- crosstalk and digital charge coupled into the I/V summing nodes
- TDR and input impedance
- wave propagation, return-current and near-field maps
- ground-plane voltage drop
- decoupling impedance at every supply pin

All of it was done with free tools: openEMS (FDTD, run on an Apple M1 GPU), ngspice, KiCad's geometry engine, and numpy/scipy.
