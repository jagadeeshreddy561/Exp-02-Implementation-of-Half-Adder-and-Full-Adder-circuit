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
```python
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: jagadeeshreddy561
RegisterNumber: 212222240059 
```
### Half Adder:
```python
module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule
```
### Full Adder:
```python
module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```
### Output:
### HALF ADDER

![HALFADD](https://github.com/jagadeeshreddy561/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120623104/dc3fabbc-2279-4ecd-8ccb-d195ce07c121)

### FULL ADDER

![FULLADD](https://github.com/jagadeeshreddy561/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120623104/060d5b72-ca5e-4ec5-9e4a-0d83e6a1ae3d)

### RTL
### HALF ADDER

![HALFADDL](https://github.com/jagadeeshreddy561/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120623104/36d0aaa7-3c45-4571-a63c-a5c1593e22c0)

### FULL ADDER

![FULLADDL](https://github.com/jagadeeshreddy561/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120623104/5fa44b26-e815-4817-b51f-7c51cb5d5356)


### TIMING DIAGRAM
### HALF ADDER

![HALFADDTD](https://github.com/jagadeeshreddy561/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120623104/a1887ff0-87c4-479a-8610-3aa2d8e08f26)

### FULL ADDER

![FULLADDTD](https://github.com/jagadeeshreddy561/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120623104/da8a5a9e-a50e-48e4-b868-aa6569eaf6a7)


### TRUTH TABLE 
### HALF ADDER

![HALFADDTT](https://github.com/jagadeeshreddy561/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120623104/d4294736-51f0-4ba3-aa27-180344ae1ce4)

### FULL ADDER

![FULLADDTT](https://github.com/jagadeeshreddy561/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120623104/8ec10417-e254-4ecd-a58b-a75b06eca76a)

### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
