# Components of the system

## Raspberry Pi
This is the main brain of the system. It is connected to every other aspect of the system and performs the high level planning involved.
There will be various types of code on it. 

[Website](https://www.raspberrypi.org/)

[Github](https://github.com/raspberrypi/)

## Smoothie Board 
Used to control stepper motors for XYZ translation and limit switches for setting up boundaries for each axis. 
It is programmed with g-code. 

[Website](http://smoothieware.org/)

[Github](https://github.com/Smoothieware/Smoothieboard) 

## Arduino Uno
Used to control the lab equipment. (Centrifuge, shaker, etc. Note: PCR controlled via Rasberry pi)
You write sketches the arduino using the Arduino Software (IDE) which uses C/C++ by default. 

[Website](https://www.arduino.cc/en/Main/ArduinoBoardUno)

[Github](https://github.com/arduino/Arduino)

## Pronterface
They run a software suite called PrintRun which allows you to communicate with 3D printers, but we will be using it to communicate with the CNC.
This suite is on the rasberry pi and sends g-code to smoothie board.

[Website](http://www.pronterface.com/)

[Github](https://github.com/kliment/Printrun)

# Previous work

## Pedro Terra

## Open trons
The original liquid handling robot, made my Arcturus, that Pedro and Luis modified and expanded into "Igor."

[Website](https://opentrons.com/)

[Github](https://github.com/OpenTrons/otone_docs/blob/master/README.md)

[Open source bioserver](https://forum.arcturus.io/t/open-source-bioserver/17/9) 
This is a great place to see the progress Pedro and Luis made.

It won't be necessary to exaustivly read through all of their documentation, but these should be good sources to look at if we run into any trouble figuring the system out.

