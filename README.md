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
