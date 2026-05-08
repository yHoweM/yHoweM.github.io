---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

I am a Ph.D. student in Integrated Circuit Science and Engineering at Southern University of Science and Technology, jointly trained with Peng Cheng Laboratory. I received my B.Eng. degree in Microelectronics Science and Engineering from Southern University of Science and Technology.

My research focuses on **AI accelerator architecture**, **neuromorphic computing**, **spiking neural network training**, **NPU operator optimization**, and **hardware-software co-design** for efficient deep learning systems. I am particularly interested in spike-aware training accelerators, Spiking Transformers, many-core neuromorphic systems, sparse attention operators, and energy-efficient AI computing across FPGA, ASIC, and commercial NPUs.

Before and during my Ph.D. study, I worked on several hardware-oriented AI computing projects, including Spiking Transformer training accelerators, many-core SNN training architectures, floating-point arithmetic IP design, and a 28 nm stereo depth co-processor ASIC.

<!-- Replace the Google Scholar link below with your own profile when available. -->
<!--
Google Scholar: <a href='https://scholar.google.com/citations?user=oreBfP8AAAAJ'>profile</a>
<a href='https://scholar.google.com/citations?user=oreBfP8AAAAJ'>
<img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations">
</a>
-->

# 🔥 News

- *2026*: &nbsp; Started to try researching on key sparse operator optimization for large-model inference on Huawei Ascend NPUs.
- *2026*: &nbsp; One paper is under reviewed by **MCSoC 2026** on communication-aware placement optimization for many-core SNN training.
- *2026*: &nbsp; One paper accepted by **IEEE NEWCAS 2026** on simulation-guided SNN training co-design with FPGA prototyping.
- *2026*: &nbsp; One first-author paper published in **Microelectronics Journal** on spike-aware training architecture for Spiking Transformers.
- *2025*: &nbsp; One first-author paper accepted by **IEEE SOCC 2025** on simulation and dataflow optimization for spike-driven Transformer systems.
- *2025*: &nbsp; One first-author paper accepted by **IEEE ICTA 2025** on reusable floating-point fused-multiply-add processor design.
- *2024*: &nbsp; One co-authored paper published in **IEEE TCAS-I** based on a 28 nm stereo depth co-processor ASIC project with the taped-out chip.

# 📝 First-author Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">MEJ 2026</div><img src='images/mej2026.png' alt="Spiking Transformer Training Architecture" width="75%"></div></div>
<div class='paper-box-text' markdown="1">

