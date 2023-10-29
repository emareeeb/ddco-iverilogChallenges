# 🚀 Digital Design and Computer Organization Laboratory - Getting Started 📚

Welcome to the Digital Design and Computer Organization Laboratory. This Read Me file provides a structured overview of the content and clear instructions for a seamless learning experience.

## Table of Contents:

### Section 1: 📖 Introduction
1.1 Verilog Language Basics
   - 📘 Identifiers, Keywords, Comments
   - 📝 Whitespaces, Case Sensitivity
   - 🧩 Verilog Modules and Ports
   - 🚧 Rules of Connecting Ports
   - 📊 Vector Data
   - 📡 Verilog $monitor
   - 🛠️ Gate Level Modeling

1.2 Installation of Icarus Verilog
   - 📥 Download and Install Icarus Verilog for Windows
   - ⚙️ Compilation and Execution

1.3 Installation and Viewing the Waveform using GTKWave
   - 🌐 Setting up GTKWave
   - ✍️ Modifying Verilog Files for Simulation
   - 🏁 Compiling and Running the Program
   - 📈 Viewing the Waveform

## Section 1: 📖 Introduction
### 1.1 Verilog Language Basics

#### Identifiers, Keywords, and Comments
- Verilog uses identifiers to name objects (e.g., modules, inputs, variables).
- Identifiers must start with an alphabetic character or an underscore and can contain alphanumeric characters, underscores, or the dollar sign.
- Keywords are reserved words in Verilog, such as module and assign.
- Proper use of single-line (//) and multi-line (/* */) comments is essential for code readability.

#### Whitespaces and Case Sensitivity
- Whitespace characters like space, tab, and newline separate elements in Verilog code.
- Proper use of whitespaces improves code readability.
- Verilog is case-sensitive; keywords are in lowercase, and identifiers are case-sensitive.

#### Verilog Modules and Ports
- Verilog uses modules to represent hierarchical building blocks.
- Modules have input, output, or inout ports that connect them.
- Module definition syntax includes the module name, input/output ports, and behavior description.

#### Rules of Connecting Ports
- Define input ports as nets internally and connect them to reg or net variables externally.
- Output ports can be nets or regs internally, but they must connect to net variables externally.
- Inout ports must always be of type net, both internally and externally.

#### Vector Data
- Verilog allows the use of vectors to represent multi-bit buses.
- Vectors are declared using syntax like `reg [7:0] eightbitbus`.
- The bit range syntax can be from most significant bit (MSB) to least significant bit (LSB) or vice versa.

#### Verilog $monitor
- The $monitor system task is used for generating input and output for verification.
- Syntax: `$monitor("format_string", parameter1, parameter2, ...);`
- Format strings specify how parameters are displayed (e.g., %d for decimal, %4b for binary).

### 1.2 Installation of Icarus Verilog

#### Download and Install Icarus Verilog for Windows
- Download the Icarus Verilog setup file from [http://bleyer.org/icarus/](http://bleyer.org/icarus/).
- Run the setup.exe file to install Icarus Verilog on Windows.

#### Compilation and Execution
- Compile a Verilog file using `iverilog -o filename filename.v`.
- Execute the compiled program with `vvp filename`.
- Alternatively, use `iverilog filename.v` to generate the `a.out` executable file and run it with `./a.out`.

### 1.3 Installation and Viewing the Waveform using GTKWave

#### Setting up GTKWave
- Add the GTKWave path to the system environment variables (e.g., C:\IcarusVerilog\gtkwave\bin).

#### Modifying Verilog Files for Simulation
- Add the following lines to the stimulus file to enable waveform dumping:
  ```verilog
  $dumpfile("test.vcd");
  $dumpvars(0, stimulus);
  ```

#### Compiling and Running the Program
- Compile the Verilog files with `iverilog -o mydesign comparator.v stimulus.v`.
- Run the simulation with `vvp mydesign`.
- Open GTKWave with `gtkwave test.vcd` to view the waveform.

## Basic Gates Implementation
- The document provides an example of implementing a NOT gate using three different modeling approaches: gate level, data flow, and behavioral.

## Verilog TUTORIAL - Running your first code
- A step-by-step guide on running a simple Verilog program that displays "Hello World."

### Instructions
1. Create a new Verilog file in the directory specified.
2. Edit the Verilog code as provided in the document.
3. Compile and execute the Verilog program using the mentioned commands.
4. Observe the output and waveform using GTKWave.



This document serves as a guide for understanding Verilog basics, installing the Icarus Verilog compiler, and viewing waveforms for digital design and computer organization experiments.

Enjoy your Verilog learning journey! 🌟🔌📊📈
//linking pending

//linking req
