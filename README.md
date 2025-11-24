AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
Equipment Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Logic Diagram
Procedure
1.	Type the program in Quartus software.
2.	Compile and run the program.
3.	Generate the RTL schematic and save the logic diagram.
4.	Create nodes for inputs and outputs to generate the timing diagram.
5.	For different input combinations generate the timing diagram.
Program:
```
F(A,B,C,D)=AB+CD+AD

module boolean_function_4var (
    input  wire A,
    input  wire B,
    input  wire C,
    input  wire D,
    output wire F
);

assign F = (~A & B) | (C & D) | (A & ~D);

endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: V Karthi  RegisterNumber: 25017522  */
RTL realization:
<img width="770" height="857" alt="image" src="https://github.com/user-attachments/assets/e3e5892a-c911-41d6-8c0d-d284a932e2b9" />

Timing Diagram:
<img width="1137" height="856" alt="image" src="https://github.com/user-attachments/assets/c7114402-3610-42f2-8254-9acf708d432a" />


Result: Thus, the given logic functions are implemented using and their operations are verified using Verilog programming.
