# Molecule Evaporation Calculator

This is a program to easily calculate the evaporation time required to deposit a specified coverage of molecules on a surface, using a quartz microbalance to calibrate deposition rate. The inputs are the molecule size (for the standard/routine options of pentacene or PTCDA, the molecule size is input by switching a toggle) and desired coverage, in monolayers (ML).

![image](https://user-images.githubusercontent.com/78166226/137356780-e3ba6a85-80ce-4749-b7b1-9ab7b6e069d0.png)

Then the molecules are heated in a crucible with the shutter closed to the known evaporation temperature. Once this temperature is reached, the shutter is opened and the molecules are evaporated onto a quartz microbalance, which is able to measure very small changes in mass. The quartz microbalance controller also has a molecule size calibration input, so as the evaporation proceeds the controller readout gives the layer thickness, in Angstroms, as a function of time. Once the rate (thickness as a function of time) is constant, calibration can begin. 

To calibrate the deposition rate, the times at which the thickness changes (recorded externally with a stopwatch) should be input as time values into the program. The input format is minutes.seconds, to allow the user to enter their stopwatch readout directly without needing to convert to seconds. The change in time (dt) is calculated by the program for each step. If the rate is constant, dt will be approximately constant for each Angstrom step. If the rate is not constant, the above should be repeated until it is constant. 

![image](https://user-images.githubusercontent.com/78166226/137357874-96143702-69cc-4896-99e5-6c36d4e863e4.png)

The program then performs three calculations. First, it converts the input monolayer coverage into Angstroms, given the molecule size. Second, it calculates the deposition rate given the average dt. Finally, it calculates the deposition time that should be used to deposit the desired coverage.

![image](https://user-images.githubusercontent.com/78166226/137358495-86b8dcea-96e2-4be2-8cf7-cd476cdbbde5.png)

The final portion of the program is to aid a user who is in the lab alone, since they need both hands for operating the hardware, and it is tricky to see the computer screen or start a stopwatch while doing so. The program has a timer that makes a noise to count down until the deposition should be started. Once the countdown noise stops, the deposition substrate is quickly moved in front of the molecule evaporator. The program displays the temporal progression through the deposision. Once there are 10 seconds remaining in the deposition time, the program again plays a noise to indicate that the user should get ready to stop the deposition. Once the sound ends, the user quickly moves the deposition surface away from the evaporator. The evaporation is complete, all shutters can be closed, and the molecule crucible temperature can be lowered. 

![image](https://user-images.githubusercontent.com/78166226/137359334-12df3447-bd6a-4d57-98ac-f270f00d9f86.png)



![image](https://user-images.githubusercontent.com/78166226/137360947-df6a80d8-15c2-4a1f-ac2c-9c42a3615c3d.png)

