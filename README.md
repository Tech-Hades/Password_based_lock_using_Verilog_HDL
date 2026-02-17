# Password-based-lock-system-using-Verilog-HDL
Password based lock system using Verilog HDL

A simple **password-based digital lock system** implemented using **Verilog HDL**.  
The lock opens only when the correct password sequence is entered.

## Features
- 4-digit password authentication
- Sequential, clock-based design
- `unlock` signal for correct password
- `alarm` signal for wrong password
- Fully verified using simulation and waveform analysis

## Password Details
- Password Length: 4 digits  
- Each Digit: 4-bit input  
- Stored Password: **1 – 2 – 3 – 4**

## ⚙️ How It Works
1. Apply `reset` to initialize the system  
2. Enter each digit on `key_in`  
3. Pulse `enter` for every digit  
4. After 4 digits:
   - Correct password → `unlock = 1`
   - Wrong password → `alarm = 1`

## Simulation
- Simulator: **Icarus Verilog**
- Platform: **EDA Playground**
- Waveform Viewer: **EPWave**

## Output Waveform
The waveform below shows successful unlocking after entering the correct password sequence (1-2-3-4):

![Output Waveform](output_waveform.png)

## Files
- `design.sv` – Password lock module  
- `testbench.sv` – Testbench for simulation  

## Applications
- Digital door locks  
- Embedded security systems  
- FPGA-based authentication projects  

