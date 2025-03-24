# BOOLEAN_FUNCTION_MINIMIZATION

**DATE :12-03-2025**

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Implementing Boolean functions in Verilog HDL (Hardware Description Language) involves translating the simplified Boolean expressions into Verilog code to describe the behavior of digital circuits. The basic building blocks in Verilog is module. The module represent a combinationa circuit. Use logical operators (&, , ~, ^) to implement Boolean functions directly. Use built-in gate primitives for basic functions: Use University program VWF to verify the functionality of your Verilog modules. Create waveform and check outputs against expected results

**Logic Diagram**
![image](https://github.com/user-attachments/assets/ab280fb6-fdaa-48bc-b667-1f75681f5dd4)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: BARATHRAJ K

RegisterNumber:212224230033

```
module exp2a(a,b,c,d,F1);
intput a,b,c,d;
output F1;
assign F1=((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule

module exp2b(w,x,y,z,F2)
intput w,x,y,z;
output F2;
assign F2=((~y&z)|(x&y)|(w&y));
endmodule
```


**RTL realization**

**Output:**

**RTL**

EXP 2A
![image](https://github.com/user-attachments/assets/eac6d3ce-7521-4e7a-8bbc-d247c88289b7)

EXP 2B
![image](https://github.com/user-attachments/assets/fd7335f4-1435-4648-936c-fa9c42c82ada)

**Timing Diagram**

EXP 2A
![image](https://github.com/user-attachments/assets/872b7bb2-18f9-4a72-894f-27342579294d)

EXP 2B
![image](https://github.com/user-attachments/assets/8a025bf0-57a9-4726-a0e9-a63549fabbcb)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

