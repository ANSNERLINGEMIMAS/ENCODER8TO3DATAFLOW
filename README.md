**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.




**PROGRAM**

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 
```
exp5encoder_8x3
module encoder_8x3(din,a,b,c);
input [0:7] din;
output a,b,c;
assign a=(din[4]|din[5]|din[6]|din[7]);
assign b=(din[2]|din[3]|din[6]|din[7]);
assign c=(din[1]|din[3]|din[5]|din[7]);
endmodule
```


Developed by:ANS NERLING EMIMA S RegisterNumber:212224040027
*/

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
![exp5](https://github.com/user-attachments/assets/05fe36a7-20b0-44ae-b22d-1eac75b1e40c)


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
![Screenshot 2025-04-16 110215](https://github.com/user-attachments/assets/e5368ad9-30bd-4f9a-965e-58b70a5ddb5c)


**RESULTS**

Thus Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables is verified.






