# Annealing Current Control

This is a program to slowly ramp current up and down. The program controls the current supplied by a Agilent Hewlett-Packard power supply to a filament heater for sample annealing. The current is set to the start current, then increased in steps of step size which have a duration of step time. Once the end current is reached, it is maintained for hold time. After hold time, the current is decreased in identical steps back to start current. Status indicators (total steps and time required, steps and time elapsed, and the current now) are also given, as is a graph which displays the history of the applied current. 

![image](https://user-images.githubusercontent.com/78166226/137366226-31830aae-bd72-4457-b3d4-431181a41a48.png)

