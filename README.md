💻 Ajay | Digital Design & Verification Engineer
https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=32&pause=1000&color=22D3EE&center=true&vCenter=true&width=700&lines=Hello+World!+%F0%9F%91%8B;I'm+Ajay+%25F0%259F%2591%258B;Digital+Design+%2526+Verification+Engineer;SystemVerilog+%257C+UVM+%257C+FPGA+%257C+RTL

<div align="center">
https://komarev.com/ghpvc/?username=ajay098&label=Profile+Views&color=0ea5e9&style=for-the-badge
https://img.shields.io/badge/Digital-Design-8b5cf6?style=for-the-badge&logo=amd
https://img.shields.io/badge/Verification-Expert-10b981?style=for-the-badge&logo=verizon
https://img.shields.io/badge/VLSI-Enthusiast-ef4444?style=for-the-badge&logo=chip

</div><div align="center"> <img src="https://raw.githubusercontent.com/platane/platane/output/github-contribution-grid-snake-dark.svg" alt="Circuit Animation" width="100%"> </div>
🎯 Design Philosophy
"In digital design, we don't guess; we verify. Every line of RTL must be proven before silicon sees the light of day."

I'm a passionate VLSI Digital Design & Verification Engineer with expertise in building robust digital systems and comprehensive verification environments. My work bridges RTL design, UVM methodology, and FPGA prototyping to ensure first-pass silicon success.

<div align="center">
https://media.giphy.com/media/26tn33aiTi1jkl6H6/giphy.gif Where hardware meets elegance

</div>
📊 GitHub Analytics
<div align="center">
https://github-readme-stats.vercel.app/api?username=ajay098&show_icons=true&theme=nightowl&hide_border=true&include_all_commits=true&count_private=true&show=reviews,discussions_started,discussions_answered	https://github-readme-stats.vercel.app/api/top-langs/?username=ajay098&layout=compact&theme=nightowl&hide_border=true&langs_count=8&exclude_repo=github-readme-stats,ajay098.github.io
https://streak-stats.demolab.com?user=ajay098&theme=nightowl&hide_border=true&date_format=M%2520j%255B%252C%2520Y%255D
https://github-profile-trophy.vercel.app/?username=ajay098&theme=onedark&no-frame=true&row=2&column=4

