# Day 1: Introduction to Verilog RTL Design & Synthesis


On the first day we have started our journey into digital design by learning Verilog, open-source simulation with **Icarus Verilog (iverilog)**, and the basics of logic synthesis using **Yosys**. This report documents my practical labs, key learnings, and hands-on experiences as I built a strong foundation in RTL design.



---
## Content Table
1. [Basic Overview](#1-basic-overview)
2. [Getting Started with iverilog](#2-getting-started-with-iverilog)
3. [My Lab Experience: Simulating a 2-to-1 Multiplexer](#3-my-lab-experience-simulating-a-2-to-1-multiplexer)
4. [My Verilog Code Analysis](#4-my-verilog-code-analysis)
5. [Introduction to Yosys & Gate Libraries](#5-introduction-to-yosys--gate-libraries)
6. [Understanding .lib Files and Gate Flavors](#6-understanding-lib-files-and-gate-flavors)
7. [My Synthesis Lab with Yosys](#7-my-synthesis-lab-with-yosys)
8. [Verification of My Synthesis](#8-verification-of-my-synthesis)
9. [Summary of My Learning](#9-summary-of-my-learning)

---
## 1. Basic Overview

### Simulator  
A **simulator** is a software tool used to test the functionality of digital circuits. It applies test inputs to the design and observes the outputs, allowing verification of correctness before hardware implementation.  

### Design  
The **design** refers to the Verilog code that describes the intended logic. It is the **behavioral representation** of the required specifications.  

### Testbench  
A **testbench** is a simulation environment created to apply different input patterns to the design and verify whether the outputs match the expected results.  

## 2. Getting Started with iverilog

**iverilog** is an open-source simulator for Verilog that I used throughout my lab. Here's the simulation flow I followed:

```
My Design (RTL) + My Testbench → iverilog → Executable → VCD file → GTKWave
```

I learned that both my design and testbench are provided as input to iverilog, and the simulator produces a `.vcd` file for waveform viewing in GTKWave.

---
