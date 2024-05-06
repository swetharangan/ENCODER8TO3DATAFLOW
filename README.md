### ENCODER 8TO3 DATAFLOW Modelling

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

/* write all the steps invloved */

~~~
1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

~~~

**PROGRAM**

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 
~~~
module EX05(din, a, b, c); 
input [0:7] din; 
output a,b,c; 
assign a= (din[4] | din[5] | din[6] | din[7]); 
assign b= (din[2] | din[3] | din[6] | din[7]);
assign c= (din[1] | din[3] | din[5] | din[7]);
endmodule
~~~

Developed by: VARSHA A 
RegisterNumber: 212223220121
*/

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

![319870155-bff96462-4812-457a-b9d9-c539895c968d](https://github.com/04Varsha/ENCODER8TO3DATAFLOW/assets/149035374/29eb045b-c9ea-4990-9d68-c73ca7e0490c)

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

![319870178-f3bb2348-3b1f-4b23-a8ca-4e1dc8e2bffe](https://github.com/04Varsha/ENCODER8TO3DATAFLOW/assets/149035374/e7d13f32-64fb-4bf0-ae63-698e23f1e3fb)

**RESULTS**

Thus the implement Encoder 8 To 3 in Dataflow Modelling using verilog in Quartus software is successfully verified.

