# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![image](https://user-images.githubusercontent.com/36288975/169644844-1a14e123-7228-4ed8-81a9-eb937dff4ac8.png)


4-bit Count Down Counter
### Procedure
/* write all the steps invloved */



### PROGRAM 

i)upcounter


![image](https://github.com/AjayM014/Exp-7-Synchornous-counters-/assets/150011759/8191ba70-75f3-4821-937a-0a47e7533d56)

ii)downcounter


![image](https://github.com/AjayM014/Exp-7-Synchornous-counters-/assets/150011759/f55881c1-945f-4a14-a7df-39c90588bc3d)

/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: AJAY M
RegisterNumber:  23013424
*/






### RTL LOGIC UP COUNTER AND DOWN COUNTER  


i)upcounter
![image](https://github.com/AjayM014/Exp-7-Synchornous-counters-/assets/150011759/adf66871-df68-4696-b008-5c8d71424674)

ii)downcounter


![image](https://github.com/AjayM014/Exp-7-Synchornous-counters-/assets/150011759/1954ac3a-d334-4809-8d54-cf86aa2b4e20)




### TIMING DIGRAMS FOR COUNTER  
i)upcounter
![image](https://github.com/AjayM014/Exp-7-Synchornous-counters-/assets/150011759/58bee7c1-3735-4e29-b49d-cdc71c6127ab)

ii)downcounter
![image](https://github.com/AjayM014/Exp-7-Synchornous-counters-/assets/150011759/4bd1c060-f7cd-4721-9ed8-8ca0120fb3e6)




### TRUTH TABLE 
i)upcounter
![image](https://github.com/AjayM014/Exp-7-Synchornous-counters-/assets/150011759/8a79ee7e-83ae-48a9-807b-e54cec13a9c3)

ii)dowmcounter

![image](https://github.com/AjayM014/Exp-7-Synchornous-counters-/assets/150011759/9ef3f81c-d9ce-450c-92eb-a07071e42582)





### RESULTS 
