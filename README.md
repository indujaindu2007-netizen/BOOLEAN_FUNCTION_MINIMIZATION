

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

The minimised expression of F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D is F1=B'D' + ABC' + A'BD


The minimised expression of F2=xy’z+x’y’z+w’xy+wx’y+wxy is F2= y′z + yw + yx



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations, generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in Quartus using Verilog programming. 
```
module exp2(a,b,c,d,f1,w,x,y,z,f2); 
input a,b,c,d,w,x,y,z; 
output f1,f2; 
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
assign f2=((~y & z)|( w & y )|(x & y)); 
endmodule
```


Developed by: Induja R Register Number:25001726

**RTL realisation**
<img width="480" height="503" alt="Screenshot 2025-10-18 105157" src="https://github.com/user-attachments/assets/e78f275a-5b77-461a-ae98-a93ea363ae18" />


**RTL**
<img width="1919" height="932" alt="Screenshot 2025-10-18 112849" src="https://github.com/user-attachments/assets/8dba101f-7b33-4dc7-a9de-6e5545b1cdc6" />



**Result:**

Thus, the given logic functions are implemented using and their operations are verified.



