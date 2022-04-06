# CPE 301 S22 Midterm Review

## Practice Midterm Solutions

- Q1: Binary AND is can be used to set bits to 0.
	-	This is true because you can have a mask that has a value of 0 in a bit position, so that ANDing it with any value results in 0

- Q2: Putting an asterisk in front of a pointer indcates that you are _deferencing_ the pointer

- Q3: The current in a resistor is directly proportional to the voltage across it. Remember the I = V/R, so I goes up as V goes up.

- Q4: A circuit has two 100Ω resistors in series connect to a 10 volt supply. The current is 		![[Pasted image 20220308171222.png]]

- Q5: The keyword volatile tells the compiler to store the value in a register and not in RAM.
	- False. The keyword prevents the compiler from optimizing the value out or cacheing the value in a register.
	
- Q6: The following code sets bit 2 in an 8-bit register to 1 and leaves all others as they were: 
 
 `unsigned char* reg = 0x24;`
`*reg |= 1 << 2;`

	- True

- Q7: Assume that the circuit has been in the configuration shown for a very long time. What is the current in the circuit?
![[SCR-20220308-o4j.png]]
	- The current is 0. In a DC circuit that has reached steady-state (as this one has, since it has been like this for a long time), the cap acts as an open circuit, so there is no current
	
- Q8: What is the current in this circuit if the forward voltage drop for the diode is 1.4 volts?

![[Pasted image 20220308173024.png]]

- Q9: Set pin 11 on the Aruindo 2560 to be an output
Pin 11 is bit 5 on port B.
```
unsigned char* ddrb = 0-x24;
*ddrb |= 1 << 5;
```

- Q10: You are asked to generate a 1200 Hz 75% duty cycle PWM wave on an Arduino 2560 Mega with a clock frequency of 16 MHz using normal mode using a 16 bit timer. Calculate the values that must be stored as starting points in the timer for both the high and low states. Show all of your work.
	- ![[Pasted image 20220308173451.png]]

- Q11: Describe the use of a parity bit to detect errors in serial transmission. Can you think of a scenario where the parity check would fail to ﬁnd an error in transmission?
	- A parity bit is added to the data bits. For even parity, the parity bit is set so that the total number of 1s is even. For odd parity, it is set so that the total number is odd. If the parity bit is set (a 1) for even parity and the number of 1s is odd, an error occurred during transmission. The system could fail if two bits have an error.

- Q12: In an I2C system, pullup resistors are used on the SCL and SDA lines. Why?
	- The I2C protocal requires the SDA and SCL lines to be held high when between tranmissions. The SDA line is pulled low to start transmissions. The pullup resistors ensure that the lines are high when no data is being tranmitted.

- Q13: Common mode rejection ratio (CMRR) is a figure of merit for a differential amplifier that is on the receiving end of a wired differential connection. What does a high CMRR mean with respect to the quality of the circuit? 
	- Amplifiers have ratings related to the amplification applied to signals that are common (same phase, amplitude) applied to their inputs. 	Ideally, the amplification for these common mode signals would be 0. The CMRR is equal to 20xlog(differential gain/common mode gain), so the smaller the common mode gain, the higher the CMRR. Since common mode signals are typically noise induced into the circuit by external sources, the more they can be rejected the better.
- Q 14: Compare and contrast SRAM and dynamic RAM.
	- SRAM is faster than dynamic RAM since it does not need to be refreshed
	- SRAM requires more components
	- DRAM is inexpensive, requiring very few components, however, it requires periodic refreshing of each cell. The makes it slower than SRAM.

## Topics not Covered in the Practice Exam

### ADC
- Review the signal chain for analog to digital conversion. 
	- Example: What is the purpose of the low pass filter at the start of the signal chain?
- Review the concept of bandwidth and the Nyquist frequency.

### Serial Transmission
Review the concepts behind using a differential amplifier on the receiving end of a transmission line.

### Memory Architectures
- Review Princeton vs Harvard architectures
- Review the material related to using address lines to select memory modules
	- Example: How many memory modules can you use if you have allocated 3 bits out of 16 for memory selection? What would be the maximum memory address for any individual chip in this scenario?
		- 3 bits would give you 2^3 = 8 possible memory chip selections using a decoder (0 through 7)
		- The 13 remaining bits would give you 2^13 -1 = 8191 as the maximum memory address