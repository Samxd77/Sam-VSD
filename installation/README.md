
#  Week 0: VLSI System Design (VSD) RISC V TAPEOUT Program – Environment & Tool Setup 

  
This week was dedicated to setting up the development environment and installing the essential open-source tools for synthesis, simulation, circuit analysis, and layout design.  

---

## 🎯 System / VM Configuration  

| Specification 💻 | Details 📋 |
|-----------------|------------|
| Operating System 🐧 | Ubuntu 20.04+ |
| RAM 💾 | 6 GB |
| Storage 💿 | 50 GB HDD |
| vCPUs ⚡ | 4 |

💡 *This setup ensures smooth performance for running EDA toolchains and simulations.*  

---

## ⚙️ Tool Installation & Verification  

The following open-source tools were installed and verified:  

### 🧠 1. Yosys – RTL Synthesis  
**Purpose:** Converts RTL code into gate-level netlists.  

```bash
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make build-essential clang bison flex \
  libreadline-dev gawk tcl-dev libffi-dev git \
  graphviz xdot pkg-config python3 libboost-system-dev \
  libboost-python-dev libboost-filesystem-dev zlib1g-dev
make
sudo make install


