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

### Program:
```
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:P.Ramsai 
RegisterNumber: 212221240041 
*/

Half adder program:

module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule


Full adder program:

module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```
Logic symbol & Truthtable RTL realization
### Output:
### RTL
## Half adder:
![Screenshot (113)](https://user-images.githubusercontent.com/94269989/190303468-9f46ad57-fb8a-4eca-8d6e-55d90cbdde16.png)
## Full adder:

![Screenshot (114)](https://user-images.githubusercontent.com/94269989/190303547-251987cb-016a-4d8b-bc37-a8dfeb71119c.png)

### TIMING DIAGRAM
## Half adder

![Screenshot (115)](https://user-images.githubusercontent.com/94269989/190303650-5a7c9d10-da75-4a0e-9495-4a90b104bce7.png)
 
## Full adder

![Screenshot (116)](https://user-images.githubusercontent.com/94269989/190303721-6328c77f-87d4-47ce-b7b4-33189cd376f8.png)

### TRUTH TABLE 
## Half adder
![Screenshot (117)](https://user-images.githubusercontent.com/94269989/190303854-01884da8-d63a-4bc2-bce8-ac3737bd7d32.png)


## Full adder
![Screenshot (118)](https://user-images.githubusercontent.com/94269989/190303875-a4149d3f-8917-45c0-b488-a6575e69970a.png)

## Resultt:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
