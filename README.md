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


## Program:

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:AMIRTHA VARSHINI V

RegisterNumber:212223040014

```

module booleanfun(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
and g1(s,ydash,z);
and g2(t,x,y);
and g3(u,w,z);
or g4(f2,s,t,u);
endmodule
```

## RTL realization

![RTL diagram](https://github.com/amirthaviswanathan05/BOOLEAN_FUNCTION_MINIMIZATION/assets/149035397/fdbc2456-94f7-4ce2-9335-83621d024804)


## Timing Diagram

![timing diagram](https://github.com/amirthaviswanathan05/BOOLEAN_FUNCTION_MINIMIZATION/assets/149035397/e03a69f3-60df-4a66-bd45-0a12002b8f60)


## Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

