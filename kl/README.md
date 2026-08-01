# Full Adder using Verilog

## Overview

A Full Adder is a combinational logic circuit that adds three single-bit binary inputs:
- A
- B
- Cin (Carry Input)

It produces two outputs:
- Sum
- Cout (Carry Output)

Unlike a Half Adder, a Full Adder can add an incoming carry bit, making it suitable for multi-bit binary addition.

---

## Truth Table

| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 0 |
| 0 | 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 0 | 0 | 1 |
| 1 | 1 | 1 | 1 | 1 |

---

## Logic Equations

Sum = A ⊕ B ⊕ Cin

Cout = (A & B) | (B & Cin) | (A & Cin)

---

## Project Files

- **full_adder.v** – Verilog source code
- **full_adder_tb.v** – Testbench
- **simulation_output.txt** – Simulation results

---

## Simulation Tools

- ModelSim
- Vivado Simulator
- Icarus Verilog
- GTKWave

---

## Expected Output

```
A B Cin | Sum Cout
0 0 0   | 0   0
0 0 1   | 1   0
0 1 0   | 1   0
0 1 1   | 0   1
1 0 0   | 1   0
1 0 1   | 0   1
1 1 0   | 0   1
1 1 1   | 1   1
```

---

## Conclusion

This project demonstrates the implementation of a Full Adder using Verilog HDL and verifies its functionality through simulation.