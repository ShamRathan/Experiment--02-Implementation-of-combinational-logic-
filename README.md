# Experiment 02 Implementation of combinational logic:
 
## AIM:
To implement the given logic function verify its operation in Quartus.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime


## Theory:
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.
 

## Logic Diagram:
![image](https://github.com/ShamRathan/Experiment--02-Implementation-of-combinational-logic-/assets/93587823/907d036c-9e3a-40d5-94c7-b0fe50d7942c)

## Procedure:
Step 1: Create a project with required entities.

Step 2: Create a module along with respective file name.

Step 3: Run the respective programs for the given boolean equations.

Step 4: Run the module and get the respective RTL outputs.

Step 5: Create university program(VWF) for getting timing diagram.

Step 6: Give the respective inputs for timing diagram and obtain the results.

## Program:
```
Developed by: Sham Rathan S
RegisterNumber: 212221230093

module Exp02(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule

```
## RTL realization

## Output:
## RTL:
![image](https://github.com/ShamRathan/Experiment--02-Implementation-of-combinational-logic-/assets/93587823/712b7a20-0fcd-48ad-9331-7bcd31542492)

## Timing Diagram:
![image](https://github.com/ShamRathan/Experiment--02-Implementation-of-combinational-logic-/assets/93587823/c888c720-d762-4e66-bd50-b406924c1814)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
