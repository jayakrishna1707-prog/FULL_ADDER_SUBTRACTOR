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

**Procedure**

Write the detailed procedure here

**Program:**

Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: SRI JAYAKRISHNA E
RegisterNumber:25009564

```
full adder

module fa(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor g1(sum,a,b,c);
assign carry=((a&b)|(b&c)|(c&a));
endmodule 

full subractor

module fs(a,b,c,diff,borr);
input a,b,c;
output diff,borr;
xor g1(diff,a,b,c);
assign borr=((~a&b)|(b&c)|(~c&a));
endmodule
```

**RTL Schematic**

![WhatsApp Image 2025-11-24 at 09 18 01_61ce493b](https://github.com/user-attachments/assets/8b7d39b4-839e-42a5-bcc5-502fa0d3a263)


![WhatsApp Image 2025-11-24 at 09 18 02_a38472f9](https://github.com/user-attachments/assets/f0be210f-8f39-4520-9ca0-49bdccf89282)


**Output Timing Waveform**


![WhatsApp Image 2025-11-24 at 09 18 02_c28607c2](https://github.com/user-attachments/assets/d498df61-b580-4b38-bdb1-f506d08a7c18)

![WhatsApp Image 2025-11-24 at 09 18 02_6eb3b09d](https://github.com/user-attachments/assets/4265535c-3ac1-4224-8105-bc283c771efd)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



