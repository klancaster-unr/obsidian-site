# Verilog Notes

## Modeling Styles

### Gate Level

- individual gates are used to create the circuit
- Example
	
```
	and(out,a,b)
	or(out, a,b,c,d)
```
	
### Dataflow Level
- the system is modelled in terms of the flow of data
- assign (continuous assignment)
	- Example:
	
```
module and_gate(a,b,out);
input a,b;
output out;

assign out = a&b;
endmodule
```

### Behavioral Level
- procedural statements used to define the functionality
```
	full_adder( A, B, Cin, S, Cout);
		input wire A, B, Cin;
		output reg S, Cout;

 		always @(A or B or Cin)
  			begin 
   				S = A ^ B ^ Cin; 
   				Cout = A&B | (A^B) & Cin; 
  			end
	endmodule
	
```
## Some Basic Terms
- input
	- designates a term as an input
- output
	- designates a term as an output
- reg
	- register: used to model a hardware register
	- you can designate the size of the register like this: 
		- reg[7:0] // this is an 8 bit register
- wire
	- used to model a physical connection between elements
	- wires can be any size, just as registers



