#Electophoresis System

http://www.instructables.com/id/Gel-electrophoresis-system-mini/


Diagram of the System here.



What are the components?
- Thing1
- DC-DC Converter
- AC-DC Converter
- More things...

Hardware and tools

From McMaster-Carr:

- 2-56 Hand Tap Taper, Cat # 2522A663
- Tap Wrench Sliding T-Handle, 0-1/4" (1.6-6.3mm) Tap Size, Cat # 2546A22
- 2x 2-56 Nylon Pan Head Slotted Machine Screw, 3/16" Length, Cat # 93135A076
- 4x 2-56 Nylon Pan Head Slotted Machine Screw, 1/8" Length, Cat # 93135A074
- Stainless steel wire, 0.01" diam. Cat # 9882K31
- 2x 6/32 Hex machine nuts Cat # 91841A007
- 2x Flat Washer, No. 6 Screw Size, 5/16"Cat #  92141A008

From TAP Plastics:

- IPS weld-on cement #3 or 4, Cat # 10792
- Hypo-type solvent cement applicator, Cat # 25658

From Digi-Key:

- 2x Banana plug, Cat #655K-ND
- Black banana plug cable, 36", Cat # 4771-36-0-ND
- Red banana plug cable, 36", Cat # 4771-36-2-ND
- 4x Rubber feet , Cat # SJ5012-0-ND


## Thing1

## DC-DC Converter <a id="dc-dc-conv"></a>
It's based on the [Electrophoresis variable power supply](http://public.iorodeo.com/docs/electrophoresis_power_supply/)
by [IO Rodeo](http://iorodeo.com/).
It requires an input voltage from 10V (this hasn't been verified and should be) to 16V.
Manufacturer's recommended input voltage is 15V.
The original unit has a variable output from 25V to 100V. It has been modified to produce an output from 30V to 200V
by substituting the original 15K resistor R3, with a 7.5K resistor. A schematic of the circuit can be found
[here](http://public.iorodeo.com/docs/electrophoresis_power_supply/intro.html).

## AC-DC Converter
This is the thing you plug into the wall.
Triad Wall Mount AC Adapter  WSU150-1600
http://www.mouser.com/ProductDetail/Triad-Magnetics/WSU150-1600/?qs=sGAEpiMZZMt5w6YCUaBPUXrfhsD5E87B75MqnVLWq%252bc%3d
It has a 15 V up to 1.6A output.
Note: Any replacement unit cannot have an output greater than 16V or damage to the [DC-DC Converter](#dc-dc-conv)
