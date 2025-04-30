# 555 Timer IC Version 1

<h2>555 Timer IC - Introduction</h2>
The 555 timer is an integrated circuit (IC) that has the ability to perform timing operations, create a single electrical pulse and can be used in a number of modes. In this case, the 555 timer IC is in astable mode. Which is where the output of the IC alternates between a HIGH voltage (close to the Vcc of the IC) and a LOW voltage (close to zero). The duration of the HIGH voltage depends on the resistor and capacitor values.
<br />
<br />
The duty cycle is the percentage of time that the output is HIGH in a cycle. For example, if the duty cycle is 70%, that means the output goes HIGH for 70% of the entire cycle and the output goes low for 30% of the entire cycle.


 ### [555 Timer IC - Video Demonstration](https://drive.google.com/file/d/1qtJKtbxpB-tIAMOESbsBYi-Mht5HvbB3/view?usp=sharing)

<h2>Circuit Description</h2>
The electronic circuit powered by an adjustable DC power supply. The IC illuminates the blue LED and turns off the green LED, then turns off the blue LED and lights up the green LED. The frequency or the length of the period can be adjusted using the potentiometer which is more closely linked to R4 (adjusting the potentiometer has no affect on the resistance of R3). The reset pin of the 555 timer IC is connected to a button, when pressed will connect the reset pin to ground and hold the output to LOW. The reset pin is active-low, which means that the reset pin is only activated when the pin is connected to ground.
<br />
<br />
The length of the period is 455ms, where the output of 555 timer IC (the portion of the wave) is HIGH for 231ms and the output will go LOW for 224ms. These numbers are obtained when the potentiometer is set at its highest resistance (22k Ohms). The duty cycle of the output is 51%. These values are obtained when R5 (the potentiometer) is set to 22kOhms (the maximum resistance). However, when the resistance of the potentiometer is set to a negligible resistance, the period is 147ms and the duration of the output at HIGH and LOW voltages is 77ms and 70ms respectively. A noticable difference between the duration of each cycle for when the potentiometer is set to its lowest and highest value.
<br />
<br />
The formulae used for the calculations are: 
<br />
* T = 0.7 * (R3 + 2(R4 + R5)) * C2
<br />
* T_H = 0.7 * (R3 + (R4 + R5)) * C2
<br />
* T_L = 0.7 * (R4 + R5) * C2
<br />
<br />
Where T represents the period of the square function, T_H represents the length of time that the output goes HIGH and T_L represents the length of time the output goes LOW. R3, R4 and R5 represent the resistors connected to pin 6 and 7 of IC. C2 refers to the capacitance of the capacitor connected to R5.

<h2>Circuit Schematic</h2>
<p align="center">
This is the circuit schematic which was created using draw.io. 
<br />
<img src="https://imgur.com/xf15KaI.png" height="70%" width="70%" alt="Main Menu"/>
<br />
<br />
One thing to note is that in the schematic above, the wire that goes from TRG (pin 2) to the THR (pin 6) is also connected between the R5 and the capacitor.

<h2>Square Wave from Oscilloscope</h2>
<p align="center">
This is a view of the square wave produced by the oscilloscope from the 555 timer IC. The duty cycle is slightly above 50%, which means that the amount of time the output goes HIGH is almost the same as the period of time the output goes LOW. The period of the square wave is 455ms. Although, if you were to measure the period using the oscilloscope, the period of the square wave is roughly 400ms, which is close to the number obtained from the formula T = 0.7 * (R3 + 2(R4 + R5)) * C2.
<br />
<img src="https://imgur.com/q2zRwlP.png" height="70%" width="70%" alt="Main Menu"/>
<br />
<br />


