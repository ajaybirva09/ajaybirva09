<!-- Header with animated VLSI theme -->
<h1 align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=30&duration=4000&pause=1000&color=22D3EE&center=true&vCenter=true&width=600&height=70&lines=Welcome+to+my+Digital+World!;VLSI+Enthusiast+%26+Embedded+Engineer;RTL+Design+%7C+Verification+%7C+FPGA" alt="Typing Animation" />
</h1>

<div align="center">
  
  <!-- Animated circuit board -->
  ![Circuit Animation](https://media.giphy.com/media/l46Cy1rHbQ92uuLXa/giphy.gif)
  
  <!-- Stats with VLSI theme -->
  <img src="https://github-readme-stats.vercel.app/api?username=ajaybirva09&show_icons=true&theme=nightowl&hide_border=true&bg_color=0d1117&title_color=22D3EE&icon_color=22D3EE" height="180" alt="stats graph" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ajaybirva09&layout=compact&theme=nightowl&hide_border=true&bg_color=0d1117&title_color=22D3EE&langs_count=8" height="180" alt="languages graph" />
</div>

---

## 🔬 **VLSI & Digital Design Portfolio**

### **🛠️ Core Technical Skills**

| **Category** | **Technologies & Tools** |
|--------------|--------------------------|
| **🖥️ HDL Languages** | ![Verilog](https://img.shields.io/badge/Verilog-FF6F00?style=for-the-badge&logo=verilog&logoColor=white) ![SystemVerilog](https://img.shields.io/badge/SystemVerilog-8A2BE2?style=for-the-badge&logo=verilog&logoColor=white) ![VHDL](https://img.shields.io/badge/VHDL-000080?style=for-the-badge) |
| **⚡ EDA Tools** | ![Vivado](https://img.shields.io/badge/Xilinx_Vivado-E01F27?style=for-the-badge&logo=xilinx&logoColor=white) ![Quartus](https://img.shields.io/badge/Intel_Quartus-0071C5?style=for-the-badge&logo=intel&logoColor=white) ![Cadence](https://img.shields.io/badge/Cadence-FF0000?style=for-the-badge) ![ModelSim](https://img.shields.io/badge/ModelSim-00BFFF?style=for-the-badge) |
| **🔌 Protocols** | ![I2C](https://img.shields.io/badge/I²C-8B008B?style=for-the-badge) ![SPI](https://img.shields.io/badge/SPI-32CD32?style=for-the-badge) ![UART](https://img.shields.io/badge/UART-FF4500?style=for-the-badge) |
| **📟 FPGA Platforms** | ![FPGA](https://img.shields.io/badge/FPGA-FF6347?style=for-the-badge) ![Xilinx](https://img.shields.io/badge/Xilinx-E01F27?style=for-the-badge&logo=xilinx&logoColor=white) ![Intel FPGA](https://img.shields.io/badge/Intel_FPGA-0071C5?style=for-the-badge&logo=intel&logoColor=white) |
| **💻 Programming** | ![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![SystemC](https://img.shields.io/badge/SystemC-FF6600?style=for-the-badge) |

---

## **🚀 Featured Projects**

### **1. Single-Port Synchronous RAM Design & Verification**
<div align="center">

```systemverilog
// Parameterized RAM Module
module sync_ram #(
    parameter ADDR_WIDTH = 8,
    parameter DATA_WIDTH = 32
)(
    input logic clk,
    input logic we,
    input logic [ADDR_WIDTH-1:0] addr,
    input logic [DATA_WIDTH-1:0] data_in,
    output logic [DATA_WIDTH-1:0] data_out
);
    // RTL Implementation
endmodule
