# Compact Diffusion Pump
A compact diffusion pump design- a modification of https://grabcad.com/library/diffusion-pump-1 for accessibility, gasket flexibility, size, and functionality 

## What is a Diffusion Pump?
A diffusion pump is a kind of vacuum pump specifically geared for HV (high vacuum) systems- in conjunction with a roughing pump, usually a rotary vane, it can produce pressures of 1e-4 to 1e-6 torr or lower, in correctly designed vacuum systems. It's notable for requiring no moving parts- merely a nozzle assembly, silicone/mineral oil, a heater, and a water cooling system. This sounds like a lot of requirements, but the requirements for an alternate kind of vacuum pump used for HV systems- turbomolecular pumps- are far greater, and these are more difficult to manufacture, balance, and operate.

A very good demonstration video is: https://www.youtube.com/watch?v=SrNVLCHrJtY&t=20s

## What does this design do?
This design fits in a 250 mm height, 200 mm diameter cylinder, which is remarkably small for a vacuum pump, and can pump several dozen L/s if correctly manufactured. The jet assembly's design is taken from a cross-section of a diffusion model in https://grabcad.com/library/diffusion-pump-1. One of the .catpart files had a splice of it. A duplication of the splice, rotation, merging and rescaling was necessary, as well as the conversion of the file to a more accessible format in the form of .step. In addition- the flange is made entirely by me- the exterior of the diffusion pump provided is subpar for several reasons. A corrugated design is harder to manufacture, it didn't have standardized inlets and outlets. I added these, as well as a custom design for a flange, complete with O-ring grooves and holes to be able to tighten screws through, so a Viton O-ring of 130 mm outer diameter and 2 mm cross-sectional thickness can be used to provide a vacuum-tight seal.

Some stills from the CAD file, as viewed from FreeCAD:
![View](https://github.com/user-attachments/assets/2c7445c5-50e3-48b4-bc69-a5a0268d8c9f)

![O-Ring Grooves](https://github.com/user-attachments/assets/5bf62865-b8f3-4680-93bd-d35e33ea14ba)

![Jet Assembly](https://github.com/user-attachments/assets/a110a4ec-9e95-4811-9a1a-faa1761cd8fc)

Note that the final image- the jet assembly- was predominantly made by https://grabcad.com/library/diffusion-pump-1, but it was in a proprietary file format, and so had to be converted to openly-accessible formats, resized, and reshaped to fit in this assembly. The rest is entirely original work.

## What can it do?
After CNC manufacturing and assembly with the right components, this may be able to produce HV vacuum pressures in a vacuum chamber. There's only one way to find out.

## Why does DiffusionPump.step look so weird?
The nozzle assembly of a diffusion pump looks weird because it needs to guide the evaporated vapors upwards and sideways, because the precise thermo- and aero-dynamics of how it functions are necessary to the creation of the high vacuum. The specific CFD calculations weren't done by me but by the original author of https://grabcad.com/library/diffusion-pump-1, who made an upscaled, half-sector design of this file. 

A rough summary is the long, column-like holes at the base are to let the oil stream in, the pinprick-like holes along the column, especially higher up, are to let the vapor out once sufficient pressure has built up, and the conic sections tapering outwards are to guide the direction of the vapors. This is a bird's eye view of how diffusion pumps work, and for a greater look at it I very much recommend you take a look at the open-access paper https://iopscience.iop.org/article/10.7567/JJAPS.2S1.25 or any other sources of information.

## How do I check it out?

Use a CAD program like Solidworks or Fusion360. If you don't know what a CAD program is, or don't know where to buy one, use FreeCAD (https://www.freecad.org/). Download and run it, download any .step files you want to see, import them to the program, and view and modify them.

## How Do I Make this Real?
Use the CAD files and get them CNC machined in aluminium or stainless steel. Then, get a nichrome heating element and place it at the base https://www.amazon.com/uxcell-0-2x6mm-Nichrome-Heating-Elements/dp/B01E5RBB3I. Don't use WD40 or some other off-brand silicone oil. Unlike every other vacuum pump- the mechanical portion is not the mechanism of action, the oil is. Use very, very low vapor pressure oil or you won't even get lower vacuum pressures than a rotary vane. Buy a nitrile or viton O-ring with 130 mm OD, like: https://www.amazon.com/uxcell-Rings-Nitrile-125-2mm-Diameter/dp/B07HGCYDBY

My recommendation? Buy Ultragrade 19 at: https://www.fishersci.com/shop/products/ultra-grade-19-oil-1l/NC9844626. It should get you to HV pressures. According to Ted Pella (https://www.tedpella.com/vacuum_html/Vacuum_Pump_Oil_Properties.aspx) it has a vapor pressure of 1 x 10^-8 mbar at 20 Celsius, which is more than good enough of a vapor pressure for most applications, and it's usually between $30-50.

Also, buy a very, very powerful fan to air-cool it. Aircooling's already used for small diffusion pumps (like in the https://www.agilent.com/en/product/vacuum-technologies/diffusion-pumps/small-diffusion-pumps/ax-65-diffusion-pump). Normal 12V fans won't cut it, probably. A heavy-duty fan like the https://www.amazon.com/-/es/wfb1212hh-Delta/dp/B00773K4UE might work.
