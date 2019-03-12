# AMS-assertions
Extensions to System Verilog to support AMS assertions

Digital semiconductor design verification engineers typically have experience using the technique called "assertions" that is part of the System Verilog standard (SVA for System verilog Assertions).  Assertions permit the verification engineer to specify the expected behaviors of a design and have the simulator check adherance to them during, or after, the simulation completes.  A problem arises, however, if the design under test is not purely digital but either analog or a mix of analog and digital (analog mixed-signal or AMS).  There is no SVA equivalent in the AMS design domain.   Not only is there no pre-defined, standardized library of checks, there's no easy syntax to express them if one wanted to write their own.  For example, while SVA supports constructs for signals being "off" or "on", there's no method to express signals oscillating between "off" and "on" with a certain waveform and frequency that's characteristic of AMS circuits.  This deficiency greatly diminishes AMS verification capability.

To improve this situation, as part of the DARPA POSH program, Synopsys is creating a series of AMS checks, initially written in Python but with the eventual goal to propose a Verilog syntax as an extension to SVA.  Python was selected for many reasons, but chief among them are that it's open source and available today, whereas it will take time for the standards committees to review and approve additional SVA syntax.

This repository will track the progress of this effort.
