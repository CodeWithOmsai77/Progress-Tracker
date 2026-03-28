# 🔬 ENTC Engineering Roadmap — Progress Tracker
> **Name:** Omsai | **Branch:** ECE 2nd Year | **Goal:** VLSI / Chip Design
> **GitHub:** [CodeWithOmsai77](https://github.com/CodeWithOmsai77)

---

## ⚡ Current Status
- **Phase 1 overall:** 20% complete
- **Digital Electronics:** ✅ Strong
- **C Programming:** 🔄 Basic done
- **Python:** 🔄 Intermediate
- **Verilog:** ❌ Not started
- **Linux / WSL2:** ❌ Not started
- **Git (proper):** 🔄 Installed, not fully used

---

## 🗓️ URGENT — Do This First
- [ ] Enroll NPTEL CMOS VLSI Design → deadline **Mar 29** → [Link](https://onlinecourses.nptel.ac.in/noc26_cs50)
- [ ] Enroll NPTEL VLSI Physical Design → deadline **Apr 25**
- [x] Install WSL2 on D: drive → run `wsl --install` in PowerShell

---

## 📦 PHASE 1 — Foundation (0–12 Months)

### 1.1 Setup & Environment
- [x] Install WSL2 (store on D: drive)
- [x] Set WSL2 default install location to D: drive
- [x] Install VS Code WSL extension
- [x] Configure Git username and email globally
- [x] Create this progress-tracking repo on GitHub
- [ ] Learn 30 essential Linux terminal commands
- [ ] Understand file permissions (`chmod`, `chown`)
- [ ] Learn bash scripting basics (variables, loops, if-else)
- [ ] Learn piping and redirection (`|`, `>`, `>>`, `grep`)
- [ ] Understand process management (`ps`, `kill`, `top`)
- [ ] Linux file system hierarchy (/home, /etc, /bin, /usr)
- [ ] Understanding environment variables (PATH, HOME)
- [ ] Package management (apt, apt-get)
- [ ] Difference: user space vs kernel space
- [ ] Install ModelSim / Icarus Verilog (basic simulator)
- [ ] Install GTKWave (waveform viewer)
- [ ] Basic simulation flow understanding (compile → simulate → waveform)
- [ ] Use VS Code for Linux development (WSL integration)
- [ ] Setup extensions: C/C++, Python, Verilog HDL
- [ ] Learn debugging basics in VS Code

### 1.2 Digital Electronics (Already Strong — Just Fill Gaps)
- [x] Boolean algebra and logic gates
- [x] Combinational circuits
- [x] Karnaugh maps and minimization
- [x] Sequential circuits — flip-flops, counters, registers
- [x] Number systems — binary, hex, 2's complement
- [ ] IEEE 754 floating point representation
- [ ] FSM (Finite State Machine) basics
- [ ] Moore vs Mealy FSM — deep understanding
- [ ] FSM design from word problems (practice 10+)
- [x] Microcontroller basics (8051)
- [ ] Computer architecture — CPU datapath, pipelining
- [ ] Memory hierarchy — cache, RAM, buses
- [ ] FPGA basics — what LUTs and CLBs are

### 1.3 Verilog HDL — Most Important Skill
#### Beginner
- [ ] Module structure and syntax
- [ ] Ports — input, output, inout
- [ ] Wire vs reg
- [ ] `assign` statement
- [ ] `always` block
- [ ] Gate-level modeling
- [ ] Build: AND, OR, NOT, XOR gates in Verilog
- [ ] Build: 2:1 MUX in Verilog
- [ ] Build: 4:1 MUX in Verilog
- [ ] Build: Decoder (2:4) in Verilog
- [ ] Build: Half adder and full adder
- [ ] HDLBits — Getting Started section ✅ all problems
- [ ] HDLBits — Verilog Language section ✅ all problems

#### Intermediate
- [ ] FSMs in Verilog (Moore)
- [ ] FSMs in Verilog (Mealy)
- [ ] Parameters and `localparam`
- [ ] `generate` statement
- [ ] Tasks and functions
- [ ] Testbench writing basics
- [ ] Simulation with ModelSim (free)
- [ ] Build: 4-bit counter
- [ ] Build: Shift register (SISO, SIPO, PISO, PIPO)
- [ ] Build: UART transmitter in Verilog with testbench
- [ ] Build: ALU (4-bit) with testbench
- [ ] HDLBits — Circuits section ✅ 70%+ problems
- [ ] nandland.com — complete beginner Verilog track

#### Advanced
- [ ] Synthesis-aware Verilog coding
- [ ] Avoiding latches in RTL
- [ ] Proper reset strategies (sync vs async)
- [ ] Clock domain crossing (CDC) basics
- [ ] HDLBits — complete 90%+ problems
- [ ] Build: 8-bit CPU (ALU + registers + control unit)

### 1.4 C Programming
- [x] Variables, data types
- [x] Loops (for, while, do-while)
- [x] Functions
- [x] Pointers basics
- [ ] Bitwise AND `&`
- [ ] Bitwise OR `|`
- [ ] Bitwise XOR `^`
- [ ] Bitwise NOT `~`
- [ ] Left shift `<<` and right shift `>>`
- [ ] Bit masking techniques
- [ ] Bit flags and setting/clearing bits
- [ ] Pointer arithmetic (deep)
- [ ] Arrays and strings
- [ ] Structs and unions
- [ ] Dynamic memory — `malloc`, `calloc`, `free`
- [ ] File I/O in C
- [ ] Build: Logic gate simulator in C (push to GitHub)
- [ ] Build: Bitwise calculator in C

### 1.5 C++ Basics
- [ ] Classes and objects
- [ ] Constructors and destructors
- [ ] Encapsulation
- [ ] Inheritance
- [ ] Polymorphism (function overloading, overriding)
- [ ] Virtual functions
- [ ] Templates basics
- [ ] STL — vectors, maps, sets
- [ ] OOP design: write a class hierarchy from scratch

### 1.6 Python (Already Intermediate — Just Fill Gaps)
- [x] Variables and data types
- [x] Loops and conditions
- [x] Functions
- [x] Lists, tuples, dictionaries
- [x] File I/O
- [x] OOP and inheritance
- [ ] `subprocess` module (run shell commands from Python)
- [ ] `os` and `pathlib` modules
- [ ] `re` (regex) basics
- [ ] Write a Python script to automate a file task
- [ ] Write a Python script to parse a log file

### 1.7 TCL Scripting (Used in ALL EDA tools)
- [ ] TCL syntax basics — variables, lists, strings
- [ ] Control flow — if, for, foreach, while
- [ ] Procedures (functions)
- [ ] File operations in TCL
- [ ] String manipulation
- [ ] Write a basic TCL script
- [ ] Understand how TCL is used in Cadence / Synopsys tools

### 1.8 Git (Properly)
- [ ] `git init`, `git add`, `git commit`
- [ ] `git push`, `git pull`, `git clone`
- [ ] Branching — `git branch`, `git checkout`, `git merge`
- [ ] `.gitignore` file setup
- [ ] Pull requests workflow
- [ ] Commit daily habit — even small changes
- [ ] GitHub profile has pinned repos
- [ ] Understand staging area vs working directory
- [ ] Write meaningful commit messages
- [ ] Resolve merge conflicts
- [ ] Use GitHub issues/projects (basic)

### 1.9 Mathematics
- [ ] Boolean algebra deep (Karnaugh maps, SOP, POS)
- [ ] Linear algebra basics (matrices, vectors)
- [ ] Probability basics (for verification coverage)
- [ ] Discrete math — sets, logic, graph theory basics
- [ ] Control theory intro — transfer functions, stability

### 1.10 Phase 1 Projects (Must Build & Push to GitHub)
- [ ] Logic gate simulator in C
- [ ] Bitwise calculator in C
- [ ] UART transmitter + receiver in Verilog (with testbench)
- [ ] 4-bit ALU in Verilog (with testbench)
- [ ] 8-bit CPU in Verilog (ALU + control unit + registers)
- [ ] Python log file parser / automation script
- [ ] WSL2 setup documented in repo README

---

## 🔬 PHASE 2 — VLSI Core (12–36 Months)
- [ ] Convert your Verilog ALU to SystemVerilog
- [ ] Add testbench using SystemVerilog
      
#### FPGA Basics (Parallel)
- [ ] Install Xilinx Vivado (or study interface if low PC power)
- [ ] Understand RTL → FPGA flow
- [ ] Synthesize simple design (MUX / ALU)
      
#### RISC-V Intro
- [ ] What is ISA
- [ ] RV32I basic instructions (ADD, SUB, LOAD, STORE)
      
#### Essential Sotwares
- [ ] ModelSim / QuestaSim (simulation)
- [ ] Quartus (optional)
      
### 2.1 RTL Design
- [ ] SystemVerilog data types
- [ ] Interfaces and packages
- [ ] Assertions (SVA basics)
- [ ] RTL coding guidelines (synthesis-friendly)
- [ ] Clock gating for low power
- [ ] Clock domain crossing (CDC) — synchronizers, FIFOs
- [ ] FPGA prototyping — map RTL to Xilinx Vivado
- [ ] RISC-V ISA — RV32I base understanding
- [ ] Build: RISC-V 5-stage pipelined CPU in Verilog
- [ ] Data types — logic, bit, int
- [ ] always_ff vs always_comb
- [ ] Interfaces basics
- [ ] Packages basics
- [ ] Assertions intro (SVA basics)

### 2.2 Functional Verification (UVM)
- [ ] SystemVerilog OOP — classes, inheritance
- [ ] Interfaces and clocking blocks
- [ ] Constrained random — `rand`, `randc`, `constraint`
- [ ] Functional coverage — covergroups, coverpoints
- [ ] UVM testbench architecture overview
- [ ] UVM Driver, Monitor, Scoreboard, Agent
- [ ] UVM Environment and test
- [ ] Build: UVM testbench for your ALU
- [ ] Difference: directed vs constrained random testing
- [ ] Scoreboard design concept
- [ ] Coverage-driven verification mindset

### 2.3 Synthesis & STA
- [ ] Logic synthesis concepts — RTL to gate netlist
- [ ] Setup time and hold time
- [ ] Critical path analysis
- [ ] Slack (positive vs negative)
- [ ] SDC constraints — `create_clock`, `set_input_delay`
- [ ] Synopsys Design Compiler basics
- [ ] Read and understand a timing report
- [ ] Setup vs hold timing deeply
- [ ] Clock skew and latency
- [ ] Critical path identification

### 2.4 Physical Design
- [ ] Floorplanning concepts
- [ ] Placement — standard cells
- [ ] Clock Tree Synthesis (CTS)
- [ ] Routing — global and detailed
- [ ] DRC and LVS sign-off
- [ ] GDSII format understanding
- [ ] OpenROAD (free tool) — basic flow
- [ ] Basic CMOS layout understanding
- [ ] Standard cell concept
- [ ] Power grid basics

### 2.5 DFT — Design for Test
- [ ] Scan chain insertion concept
- [ ] ATPG — automatic test pattern generation
- [ ] BIST — Built-In Self Test
- [ ] JTAG / Boundary Scan (IEEE 1149.1)
- [ ] Stuck-at fault model
- [ ] Scan shift vs capture mode
- [ ] Why testing is required in chips

### 2.6 RISC-V
- [ ] RV32I base ISA specification
- [ ] RV64I overview
- [ ] 5-stage pipeline design (IF, ID, EX, MEM, WB)
- [ ] Hazard detection (data, control, structural)
- [ ] Spike simulator setup
- [ ] RISC-V GNU toolchain setup
- [ ] Read PicoRV32 source code on GitHub
- [ ] Build: 5-stage pipelined RISC-V CPU
- [ ] Instruction formats (R, I, S, B, U, J types)
- [ ] Pipeline hazards (data, control, structural)
### 2.7 Phase 2 Projects
- [ ] 5-stage pipelined RISC-V CPU in Verilog
- [ ] UVM testbench for AXI4 bus controller
- [ ] Synthesis + STA run on your CPU (free tools)
- [ ] FPGA implementation on Xilinx Arty board

---

## 🔧 PHASE 3 — Electronics & Embedded (18–30 Months)

### 3.1 PCB Design
- [ ] Schematic capture basics in KiCad
- [ ] Reading datasheets (practice 1/week)
- [ ] PCB layout basics — layers, traces, vias
- [ ] Design rules check (DRC)
- [ ] High-speed PCB — impedance matching basics
- [ ] Signal integrity concepts
- [ ] Power integrity — decoupling capacitors
- [ ] Build: Design a PCB with STM32 + sensors in KiCad
- [ ] Grounding techniques (VERY IMPORTANT)
- [ ] Decoupling capacitor placement rules
- [ ] EMI basics

### 3.2 Analog Electronics
- [ ] Op-amp circuits — inverting, non-inverting amplifier
- [ ] Filters — low pass, high pass, band pass
- [ ] Comparators
- [ ] ADC / DAC concepts
- [ ] DC-DC converters — buck converter basics
- [ ] LTSpice installation and simulation
- [ ] Simulate a buck converter in LTSpice
- [ ] Oscillator circuits basics
- [ ] Frequency response (Bode plot basics)
- [ ] Stability basics

### 3.3 Embedded Systems
- [ ] Arduino Uno — GPIO, ADC, UART, SPI, I2C, timers
- [ ] STM32 — bare-metal C, HAL drivers
- [ ] DMA concepts
- [ ] FreeRTOS — tasks, queues, semaphores
- [ ] Bootloader basics
- [ ] Build: Custom RTOS task scheduler on STM32
- [ ] Build: SPI/I2C controller in Verilog (combo project)
- [ ] Interrupt handling (deep)
- [ ] Register-level programming
- [ ] Memory-mapped I/O

### 3.4 Hardware Debugging
- [ ] Oscilloscope usage basics
- [ ] Logic analyzer usage
- [ ] JTAG debugger (ST-Link)
- [ ] Protocol decode — SPI, I2C, UART
- [ ] STM32CubeIDE
- [ ] Proteus (optional simulation)
---

## 🤖 PHASE 4 — Robotics & Automation (24–36 Months)

### 4.1 Control Systems
- [ ] PID controller theory
- [ ] Implement PID on STM32 for motor control
- [ ] Transfer functions and Bode plots
- [ ] Kalman filter basics
- [ ] MATLAB / Simulink basics
- [ ] Stability criteria (basic idea)
- [ ] Real-world tuning of PID

### 4.2 ROS2
- [ ] ROS2 architecture — nodes, topics, services
- [ ] Sensor integration (LiDAR, IMU, cameras)
- [ ] Gazebo simulator setup
- [ ] URDF robot modeling
- [ ] Nav2 navigation stack
- [ ] Build: Autonomous robot with obstacle avoidance
- [ ] ROS2 communication internals (DDS concept)

### 4.3 Computer Vision & AI
- [ ] OpenCV — image processing, edge detection
- [ ] Object detection — YOLO basics
- [ ] Camera calibration
- [ ] SLAM introduction — GMapping
- [ ] Image coordinate systems
- [ ] Basic transformations (rotation, scaling)

### 4.4 Industrial Automation
- [ ] PLC basics — ladder logic
- [ ] SCADA system overview
- [ ] Modbus protocol
- [ ] Ladder logic real examples

---

## 💻 PHASE 5 — Software Engineering (Ongoing)

### 5.1 Data Structures & Algorithms
- [ ] Arrays and strings (C++)
- [ ] Linked lists
- [ ] Stacks and queues
- [ ] Trees (BST, AVL basics)
- [ ] Hash maps
- [ ] Sorting — QuickSort, MergeSort
- [ ] Binary search
- [ ] BFS and DFS
- [ ] Dynamic programming (basic)
- [ ] Bit manipulation problems (LeetCode 10+)
- [ ] Graph algorithms — Dijkstra
- [ ] Time complexity (Big-O analysis)
- [ ] Space complexity

### 5.2 OOP & Design Patterns
- [ ] SOLID principles
- [ ] Factory pattern
- [ ] Observer pattern
- [ ] Singleton pattern
- [ ] UML class diagrams
- [ ] Memory management in C++
- [ ] Smart pointers

### 5.3 Build Systems & DevOps
- [ ] Makefile for C/C++ project
- [ ] CMake basics
- [ ] Git branching strategy (feature branches)
- [ ] Docker basics
- [ ] CI/CD concepts
- [ ] Bash scripting for automation
- [ ] Linux shell scripting projects
- [ ] Writing automation pipelines

---

## 🚀 PHASE 6 — Emerging Tech (36+ Months)

### 6.1 AI Hardware Design
- [ ] How CNNs map to hardware (MACs, systolic arrays)
- [ ] NPU/TPU architecture overview
- [ ] Google TPU paper (read)
- [ ] Apple Neural Engine overview
- [ ] NVDLA open-source accelerator — read the docs
- [ ] Chipyard framework intro
- [ ] MAC operation (multiply-accumulate concept)
- [ ] Dataflow in neural networks

### 6.2 Chiplet Architecture
- [ ] UCIe die-to-die interconnect standard
- [ ] AMD Ryzen chiplet architecture (read)
- [ ] Apple M-series chiplet design (read)
- [ ] 2.5D/3D packaging — CoWoS basics
- [ ] Model optimization (quantization basics)

### 6.3 Edge AI
- [ ] TensorFlow Lite on microcontroller
- [ ] ONNX Runtime basics
- [ ] NVIDIA Jetson setup
- [ ] TinyML — MCUNet paper (read)

---

## 📜 Certifications Tracker
- [ ] NPTEL CMOS VLSI Design — enroll by **Mar 29** 🔴
- [ ] NPTEL VLSI Physical Design — enroll by **Apr 25**
- [ ] RISC-V free course → [riscv.org](https://riscv.org)
- [ ] Cisco NetAcad networking basics → [netacad.com](https://netacad.com)
- [ ] Google Cloud Skills Boost → [cloudskillsboost.google](https://cloudskillsboost.google)
- [ ] AWS Skill Builder → [skillbuilder.aws](https://skillbuilder.aws)

---

## 📚 Resources Reference
| Topic | Resource |
|---|---|
| Verilog | [nandland.com](https://nandland.com/learn-verilog) |
| Verilog Practice | [HDLBits](https://hdlbits.01xz.net) |
| Verilog Reference | [chipverify.com](https://chipverify.com/tutorials/verilog) |
| C (Hindi) | [Jenny's Lectures](https://youtube.com/@JennyslecturesCandDSA) |
| Python | [CodeWithHarry](https://youtube.com/@CodeWithHarry) |
| Linux | [YouTube video](https://youtube.com/watch?v=vxTW22y8zV8) |
| NPTEL | [nptel.ac.in](https://nptel.ac.in) |

---

## 🏆 Golden Rules
1. Push something to GitHub **every single day**
2. VLSI is your superpower — go deepest here
3. Build **real projects**, not just tutorials
4. Read **1 datasheet per week**
5. Your software skills are a HUGE advantage in VLSI — use them
6. Follow RISC-V and AI chip trends
7. Network on LinkedIn — follow VLSI engineers, apply to internships

---

*Last updated: March 2026 | Phase 1 in progress 🔥*
