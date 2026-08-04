# Full Subtractor using Verilog

## Overview

A Full Subtractor is a combinational logic circuit used to subtract three binary bits:

- A (Minuend)
- B (Subtrahend)
- Bin (Borrow Input)

It produces two outputs:

- Difference (Diff)
- Borrow Output (Bout)

This project implements a Full Subtractor using Verilog HDL and verifies its functionality using a testbench.

---

## Truth Table

| A | B | Bin | Diff | Bout |
|---|---|-----|------|------|
|0|0|0|0|0|
|0|0|1|1|1|
|0|1|0|1|1|
|0|1|1|0|1|
|1|0|0|1|0|
|1|0|1|0|0|
|1|1|0|0|0|
|1|1|1|1|1|

---

## Logic Equations

Difference:

Diff = A ⊕ B ⊕ Bin

Borrow:

Bout = (~A & B) | (~A & Bin) | (B & Bin)

---

## Files

- `full_subtractor.v` → Verilog source code
- `full_subtractor_tb.v` → Testbench
- `simulation_results.png` → Simulation waveform
- `README.md` → Documentation

---

## Tools Used

- Verilog HDL
- ModelSim / Vivado / Icarus Verilog
- GTKWave (optional)

---

## Simulation Output

(Add your waveform screenshot here)

![Simulation](simulation_results.png)

---

## Author

**Lathasree M**

B.Tech Electronics and Communication Engineering