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

Developed by: KATHIRVEL.A

RegisterNumber: 212221230047

```
module booleanmin(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
and(s,ydash,z);
and(t,x,y);
and(u,w,y);
or(f2,s,t,u);
endmodule
 

Developed by:R Adarsh Chowdary
 RegisterNumber:212223040166

```


**RTL realization**

**Output:**

**RTL**


![image](https://github.com/KathirvelAIDS/BOOLEAN_FUNCTION_MINIMIZATION/assets/94911373/0eac37d9-fbc6-4760-b6a0-b2d450a0d131)




**Timing Diagram**




![image](https://github.com/KathirvelAIDS/BOOLEAN_FUNCTION_MINIMIZATION/assets/94911373/b4ca1d4f-bebf-42ee-b77f-75013e3b74b3)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

