# Compact Diffusion Pump
A compact diffusion pump design- a modification of https://grabcad.com/library/diffusion-pump-1 for accessibility, gasket flexibility, size, and functionality 

## What is a Diffusion Pump?
A diffusion pump is a kind of vacuum pump specifically geared for HV (high vacuum) systems- in conjunction with a roughing pump, usually a rotary vane, it can produce pressures of 1e-4 to 1e-6 torr or lower, in correctly designed vacuum systems. It's notable for requiring no moving parts- merely a nozzle assembly, silicone oil, a heater, and a water cooling system. This sounds like a lot of requirements, but the requirements for an alternate kind of vacuum pump used for HV systems- turbomolecular pumps- are far greater, and these are more difficult to manufacture, balance, and operate.

## What does this design do?
This design fits in a 250 mm height, 200 mm diameter cylinder, which is remarkably small for a vacuum pump, and can pump several dozen L/s if correctly manufactured. The jet assembly's design is taken from a cross-section of a diffusion model in https://grabcad.com/library/diffusion-pump-1. One of the .catpart files had a splice of it. A duplication of the splice, rotation, merging and rescaling was necessary, as well as the conversion of the file to a more accessible format in the form of .step. In addition- the Diffusion_Pump.step file is made entirely by me- the exterior of the diffusion pump provided is subpar for several reasons. A corrugated design is harder to manufacture, it didn't have standardized inlets and outlets. The flange is custom-designed by me, with the holes in the gasket being exactly 8 mm long to allow for the utilization of 9 mm ID Viton O-rings, instead of a gasket. 

## What can it do?
After CNC manufacturing and assembly with the right components, this may be able to produce HV vacuum pressures in a vacuum chamber. There's only one way to find out.

## Why does Diffusion_Pump_Internals.step look so weird?
The nozzle assembly of a diffusion pump looks weird because it needs to guide the evaporated vapors upwards and sideways, because the precise thermo- and aero-dynamics of how it functions are necessary to the creation of the high vacuum. The specific CFD calculations weren't done by me but by the original author of https://grabcad.com/library/diffusion-pump-1, who made an upscaled, half-sector design of this file. 

A rough summary is the long, column-like holes at the base are to let the oil stream in, the pinprick-like holes along the column, especially higher up, are to let the vapor out once sufficient pressure has built up, and the conic sections tapering outwards are to guide the direction of the vapors. This is a bird's eye view of how diffusion pumps work, and for a greater look at it I very much recommend you take a look at the open-access paper https://iopscience.iop.org/article/10.7567/JJAPS.2S1.25 or any other sources of information.

## How do I check it out?

Use a CAD program like Solidworks or Fusion360. If you don't know what a CAD program is, or don't know where to buy one, use FreeCAD (https://www.freecad.org/). Download and run it, download any .step files you want to see, import them to the program, and view and modify them.

## What license is this with?
None. Use this as you will, modify it, share it, there are no limitations.
