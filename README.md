# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

![WhatsApp Image 2024-11-22 at 10 50 12 AM](https://github.com/user-attachments/assets/f698bb7c-5772-4048-9717-4ba0a4439897)


![WhatsApp Image 2024-11-22 at 10 50 13 AM](https://github.com/user-attachments/assets/804a67b7-a1c7-42bc-8174-1783f4c00bc2)


**Procedure**

1. Type the program in Quartus software.
 2. Compile and run the program.
 3. Generate the RTL schematic and save the logic diagram.
4. Create nodes for inputs and outputs to generate the timing diagram.
 5. For different input combinations generate the timing diagram.

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

```
module exp4 (df, bo, a, b, bin);
 output df;
 output bo;
 input a;
 input b;
 input bin;
 wire w1,w2,w3;
 assign w1=a^b;
 assign w2=(~a&b); 
 assign w3=(~w1&bin);
 assign df=w1^bin;
 assign bo=w2|w3;
 endmodule
```

Developed by: RegisterNumber: 24000491*/

**RTL Schematic**

![Screenshot (7)](https://github.com/user-attachments/assets/eca59804-ecad-4867-ac5a-17705cc99f9e)


**Output Timing Waveform**


![Screenshot (8)](https://github.com/user-attachments/assets/771712d0-2fc0-4f74-869d-d82fc6b22c78)



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



