# 555 Timer IC Version 1

<h2>555 Timer IC - Introduction</h2>
The 555 timer is an integrated circuit (IC) that has the ability to perform timing operations, create a single electrical pulse and can be used in a number of modes. In this case, the 555 timer IC is in astable mode. Which is where the output of the IC alternates between a HIGH voltage (close to the Vcc of the IC) and a LOW voltage (close to zero). The duration of the HIGH voltage depends on the resistor and capacitor values.
<br />
<br />
The duty cycle is the percentage of time that the output is HIGH in a cycle. For example, if the duty cycle is 70%, that means the output goes HIGH for 70% of the entire cycle and the output goes low for 30% of the entire cycle.


 ### [555 Timer IC - Video Demonstration](https://drive.google.com/file/d/1qtJKtbxpB-tIAMOESbsBYi-Mht5HvbB3/view?usp=sharing)

<h2>Circuit Description</h2>
The electronic circuit illuminates the blue LED and turns off the green LED, then turns off the blue LED and lights up the green LED. The frequency or the length of the period can be adjusted using the potentiometer which is more closely linked to R2 (adjusting the potentiometer has no affect on the resistance of R1). The reset pin of the 555 timer IC is connected to a button, when pressed will connect the reset pin to ground and hold the output to LOW. The reset pin is active-low, which means that the reset pin is only activated when the pin is connected to ground.
<br />
<br />
The length of the period is 455ms, where the output of 555 timer IC(the portion of the wave) is HIGH for 231ms and the output will go LOW for 224ms. These numbers are obtained when the potentiometer is set at its highest resistance (22k Ohms). The duty cycle of the output is 51%. These values are obtained when R5 (the potentiometer) is set to 22kOhms (the maximum resistance). However, when the resistance of the potentiometer is set to near negligible value, the period is 147ms and the duration of the output at HIGH and LOW voltages is 77ms and 70ms respectively. A noticable difference between the duration of each cycle for when the potentiometer is set to its lowest and highest value.
<br />
<br />
The formulae used for the calculations are:
* T = 0.7 * (R1 + 2R2) * C1
<br />
* T_H = 0.7 * (R1 + R2) * C1
<br />
* T_L = 0.7 * R2 * C1
<br />
<br />
Where T represents the period of the square function, T_H represents the length of time that the output goes HIGH and T_L represents the length of time the output goes LOW. R1 and R2 represent the resistors connected to pin 6 and 7 of IC.

