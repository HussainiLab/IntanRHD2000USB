# IntanRHD2000USB
Version 1.6

I made a few changes to the source code to match my recording needs.

Changes from source code:
- I added a 24k Hz sampling frequency. This was made because we convert the .RHD files to Tint (Axona) format, and thus it is easy to upsample from 24k to 48k.
- I added a QLineEdit that will contain the information for the settings filename. This is because I will be using a different settings file for each probe, and it would be nice to read the name of the settings file so I know how to map the channel numbers. The string representing the settings filename will be saved in the header. I had to update the read_header Python function to read this value if the version number matches the one of this custom code. I changed the version number from 1.5 to 1.6.

There is also a python notebook (FPGA_Calculations.ipynb) that will aid in calculating the M and D values needed for the FPGA to sample at a desired frequency, if someone wants to add one for themselves.
