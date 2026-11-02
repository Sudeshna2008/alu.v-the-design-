# alu.v(the design)
# 4-bit ALU in Verilog

A 4-bit Arithmetic Logic Unit with a self-checking testbench.

## Operations

| op  | Operation        |
|-----|------------------|
| 000 | ADD              |
| 001 | SUB              |
| 010 | AND              |
| 011 | OR               |
| 100 | XOR              |
| 101 | NOT A            |
| 110 | Shift A left     |
| 111 | Shift A right    |

Outputs: 4-bit `result`, `carry` (carry out, or borrow for SUB) and `zero` flag.

## Run the simulation

    iverilog -o alu_sim alu.v alu_tb.v
    vvp alu_sim
    gtkwave alu.vcd

## Waveform

![Waveform](images/waveform.png)

## Tools
Icarus Verilog and GTKWave
