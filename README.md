# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

 Half adder

 ![Screenshot 2025-01-03 104502](https://github.com/user-attachments/assets/7df3ce44-35c7-41fe-a39c-f9ea53ac6e0c)

 Half subtractor

 ![Screenshot 2025-01-03 105533](https://github.com/user-attachments/assets/12ca5528-3fb0-4944-b8f1-d4f642d9509a)



Developed by:A.AKILA RegisterNumber:24900889

**RTL Schematic**
HALF SUBTRACTOR

![HALF SUTRACTOR](https://github.com/user-attachments/assets/67904597-3982-469a-b8e9-0282580a5041)

HALF ADDER

![HALF ADDER](https://github.com/user-attachments/assets/de38e6cc-493d-482b-afc1-281713851075)



**Output/TIMING Waveform**

```
module halfadderandsubtractor (a,b,dif,bor);
input a,b;
output dif,bor;
assign dif=a^b;
assign x=~a;
assign bor=b&x;
endmodule
```

```
module adder (a,b,v,j);
input a,b;
output v,j;
assign v=a^b;
assign j=a&b;
endmodule
```

HALF SUBTRACTOR

![half subtractor waveform](https://github.com/user-attachments/assets/8eaae2cb-c7de-405e-8af0-62a8c5caee05)

HALF ADDER

![half adder waveform](https://github.com/user-attachments/assets/84fdbabb-617a-414c-b8dd-16cb1b5f93ec)



**Result:**
Thus a half adder and half subtractor circuit and  its truth table  is verified in Quartus using Verilog programming.

