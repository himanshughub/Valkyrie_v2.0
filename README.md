[![License](https://img.shields.io/badge/License-GPL--3.0-blue)](https://github.com/himanshughub/Valkyrie_v2.0/blob/main/LICENSE)

# Valkyrie_v2.0 - Vulnerability Assessment Tool and Attack for Provably-Secure Logic Locking Techniques

**Reimplementation of an IEEE Research Paper**

![Valkyrie Logo](https://github.com/himanshughub/Valkyrie_v2.0/blob/main/Images/Valkyrie_logo.png)

This project was reimplemented under the guidance of **Prof. Satwik Patnaik**, one of the authors of the original published research work on **Valkyrie: Vulnerability Assessment Tool and Attack for Provably-Secure Logic Locking Techniques**.  

During my Master's in Cybersecurity at the University of Delaware in **Spring 2024**, I enrolled in the **IoT and Embedded Systems Security** course. As part of this course project, I successfully reimplemented the top IEEE research conference journal paper authored by **Dr. Satwik Patnaik**, **Dr. Nimisha Limaye** & **Dr. Ozgur Sinanoglu**.

## Citation:
```bash
   •Author: Dr. Satwik Patnaik, Dr. Nimisha Limaye, & Dr. Ozgur Sinanoglu
   •DOI: 10.1109/TIFS.2022.3149147
   •Reference Link:https://ieeexplore.ieee.org/document/9703350/references#references
```
```bash
   •Research work enhanced & reimplemented by: Himanshu Kumar
   •LinkedIn:https://www.linkedin.com/in/himanshuk8/
   •Github:https://www.github.com/himanshughub
   •Email: himkumar@udel.edu
```
```bash
'This project validity can be verified by Dr. Satwik Patnaik, who can be reached at satwik@udel.edu'

'As responsible cybersecurity professionals, we cannot share the source code publicly, as it could be
 exploited by adversaries. If you have any questions, feel free to reach out to  himkumar@udel.edu,
 and I will be happy to assist you.'
```

## Description:
Valkyrie is an open-source tool developed using academic methodologies that assists defenders
in identifying vulnerabilities (critical signal wires) in provably secure logic locking (PSLL)
hardware chip designs. In addition to identifying vulnerabilities, it also demonstrates a proof
of concept on how to leverage these vulnerabilities to restore the original circuit design by
strategically inserting faults at critical signal points.

## Problem motivation:
→ IP piracy and IC overproduction are causing losses worth millions of US dollars to the United States
  and the global semiconductor market.
  
→ There is a lack of vulnerability testing tools for identifying security flaws in chip logic designs.

→ Due to the very limited availability and inaccuracy of existing vulnerability testing tools, millions
  of chips worldwide remain exposed to open vulnerabilities, making them susceptible to reverse engineering.

→ This includes the risk of top-secret military chip technology being exposed to intellectual property
  piracy.

## Why use this tool?
→ IP piracy and IC overproduction in the market are causing millions of dollars in losses to 
  a country's GDP and the company's revenue.
→ This project aims to help the United States and global semiconductor blockchain to secure their
  intellectual property from adversaries by preventing IP piracy and reverse engineering attacks.
→ This tool helps defenders identify vulnerable wires in their logic-locked circuits, allowing
  them to fix circuit design flaws before the IC chips go into manufacturing.
  
→ This results in protect chip intellectual property (IP) from being pirated and sold illegally.

    This tool will analyze the chip logic design and identify the following values:
    → Primary Inputs (PI)
    → Key Inputs (KI)
    → Primary Outputs (POP)
    → Critical Signal(s) (CS)

## Goal:
→ The goal is to identify the wire(s) in the chip logic circuit design where inserting a fault will
  recover the original or unmasked all variant of PSLL (provable secure login locking) chip design.

## Challenges:
- Identifying the critical signal wire from millions or billions of lines in the chip logic design
  is like finding a needle in a haystack.
- Analyzing and applying the structural properties of logic-locked circuits to identify critical
  signal wires for all provably secure logic-locked designs.
- Utilizing open-source libraries that are not compatible with the current version of the operating
  system.
- Recovering the original circuit without access to the oracle design.

## Features:
- Used open-source libraries for the implementation, eliminating the need for costly commercial tools

- Added argument "--parallel_process enable" to enable parallel processing feature for fast computation

- Increased the performance speed by 6x than standard computation by utilizing CPU parallel processing

- This tool work for all SFLT and DFLT known PSLL Provable logic locked circuits

- This tool has the ability to detect multiple critical signals, if present, in a PSLL circuit

- This tool can detect PI, KI, POP, and CS, even in synthesized locked benchmark files

- Improved the script UI, performance, error handling and added audit logs features
   
## Academic Open Source tools used in the project
- ABC tool (an academic synthesis tool) - https://github.com/berkeley-abc/abc
   
- Atlanta (an academic test pattern generation tool) - https://github.com/hsluoyz/Atalanta
   
- iverilog (an academic tool to simulate verilog file (.v) created by abc tool in graph) - https://github.com/steveicarus/iverilog?tab=readme-ov-file

## 📚 Library Dependencies
- colorama>=0.4.6
- alive_progress:>=3.1.5

## ⚙️ Commands to install libraries
Note: Run these commands in the Valkyrie files directory
 ```bash
    sudo make   #This will automatically setup script permissions
    sudo apt install python3 python3-pip -y
    pip3 install colorama alive-progress
    
 ```

## This project is implemented in two parts:
   **1. Defender View: Identifying vulnerabilities assuming access to the circuit oracle**
   
   **2. Attacker View: Exploiting vulnerabilities to recover the original circuit without access to the oracle**

# **Part 1: Defender View: Identifying vulnerabilities assuming access to the circuit oracle**

In the defender's shoes, it is assumed that you have access to the original chip logic design (Oracle) to compare
with the key-locked chip logic circuit in order to identify structural vulnerabilities and recover the original 
chip design.

## SFLT Demos:

**Demo 1: Without Parallel processing** 

![SFLT_without_parallel_process_demo_gif](https://github.com/himanshughub/Valkyrie_v2.0/blob/main/Images/SFLT/SFLT_without_parallel_process_demo.gif)

**Demo 2: With Parallel processing** 

![SFLT_with_parallel_process_demo_gif](https://github.com/himanshughub/Valkyrie_v2.0/blob/main/Images/SFLT/SFLT_with_parallel_processing_demo.gif)

## DFLT Demos:

**Demo 1: With Parallel processing**

![DFLT_with_parallel_process_demo_gif](https://github.com/himanshughub/Valkyrie_v2.0/blob/main/Images/DFLT/DFLT_with_parallel_processing_demo.gif)


# **Part 2: Attacker View: Exploiting vulnerabilities to recover the original circuit without access to the designer oracle**

In the attacker's shoes, it is assumed that you don't have access to the designere original chip logic design (Oracle) to 
compare with the key-locked chip logic circuit in order to identify structural vulnerabilities and recover the 
original chip design. The script creates it's own oracle from the locked design.

## Demos:

**Demo 1: Circuit recovery attack** 

![CR_Attack_demo_gif](https://github.com/himanshughub/Valkyrie_v2.0/blob/main/Images/CR_Attack/Circuit_Recovery_Attack_demo.gif)

