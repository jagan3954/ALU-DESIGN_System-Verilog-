# Experiment 1: Design and Simulation of an Arithmetic Logic Unit (ALU) using SystemVerilog

---

## Aim  
To design and simulate a **4-bit Arithmetic Logic Unit (ALU)** using **SystemVerilog HDL** and verify its functionality using **ModelSim 2020.1**.

---

## Apparatus Required  
- Computer with **Windows** OS  
- **ModelSim 2020.1** (or later) installed  
- SystemVerilog source code editor  

---

## Description about ALU  
An **Arithmetic Logic Unit (ALU)** is the core component of a processor that performs arithmetic and logical operations. It takes two input operands and a control signal (opcode) to determine the operation to be executed.  

Common ALU operations include:  
- **Arithmetic:** Addition, Subtraction, Multiplication, Division  
- **Logical:** AND, OR, XOR, NOT  
- **Shift Operations:** Logical Shift Left, Logical Shift Right, Rotate  

The ALU plays a crucial role in executing instructions in microprocessors and digital systems.

## Features
- Designed in **SystemVerilog** for clarity and modularity  
- Supports:
  - Arithmetic: Addition, Subtraction  
  - Logical: AND, OR, XOR, NOT  
  - Shift Operations: Left Shift, Right Shift  
- Parameterized design for scalability  
- Testbench for functional verification  
- Compatible with **ModelSim 2020.1**  
---

## Procedure  

1. **Open ModelSim 2020.1**  
   - Launch the ModelSim IDE from the Start Menu (Windows) or terminal (Linux).  

2. **Create a New Project**  
   - Go to `File → New → Project`.  
   - Enter a project name (e.g., `ALU_Project`).  
   - Set the project location.  
   - Click **OK**.  

3. **Add SystemVerilog Source Files**  
   - Create a new source file named `alu.sv` and type the ALU design code.  
   - Create a new source file named `alu_tb.sv` and type the testbench code.  

4. **Compile the Design and Testbench**  
   - Select both files (`alu.sv` and `alu_tb.sv`).  
   - Right-click → **Compile Selected**.  
   - Ensure there are no syntax errors.  

5. **Start Simulation**  
   - Go to `Simulate → Start Simulation`.  
   - In the **Library window**, expand **work**.  
   - Select the testbench module (`alu_tb`).  
   - Click **OK**.  

6. **Add Signals to Waveform**  
   - In the simulation window, select all signals (A, B, ALU_Sel, ALU_Out, CarryOut).  
   - Right-click → **Add to → Wave → Selected Signals**.  

7. **Run Simulation**  
   - In the simulation console, type:  
     ```
     run 100ns
     ```  
   - Or use the **Run button** to observe waveforms.  

8. **Analyze Waveforms**  
   - Verify the outputs of the ALU for different operations.  
   - Check that addition, subtraction, logical operations, and shifts are working as expected.  

9. **Save Results**  
   - Save the waveform (`.wlf` file) for documentation.  
   
---

## SystemVerilog Code  

### ALU Design (`alu.sv`)
```systemverilog
module alu #(parameter WIDTH = 4) (
    input  logic [WIDTH-1:0] A, B,
    input  logic [2:0] ALU_Sel,
    output logic [WIDTH-1:0] ALU_Out,
    output logic CarryOut
);

    

endmodule

---

## Testbench Code

## Simulation Output

- The simulation is carried out using ModelSim 2020.1.

- Waveforms will show the result of different ALU operations for the given inputs.

(Insert waveform screenshot here after running simulation in ModelSim)

## Result

The design and simulation of a 4-bit ALU using SystemVerilog HDL was successfully carried out in ModelSim 2020.1.
The ALU performed arithmetic, logical, and shift operations correctly as verified from the simulation outputs.
