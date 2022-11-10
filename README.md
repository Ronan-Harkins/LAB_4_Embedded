# LAB_4_Embedded
#### By: Ronan Harkins, 
## Introduction
The goal of lab for was to toggle the on board LED and produce a duty cycle with the timer within the MSP430FR2355. With this the the ouput should be sent to a pin on the board and the values should be able to be seen on the oscilloscope within the lab. 


### 10 Percent Duty Cycle 
For the ten percent duty cycle the values of TB0CCR0 was chnaged to be 500 and the value of TB0CCR1 was change to a value of 50. The reason this value was changed to 50 was because of the way the duty cycle is set. In order to obtain a duty cycle of 10% a value of 0.1 was needed from the combination of  TB0CCR1 divided by TB0CCR0. Since the values used within the code was 50/500 the output of this is 0.1 providing the correct duty cycle that is needed for part 1 of the lab. The duty cycle that was produced can be seen within the figure below. This process was done using the polling method. 

![scope_12](https://user-images.githubusercontent.com/98828696/201200352-896f0096-a02c-4281-add8-218aef6fe114.png)




### 20 Percent Duty Cycle 
For the 20% duty cycle the same method was applied however instead of using the polling method 
![scope_13](https://user-images.githubusercontent.com/98828696/201200302-80c244d6-a2ee-4e86-aa75-b55e915f9e8e.png)