</div>
🏗️ Technical Stack
Digital Design & Verification
systemverilog
// My Typical UVM Environment Structure
class my_env extends uvm_env;
  `uvm_component_utils(my_env)
  
  // Agents, scoreboards, coverage collectors
  my_agent       agent;
  my_scoreboard  scb;
  my_cov         coverage;
  
  virtual function void build_phase(uvm_phase phase);
    // Building verification components
    agent = my_agent::type_id::create("agent", this);
    scb = my_scoreboard::type_id::create("scb", this);
    coverage = my_cov::type_id::create("coverage", this);
  endfunction
endclass
Domain	Technologies	Proficiency	Tools
RTL Design	Verilog, SystemVerilog, VHDL	🔵🔵🔵🔵⚪	Cadence Genus, Synopsys DC
Verification	SystemVerilog, UVM, SVA	🔵🔵🔵🔵🔵	Cadence Xcelium, Synopsys VCS
FPGA Design	Vitis HLS, Vivado	🔵🔵🔵🔵⚪	Xilinx Vivado, Intel Quartus
Scripting	TCL, Python, Makefiles	🔵🔵🔵🔵⚪	Bash, Perl, CMake
Methodology	OOP, CDV, Formal	🔵🔵🔵🔵⚪	UVM, JasperGold, VC Formal
Tool Ecosystem
<div align="center">
EDA Tools
https://img.shields.io/badge/Cadence-FF0000?style=flat-square&logo=cadence&logoColor=white
https://img.shields.io/badge/Synopsys-FF6F00?style=flat-square&logo=synopsys&logoColor=white
https://img.shields.io/badge/Siemens_EDA-00A3E0?style=flat-square&logo=siemens&logoColor=white
https://img.shields.io/badge/Xilinx-E01F27?style=flat-square&logo=xilinx&logoColor=white

Programming
https://img.shields.io/badge/SystemVerilog-DA1F26?style=flat-square&logo=verilog&logoColor=white
https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white
https://img.shields.io/badge/TCL-808080?style=flat-square&logo=tcl&logoColor=white
https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%252B%252B&logoColor=white

Platforms
https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black
https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white
https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white

</div>
🚀 Featured Projects
📟 Single-Port Synchronous RAM with UVM Verification (Coming Soon)
A complete digital design and verification flow demonstrating industry best practices

systemverilog
// Parameterized Single-Port SRAM
module sp_sram #(
  parameter ADDR_WIDTH = 8,
  parameter DATA_WIDTH = 32,
  parameter DEPTH      = 256
)(
  input  logic                     clk,
  input  logic                     wr_en,
  input  logic [ADDR_WIDTH-1:0]    addr,
  input  logic [DATA_WIDTH-1:0]    data_in,
  output logic [DATA_WIDTH-1:0]    data_out
);

  logic [DATA_WIDTH-1:0] memory [0:DEPTH-1];
  
  always_ff @(posedge clk) begin
    if (wr_en) begin
      memory[addr] <= data_in;
    end
    data_out <= memory[addr];
  end
  
  // SVA Assertions
  property no_write_read_same_addr;
    @(posedge clk) !(wr_en && $past(wr_en) && (addr == $past(addr)));
  endproperty
  
  assert_no_write_read_same_addr: assert property (no_write_read_same_addr);
endmodule
Achievements:

✅ 100% Functional Coverage with constrained random testing

✅ UVM Testbench with reusable sequences and scoreboard

✅ Formal Verification using SVA assertions

✅ Gate-Level Simulation with SDF annotations

✅ Power-Aware Simulation with UPF

🔄 AXI4-Lite Interface Controller (Coming Soon)
Industry-standard bus protocol implementation with full verification suite

Features:

🔹 Configurable data width (32/64/128-bit)

🔹 Multiple outstanding transactions

🔹 Error injection and detection

🔹 Performance monitoring with built-in counters

🔹 UVC (Universal Verification Component) for reuse

Verification Metrics:

📈 Code Coverage: 98.5%

📈 Functional Coverage: 100% (all scenarios)

📈 Assertion Coverage: 100%

🧪 Regression Tests: 750+ unique tests

🎛️ RISC-V RV32I Core Verification (Coming Soon)
Complete UVM verification environment for processor core

systemverilog
// UVM Test Class
class riscv_base_test extends uvm_test;
  `uvm_component_utils(riscv_base_test)
  
  riscv_env env;
  riscv_vseq  vseq;
  
  virtual function void build_phase(uvm_phase phase);
    super.build_phase(phase);
    env = riscv_env::type_id::create("env", this);
    
    // Factory override for different test types
    set_type_override_by_type(
      riscv_instr::get_type(),
      riscv_branch_instr::get_type()
    );
  endfunction
  
  task run_phase(uvm_phase phase);
    vseq = riscv_vseq::type_id::create("vseq");
    phase.raise_objection(this);
    vseq.start(env.vsequencer);
    phase.drop_objection(this);
  endtask
endclass
📚 Learning Journey
Certifications
Course	Provider	Date	Status
SystemVerilog UVM Verification	Maven Silicon	2024	🏆 Completed
Advanced Digital Design with Verilog	Udemy	2024	🏆 Completed
FPGA Design with Vivado HLS	Xilinx	2023	🏆 Completed
Formal Verification Fundamentals	Cadence	2023	🏆 Completed
Low-Power Design with UPF	Synopsys	2023	🏆 Completed
Currently Exploring











🏆 Achievements
Research Publication
"Development of an Autonomous Surface Vehicle for Real-Time Aquatic Environment Monitoring and Depth Mapping"
*Presented at CSEAi 2024 (SCOPUS-indexed Conference)*

🎖️ KSCST Funding: ₹4,500 for project development

🔬 Innovation: Solar-powered ASV with real-time data processing

📊 Impact: 95% accuracy in water quality parameter measurement

Academic Excellence
🥇 Department Rank: Top 10% in ECE Batch

🏅 Project Exhibition: First Prize in Technical Fest 2023

📝 Technical Papers: 2 conference publications in VLSI domain

