# 🔬 RTL / ASIC Engineering — Detailed Progress Tracker

> **Primary goal:** Become a strong RTL design engineer with practical verification and open-source ASIC-flow experience.
> **Working style:** Understand the specification, derive expected behaviour, write RTL, test it, investigate failures and record evidence.
> **Status policy:** Completed / In Progress / Next / Optional. No estimated percentages without a defined, countable checklist.

## 📍 Current Status Snapshot

| Track | Status | Evidence / note |
|---|---|---|
| Digital logic and combinational RTL | ✅ **Completed foundation** | Logic gates, MUX/DEMUX, encoders/decoders and hierarchical implementations are represented in the Verilog-Fundamentals repository. |
| Basic sequential RTL | ✅ **Foundation completed** | Basic D flip-flop and resettable D flip-flop examples and testbenches are present in the repository. |
| Verilator command workflow | 🔄 **In Progress** | Primary simulator/linter for this learning track; improve command fluency, warning diagnosis, builds and waveform traces. |
| SystemVerilog and sequential RTL | 🔄 **In Progress** | Start with a JK flip-flop and learn SystemVerilog syntax/semantics deliberately. The JK project is not marked complete until its source, testbench and run evidence are committed. |
| 6-to-64 decoder RTL-to-GDSII | 🧪 **Introductory flow executed** | Public project contains the design, testbench, layout image and GDS/ODB/DEF artifacts. This is not proof of timing closure, DRC/LVS cleanliness or signoff. |
| Python for verification | ➡️ **Next** | Learn the Python features needed to write clean test automation. |
| cocotb / reusable verification | ➡️ **Next, after Python basics** | Introduce only after the simulator workflow and required Python fundamentals are comfortable. |
| Standalone Yosys / OpenSTA workflows | ➡️ **Next, after RTL foundations** | Yosys was exercised as part of ORFS flow; learn its independent command flow and reports. Timing analysis needs explicit constraints and report interpretation. |

---

## ✅ Completed Foundations

### 1. Digital Logic and Combinational RTL

