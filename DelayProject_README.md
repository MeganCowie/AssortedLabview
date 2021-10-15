# Delay Project

The delay project has two programs, which each move a different delay stage (translational for air delay, wedge for wedge delay). They are nearly identical, so only the air delay program is explained here. The purpose of this program is to vary the delay of two laser beams with respect to one another via the delay stage motor. The beams are sent into a photodiode and a fm-AFM tip-sample junction, and this program measures the optical and AFM signal simultaneously. 

The air delay program does two distinct things: It can either move or sweep. If the user wants to move, they can enter the desired position in either the A or B position value, and then select "Start Move". The delay stage will move at its maximum motor speed until it reaches the position, and then it will stop moving. 

![image](https://user-images.githubusercontent.com/78166226/137533562-6334d1c0-3746-498c-9c3b-d17322db0157.png)

The user can also perform a sweep, meaning that the motor will take defined steps according to the user input parameters (start and end position, step size, wait times before and after moving, and the number of data points averaged per step). The sweep gives readouts of the total distance (mm) travelled, the total range in time swept (fs), the conversion of the step size in mm to the step size in fs, and the total time required for the sweep and the time remaining. 

![image](https://user-images.githubusercontent.com/78166226/137533701-44515a78-49fb-48e1-89ed-a5c00a53a053.png)

The program also has two graphs for displaying sweep data. The first is the signal measured with a photodiode on an optical table, and the second is the "frequency shift" signal measured via Nanonis software controlling an fm-AFM experiment. Within the "Sweep" section, the user can choose which Nanonis channel is displayed on the graph. Up to three curves can be shown at a time on each graph, and the user selects which curve is plotted as Plot1, Plot2, and Plot3. Finally, sweep data can be saved by selecting "save sweep", which in the saved file will record all of the attributes (location, notes, wavelength, etc.) that are entered as user inputs.  

The program at all times displays the position of the stage, and prevents the user from entering parameters which would bring the stage outside of its safe limits. The position of the second delay (in this case, the wedge delay) is displayed on-screen, since changing the second delay will change all of the relevant positions of the first display, so the user needs to remember to only move one at a time. 

![image](https://user-images.githubusercontent.com/78166226/137535905-b2ea2a2d-cdbd-4add-8af0-0c8b038dcb4e.png)

![image](https://user-images.githubusercontent.com/78166226/137532663-7e46381f-4d33-4d5d-b3ad-0ab2996e6f4d.png) 
