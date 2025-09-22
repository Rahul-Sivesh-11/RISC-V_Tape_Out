# Week_0_RISC-V_Tape_Out
This document describes the setup and verification of the required tools for the VSD RISC-V Tapeout program.
## Tools Installation
All the instructions for installation of required tools can be found here.
## System Information
![System Informaton](https://github.com/Rahul-Sivesh-11/Week_0_RISC-V_Tape_Out/blob/main/Images/Screenshot%20from%202025-09-19%2022-54-15.png)
## TOOLS INSTALLATION
### <ins>Yosys Installation</ins>
<pre>sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make
sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
git submodule update --init --recursive
make
sudo apt install yosys</pre>
### TOOL CHECK:
<pre>yosys</pre>
![Tools](https://github.com/Rahul-Sivesh-11/Week_0_RISC-V_Tape_Out/blob/main/Images/Screenshot%20from%202025-09-19%2021-51-36.png)
###  Iverilog
Iverilog comes bundled with the OSS-CAD Suite, but the problem is, it comes with the latest version 13 which isn't regarded as a stable version in Iverilog's documentation Thus, we have to manually revert back to a stable version. This is done by deleting all iverilog files that came bundled with OSS-CAD Suite 
### Installation:
<pre>sudo apt-get update
sudo apt-get install iverilog</pre>
### Verification:
<pre>iverilog -v</pre>
![Tool Check](https://github.com/Rahul-Sivesh-11/Week_0_RISC-V_Tape_Out/blob/main/Images/Screenshot%20from%202025-09-19%2022-42-16.png)
## GTKWave Installation & Verification
GTKWave is a waveform analyzer for viewing .vcd simulation results.

### Installation
Recommended:
<pre>sudo apt update
sudo apt install gtkwave</pre>
![gtk](https://github.com/Rahul-Sivesh-11/Week_0_RISC-V_Tape_Out/blob/main/Images/Screenshot%20from%202025-09-19%2022-42-49.png)

![Wave](https://github.com/Rahul-Sivesh-11/Week_0_RISC-V_Tape_Out/blob/main/Images/Screenshot%20from%202025-09-19%2022-55-38.png)



