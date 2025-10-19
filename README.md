# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
module Exp2_1(a, b, c, d, f1);
    input a, b, c, d;
    output f1;

    assign f1 = ((~b & ~d) | (~a & b & d) | (a & b & ~c));
endmodule


module Exp2_2(w, x, y, z, f2);
    input w, x, y, z;
    output f2;

    assign f2 = ((~y & z) | (w & y) | (x & y));
endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Sujitha Mahalakshmi M RegisterNumber:25018945


**RTL realization**

**Output:**

**RTL**
<img width="1920" height="1080" alt="Screenshot 2025-10-19 203937" src="https://github.com/user-attachments/assets/d30bd2d4-e079-4d33-aefc-0aff2bf3b721" />

**Timing Diagram**
![exp 2](https://github.com/user-attachments/assets/8f6f3a99-96ca-4b87-84d8-6bfaa2987a37)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

