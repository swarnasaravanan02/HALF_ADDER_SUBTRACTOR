# HALF_ADDER_SUBTRACTOR
## NAME: SWARNA PRIYA S
## REG .NO: 212225040447
## DATE: 21.11.2026

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
half adder
module exp3 (
    input  wire a, b,     
    output wire sum,     
    output wire carry    
);

    
    assign sum   = a ^ b;   
    assign carry = a & b;   
    endmodule

    half subracter

    module half_subtractor (
    input  wire a, b,         // Inputs
    output wire diff, borrow  // Outputs
);

    // Logic equations
    assign diff   = a ^ b;     // XOR for difference
    assign borrow = ~a & b;    // Borrow when a < b

endmodule
/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: RegisterNumber:*/25004301

**RTL Schematic**
half adder

<img width="356" height="247" alt="half adder 1" src="https://github.com/user-attachments/assets/e9460b5e-476e-43b5-ac04-dcf6b7f30faa" />

half subracter

<img width="460" height="227" alt="half subracter 1" src="https://github.com/user-attachments/assets/6ee6e35b-9005-4b4b-a8f1-e6a04d9a1cc6" />



**Output/TIMING Waveform**
half adder

<img width="1025" height="468" alt="half adder" src="https://github.com/user-attachments/assets/7fd8ff5c-4531-4ee7-9391-1a9716494a45" />

half subracter


<img width="1034" height="504" alt="half subracter" src="https://github.com/user-attachments/assets/a6afe2bb-8ef1-4c82-807f-f54c57cefa8a" />


**Result:**
This Program was excecuted successfully

