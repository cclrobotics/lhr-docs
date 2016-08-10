#Electophoresis System

Diagram of the System here.

What are the components?
- Thing1
- DC-DC Converter
- AC-DC Converter
- More things...

## Thing1

## DC-DC Converter <a id="dc-dc-conv"></a>
It's based on the [Electrophoresis variable power supply](http://public.iorodeo.com/docs/electrophoresis_power_supply/)
by [IO Rodeo](http://iorodeo.com/).
It requires an input voltage from 10V (this hasn't been verified and should be) to 16V.
The original unit has a variable output from 25V to 100V. It has been modified to produce an output from 30V to 200V
by substituting the original 15K resistor R3, with a 7.5K resistor. A schematic of the circuit can be found
[here](http://public.iorodeo.com/docs/electrophoresis_power_supply/intro.html).

## AC-DC Converter
This is the thing you plug into the wall.
It has a 2 million V output.
Note: Any replacement unit cannot have an output greater than 16V or damage to the [DC-DC Converter](#dc-dc-conv)