💼 Professional Experience
Embedded Systems Engineer Intern @ TIF Labs (Robocraze)
*June 2024 - Present*

🔹 Developed FPGA-based motor control systems using Verilog

🔹 Implemented real-time sensor data processing pipelines

🔹 Reduced power consumption by 15% through clock gating techniques

🔹 Created UVM testbenches for custom IP verification

VLSI Project Trainee @ Sahyadri College
*Jan 2024 - May 2024*

🔹 Designed and verified 8-bit RISC processor

🔹 Implemented AMBA AHB protocol verification environment

🔹 Achieved 97% coverage score on processor core

🔹 Developed Python scripts for regression automation

🎓 Education
Bachelor of Engineering in Electronics & Communication
Sahyadri College of Engineering and Management, Mangaluru
*2020 - 2024* | CGPA: 8.5/10

Relevant Coursework:

Digital System Design

VLSI Design & Technology

Embedded Systems

Computer Architecture

Verification Methodologies

Signal Processing

📝 Technical Blog
Latest Articles
markdown
📖 **Understanding UVM Phases** - Deep dive into UVM execution flow
📖 **SVA Cookbook** - Practical assertions for common scenarios
📖 **Coverage-Driven Verification** - Strategies for coverage closure
📖 **FPGA Prototyping Best Practices** - From RTL to bitstream
📖 **Low-Power Verification with UPF** - Power-aware simulation techniques
🤝 Collaboration Opportunities
I'm actively looking to collaborate on:

Project Type	Interest Level	Availability
Open-Source VLSI Cores	🔵🔵🔵🔵🔵	High
UVM Verification IP	🔵🔵🔵🔵⚪	Medium
FPGA Acceleration	🔵🔵🔵🔵⚪	High
Research Papers	🔵🔵🔵⚪⚪	Medium
Mentoring	🔵🔵🔵🔵⚪	Limited
Current Open Source Contributions
bash
# Projects I'm contributing to
1. verilog-ethernet - Ethernet cores in Verilog
2. riscv-formal - Formal verification of RISC-V cores
3. uvvm - Universal VHDL Verification Methodology
4. cocotb - Python-based verification framework
📫 Connect With Me
<div align="center">
https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white
https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white
https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white
https://img.shields.io/badge/Portfolio-Visit-8B5CF6?style=for-the-badge&logo=google-chrome&logoColor=white
https://img.shields.io/badge/Twitter-Follow-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white

</div>
Let's Talk About:
🔍 Code Reviews - RTL, UVM testbenches, scripts

🧪 Verification Strategies - Coverage closure, formal methods

🚀 Career Growth - VLSI industry trends, skill development

📚 Learning Resources - Books, courses, online materials

💡 Project Ideas - FPGA, ASIC, verification IP development

📈 GitHub Activity
<!--START_SECTION:activity--><!-- This section is automatically generated by GitHub Actions --><!--END_SECTION:activity--><div align="center">
Weekly Development Breakdown
https://github-readme-stats.vercel.app/api/wakatime?username=ajay098&theme=nightowl&hide_border=true&layout=compact&langs_count=6

</div>
🎯 Current Goals
💬 Testimonials
"Ajay's understanding of UVM methodology is exceptional for his experience level. His verification environments are robust and well-documented."
- Dr. Suresh Kumar, Professor of VLSI

"The Single-Port RAM project demonstrated professional-grade verification techniques. The coverage closure strategy was particularly impressive."
- Mentor, Cadence Design Systems

<div align="center">
⚡ Quick Stats
https://img.shields.io/badge/Lines%2520of%2520Code-50K+-blue?style=flat-square
https://img.shields.io/badge/UVM%2520Tests-500%252B-green?style=flat-square
https://img.shields.io/badge/Projects-15%252B-orange?style=flat-square
https://img.shields.io/badge/Open%2520Source-3%2520repos-yellow?style=flat-square


"Every chip tells a story. My job is to ensure it's a success story."

⭐ Star my repositories if you find them useful!
🔭 Watching for exciting VLSI projects to contribute to!


https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer&text=Keep%2520Designing%252C%2520Keep%2520Verifying!&fontSize=20&fontAlignY=70

</div>
