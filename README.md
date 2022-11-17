# LAB_4_Embedded
#### By: Ronan Harkins, Zachary Bravo, Ike-Anyanwu Chinedu
## Introduction
The goal of lab for was to toggle the on board LED with a 250 ms delay and produce a duty cycle with the timer within the MSP430FR2355. With this the the ouput should be sent to a pin on the board and the values should be able to be seen on the oscilloscope within the lab. 


### 10 Percent Duty Cycle 
For the ten percent duty cycle the values of TB0CCR0 was changed to be 500 and the value of TB0CCR1 was change to a value of 50. The reason this value was changed to 50 was because of the way the duty cycle is set. In order to obtain a duty cycle of 10% a value of 0.1 was needed from the combination of  TB0CCR1 divided by TB0CCR0. Since the values used within the code was 50/500 the output of this is 0.1 providing the correct duty cycle that is needed for part 1 of the lab. The duty cycle that was produced can be seen within the figure below.Within this figure it can be seen that a duty cycle of about ten can be seen. The reason it is not excat is beause of the wires that are being used are going to lose some of the signal. This process was done using the polling method. 
![image](https://user-images.githubusercontent.com/98828696/202477753-bec8b7b1-f677-4a24-b3d7-03214d3ed439.png)

![scope_12](https://user-images.githubusercontent.com/98828696/201200352-896f0096-a02c-4281-add8-218aef6fe114.png)

### UML diagram for Q2

![UML_LAB4](https://user-images.githubusercontent.com/98828696/201210373-0a4fcdb6-2d92-492f-8bf3-f40fe1e946f5.jpg)


### 20 Percent Duty Cycle 
For the 20% duty cycle the same method was applied however instead of using the polling method the interupt method was used. This does not change how the duty cycle is calculated. The values of TB0CCR0 and TB0CCR1 needed to create a value of 0.2 in order to get the 20% duty cycle. So the value of TB0CCR1 was keep at 50 and the value of TB0CCR0 was changed to 250. The reason for this change is becasue the value 0.2 is need so 50/250 produces the value of 0.2 needed for the 20% duty cycle. This duty cycle can be seen within the figure below. Within the figure below it can be seen that the duty cycle is again off by a small amount. This is again due to the wires being used.
![image](https://user-images.githubusercontent.com/98828696/202477871-f6223e88-f486-46a1-a0eb-aea6a5ef56bf.png)

![scope_13](https://user-images.githubusercontent.com/98828696/201200302-80c244d6-a2ee-4e86-aa75-b55e915f9e8e.png)


![image](https://user-images.githubusercontent.com/98828696/202478407-88a678f6-dc78-4c54-8cc3-5cd2e9cd48db.png)
