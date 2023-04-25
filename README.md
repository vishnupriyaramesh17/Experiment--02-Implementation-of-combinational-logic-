# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory

Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.Combinational logic gates are digital circuits that produce outputs based solely on the current inputs. These gates are the building blocks for implementing digital systems and are used in a wide range of applications, including arithmetic and logic operations, memory devices, and control circuits.The two functions, F1 and F2, can be implemented using a combination of logic gates such as AND gates, OR gates, and NOT gates.

## Procedure:

1.Use module projname(input,output) to start the Verilog programmming.

2.Assign inputs and outputs using the word input and output respectively.

3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.

4.Use each output(RTL Viewer and Timing Diagram) to represent F1 and F2.

5.End the verilog program using keyword endmodule.

## Program:

/*

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by: Vishnupriya.R

RegisterNumber: 212222110054



F1= A'B'C'D'+AC'D'+B'CD'+A'BCD+BC'D

module exp2f1(A,B,C,D,F1);

input A,B,C,D;

output F1;

assign F1=(~B&~D)|(A&B&~C)|(~A&B&D);

endmodule



f2=xy'z+x'y'z+w'xy+wx'y+wxy


module exp2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=(~y&z)|(x&y)|(w&y);

endmodule


*/


## Output:

## RTL Diagram


## F1= A'B'C'D'+AC'D'+B'CD'+A'BCD+BC'D


![rtl exp2](https://user-images.githubusercontent.com/119393589/234242982-a3c5c7a8-6c16-4575-8d95-e8ec094bed0b.png)


## f2=xy'z+x'y'z+w'xy+wx'y+wxy

![exp 2 2 rtl](https://user-images.githubusercontent.com/119393589/234243078-51849feb-3907-4818-81bd-728299276d18.png)
## Timing Diagram
## F1= A'B'C'D'+AC'D'+B'CD'+A'BCD+BC'D

![exp 2 1 timing](https://user-images.githubusercontent.com/119393589/234243770-48a0dfc4-01f6-40a5-b834-40de30bf74e6.png)

## f2=xy'z+x'y'z+w'xy+wx'y+wxy
![exp2 2 timing](https://user-images.githubusercontent.com/119393589/234243812-2fbaf537-705e-408d-a5a3-01633bfe6f0b.png)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
