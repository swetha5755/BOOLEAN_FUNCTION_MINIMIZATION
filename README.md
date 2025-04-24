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
```
module exp2(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
output F1,F2;
wire X1,X2,X3,X4,X5,X6;
assign X1=(~B)&(~D);
assign X2=(A)&(B)&(~C);
assign X3=(~A)&(B)&(D);
assign X4=(~Y)&(Z);
assign X5=(X)&(Y);
assign X6=(W)&(Y);
assign F1=X1|X2|X3;
assign F2=X4|X5|X6;
endmodule
```

**RTL realization**

![Screenshot 2025-04-24 105355](https://github.com/user-attachments/assets/0d879057-e7b9-45b0-903d-3cc5ec06665f)

**Output:**

![WhatsApp Image 2025-04-24 at 10 55 14_290287d6](https://github.com/user-attachments/assets/25fe416e-a2dc-4fea-9817-937f6d4834a0)

**Timing Diagram**

![Screenshot 2025-04-24 110112](https://github.com/user-attachments/assets/edb55a47-5e18-41f7-a83a-c6184e3fbfaf)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

