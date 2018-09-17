# IntanRHD2000USB
Custom RHD2000 USB software that includes a 24k Hz sampling frequency.

This was made because we convert the .RHD files to Tint (Axona) format, and thus it is easy to upsample from 24k to 48k.

There is also a python notebook (FPGA_Calculations.ipynb) that will aid in calculating the M and D values needed for the FPGA to sample at a desired frequency, if someone wants to add one for themselves.
