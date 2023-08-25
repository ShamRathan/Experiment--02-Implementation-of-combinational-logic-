# Experiment 02 Implementation of combinational logic:
 
## AIM:
To implement the given logic function verify its operation in Quartus.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
 
 
 
## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime


## Theory:
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.
 

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

## Output:
## RTL:
![image](https://github.com/ShamRathan/Experiment--02-Implementation-of-combinational-logic-/assets/93587823/712b7a20-0fcd-48ad-9331-7bcd31542492)

## Truth Diagram:
![image](https://github.com/ShamRathan/Experiment--02-Implementation-of-combinational-logic-/assets/93587823/00724f15-1e45-4fd7-976e-0eae90e2919d)


## Waveform verified:
![image](https://github.com/ShamRathan/Experiment--02-Implementation-of-combinational-logic-/assets/93587823/a13fe4c6-e94f-4237-b08d-b3536e599825)



## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
