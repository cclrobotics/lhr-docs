Several of the instruments are controlled using relay circuits so here is a little information about how they work.
<img src="https://github.com/cclrobotics/lhr-docs/blob/master/System-Diagrams/Relay-Circuit/Relay%20Circuit%20Diagram%20-%20Relay%20Circuit%20Diagram.png" height="250px" /> <img src="https://github.com/cclrobotics/lhr-docs/blob/master/System-Diagrams/Relay-Circuit/20160806_173530.jpg" height="250px" />

- Four pin connector on the left links to a shield on the arduino board. The pins are as follows:
  - SIG: Signal from Arduino for the relay to open/close the circuit.
  - N/C: No connection (Doesn't actually do anything, only in place so a common connector can be used)
  - VCC: Provides power from the Arduino for the relay logic.
  - GND: Ground to the Arduino.

- Power Terminals switch power to one of the following instruments by completing their AC connection:
  - Shaker (on/off control)
  - Centrifuge (on/off control)
  - WL Transiluminator (on/off control)
  - UV Transiluminator (on/off control)
  - Incubator (Arduino uses a [hysteresis controller](https://www.google.com) to maintain temperature at 37&deg;C)
  - Igor Light (on/off control, suspected to be the overhead lights)
  - Gel Electrophoresis (on/off control)
  - Shaker Incubator Light (on/off control, there should be an incubator light to warm shaking tubes but I'm not sure where it is)
Some of these are assumed based on the [arduino code](https://github.com/griswaldbrooks/lhr-equipment-controller/blob/master/controller_firmware/controller_firmware.ino).

- Relay
  - Model #: HLS8L-DC5V-S-C
  - The relay receives a signal from the Arduino telling it to close or open the circuit. This will power on or off the instrument connected to the power terminals. Most of these can just be turned on/off (light boxes). In the case of the shaker and centrifuge, they are set to a specific rpm and just turned on/off by the Arduino. The hysteresis controller code is already loaded onto the Arduino. The Incubator also has a temperature sensor attached. When the temperature falls below 37&deg;C the Arduino turns the Incubator power source on (a lamp for now), once the temperature is above 3&deg;7C it is turned off. (We can make this more sophisticated in the future)
