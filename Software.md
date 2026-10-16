# 🛠️ RTL / ASIC Learning — Toolchain Status

> This list separates tools actually used from tools included inside a larger flow and tools planned for later. Installing or invoking a tool once does not imply proficiency.

## ✅ Currently Available / Used in the Workflow

| Tool | Current status | Use / note |
|---|---|---|
| WSL2 + Ubuntu | **In use** | Main Linux environment for commands, development and builds. |
| Bash / core Linux utilities | **In use** | Navigate the workspace, inspect files, run builds and diagnose tool output. |
| Git + GitHub | **In use** | Version control, project history, repository and README maintenance. |
| Make / Makefile | **In use** | Repeatable project commands; the Verilog-Fundamentals repo has Makefile automation. |
| Verilator | **Primary simulator/linter** | Current learning focus: lint warnings, top-module selection, binary builds, timing support and waveform tracing. Check the local version with `verilator --version`. |
| GTKWave | **Available / used** | Waveform inspection for simulation debugging where a compatible trace is generated. |
| Icarus Verilog | **Available / used in earlier exercises** | Retained as a secondary/historical simulator; Verilator is the primary simulator for the current project track. |
| Python 3 | **Available / learning for verification** | Strengthen Python fundamentals before adopting cocotb for test automation. |
| Docker | **In use** | Runs the OpenROAD Flow Scripts environment without installing the entire flow natively. |
| C/C++ build toolchain | **Available** | g++ and build tooling used by compiled simulation/build workflows. |

## 🧪 Used Through an Integrated RTL-to-GDSII Flow

| Tool / platform | Evidence and accurate status |
|---|---|
| OpenROAD Flow Scripts (ORFS) | A flow was run in Docker for the 6-to-64 decoder project. Flow use is demonstrated; in-depth stage/report interpretation remains to be learned. |
| Yosys | Used as the synthesis stage within the ORFS flow. **Standalone Yosys scripting and independent report/netlist analysis remain next steps.** |
| OpenROAD | Used through ORFS for physical-design stages and generation of output artifacts. This does not itself prove timing closure or signoff. |
| Nangate45 | Platform/standard-cell library selected for the introductory flow. It is a learning platform, not a claim about a production process node. |
| OpenSTA / timing stage | Timing checks appeared in the flow output, including a warning that clock `*` was not found. Learn proper SDC constraints and standalone timing reports before making timing-closure claims. |

Flow evidence: [RTL-to-GDSII Decoder project](https://github.com/CodeWithOmsai77/RTL-to-GDSII-Projects/tree/main/01_Decoder_6to64).

**Important:** generated GDS/ODB/DEF files demonstrate a flow run; they do not alone prove DRC/LVS cleanliness, valid timing constraints, timing closure or fabrication signoff.

---

## 🔄 Current Tool-Learning Priority

1. **Verilator CLI and workflow:** version, top module, `--lint-only -Wall`, `--binary --timing`, build output, executable launch, trace options and useful error diagnosis.
2. **SystemVerilog:** learn syntax and semantics with small RTL projects and self-checking testbenches.
3. **Python for verification:** functions, collections, exceptions, modules, file handling and virtual environments.
4. **cocotb:** Python-based simulation tests, clocking, assertions, logs and reproducible regression.
5. **Standalone Yosys:** script a small design, synthesize it, read statistics and inspect the mapped/generic netlist.
6. **OpenSTA and OpenROAD deeper use:** SDC constraints, timing reports, critical paths, flow logs and physical-check reports.

## ➡️ Next / Not Yet Confirmed as In Use

| Tool | Planned purpose | Status |
|---|---|---|
| cocotb | Python-driven RTL testbenches and regression | **Next**, after Python fundamentals and simulator workflow. |
| Verible | SystemVerilog lint/format workflow | **Later**; installation and current use have not been confirmed. |
| SymbiYosys | Formal verification experiments | **Later**, after RTL and assertion fundamentals. |
| OpenLane / SKY130 | Alternative educational RTL-to-GDSII platform/PDK | **Later**; not the current active flow. |
| Surfer | Alternative waveform viewer | Optional; use only if it adds value beyond current waveform workflow. |

## ⏸️ Optional / Not Needed for the Current Stage

- Paid simulators such as Questa/ModelSim or VCS: useful in industry contexts, but not required for the current open-source learning path.
- Embedded/robotics/PCB toolchains: keep these in the optional track until the core RTL/verification sequence is stronger.

## 🔗 Related Notes

- [Main progress dashboard](README.md)
- [Detailed learning checklist](Shortlisted_ProgressTracker.md)
- [Project portfolio](PROJECTS.md)