# Valkyrie_v2.0 - Vulnerability Assessment Tool and Attack for Provably-Secure Logic Locking Techniques

**Reimplementation of a published IEEE Research Paper**

![Valkyrie Logo](https://github.com/himanshughub/Valkyrie_v2.0/blob/main/Images/Valkyrie_logo.png)

This project was reimplemented under the guidance of **Prof. Satwik Patnaik**, one of the authors of the original published research work on **Valkyrie: Vulnerability Assessment Tool and Attack for Provably-Secure Logic Locking Techniques**.  

During my Master's in Cybersecurity at the University of Delaware in **Spring 2024**, I enrolled in the **IoT and Embedded Systems Security** course. As part of this course project, I successfully reimplemented the research work published in an IEEE journal paper authored by **Dr. Satwik Patnaik** and **Dr. Nimisha Limaye**.

## Citation:
```bash
   •Author: Dr. Satwik Patnaik & Dr. Nimisha Limaye
   •DOI: 10.1109/TIFS.2022.3149147
   •Reference Link:https://ieeexplore.ieee.org/document/9703350/references#references
```
```bash
   •Research work enhanced & reimplemented by: Himanshu Kumar
   •LinkedIn:https://www.linkedin.com/in/himanshuk8/
   •Github:https://www.github.com/himanshughub
   •email: himkumar@udel.edu
```

## Description:
Valkyrie is an open-source tool developed using academic methodologies that assists defenders
in identifying vulnerabilities (critical signal wires) in provably secure logic locking (PSLL)
hardware chip designs. In addition to identifying vulnerabilities, it also demonstrates a proof
of concept on how to leverage these vulnerabilities to restore the original circuit design by
strategically inserting faults at critical signal points.

## Why use this tool?
→ IP piracy and IC overproduction in the market are causing millions of dollars in losses to 
  a country's GDP and the company's revenue.
→ This tool helps defenders identify vulnerable wires in their logic-locked circuits, allowing
  them to fix circuit design flaws before the IC chips go into manufacturing.
→ This results in protect chip intellectual property (IP) from being pirated and sold illegally.

    This tool, part of the Valkyrie suite, assists in finding:
    → Primary Inputs (PI)
    → Key Inputs (KI)
    → Primary Outputs (POP)
    → Critical Signal(s) (CS)

## Features:
   • This tool work for both SFLT and DFLT PSLL logic locked circuits
   
   • This tool has the ability to detect multiple critical signals, if present, in a PSLL circuit
   
   • This tool can detect PI, KI, POP, and CS, even in synthesized locked benchmark files

## Academic Open Source tools used in the project
   • ABC tool (an academic synthesis tool) - https://github.com/berkeley-abc/abc
   
   • Atlanta (an academic test pattern generation tool) - https://github.com/hsluoyz/Atalanta
   
   • iverilog (an academic tool to simulate verilog file (.v) created by abc tool in graph) - https://github.com/steveicarus/iverilog?tab=readme-ov-file

## 📚 Library Versions Used in the Project
- colorama: 0.4.6
- alive_progress: 3.1.5

## ⚙️ Commands to install libraries
Note: Run these commands in the Valkyrie files directory
 ```bash
    sudo make   #This will automatically setup script permissions
    sudo apt install python3 python3-pip -y
    pip3 install colorama alive-progress
    
 ```


# Demos:

** Demo 1: ** 


** Demo 2: ** 


** Demo 3: ** 


** Demo 4: ** 