[An Energy-Efficient Spike-Aware Training Architecture for Spiking Transformers](#)

**Yunhao Ma**, Yanyu Lin, Mingjing Li, Puli Quan, Chenlin Zhou, Wanyi Jia, Xueke Zhu, Qingyan Meng, Huihui Zhou, Fengwei An

**Microelectronics Journal**, 2026.

[**PDF**](#) | [**DOI**](#) | [**BibTeX**](#)

- Proposed a spike-aware training architecture for Spiking Transformers, supporting FP, BP, and WG stages.
- Designed a reuse processing element array for both spike-gated FP16 accumulation and FP16 MAC computation.
- Developed a cross-layer simulation framework for energy, latency, and dataflow analysis.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">NEWCAS 2026</div><img src='images/newcas2026.png' alt="SNN Training Co-Design Framework" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[A Simulation-Guided Co-Design Framework for SNN Training with FPGA Prototyping](#)

**Yunhao Ma**, Wanting Wen, Wanyi Jia, Boyang Ma, Yanyu Lin, Xueke Zhu, Qingyan Meng, Huihui Zhou, Yonghong Tian, Fengwei An

**IEEE International NEWCAS Conference**, 2026.

[**PDF**](#) | [**BibTeX**](#)

- Proposed a simulation-guided hardware-software co-design framework for SNN training.
- Covered forward propagation, backward propagation, and weight-gradient computation.
- Validated the selected architecture and dataflow through FPGA prototyping.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">MCSoC 2026</div><img src='images/mcsoc2026' alt="Many-Core SNN Training Placement" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Communication-Aware Placement Optimization for Many-Core SNN Training via Graph-based Reinforcement Learning](#)

**Yunhao Ma**, Wanting Wen, Yanyu Lin, Wenjie Lin, Wenxiang Cheng, Boyang Ma, Xiang Li, Wanyi Jia, Zhengyu Ma, Fengwei An, Xueke Zhu, Yonghong Tian, Huihui Zhou

**IEEE International Symposium on Embedded Multicore/Many-core Systems-on-Chip**, 2026.

[**PDF**](#) | [**BibTeX**](#)

- Studied communication-aware placement for SNN training on many-core near-memory systems.
- Proposed a graph-based PPO placement optimizer to reduce NoC communication cost and hotspots.
- Evaluated the method on Spike-ResNet and Spike-VGG workloads under 32- and 64-tile mesh settings.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">SOCC 2025</div><img src='images/socc2025' alt="SimST Framework" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[SimST: Simulation Framework for Energy-Dataflow Co-Optimization in Spike-Driven Transformer](#)

**Yunhao Ma**, Yanyu Lin, Wanyi Jia, Puli Quan, Mingjing Li, Zhiwei Zhong, Fengwei An, Huihui Zhou

**IEEE International System-on-Chip Conference**, 2025.

[**PDF**](#) | [**BibTeX**](#)

- Built a simulation framework for spike-driven Transformer workloads.
- Analyzed energy and dataflow trade-offs for spike-aware AI computing.
</div>
</div>

- [Multiple Precision Floating-Point Fused-Multiply-Add Processor with Hardware Reuse Architecture](#), **Yunhao Ma**, et al., **IEEE ICTA 2025**.
- [Stereo Depth Co-Processor ASIC Design](#), Collaborative work, **IEEE Transactions on Circuits and Systems I: Regular Papers**, 2024.
- [Sensors-based Stereo Depth Processing Work](#), **Yunhao Ma**, et al., **Sensors**, 2022.
- [Stereo Vision Accelerator Design](#), **Yunhao Ma**, et al., **APCCAS 2022**.

# 🔬 Research Projects

## NPU Sparse Attention Operator Optimization
- *2026.03 - Present*
- Optimizing sparse attention operators for large-model inference on Huawei Ascend NPUs.
- Research topics include block-sparse attention, selected attention, sparse index layout, irregular KV access, load balancing, and hardware-aware scheduling.
- Keywords: **Ascend NPU**, **BSA/DSA**, **KV Cache**, **Sparse Attention**, **Operator Optimization**.

## Spiking Transformer Training Accelerator and Simulator
- *2024.12 - 2026.02*
- Proposed a spike-aware training architecture and a software-hardware co-design simulator for Spiking Transformers.
- Covered key operators including MM, BN, LIF/SOMA, GRAD, and RES.
- Supported full FP/BP/WG training mapping with energy-dataflow analysis.
- Validated key components through Verilog/HLS-based FPGA synthesis and implementation.

## Many-Core CSNN Training Accelerator Architecture
- *2023.12 - 2025.11*
- Participated in the design and implementation of array engines and spike-delivery operators for multi-core CSNN training.
- Focused on floating-point spike-based computation, DRAM traffic reduction, and training-phase mapping on FPGA and many-core architectures.

## Floating-Point Arithmetic IP Design
- *2023.04 - 2025.02*
- Designed floating-point multiplier, adder, comparator, and fused-multiply-add IPs using Verilog.
- Evaluated resource overhead, pipeline structure, and synthesis frequency against Xilinx Vivado floating-point IPs.
- Keywords: **Verilog**, **FP16**, **RTL Design**, **FPGA**, **Arithmetic IP**.

## Stereo Depth Co-Processor ASIC Design
- *2021.08 - 2023.04*
- Worked on a 28 nm CMOS ASIC for pixel-level Semi-Global Matching.
- Completed DC synthesis, sub-module APR, PrimeTime timing analysis, and Calibre LVS/DRC verification.
- Proposed post-processing optimization modules including sub-pixel interpolation and multi-directional refinement.
- The project was successfully taped out.

# 🎖 Honors and Awards

- *2024*: Huawei Intelligent Foundation Scholarship, Top 10.
- *2023*: Outstanding Graduate, School of Microelectronics, Southern University of Science and Technology.
- *2022*: APCCAS 2022 Best Paper Nomination.
- *2022*: Zhicheng College Innovation and Entrepreneurship Scholarship, Top 2.
- *2021*: International First Prize in academic competitions at Southern University of Science and Technology.
- *2021*: Global Intelligent Robot Competition, Best Performance Award and Global Champion.

# 📖 Educations

- *2023.09 - Present*, Ph.D. Student, Integrated Circuit Science and Engineering, Southern University of Science and Technology / Peng Cheng Laboratory.
- *2019.09 - 2023.06*, B.Eng., Microelectronics Science and Engineering, Southern University of Science and Technology. GPA: 3.68 / 4.0. IELTS: 7.0.

# 💻 Technical Skills

- **Hardware Design**: RTL design, Verilog, FPGA, HLS, ASIC flow, DC synthesis, APR, STA, LVS/DRC.
- **AI Computing Systems**: AI accelerator architecture, SNN training, Spiking Transformer, sparse attention, NPU operator optimization.
- **Modeling and Simulation**: Energy modeling, dataflow simulation, memory hierarchy analysis, CACTI, Vivado/Vitis HLS, Synopsys, Calibre.
- **Programming**: Python, C/C++, Verilog, HLS C/C++, shell scripting.

# 💬 Selected Research Interests

- Spike-aware training accelerator architecture.
- Hardware-software co-design for efficient AI systems.
- Sparse attention operator optimization on commercial NPUs.
- Many-core neuromorphic systems and NoC-aware mapping.
- Energy-efficient FPGA/ASIC implementation for deep learning workloads.
