# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**
**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module exp22(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule

```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:
vignesh raaj
RegisterNumber:212223230239


**Logic Diagram**
![ex 2(2) gate](https://github.com/23002776/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742657/5eff3a58-6b34-43e1-aad0-00e776b37f2b)

**RTL realization**
![ex 2(1) gate](https://github.com/23002776/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742657/7e13c989-c381-42d8-a34a-88075f794685)


**Output:**
**truthtable**
![ex 2 gate](https://github.com/23002776/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742657/1902cbbc-b9ed-4a11-84e4-0b4328c65387)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
