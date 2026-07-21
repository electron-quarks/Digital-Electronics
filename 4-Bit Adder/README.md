# 4-Bit Binary Adder

This project implements a 4-bit Binary Adder on a breadboard using the 74LS83 4-bit Full Adder IC. The circuit performs binary addition of two 4-bit input numbers and produces a 4-bit Sum along with a Carry output.

## Objective

To design and implement a 4-bit Binary Adder capable of adding two 4-bit binary numbers using the 74LS83 Full Adder IC.

## Boolean Function

The 74LS83 internally performs four full-adder operations.

For each bit:

- Sum = A ⊕ B ⊕ Cin
- Carry = AB + Cin(A ⊕ B)

## Logic IC Used

- 1 × 74LS83 4-Bit Full Adder IC

## Components Required

- Breadboard
- 74LS83 4-Bit Full Adder IC
- DIP Switches (for inputs)
- LEDs (for outputs)
- 330 Ω Resistors
- Jumper Wires
- 5 V Power Supply

## Inputs

- A3, A2, A1, A0
- B3, B2, B1, B0
- Carry Input (Cin)

## Outputs

- S3, S2, S1, S0
- Carry Output (Cout)

## Truth Table

Since the circuit has 9 input bits (A3–A0, B3–B0, and Cin), a complete truth table would contain 512 combinations. Instead, a few sample cases are shown below.
## Sample Input and Output Table

| A    | B    | Cin | Sum  | Cout |
|------|------|-----|------|------|
| 0000 | 0000 | 0 | 0000 | 0 |
| 0000 | 0001 | 0 | 0001 | 0 |
| 0001 | 0001 | 0 | 0010 | 0 |
| 0010 | 0011 | 0 | 0101 | 0 |
| 0011 | 0101 | 0 | 1000 | 0 |
| 0100 | 0011 | 0 | 0111 | 0 |
| 0101 | 0101 | 0 | 1010 | 0 |
| 0110 | 0111 | 0 | 1101 | 0 |
| 0111 | 1000 | 0 | 1111 | 0 |
| 1000 | 0001 | 0 | 1001 | 0 |
| 1001 | 0110 | 0 | 1111 | 0 |
| 1010 | 0101 | 1 | 0000 | 1 |
| 1100 | 0011 | 0 | 1111 | 0 |
| 1111 | 0001 | 0 | 0000 | 1 |
| 1111 | 1111 | 0 | 1110 | 1 |

## Circuit Operation

The 74LS83 consists of four cascaded full adders. Each stage adds one bit from input A and input B along with the carry from the previous stage. The least significant stage receives the external Carry Input (Cin), while the final stage generates the Carry Output (Cout). The resulting 4-bit Sum is available at outputs S0 through S3.

## Applications

- Arithmetic Logic Units (ALUs)
- Digital Calculators
- Microprocessors
- Binary Arithmetic Circuits
- Digital Signal Processing Systems


## Author

Nithish AS
