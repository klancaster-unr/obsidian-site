# CPE 301 Check Your Understanding
## Topic: Basic Electronics for Embedded Systems

This is an ungraded assignent designed to give you practice working problems from class.

For each math problem, work through the math and then check your answer against the one given.

1\. Three resistors are connected in parallel. The resistors have values of 200,300, and 1000 Ohms. Find the total resistance. <details><summary>Answer</summary>**Answer: 107.1 Ohms**</details>
2\. Repeat problem 1 using resistor values of 100, 100, and 1000000 Ohms. <details><summary>Answer</summary>**49.997 Ohms**</details>
3\. Choose some random resistance values and repeat the parallel resistance calculation. What can you say about how the total resistance relates to the individual resistance values?<details><summary>Answer</summary>The total resistance is always less than the smallest resistor in the circuit.</details>
4\. Referring to the image below, calculate the total current and the voltage across R1 assuming that the LED has a forward voltage rating of 1.3 volts. <details><summary>Answer</summary>VR1=3.7, I=3.7/500=0.0074 A</details>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
&NewLine;  
&NewLine;  
&NewLine;  
&NewLine;  
&NewLine;  
&NewLine;  
6. \\
7. \\\\\\\<tab>![[led.png]]
8. Capacitors have an impedance that goes down as frequency increases, so that at very high frequencies they can act almost like a short circuit. Think about how a voltage divider works with two resistors. Given the circuit below, how do you think the output voltage `out` would change as the frequency of the source `V2` increases? What would the output voltage be if `V2` were DC (frequency = 0)?	
9. &NewLine;  
10. &NewLine;  
11. &NewLine;  
12. &NewLine;  
13. &NewLine;  
14. &NewLine;  
    ![[low-pass-filter.png]]
	<details><summary>Answer</summary>As the frequency increases, the voltage `out` would decrease. If the voltage source were to be DC, the output would be the same as the source voltage. This circuit acts as a low-pass filter.</details>

6. The output voltage of an Arduino pin is 5 volts. Review the diode spec sheet attached to this exercise and determine the value of a resistor that you would need to use to make the current in the circuit equal to 20 mA (.020 Amps). The circuit would be the same as that shown in problem 4 with the Arduino playing the role of Vs. <details><summary>Answer</summary>From the datasheet, VF, the typical forward voltage, is 1.85 volts. The voltage across the resistor is going to be 5 - 1.85 = 3.15 volts. From Ohm's Law, we have R = V/I = 3.15/0.02 = 157 Ohms</details>  
  
## Challenge
Assume that you want a circuit that will filter out low frequencies. How could you build such a circuit using a resistor and a capacitor?




  

    
    
   
    





