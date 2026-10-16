# 🧭 RTL / ASIC Engineering — Progress Tracker

> **Primary goal:** Build demonstrable RTL design and verification skills, then deepen understanding of the ASIC flow.
> **Method:** Specification → architecture/truth table → RTL → self-checking testbench → lint → simulation → waveform/debug → synthesis/physical flow where applicable.

Use this page as the dashboard. The detailed checklist lives in [Shortlisted_ProgressTracker.md](Shortlisted_ProgressTracker.md); the project portfolio and tool inventory are maintained separately so the same status is not duplicated across long roadmaps.

---

## 📍 Current Status

| Area | Status | Current evidence / next action |
|---|---|---|
| Combinational RTL foundations | ✅ **Completed foundation** | Gates, MUX/DEMUX, encoder/decoder designs, including hierarchical designs, are in [Verilog-Fundamentals](https://github.com/CodeWithOmsai77/Verilog-Fundamentals). |
| Basic sequential RTL | ✅ **Foundation completed** | D flip-flop and resettable D flip-flop examples are present in the Verilog repository. Continue with additional sequential designs. |
| Verilator workflow | 🔄 **In Progress** | Verilator is the primary simulator/linter for the current track. Focus on command options, lint diagnostics, builds, timing and trace workflows. |
| SystemVerilog / JK flip-flop | 🔄 **In Progress** | Use a JK flip-flop as a focused exercise while learning SystemVerilog fundamentals. Do not mark the project complete until the RTL, testbench and run evidence are committed. |
| RTL-to-GDSII flow | 🧪 **Introductory flow run** | A 6-to-64 decoder flow produced GDS, ODB, DEF and a layout image using OpenROAD Flow Scripts and the Nangate45 platform. Timing closure/signoff has **not** been established. |
| Python verification / cocotb | ➡️ **Next** | First strengthen the Python fundamentals needed for verification, then add cocotb tests. |
| Standalone synthesis and timing analysis | ➡️ **Next, after RTL foundations** | Yosys was exercised as part of the ORFS flow; learn its independent command flow and reports. Timing analysis needs explicit constraints and report interpretation. |

---

## 🎯 Recommended Learning Order

1. **Finish the core Verilator workflow:** lint, compile/build, execute, diagnose warnings/errors, use Make targets and inspect traces.
2. **Learn SystemVerilog carefully:** syntax and semantics compared with Verilog; apply each concept in a small sequential RTL example.
3. **Learn the Python required for verification:** functions, data structures, modules, exceptions and environment/package basics.
4. **Start cocotb:** drive inputs, observe outputs, write self-checking checks and run repeatable tests.
5. **Deepen the ASIC flow:** standalone Yosys synthesis and reports, then OpenSTA timing constraints/reports and OpenROAD physical-design checks.

Keep the order deliberate. Do not add a tool to the “in use” list just because it is planned or appears indirectly in a flow.

---

## 📂 Tracker Documents

- [Detailed learning checklist](Shortlisted_ProgressTracker.md) — current status, sequence and completion criteria.
- [Project portfolio](PROJECTS.md) — implemented projects, active work and next RTL milestones.
- [Toolchain status](Software.md) — tools in active use, tools used through an integrated flow and tools still to learn.
- [Linux + Git command reference](🐧LINUX%20+%20GIT%20COMMAND%20LIST.md).
- [Linux course notes (PDF)](Linux_Course_Notes.pdf).

## 🧪 Evidence-First Progress

Statuses use **Completed / In Progress / Next / Optional** instead of guessed percentages. A source file existing is evidence of implementation, but a project is only called verified when its testbench has been run and its expected behaviour checked. An RTL-to-GDSII run is not described as signoff unless timing, physical checks and their reports support that claim.

## 🧭 Optional Tracks

Embedded systems, STM32, PCB design, robotics/ROS 2, computer vision and industrial automation remain useful interests, but they are **optional / later tracks**. They should not displace the current RTL/ASIC learning sequence.