# Experiment--04-Implementation-of-combinational-logic-using-universal-gates
Implementation of combinational logic using universal-gates
 
## AIM:
To implement the given logic function using NAND and NOR gates and to verify its operation in Quartus using Verilog programming.

F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate
F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')' using NOR gate
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output. 

## Using NAND gates
NAND gate is actually a combination of two logic gates i.e. AND gate followed by NOT gate. So its output is complement of the output of an AND gate.This gate can have minimum two inputs, output is always one. By using only NAND gates, we can realize all logic functions: AND, OR, NOT, X-OR, X-NOR, NOR. So this gate is also called as universal gate. First note that the entire expression is inverted and we have three terms ANDed. This means that we must use a 3-input NAND gate. Each of the three terms is, itself, a NAND expression. Finally, negated single terms can be generates with a 2-input NAND gate acting as an inverted.

F=((C'.B.A)'(D'.C.A)'(C.B'.A)')'

## Logic Diagram

Using NOR gates
NOR gate is actually a combination of two logic gates: OR gate followed by NOT gate. So its output is complement of the output of an OR gate. This gate can have minimum two inputs, output is always one. By using only NOR gates, we can realize all logic functions: AND, OR, NOT, Ex-OR, Ex-NOR, NAND. So this gate is also called universal gate. Designing a circuit with NOR gates only uses the same basic techniques as designing a circuit with NAND gates; that is, the application of deMorgan’s theorem. The only difference between NOR gate design and NAND gate design is that the former must eliminate product terms and the later must eliminate sum terms.

F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')'

## Program:
/*
Program to implement the given logic function using NAND and NOR gates and to verify its operations in quartus using Verilog programming.
Developed by: NIRAUNJANA GAYATHRI G R
RegisterNumber:  22008369

![WhatsApp Image 2023-01-21 at 09 58 18](https://user-images.githubusercontent.com/119395610/213843348-5f5ef2d7-961b-4a46-a57f-7e06002eebdc.jpg)


## Truth Table:

![WhatsApp Image 2023-01-21 at 09 32 18](https://user-images.githubusercontent.com/119395610/213842823-46f3019f-b867-4849-922f-3efd81d31aee.jpg)

## RTL realization:
![WhatsApp Image 2023-01-21 at 09 30 03](https://user-images.githubusercontent.com/119395610/213842708-e43a5829-321b-4b8b-a9f2-16290cb4a55a.jpg)
![WhatsApp Image 2023-01-21 at 09 31 21](https://user-images.githubusercontent.com/119395610/213842718-92aaf0ed-25ad-4b17-a9db-f9d4e6fa3479.jpg)


## Output:
![WhatsApp Image 2023-01-21 at 09 33 16](https://user-images.githubusercontent.com/119395610/213842777-ec5b2af8-bede-4ab3-9b45-57cfa5513eff.jpg)


## Timing Diagram:
![WhatsApp Image 2023-01-21 at 09 33 16](https://user-images.githubusercontent.com/119395610/213842769-c98b243a-b020-4ea0-94a7-dc469ee8bbc9.jpg)

## Result:
Thus the given logic functions are implemented using NAND and NOR gates and their operations are verified using Verilog programming.
