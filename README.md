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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/

i)

module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

ii)

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule


**RTL realization**

F1:

<img width="1147" height="602" alt="Screenshot 2025-10-08 132950" src="https://github.com/user-attachments/assets/6e30120b-5a41-4ce4-9b5e-0970821333d3" />

F2:

<img width="979" height="532" alt="Screenshot 2025-10-08 133628" src="https://github.com/user-attachments/assets/35895529-b59b-411f-95e4-9cae1388b010" />


**Output:**

**RTL**

**Timing Diagram**

F1:

<img width="1919" height="596" alt="Screenshot 2025-10-08 133325" src="https://github.com/user-attachments/assets/7e2c112d-965d-471c-84d1-a3a2fdf1cdf1" />

F2:


<img width="1919" height="616" alt="Screenshot 2025-10-08 134006" src="https://github.com/user-attachments/assets/415a4296-8434-4580-a2be-ced0181fad0d" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

