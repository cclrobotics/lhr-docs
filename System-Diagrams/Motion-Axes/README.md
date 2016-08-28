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
| LS-Y1     |Y-Axis Limit Switch      | 
| LS-Z     |Z-Axis Limit Switch      |
| LS-A     |A-Axis Limit Switch      |

##Top-Down View
###X-Axis
There is one X-axis motor (M-X) which is attached the pipettes and moves along the central beam. It uses the limit switch (LS-X) as it's minimum value, so that end is essentially zero for the X-axis. 
###X-Axis
There are two Y-axis motors (M-Y1 and M-Y2) which are attached to either end of the central beam. Their phases are inverted so they will travel in synch together, moving the central beam. They use one limit switch (LS-Y1) on the as minimum value for the Y-1 motor. This is the zero for the Y-axis. Only one side hits it, and the stop signal should be sent to both of them. 
##Side View
