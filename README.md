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

Developed by: HEMANTH A Register Nnmber :212223220035
program

module combinationalcircuit(A,B,C,D,F1)
output F1;
wire x1,x2,x3,x4,x5;

assign x1=(~A)&(~B)&(~C)&(~D);

assign x2=(A)&(~C)&(~D);

assign x3=(~B)&(C)&(~D);

assign x4=(~A)&(B)&(C)&(D);

assign x5=(B)&(~C)&(D);

assign F1=x1|x2|x3|x4|x5;

endmodule

**RTL realization**
![image](https://github.com/Hemanthreddy0321/BOOLEAN_FUNCTION_MINIMIZATION/assets/150005937/5ec9f4c6-1da0-4d79-aea5-810ab4d72976)

Truth Table :
![image](https://github.com/Hemanthreddy0321/BOOLEAN_FUNCTION_MINIMIZATION/assets/150005937/cb29a431-cc89-4c19-90bd-7a8da8342085)


**Timing Diagram**
![image](https://github.com/Hemanthreddy0321/BOOLEAN_FUNCTION_MINIMIZATION/assets/150005937/a80833fa-14d6-4b36-89c7-42cef2b9b3db)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

