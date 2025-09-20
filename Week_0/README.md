# 🚀 Week 0: RISC-V VSD Program Foundation & Tool Setup
📌 *Status: Completed Environment & Tool Setup*

Welcome to my **RISC-V VSD Program** repository!  
This week focused on setting up the development environment and installing the essential open-source tools that will be used throughout the program.  

The goal: create a reliable and efficient workspace for synthesis, simulation, and design tasks.

---

## 🎯 System / VM Configuration
To ensure optimal performance, I configured a Virtual Machine (VM) with the following specifications:

| Specification 💻 | Details 📋 |
|------------------|------------|
| Operating System 🐧 | Ubuntu 20.04+ |
| RAM 💾 | 6 GB |
| Storage 💿 | 50 GB HDD |
| vCPUs ⚡ | 4 |

💡 *Pro Tip: This setup ensures smooth toolchain execution and fast simulation runs.*

---

## ⚙️ Tool Installation & Verification
The following open-source tools were installed for RTL synthesis, simulation, waveform analysis, circuit simulation, and layout design.

**🧠 Yosys → 📟 Iverilog → 📊 GTKWave → ⚡ Ngspice → 🎨 Magic VLSI**

---

# 🧠 1. Yosys – RTL Synthesis Tool
**Purpose:** Converts RTL (Verilog) code into gate-level netlists.

✅ **Installation Steps**
```bash
# Day 0 - Tools Installation
## Yosys
git clone [https://github.com/YosysHQ/yosys.git](https://github.com/YosysHQ/yosys.git)
cd yosys
sudo apt install make
sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
make
sudo make install
```
📷 Verification: <img width="1239" height="895" alt="Screenshot 2025-09-20 235057" src="https://github.com/user-attachments/assets/696d3104-96d1-4711-946f-22859b3b77f1" />

✅ Yosys Successfully Installed
---
# 📟 2. Iverilog – Verilog Simulator
**Purpose:** Compiles and simulates Verilog designs for functional verification.

**✅ Installation Steps**

```Bash

sudo apt-get install iverilog
```
📷 Verification: <img width="1107" height="827" alt="Screenshot 2025-09-20 235249" src="https://github.com/user-attachments/assets/c82cff21-866a-42c8-bc4b-7a7b14c13847" />


✅ Iverilog Successfully Installed

# 📊 3. GTKWave – Waveform Viewer
**Purpose:** Visualizes simulation results for debugging and analysis.

**✅ Installation Steps**

```Bash

sudo apt update
sudo apt install gtkwave
```
📷 Verification: <img width="1151" height="828" alt="Screenshot 2025-09-20 235350" src="https://github.com/user-attachments/assets/4e3d7a5a-93de-4c49-80b9-000ddd69bb38" />


✅ GTKWave Successfully Installed

# ⚡ 4. Ngspice – Circuit Simulator
**Purpose:** Performs analog and mixed-signal circuit simulations.

**✅ Installation Steps**

```Bash

sudo apt update
sudo apt install ngspice
```
📷 Verification: <img width="1228" height="366" alt="Screenshot 2025-09-20 235444" src="https://github.com/user-attachments/assets/62dea6ae-5cd3-477e-9f71-1035cddd7998" />


✅ Ngspice Successfully Installed

# 🎨 5. Magic VLSI – Layout Design Tool
**Purpose:** Creates and edits VLSI layouts with DRC (Design Rule Checking).

**✅ Installation Steps**

```Bash

# Install required dependencies
sudo apt-get install m4
sudo apt-get install tcsh
sudo apt-get install csh
sudo apt-get install libx11-dev
sudo apt-get install tcl-dev tk-dev
sudo apt-get install libcairo2-dev
sudo apt-get install mesa-common-dev libglu1-mesa-dev
sudo apt-get install libncurses-dev

### Clone Magic repository
git clone [https://github.com/RTimothyEdwards/magic](https://github.com/RTimothyEdwards/magic)
cd magic

### Configure build
./configure

### Build Magic
make

### Install system-wide
sudo make install
```
📷 Verification: <img width="907" height="202" alt="Screenshot 2025-09-20 235745" src="https://github.com/user-attachments/assets/f602c291-2726-400a-8202-362939353a52" />


✅ Magic VLSI Successfully Installed

🚀 Environment Ready for the RISC-V VSD Journey!

📂 Repository: RISC-V

👨‍💻 Author: ANURAG SINGH

📚 Program: RISC-V VSD

⭐ Don’t forget to star the repo if you found this useful!