Implemented designs present in [Verilog-Fundamentals](https://github.com/CodeWithOmsai77/Verilog-Fundamentals):

- Logic gates: AND, NAND, NOR, NOT, OR, XOR and XNOR.
- Multiplexers: 2:1, 4:1, 8:1 and 16:1, including a hierarchical 16:1 design from 4:1 MUXes.
- Demultiplexers: 1:2, 1:4, 1:8 and 1:16, including hierarchical designs.
- Encoders: 4:2, 8:3, 8:3 built using 4:2 blocks, 16:4, priority 4:2 and priority encoder with valid output.
- Decoders: 2-to-4, hierarchical 4-to-16 using 2-to-4 blocks, and 6-to-64.

Use the source folders and each project testbench as the evidence for the individual implementation. Avoid claiming a project passed every possible test unless the test run supports that statement.

### 2. Basic Sequential RTL

- Basic D flip-flop.
- D flip-flop with asynchronous reset.
- Clock generation and basic testbench simulation concepts.
- Introductory setup/hold timing concepts.

### 3. Development Environment

- WSL2 with Ubuntu and Bash.
- Git/GitHub workflow and repository organization.
- Makefile-based workflow in the Verilog repository.
- Verilator installed and being used as the primary simulator/linter for the current learning track.
- Docker used to run the open-source RTL-to-GDSII flow.

### 4. Initial RTL-to-GDSII Flow Run

The [RTL-to-GDSII-Projects repository](https://github.com/CodeWithOmsai77/RTL-to-GDSII-Projects) contains a 6-to-64 decoder, SystemVerilog testbench, layout preview, and generated GDS/ODB/DEF artifacts from an OpenROAD Flow Scripts run using the Nangate45 platform.

**Correct interpretation:** a first end-to-end flow was executed and artifacts were generated. The run included a timing warning that the clock was not found, so do not claim timing closure or signoff. Independent STA, floorplan/placement/routing analysis and physical verification remain learning tasks.

---

## 🔄 In Progress — Current Priority

### Priority A — Verilator Workflow

Goal: use Verilator deliberately instead of memorising commands blindly.

- [ ] Check local tool version with `verilator --version`.
- [ ] Understand top-module selection and source-file ordering.
- [ ] Use `--lint-only -Wall` and resolve or explain relevant warnings.
- [ ] Use `--binary --timing` to build a runnable simulation where appropriate.
- [ ] Understand the generated build directory and executable before running it.
- [ ] Understand waveform trace options and inspect the resulting trace when enabled.
- [ ] Run the same project through a small, readable Makefile with clear targets.
- [ ] Record common errors, their causes and the fix in the project documentation.

### Priority B — SystemVerilog + Sequential RTL

Active exercise: **JK flip-flop**. Treat it as a learning target until its implementation is pushed and verified.

- [ ] Derive the JK truth table and next-state behaviour before writing RTL.
- [ ] Learn the SystemVerilog constructs needed for the module and testbench.
- [ ] Keep synthesizable design RTL separate from the testbench.
- [ ] Build a self-checking testbench covering hold, set, reset and toggle behaviour as required by the specification.
- [ ] Run Verilator lint, simulation and a waveform inspection.
- [ ] Review the design/testbench against the expected behaviour and document fixes.
- [ ] Commit source, testbench, simulation/build files and a short README.

Concept sequence to learn in context:

- `logic`, `bit`, and how four-state modelling differs from two-state types.
- `always_comb` and `always_ff`; when each construct is appropriate.
- Blocking (`=`) versus non-blocking (`<=`) assignments.
- Synchronous versus asynchronous reset and reset priority.
- Parameters / `localparam`, functions and tasks where they make the design clearer.
- Packed versus unpacked arrays and enumerated types when they become relevant.

---

## ➡️ Next — Follow This Order

### 1. SystemVerilog Fundamentals

- [ ] Explain key Verilog/SystemVerilog differences rather than translating syntax mechanically.
- [ ] Practice combinational and sequential examples with lint, simulation and expected-result checks.
- [ ] Use clear naming, small modules, and reusable self-checking testbench code.

### 2. Python for Verification

- [ ] Variables, types, expressions, conditionals and loops.
- [ ] Functions, lists, tuples, dictionaries, sets and modules.
- [ ] Exceptions, file handling and virtual environments.
- [ ] Read/write structured test inputs and report test results.
- [ ] Learn only the Python OOP concepts needed for the upcoming verification framework.

### 3. cocotb and Automated Verification

- [ ] Connect a Python test to a supported simulator and the selected RTL top.
- [ ] Drive inputs and sample outputs correctly with respect to clock timing.
- [ ] Add self-checking assertions, clear logs and meaningful failure messages.
- [ ] Add deterministic tests first; introduce seeded/random testing after the reference behaviour is clear.
- [ ] Run a repeatable regression using Make or the cocotb runner.

### 4. Standalone Synthesis and Timing Analysis

- [ ] Run a small design through a standalone Yosys script and understand the main commands.
- [ ] Read synthesis statistics and inspect a generated netlist.
- [ ] Learn SDC basics and the purpose of clock, input-delay and output-delay constraints.
- [ ] Learn OpenSTA reports: startpoint/endpoint, arrival/required time, slack and critical paths.
- [ ] Revisit the decoder flow warning; do not claim timing closure until constraints and reports support it.

### 5. Deeper OpenROAD / RTL-to-GDSII Practice

- [ ] Understand the major stages and generated outputs: synthesis, floorplan, placement, CTS, routing and GDS export.
- [ ] Inspect logs and reports after each stage instead of treating a final file as sufficient evidence.
- [ ] Learn what DRC, LVS, timing closure and signoff mean; distinguish them from producing GDS.
- [ ] Keep the platform, constraints, commands and known warnings documented for reproducibility.

---

## 🧱 Later RTL Project Backlog

Build in small steps. For each project, complete the specification, RTL, self-checking testbench, lint/simulation and documentation before moving on.

1. Half adder and full adder.
2. Subtractors, magnitude comparator, parity generator/checker and binary/Gray conversion.
3. Counters and shift registers.
4. Moore and Mealy FSMs, including a sequence detector or traffic-light controller.
5. ALU with a clear operation table and comprehensive tests.
6. UART transmitter/receiver and FIFO.
7. Simple CPU / RISC-V exploration after the core RTL and verification workflow is dependable.

These are planned milestones, not completed projects.

---

## 🧭 Optional / Later Tracks

These remain valid interests but are not part of the current primary execution queue:

- Embedded C, microcontrollers, STM32, RTOS and hardware debugging.
- PCB design, KiCad and analog simulation.
- Robotics, ROS 2, control systems, computer vision and PLC/industrial automation.
- Broader DSA / advanced software engineering beyond what directly supports the current RTL/verification work.

Keep these tracks optional so that the main ASIC/RTL path does not become fragmented.

---

## ✅ Project Completion Criteria

**RTL project:**

- [ ] Specification/truth table and intended behaviour written down.
- [ ] Synthesizable RTL committed.
- [ ] Testbench covers normal cases and important corner cases.
- [ ] Lint and simulation executed; failures resolved or documented.
- [ ] Expected outputs checked, and a waveform inspected where useful.
- [ ] README includes how to build/run and what was verified.

**RTL-to-GDSII project:**

- [ ] Reproducible design, constraints, platform and flow configuration.
- [ ] Simulation/lint evidence kept separate from synthesis/physical-flow results.
- [ ] Synthesis and timing reports reviewed; clocks and I/O constraints are correct for the target.
- [ ] Physical checks (such as DRC/LVS where applicable) are explicitly reported.
- [ ] Claims are limited to the evidence produced; generated GDS alone is not signoff.

## 🔗 Evidence Repositories

- [Verilog-Fundamentals](https://github.com/CodeWithOmsai77/Verilog-Fundamentals)
- [RTL-to-GDSII-Projects](https://github.com/CodeWithOmsai77/RTL-to-GDSII-Projects)
- [Project portfolio](PROJECTS.md)
- [Toolchain status](Software.md)

**Update rule:** update status when code, test output, a flow report or a clearly completed learning checkpoint provides evidence. Do not keep percentage estimates that no longer match actual work.