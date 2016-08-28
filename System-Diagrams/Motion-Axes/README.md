![Motion Axes Diagram](https://github.com/cclrobotics/lhr-docs/blob/master/System-Diagrams/Motion-Axes/Motion%20axes%20diagram.png) 

|Key       |      Item               | 
|----------|-------------------------|
| M-X      |X-Axis Motor             |
| M-Y1     |Y-Axis Motor 1           |
| M-Y2     |Y-Axis Motor 2           |
| M-Z      |Z-Axis Motor             |
| P-A      |Single Channel Pipette   |
| P-B      |Multi Channel Pipette    |
| M-A      |A-Axis Motor             |
| M-B      |B-Axis Motor             |
| LS-X     |X-Axis Limit Switch      |
| LS-Y1    |Y-Axis Limit Switch      | 
| LS-Z     |Z-Axis Limit Switch      |
| LS-A     |A-Axis Limit Switch      |

##Top-Down View
###X-Axis
There is one X-axis motor (M-X) which is attached to the pipettes and moves along the central beam. It uses the limit switch (LS-X) as it's minimum value, so that end is essentially zero for the X-axis. 
###Y-Axis
There are two Y-axis motors (M-Y1 and M-Y2) which are attached to either end of the central beam. Their phases are inverted so they will travel in synch together, moving the central beam. They use one limit switch (LS-Y1) as the minimum value for the Y-1 motor. This is the zero for the Y-axis. Only Y1 side hits it, and the stop signal should be sent to both Y motors. 

##Side View
###Z-Axis
There is one Z-axis motor (M-Z) which is attached to the set of pipettes and moves up and down perpendicular to the central beam. It uses the limit switch (LS-Z) as it's minimum value. This is the zero for the Z-axis. Moving along the Z-axis in a positive direction translates to moving **down**. 
###A-Axis
There is one A-axis motor (M-A) which is attached to the plunger of the single-channel pipette (P-A). It controls the depression of the plunger allowing us to propgram how much volume is pipetted up/down. It uses the limit switch (LS-A) as it's minimum value. This is the zero for the A-axis.
###B-Axis
There is one B-axis motor (M-B) which is attached to the plunger of the multi-channel pipette (P-B). It controls the depression of the plunger allowing us to propgram how much volume in pipetted up/down. There is currently no limit switch attached for this motor.
