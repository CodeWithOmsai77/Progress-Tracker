# 🔬 RTL / ASIC Design — Project Portfolio

> This file records project status based on the current repositories. “Implemented in repo” means source files are present; “verified” additionally requires an appropriate test/run record.

## ✅ Completed / Implemented Foundations

### 1. Verilog Fundamentals — Combinational RTL

Repository: [CodeWithOmsai77/Verilog-Fundamentals](https://github.com/CodeWithOmsai77/Verilog-Fundamentals)

| Group | Implemented work | Evidence |
|---|---|---|
| Logic gates | AND, NAND, NOR, NOT, OR, XOR, XNOR | [Gate projects](https://github.com/CodeWithOmsai77/Verilog-Fundamentals/tree/main/Verilog_Basics/Gates) |
| Multiplexers | 2:1, 4:1, 8:1, 16:1 and hierarchical 16:1 using 4:1 blocks | [MUX projects](https://github.com/CodeWithOmsai77/Verilog-Fundamentals/tree/main/Verilog_Basics/Combinational/Multiplexers) |
| Demultiplexers | 1:2, 1:4, 1:8, 1:16 and hierarchical implementations | [DEMUX projects](https://github.com/CodeWithOmsai77/Verilog-Fundamentals/tree/main/Verilog_Basics/Combinational/Demultiplexer) |
| Encoders | 4:2, 8:3, 8:3 using 4:2 blocks, 16:4, priority 4:2 and valid-output priority encoder | [Encoder projects](https://github.com/CodeWithOmsai77/Verilog-Fundamentals/tree/main/RTL_Design/Combinational/Encoder) |
| Decoders | 2-to-4, hierarchical 4-to-16, 6-to-64 | [Decoder projects](https://github.com/CodeWithOmsai77/Verilog-Fundamentals/tree/main/RTL_Design/Combinational/Decoders) |

### 2. Sequential RTL Foundations

- Basic D flip-flop and testbench: [D flip-flop folder](https://github.com/CodeWithOmsai77/Verilog-Fundamentals/tree/main/RTL_Design/Sequential/Flip-Flops/D_Flip-Flop).
- D flip-flop with asynchronous reset and testbench: [Resettable DFF folder](https://github.com/CodeWithOmsai77/Verilog-Fundamentals/tree/main/RTL_Design/Sequential/Flip-Flops/D_FF_With_Reset).

### 3. Introductory RTL-to-GDSII Flow

Project: [6-to-64 Decoder](https://github.com/CodeWithOmsai77/RTL-to-GDSII-Projects/tree/main/01_Decoder_6to64)

The repository contains SystemVerilog RTL and testbench, a layout preview, and generated GDS, ODB and DEF artifacts from a run using OpenROAD Flow Scripts with the Nangate45 platform.

**Status:** introductory flow executed and output artifacts generated. The run reported a missing-clock timing warning. It is **not** being described as timing closure, DRC/LVS-clean or signoff.

---

## 🔄 In Progress

### 4. JK Flip-Flop — SystemVerilog / Verilator

**Purpose:** use one manageable sequential design to practise the Verilator workflow and SystemVerilog syntax.

Expected deliverables:

- [ ] Define the JK truth table and next-state behaviour.
- [ ] Synthesizable JK flip-flop RTL.
- [ ] Self-checking SystemVerilog testbench with hold, set, reset and toggle cases.
- [ ] Verilator lint and simulation run with test results recorded.
- [ ] Waveform trace review and short debugging notes.
- [ ] Clear README and reproducible build/run instructions.

**Status note:** this is the active learning target; it is not listed as a completed public project yet.

---

## ➡️ Next Projects — Suggested Order

1. Half adder and full adder.
2. Half/full subtractor, comparator and parity circuits.
3. Counters and shift registers.
4. Moore/Mealy FSM and sequence detector.
5. ALU with self-checking tests.
6. UART and FIFO.
7. Simple CPU / RISC-V only after the design and verification foundations are solid.

For each project, keep design RTL, testbench, simulation instructions, waveforms/reports where useful, and a short README. Use a project status only after the files and test evidence match it.

---

## 🔗 Repositories

- [Verilog-Fundamentals](https://github.com/CodeWithOmsai77/Verilog-Fundamentals)
- [RTL-to-GDSII-Projects](https://github.com/CodeWithOmsai77/RTL-to-GDSII-Projects)
- [Progress tracker README](README.md)
- [Detailed learning tracker](Shortlisted_ProgressTracker.md)