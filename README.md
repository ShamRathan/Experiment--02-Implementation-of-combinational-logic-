# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
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

## Timing Diagram
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
