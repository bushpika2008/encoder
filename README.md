# encoder
# Developed by: BUSHPIKA C
# REGISTER NO:25007434
# ENCODER 8TO3 DATAFLOW Modelling
# AIM:

To implement Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

# SOFTWARE REQUIRED: Quartus prime

# THEORY

# Encoder 8 To 3

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.
# BLOCK DIAGRAM:
<img width="396" height="327" alt="image" src="https://github.com/user-attachments/assets/10e7408d-cff0-4984-bb75-062fa595278b" />
# TruthTable:
<img width="552" height="413" alt="image" src="https://github.com/user-attachments/assets/0edc239d-a2cd-42d3-a364-20670ea59e6c" />
The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

<img width="825" height="467" alt="image" src="https://github.com/user-attachments/assets/191a018d-1ff7-4774-ad90-c3ec9f2c1a5d" />
# Procedure


# PROGRAM
```
module exp5(din,a,b,c);
input [0:7] din;
output a,b,c;
assign a=(din[4]| din[5]| din[6 ]| din[7]);
assign b=(din[2]| din[3]| din[6]| din[7]);
assign c=(din[1]| din[3]| din[5 ]| din[7]);
endmodule
```


# RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling:
<img width="1920" height="1080" alt="Screenshot 2025-12-05 094435" src="https://github.com/user-attachments/assets/4567b3c8-4dc5-4cac-a6b7-f44639ce324a" />


# TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling
<img width="1920" height="1080" alt="Screenshot 2025-12-06 131047" src="https://github.com/user-attachments/assets/ed3ce215-3fcb-4cc2-996d-1a003ec43ae1" />


# RESULTS:
  Thus the program to execute the encoder has beeen executed successfully with the help of RTL viewer.
