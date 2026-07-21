# Half Subtractor Using Simplified Boolean Logic

This project implements a  Half Subtractor on a breadboard using simplified Boolean expressions and standard TTL logic ICs. The circuit is built using XOR, AND, and NOT gates to perform binary subtraction of two input bits.

## Objective

To design and implement a Half Subtractor that subtracts one binary input from another, producing a Difference and Borrow output using simplified Boolean logic.

## Boolean Expressions

- Difference (D) = A ⊕ B
- Borrow (Bout) = A'B

## Logic Gates Used

- 1 × XOR Gate (74LS86)
- 1 × AND Gate (74LS08)
- 1 × NOT Gate (74LS04)

## Components Required

- Breadboard
- 74LS86 XOR Gate IC
- 74LS08 AND Gate IC
- 74LS04 NOT Gate IC
- DIP Switches (for inputs)
- LEDs (for outputs)
- 330 Ω Resistors
- Jumper Wires
- 5 V Power Supply

## Truth Table

| A | B | Difference (D) | Borrow (Bout) |
|---|---|----------------|---------------|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 0 |

## Circuit Operation

The XOR gate computes the Difference (D) by performing the exclusive OR operation on inputs A and B. Input A is inverted using a NOT gate, and the result is ANDed with input B to generate the Borrow (Bout) output.

## Applications

- Binary Subtractors
- Arithmetic Logic Units (ALUs)
- Digital Calculators
- Microprocessors
- Building Block for Full Subtractors

## Project Files

- `half_subtractor.pdsprj` – Proteus simulation
- `half_subtractor_breadboard.jpg` – Breadboard implementation
- `circuit_diagram.png` – Circuit schematic
- `README.md` – Project documentation

## Author

Nithish AS
