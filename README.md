# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: U.koti sai sankar

RegisterNumber:  212222240111

## Half Adder
```
module Adder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule 

```
## Full Adder
```
module FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule

```
*/
Logic symbol & Truthtable
## HALF Adder:
## output

![image](https://user-images.githubusercontent.com/118344248/228606114-f118ff67-34dc-4576-a107-d6e130b9f0d2.png)

## RTL
![image](https://user-images.githubusercontent.com/118344248/228606243-cdcf1cc8-5a75-45dc-b05c-db14e0a9d13a.png)

## Timing diagram
![image](https://user-images.githubusercontent.com/118344248/228606354-6f891a0a-9f14-41d1-8a50-524d46219f30.png)

## Truth Table
![image](https://user-images.githubusercontent.com/118344248/228606510-b9439107-200e-4198-8c64-8f931ecf9718.png)

## Full Adder:

### Output:
![image](https://user-images.githubusercontent.com/118344248/228606846-bfd36cbc-a959-4ee0-904a-e0a3a96e1dc5.png)


### RTL
![image](https://user-images.githubusercontent.com/118344248/228606892-a05d136d-bd3b-4264-adfe-5d3ad9ec0409.png)


### TIMING DIAGRAM
![image](https://user-images.githubusercontent.com/118344248/228606953-c1670a03-89b1-49bc-8fb2-e4675d216920.png)


### TRUTH TABLE 
![image](https://user-images.githubusercontent.com/118344248/228607028-df5382c7-7772-42d3-9376-e639fe171b90.png)


### Result:
Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.
