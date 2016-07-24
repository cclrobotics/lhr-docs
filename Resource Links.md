# Components of the system

## Raspberry Pi
This is the main brain of the system. It is connected to every other aspect of the system and performs the high level planning involved.
There will be various types of code on it.   
- [Website](https://www.raspberrypi.org/)
- [Github](https://github.com/raspberrypi/)

## Smoothieboard 
Used to control stepper motors for XYZ translation and limit switches for setting up boundaries for each axis. 
It is programmed with g-code.   
- [Website](http://smoothieware.org/)
- [Github](https://github.com/Smoothieware/Smoothieboard) 

## Arduino Uno
Used to control the lab equipment (Centrifuge, shaker, etc. Note: PCR controlled via Rasberry pi).
You write sketches the arduino using the Arduino Software (IDE) which uses C/C++ by default.     
- [Website](https://www.arduino.cc/en/Main/ArduinoBoardUno)
- [Github](https://github.com/arduino/Arduino)

## Pronterface
They run a software suite called PrintRun which allows you to communicate with 3D printers, but we will be using it to communicate with the CNC.
This suite is on the rasberry pi and sends g-code to smoothie board.    
- [Website](http://www.pronterface.com/)
- [Github](https://github.com/kliment/Printrun)

# Previous Work

## Pedro Terra  
- [Website](http://www.pedroterralab.com/)

## OpenTrons
The original liquid handling robot, made by Arcturus, that Pedro and Luis modified and expanded into "Igor."  
- [Website](https://opentrons.com/)
- [Github](https://github.com/OpenTrons/otone_docs/blob/master/README.md)
- [Open source bioserver](https://forum.arcturus.io/t/open-source-bioserver/17/9)    
This is a great place to see the progress Pedro and Luis made.
- [BioBot 1.0 Assembly Guide](https://synbiota.com/projects/1p_XD0znG/entries/0DATTrmqW?preview=true)  
Note: The assembly guide is for the original OpenTrons DIY BioBot. Pedro and Luis' "Igor" is larger, includes more components, and most importantly is using the Smoothieboard NOT the TinyG. Therefore it's best we dont' follow this to a T.

### Google Drives
- [OpenTrons](https://drive.google.com/folderview?id=0B5OBQhwEUbwUNXZKVWYxeHo2elE&usp=drive_web)
- [bioserver](https://drive.google.com/folderview?id=0B-Zkc0hbJe19flF1MlRUblBJQXgwSndyNnloMTdwX3RLWDdDbHZKZWNnNkw3X2VXVVI1NTQ&usp=sharing_eid&ts=5793e682&tid=0B-Zkc0hbJe19fnZCaVJCVV94anc3VTIza1RIY2NROVA0Y3k5WFkwLXlHTVhuWUJlSHNiUjg)
- [igor general photos](https://drive.google.com/folderview?id=0B-Zkc0hbJe19fngyQjl0aVNkTVAtWXp1SXZqM2R2NjhEYlBfbjJwbkE5WlpJcExVeXA4S0k&usp=sharing_eid&ts=5793e5f9)
- [igor bioserver parts](https://drive.google.com/folderview?id=0B-Zkc0hbJe19fkMwcWhoSDREVUR6Q3pRLUl2SXI2SWdoLXMtYVhmOHMzUTlCMG1rVWFIUFE&usp=sharing_eid&ts=5793e5b6)

It won't be necessary to exaustivly read through all of their documentation, but these should be good sources to look at if we run into any trouble figuring the system out. I will be compiling files and information from these sources throughout the repo in appropriate locations (ex. photos in a photos folder).

