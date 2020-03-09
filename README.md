# MiniiPS
Custom regulator board for miniaturized Wii. Provides 1V, 1.15V, 3.3V, 5V. Similar to the PowerMiiLite, but larger and a few extra features specific to my personal project. Should be good for any wall-powered mini Wii project.

### Goals for this power supply
* Be small. Can't really afford much more space than 20mm by 60mm
* Use a 5V 3A USB-C charger for input power
* Have an enable pin for turning on and off the power supply. The slide switch I'm using for power is only rated for 200mA.
* Design the 3.3V, 1.15V, and 1V regulators for 3A output, and 15V input voltage. I'm over-engineering to give myself maximum chance of getting it right on the first try, instead of pushing all my components right to their spec. There could be some reason I this is a bad idea, but I can't think of one.
* Be easy to hand assemble (using skillet reflow) and rework. An automated assembly run is out of the question. Smallest passives are 0603 (1608 metric).

To power on the outputs, the enable pad must be pulled high with your power switch. By default, that pad is pulled low with a 10K resistor.