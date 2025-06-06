# 🔐 128-bit Cryptographic Processor using AES  
**A Verilog HDL-based hardware implementation of AES-128 encryption core**

---

## 🧠 Overview

This project implements a **128-bit AES cryptographic processor** using **Verilog HDL**, aimed at demonstrating how symmetric encryption can be translated into hardware logic. The design simulates AES encryption through **ModelSim-Altera** and is suitable for FPGA.

AES (Advanced Encryption Standard) is a widely-used symmetric key encryption algorithm standardized by NIST. This implementation focuses on the **AES-128** variant, involving 10 rounds of encryption over 128-bit plaintext and key inputs.

---

## 🚀 Features

- 🔒 **AES-128 Bit Encryption**: Implements the standard 10-round AES encryption algorithm  
- 🧩 **Modular Design**: Each AES operation is developed as an independent Verilog module  
- ✅ **Simulation-Ready**: Includes testbench for validating encryption output against standard vectors  
- 💡 **Synthesizable RTL**: Designed for FPGA implementation and educational hardware design use  
- 🔁 **Round-Key Expansion Logic**: Built-in key expansion to support all encryption rounds  
- 📦 **Compact & Portable**: Clean, well-documented codebase for easy reuse and extension

---

## 🔧 Key Components

- **aes_top.v** – Integrates all internal modules and drives the overall AES core  
- **sub_bytes.v** – Performs S-Box substitution using a lookup table  
- **shift_rows.v** – Shifts the rows of the state matrix as per AES spec  
- **mix_columns.v** – Mixes the state matrix columns using Galois Field operations  
- **add_round_key.v** – Performs XOR with round keys  
- **key_expansion.v** – Generates round keys using RCON and byte substitution  
- **sbox.v** – Lookup-based S-Box used in SubBytes and Key Expansion  
- **testbench.v** – Contains input vectors and verification logic  
- **simulation.do** – TCL script for simulating the design in ModelSim-Altera

---

## 🛠 Tools Used

| Tool               | Purpose                                |
|--------------------|----------------------------------------|
| **Verilog HDL**     | RTL design of the AES encryption core  |
| **ModelSim-Altera** | Simulation and waveform debugging      |

---

