# Awesome AI Engineering Agents

[English](README.md) | [简体中文](README_CN.md)

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![更新时间](https://img.shields.io/badge/updated-2026--08-blue)
![许可证](https://img.shields.io/github/license/whut09/Awesome-AI-Engineering-Agents)

本项目精选 **2020 年及以后**将人工智能应用于工程岗位的论文和开源项目，覆盖
光学工程、硬件与 PCB 设计、结构与 CAD 工程，以及 FPGA 工程四条技术路线。

条目按照实际工程工作流组织，包括设计、仿真、分析、审查、生成、综合和布线。
早期基础工具只有在 2020 年以后仍有实质维护、并且仍是当前 AI 工程流程的重要
组成部分时才会收录。

> [!NOTE]
> 开源项目必须提供明确的许可证。没有声明许可证的论文代码或数据集会单独列出，
> 不视为开源项目。用于商业场景前，请同时核查模型、数据集、第三方资产及厂商
> EULA 的具体条款。

## 目录

- [光学工程](#光学工程)
- [硬件与 PCB 设计](#硬件与-pcb-设计)
- [结构与 CAD 工程](#结构与-cad-工程)
- [FPGA 工程](#fpga-工程)
- [贡献](#贡献)
- [许可证](#许可证)

## 光学工程

### 设计、仿真与逆向设计论文

| 年份 | 会议/期刊 | 论文 | 工程流程 |
|:---:|:---:|:---|:---|
| 2026 | arXiv | [OptiAgent: A Physics-Driven Agentic Framework for Automated Optical Design](https://arxiv.org/abs/2602.23761) | 智能体驱动的自动光学设计 |
| 2025 | DATE | [MAPS: Multi-Fidelity AI-Augmented Photonic Simulation and Inverse Design Infrastructure](https://arxiv.org/abs/2503.01046) | 光子仿真与逆向设计 |
| 2024 | Advanced Engineering Informatics | [Artificial intelligence in optical lens design](https://doi.org/10.1007/s10462-024-10842-y) | AI 镜头设计综述 |
| 2024 | arXiv | [TorchOptics: An open-source Python library for differentiable Fourier optics](https://arxiv.org/abs/2411.18591) | 可微分波动光学 |
| 2024 | Nature Communications | [Curriculum learning for ab initio deep learned refractive optics](https://doi.org/10.1038/s41467-024-50835-7) | 自动镜头设计 |
| 2023 | ASPLOS | [LightRidge: An End-to-end Agile Design Framework for Diffractive Optical Neural Networks](https://doi.org/10.1145/3623278.3624757) | 衍射光学神经网络 |
| 2020 | TOG | [Neural Holography with Camera-in-the-loop Training](https://doi.org/10.1145/3414685.3417802) | 全息图生成与闭环标定 |
| 2020 | CVPR | [Deep Optics for Single-Shot High-Dynamic-Range Imaging](https://doi.org/10.1109/CVPR42600.2020.00145) | 学习式光学编码 |

### 智能体光学设计论文

| 年份 | 论文 | 工程流程 |
|:---:|:---|:---|
| 2026 | [OptiAgent: End-to-End Optimization Modeling via Multi-Agent Iterative Refinement](https://arxiv.org/abs/2607.05346) | 多智能体优化建模 |
| 2026 | [OPTIAGENT: A Physics-Driven Agentic Framework for Automated Optical Design](https://arxiv.org/abs/2602.23761) | 物理验证的光学设计智能体 |

### 开源项目

| 项目 | 工程用途 | 许可证 |
|:---|:---|:---:|
| [DeepLens](https://github.com/singer-yang/DeepLens) | 可微分几何光学与自动镜头设计 | Apache-2.0 |
| [DeepTrack 2.0](https://github.com/softmatterlab/DeepTrack2) | 显微成像、粒子跟踪与光学表征 | MIT |
| [diffractsim](https://github.com/rafael-fuente/diffractsim) | 可微分衍射仿真 | MPL-2.0 |
| [Dolphindes](https://github.com/physical-design-bounds/dolphindes) | 光子逆向设计的性能边界与优化 | MIT |
| [MAPS](https://github.com/ScopeX-ASU/MAPS) | 多保真 AI 光子仿真与逆向设计 | MIT |
| [pinn-shaper](https://github.com/rafael-fuente/pinn-shaper) | 基于 PINN 的平面光学光束整形 | MPL-2.0 |
| [TorchOptics](https://github.com/matthewfilipovich/torchoptics) | 基于 PyTorch 的傅里叶光学仿真与优化 | MIT |
| [waveprop](https://github.com/ebezzam/waveprop) | 自由空间传播与全息模型 | MIT |

## 硬件与 PCB 设计

本节覆盖 IC/SoC 物理设计、模拟版图、PCB 原理图与布线、设计规则检查、热分析和
图纸审查。FPGA RTL 生成与实现请参见 [FPGA 工程](#fpga-工程)。

### 原理图、PCB 与 CAD 生成论文

| 年份 | 会议/期刊 | 论文 | 工程流程 |
|:---:|:---:|:---|:---|
| 2026 | arXiv | [SchGen: PCB Schematic Generation with Semantic-Grounded Code Representations](https://arxiv.org/abs/2605.30345) | PCB 原理图生成 |
| 2026 | arXiv | [PCBSchemaGen: Constraint-Guided Schematic Design via LLM](https://arxiv.org/abs/2602.00510) | 约束驱动的原理图设计 |
| 2026 | ICLR | [PCB-Bench: Benchmarking LLMs for Printed Circuit Board Placement and Routing](https://jdzhu19.github.io/publication/conference_2026iclr_li/conference_2026ICLR_Li.pdf) | PCB 布局布线基准 |
| 2024 | IEEE | [AI-Optimized Placement and Routing for PCB Design](https://ieeexplore.ieee.org/document/10568665) | PCB 布局布线 |
| 2024 | arXiv | [LLM4EDA: Emerging Progress in Large Language Models for Electronic Design Automation](https://arxiv.org/abs/2401.12224) | 大模型 EDA 综述 |
| 2024 | arXiv | [CadVLM: Bridging Language and Vision in the Generation of Parametric CAD](https://arxiv.org/abs/2409.17457) | 工程图与 CAD 理解 |
| 2023 | TCAD | [TRouter: Thermal-driven PCB Routing via Non-Local Crisscross Attention Networks](https://ieeexplore.ieee.org/abstract/document/10042057) | 热感知 PCB 布线 |
| 2023 | ASP-DAC | [DPRoute: Deep Learning Framework for Package Routing](https://doi.org/10.1145/3566097.3567902) | 封装与电路板布线 |
| 2023 | NeurIPS Workshop | [CAD-LLM: Large Language Model for CAD Generation](https://neurips.cc/virtual/2023/75064) | 文本生成 CAD |
| 2022 | DAC | [Automated Accelerator Optimization Aided by Graph Neural Networks](https://doi.org/10.1145/3489517.3530409) | 硬件设计空间探索 |
| 2022 | ML4CAD | [A Thermal Machine Learning Solver for Chip Simulation](https://doi.org/10.1145/3551901.3556484) | 芯片热仿真 |
| 2021 | NeurIPS | [On Joint Learning for Solving Placement and Routing in Chip Design](https://proceedings.neurips.cc/paper/2021/file/898aef0932f6aaecda27aba8e9903991-Paper.pdf) | 联合布局布线 |
| 2021 | DAC | [AutoSVA: Democratizing Formal Verification of RTL Module Interactions](https://doi.org/10.1109/DAC18074.2021.9586118) | 设计审核与形式检查 |
| 2020 | ICCAD | [A Customized Graph Neural Network Model for Guiding Analog IC Placement](https://doi.org/10.1145/3400302.3415624) | 模拟 IC 布局 |

### 智能体 EDA 与硬件设计论文

| 年份 | 论文 | 工程流程 |
|:---:|:---|:---|
| 2026 | [ZhuLong: Execution-Grounded LLM Agent for EDA Scripting with Offline API Self-Exploration](https://arxiv.org/abs/2608.07925) | EDA 脚本智能体 |
| 2026 | [EDATracer: An Agentic Framework for Large-Scale EDA Artifact Analysis](https://arxiv.org/abs/2608.04032) | EDA 产物分析与审查 |
| 2026 | [Can AI Agents Really Complete RTL-to-GDS? Lessons from Benchmarking Tool-Interactive EDA Workflows](https://arxiv.org/abs/2607.17528) | 端到端 RTL-to-GDS 智能体 |
| 2026 | [SABLE: An NDA-Safe Closed-Loop LLM Framework for Analog Circuit Optimization in Industrial EDA Flows](https://arxiv.org/abs/2607.03701) | 模拟电路闭环优化 |
| 2025 | [AutoEDA: Enabling EDA Flow Automation through Microservice-Based LLM Agents](https://arxiv.org/abs/2508.01012) | EDA 流程编排 |
| 2025 | [JARVIS: A Multi-Agent Code Assistant for High-Quality EDA Script Generation](https://arxiv.org/abs/2505.14978) | EDA 脚本生成 |
| 2024 | [Agentic-HLS: An Agentic Reasoning Based High-Level Synthesis System Using Large Language Models](https://arxiv.org/abs/2412.01604) | HLS 代码与指令生成 |
| 2024 | [EDA-Aware RTL Generation with Large Language Models](https://arxiv.org/abs/2412.04485) | 结合综合反馈的 RTL 生成 |
| 2024 | [Automatically Improving LLM-based Verilog Generation using EDA Tool Feedback](https://arxiv.org/abs/2411.11856) | 工具反馈驱动的 Verilog 修复 |
| 2024 | [IICPilot: An Intelligent Integrated Circuit Backend Design Framework Using Open EDA](https://arxiv.org/abs/2407.12576) | 芯片后端设计自动化 |
| 2024 | [Ask-EDA: A Design Assistant Empowered by LLM, Hybrid RAG and Abbreviation De-hallucination](https://arxiv.org/abs/2406.06575) | EDA 设计助手 |
| 2023 | [ChatEDA: A Large Language Model Powered Autonomous Agent for EDA](https://arxiv.org/abs/2308.10204) | 自主 EDA 助手 |

### 开源项目

| 项目 | 工程用途 | 许可证 |
|:---|:---|:---:|
| [ALIGN](https://github.com/ALIGN-analoglayout/ALIGN-public) | 模拟电路原理图到版图自动化 | BSD-3-Clause |
| [CircuitLM](https://github.com/Khandakar227/circuitlm) | 多智能体自然语言到电路原理图生成 | MIT |
| [DeepPCB KiCad plugin](https://github.com/instadeepai/deeppcb-kicad-plugin) | KiCad 中的 AI 辅助 PCB 布局工作流 | Apache-2.0 |
| [DREAMPlace](https://github.com/limbo018/DREAMPlace) | GPU 加速的布局优化 | BSD-3-Clause |
| [KiCad](https://github.com/KiCad/kicad-source-mirror) | 原理图、PCB 布局、DRC 与 3D 检查基础平台 | GPL-3.0 |
| [KiCad Copilot](https://github.com/biosshot/kicad-copilot) | KiCad 项目的大模型助手 | MIT |
| [MAGICAL](https://github.com/magical-eda/MAGICAL) | 机器学习辅助模拟版图设计 | BSD-3-Clause |
| [OpenLane](https://github.com/The-OpenROAD-Project/OpenLane) | 自动化 RTL 到 GDS 流程 | Apache-2.0 |
| [OpenROAD](https://github.com/The-OpenROAD-Project/OpenROAD) | 布局、布线、时序与物理设计自动化 | BSD-3-Clause |
| [PCBFlow](https://github.com/NijoP/pcbflow) | 程序化 PCB 生成与布局 | MIT |
| [SchGen](https://github.com/microsoft/SchGen) | 基于语义代码表示的 PCB 原理图生成 | MIT |

### 许可证不明确的数据集与代码

- [CircuitNet](https://circuitnet.github.io/)：用于拥塞、时序、功耗和 IR 压降
  预测的 EDA 数据集。仓库当前未提供标准软件许可证，复用前请核实条款。
- [PCBSchemaGen](https://github.com/Sthyao/PCBSchemaGen)：2026 年原理图生成
  论文的研究代码，当前未发现明确的仓库许可证。
- [Pro-CAD](https://github.com/BoYuanVisionary/Pro-CAD)：主动澄清需求并生成
  CAD 的官方代码，当前未发现明确的仓库许可证。

### PCB 智能体与多模态基准论文

| 年份 | 论文 | 工程流程 |
|:---:|:---|:---|
| 2026 | [OmniRouting: A Semantic-Coupled Multimodal Benchmark for Constraint-Aware Spatial Reasoning in PCB Routing](https://arxiv.org/abs/2608.04434) | PCB 布线推理 |
| 2026 | [PCBWorld: A Benchmark Environment for Engine-Grounded PCB Design Automation](https://arxiv.org/abs/2607.05915) | 工具交互式 PCB 智能体 |
| 2026 | [OmniLayout: A Schematic-Coupled Multimodal Benchmark for Constraint-Aware Geometric Reasoning in PCB Layout](https://arxiv.org/abs/2607.03261) | PCB 布局推理 |
| 2026 | [PCB-QA: Evaluating LLMs over the First Printed Circuit Board Design Question-Answer Dataset](https://arxiv.org/abs/2606.23704) | PCB 设计知识评测 |
| 2026 | [OmniSch: A Multimodal PCB Schematic Benchmark for Structured Diagram Visual Reasoning](https://arxiv.org/abs/2604.00270) | 原理图审查与推理 |
| 2026 | [HWE-Bench: Can Language Models Perform Board-level Schematic Designs?](https://arxiv.org/abs/2603.18102) | 板级原理图设计基准 |
| 2026 | [CircuitLM: A Multi-Agent LLM-Aided Design Framework for Generating Circuit Schematics from Natural Language Prompts](https://arxiv.org/abs/2601.04505) | 多智能体原理图生成 |
| 2025 | [EEschematic: Multimodal-LLM Based AI Agent for Schematic Generation of Analog Circuit](https://arxiv.org/abs/2510.17002) | 模拟电路原理图智能体 |
| 2024 | [Schemato: An LLM for Netlist-to-Schematic Conversion](https://arxiv.org/abs/2411.13899) | 网表到原理图转换 |
| 2024 | [AmpAgent: An LLM-based Multi-Agent System for Multi-stage Amplifier Schematic Design](https://arxiv.org/abs/2409.14739) | 多级放大器原理图设计 |

## 结构与 CAD 工程

本节覆盖生成式 CAD、拓扑与壁厚感知设计、载荷与应力预测、有限元代理模型、
物理信息仿真，以及工程图和 BIM 审查。

### 智能体 CAD 与结构设计论文

| 年份 | 论文 | 工程流程 |
|:---:|:---|:---|
| 2026 | [RA-CAD: Learning Post-Execution Critique for State-Aware Text-to-CAD Generation](https://arxiv.org/abs/2608.05714) | 状态感知的 CAD 修复 |
| 2026 | [TraceCAD: Trace-Guided Repair for Agentic CAD Generation](https://arxiv.org/abs/2608.03062) | 执行轨迹驱动的 CAD 修复 |
| 2026 | [CADIR: A Cross-Backend Editable Intermediate Representation for Agentic CAD Generation](https://arxiv.org/abs/2608.00891) | 跨 CAD 后端生成 |
| 2026 | [ArtisanCAD: An Industrial-Level CAD Agent with Expert-Grounded Knowledge Distillation](https://arxiv.org/abs/2607.05750) | 工业级 CAD 智能体 |
| 2026 | [AgentsCAD: Automated Design for Manufacturing of FDM Parts via Multi-Agent LLM Reasoning and Geometric Feature Recognition](https://arxiv.org/abs/2607.02448) | 面向增材制造的设计 |
| 2026 | [Embodied CAD: Solver-Grounded LLM Agents for Parametric B-Rep Assembly Modeling](https://arxiv.org/abs/2606.31252) | 参数化装配建模 |
| 2026 | [IterCAD: An Iterative Multimodal Agent for Visually-Grounded CAD Generation and Editing](https://arxiv.org/abs/2606.13368) | CAD 生成与编辑 |
| 2026 | [Physics-in-the-Loop: A Hybrid Agentic Architecture for Validated CAD Engineering Design](https://arxiv.org/abs/2605.19717) | 物理验证的 CAD 设计 |
| 2026 | [Self-Improving CAD Generation Agents with Finite Element Analysis as Feedback](https://arxiv.org/abs/2605.17448) | 有限元反馈闭环 CAD 优化 |
| 2026 | [Zero-to-CAD: Agentic Synthesis of Interpretable CAD Programs at Million-Scale Without Real Data](https://arxiv.org/abs/2604.24479) | 大规模 CAD 程序合成 |
| 2026 | [ArtiCAD: Articulated CAD Assembly Design via Multi-Agent Code Generation](https://arxiv.org/abs/2604.10992) | 可动装配体设计 |
| 2026 | [CADSmith: Multi-Agent CAD Generation with Programmatic Geometric Validation](https://arxiv.org/abs/2603.26512) | 几何验证的 CAD 生成 |
| 2026 | [Clarify Before You Draw: Proactive Agents for Robust Text-to-CAD Generation](https://arxiv.org/abs/2602.03045) | 交互式需求澄清 |
| 2025 | [CADDesigner: Conceptual CAD Model Generation with a General-Purpose Agent](https://arxiv.org/abs/2508.01031) | 概念 CAD 生成 |
| 2025 | [From Idea to CAD: A Language Model-Driven Multi-Agent System for Collaborative Design](https://arxiv.org/abs/2503.04417) | 协同 CAD 设计 |
| 2024 | [CAD-Assistant: Tool-Augmented VLLMs as Generic CAD Task Solvers](https://arxiv.org/abs/2412.13810) | 通用 CAD 任务助手 |

### 论文

| 年份 | 会议/期刊 | 论文 | 工程流程 |
|:---:|:---:|:---|:---|
| 2026 | arXiv | [Developing Large Language Model for BIM-based Design with Domain Knowledge](https://arxiv.org/abs/2602.20812) | BIM 设计助手 |
| 2025 | arXiv | [Optimize Any Topology: A Foundation Model for Shape- and Resolution-Agnostic Topology Optimization](https://arxiv.org/abs/2510.23667) | 拓扑优化基础模型 |
| 2025 | arXiv | [Generative Topology Optimization: Exploring Diverse Solutions in Engineering Design](https://arxiv.org/abs/2502.13174) | 多样化生成式设计 |
| 2025 | NeurIPS | [GeoCAD: Local Geometry-Controllable CAD Generation with Large Language Models](https://arxiv.org/abs/2505.21877) | 参数化 CAD 生成 |
| 2024 | arXiv | [Structural Design Through Reinforcement Learning](https://arxiv.org/abs/2407.07288) | 结构构件与布局设计 |
| 2024 | arXiv | [Multi-scale Topology Optimization using Neural Networks](https://arxiv.org/abs/2404.08708) | 多尺度拓扑优化 |
| 2024 | arXiv | [A Dual Physics-Informed Neural Network for Topology Optimization](https://arxiv.org/abs/2410.14342) | 物理约束拓扑优化 |
| 2024 | arXiv | [NITO: Neural Implicit Fields for Resolution-free Topology Optimization](https://arxiv.org/abs/2402.05073) | 分辨率无关拓扑优化 |
| 2023 | FEAD | [A Finite-Element-Informed Neural Network for Parametric Simulation in Structural Mechanics](https://doi.org/10.1016/j.finel.2022.103904) | 载荷与响应代理模型 |
| 2023 | NeurIPS Workshop | [TopologyGAN: Topology Optimization Using Generative Adversarial Networks](https://arxiv.org/abs/2003.04685) | 生成式拓扑优化 |
| 2022 | SMO | [Deep Learning Accelerated Topology Optimization with Inherent Control of Image Quality](https://doi.org/10.1007/s00158-022-03433-4) | 快速拓扑生成 |
| 2022 | SMO | [Accelerated Topology Optimization Design of 3D Structures Based on Deep Learning](https://doi.org/10.1007/s00158-022-03194-0) | 三维结构设计 |
| 2021 | Nature Machine Intelligence | [Learning Nonlinear Operators via DeepONet](https://doi.org/10.1038/s42256-021-00302-5) | 仿真代理与算子学习 |

### 开源项目

| 项目 | 工程用途 | 许可证 |
|:---|:---|:---:|
| [DeepXDE](https://github.com/lululxvi/deepxde) | PDE 与力学问题的 PINN 和算子学习 | LGPL-2.1 |
| [DiffFE-Physics-Lab](https://github.com/danieleschmidt/DiffFE-Physics-Lab) | 集成机器学习的可微分有限元 | MIT |
| [FEINN](https://github.com/ThangLe-duc/FEINN) | 桁架、梁和板响应的有限元信息神经网络 | Apache-2.0 |
| [IF-TONIR](https://github.com/jbHu67/IF-TONIR) | 基于隐式神经表示的免迭代拓扑优化 | GPL-2.0 |
| [NeuralOperator](https://github.com/neuraloperator/neuraloperator) | 快速场分布和结构响应预测 | MIT |
| [NVIDIA Warp](https://github.com/NVIDIA/warp) | 面向力学的可微分 GPU 仿真与优化 | Apache-2.0 |
| [PhysicsNeMo](https://github.com/NVIDIA/physicsnemo) | 结构力学与 CFD 的物理信息代理模型 | Apache-2.0 |
| [Text2BIM](https://github.com/dcy0577/Text2BIM) | 文本生成 BIM 与建筑设计原型 | MIT |
| [TopOpt.jl](https://github.com/JuliaTopOpt/TopOpt.jl) | 可微分拓扑优化组件 | MIT |

> 壁厚检查、载荷路径验证、公差审查和图纸审批仍是快速发展的工业应用方向。
> 欢迎贡献带有可复现论文、数据集、插件或基准的相关工作。

## FPGA 工程

本节覆盖 RTL 生成、仿真、断言检查、HLS、量化、综合、布局布线、时序预测，
以及面向比特流交付的智能体工作流。

### RTL、验证与 HLS 论文

| 年份 | 会议/期刊 | 论文 | 工程流程 |
|:---:|:---:|:---|:---|
| 2026 | ASP-DAC | [LLM-Assisted Circuit Verification: A Comprehensive Survey](https://www.cse.cuhk.edu.hk/~byu/papers/C312-ASPDAC2026-Verif-slides.pdf) | 电路验证综述 |
| 2025 | arXiv | [REvolution: An Evolutionary Framework for RTL Generation](https://arxiv.org/abs/2510.21407) | 迭代式 RTL 生成 |
| 2025 | TODAES | [High-level Synthesis Directives Design Optimization via Large Language Model](https://doi.org/10.1145/3747291) | HLS 指令优化 |
| 2025 | ASP-DAC | [LLSM: LLM-enhanced Logic Synthesis Model](https://doi.org/10.1145/3658617.3697618) | 逻辑综合 |
| 2025 | ASP-DAC | [AssertLLM: Generating Hardware Verification Assertions from Design Specifications](https://doi.org/10.1145/3658617.3697756) | 验证断言生成 |
| 2025 | arXiv | [OpenLLM-RTL: Open Dataset and Benchmark for LLM-Aided Design RTL Generation](https://arxiv.org/abs/2503.15112) | RTL 生成基准 |
| 2025 | ACM | [ResBench: A Resource-Aware Benchmark for LLM-Generated FPGA Designs](https://doi.org/10.1145/3728179.3728192) | FPGA 资源感知基准 |
| 2024 | TCAD | [RTLCoder: Fully Open-Source and Efficient LLM-Assisted RTL Code Generation](https://zhiyaoxie.github.io/files/TCAD25_RTLCoder.pdf) | RTL 生成 |
| 2024 | ICCAD | [OpenLLM-RTL: Open Dataset and Benchmark for LLM-Aided Design RTL Generation](https://zhiyaoxie.com/files/ICCAD24_OpenLLM.pdf) | RTL 生成评测 |
| 2024 | ASP-DAC | [RTLLM: An Open-Source Benchmark for Design RTL Generation with Large Language Models](https://www.aspdac.com/aspdac2024/archive/pdf/7C-1.pdf) | RTL 生成基准 |
| 2024 | TODAES | [Survey of Machine Learning for Software-Assisted Hardware Design Verification](https://doi.org/10.1145/3661308) | 硬件设计验证综述 |
| 2024 | arXiv | [Revisiting VerilogEval: Newer LLMs, In-Context Learning, and Specification-to-RTL Tasks](https://arxiv.org/abs/2408.11053) | 规格到 RTL 评测 |
| 2023 | ICCAD | [VerilogEval: Evaluating Large Language Models for Verilog Code Generation](https://arxiv.org/abs/2309.07544) | Verilog 生成基准 |
| 2023 | ICCAD | [Robust GNN-based Representation Learning for HLS](https://ieeexplore.ieee.org/abstract/document/10323853) | HLS 性能预测 |
| 2022 | DAC | [High-Level Synthesis Performance Prediction Using GNNs](https://doi.org/10.1145/3489517.3530408) | 综合质量预测 |
| 2021 | JMLR | [hls4ml: An Open-Source Codesign Workflow for Low-Power ML Devices](https://arxiv.org/abs/2103.05579) | 机器学习模型到 HLS |
| 2020 | FPL | [LogicNets: Co-Designed Neural Networks and Circuits for Extreme-Throughput Applications](https://arxiv.org/abs/2004.03021) | 基于 LUT 的神经网络推理 |

### FPGA 与 RTL 智能体论文

| 年份 | 论文 | 工程流程 |
|:---:|:---|:---|
| 2026 | [HLSmith: An Expert-Guided Agentic Framework for C/C++-to-HLS Translation](https://arxiv.org/abs/2608.06791) | C/C++ 到 HLS 翻译 |
| 2026 | [VPR-Evolve: Multi-Agent-Driven Algorithm Evolution for FPGA Place and Route](https://arxiv.org/abs/2607.24998) | FPGA 布局布线优化 |
| 2026 | [CHIA: An Open-Source Framework for Principled, Agentic AI-Driven Hardware/Software Co-design Research](https://arxiv.org/abs/2606.27350) | 软硬件协同设计智能体 |
| 2026 | [HSCO-Bench: An Agent-Driven End-to-End Hardware-Software Co-design Benchmark for Systems-on-Chip](https://arxiv.org/abs/2605.19399) | SoC 协同设计基准 |
| 2026 | [Design Conductor 2.0: An Agent Builds a TurboQuant Inference Accelerator in 80 Hours](https://arxiv.org/abs/2605.05170) | 加速器设计智能体 |
| 2026 | [ChipCraftBrain: Validation-First RTL Generation via Multi-Agent Orchestration](https://arxiv.org/abs/2604.19856) | 多智能体 RTL 生成 |
| 2026 | [Dr. RTL: Autonomous Agentic RTL Optimization through Tool-Grounded Self-Improvement](https://arxiv.org/abs/2604.14989) | RTL 优化智能体 |
| 2026 | [VeriAgent: A Tool-Integrated Multi-Agent System with Evolving Memory for PPA-Aware RTL Code Generation](https://arxiv.org/abs/2603.17613) | PPA 感知 RTL 生成 |
| 2026 | [LAAFD: LLM-based Agents for Accelerated FPGA Design](https://arxiv.org/abs/2602.06085) | FPGA 设计自动化 |
| 2025 | [A2H-MAS: An Algorithm-to-HLS Multi-Agent System for Automated and Reliable FPGA Implementation](https://arxiv.org/abs/2508.10904) | 算法到 HLS 实现 |
| 2025 | [TimelyHLS: LLM-Based Timing-Aware and Architecture-Specific FPGA HLS Optimization](https://arxiv.org/abs/2507.17962) | 时序感知 HLS 优化 |

### 开源项目

| 项目 | 工程用途 | 许可证 |
|:---|:---|:---:|
| [Brevitas](https://github.com/Xilinx/brevitas) | 面向 FPGA 部署的量化感知训练 | BSD-3-Clause |
| [CIRCT](https://github.com/llvm/circt) | 基于 MLIR 的 RTL 与硬件编译基础设施 | Apache-2.0 WITH LLVM exception |
| [FINN](https://github.com/Xilinx/finn) | 量化神经网络的数据流编译 | BSD-3-Clause |
| [F4PGA](https://github.com/f4pga/f4pga) | 开源 FPGA 综合与布局布线流程 | Apache-2.0 |
| [FPGA-Agent-skills](https://github.com/adeleempurpled290/FPGA-Agent-skills) | HLS、仿真、综合、时序与调试工作流 | GPL-2.0 |
| [hls4ml](https://github.com/fastmachinelearning/hls4ml) | 将训练好的模型转换为 HLS 实现 | Apache-2.0 |
| [nextpnr](https://github.com/YosysHQ/nextpnr) | 开源流程中的 FPGA 布局布线后端 | ISC |
| [SiliconCompiler](https://github.com/siliconcompiler/siliconcompiler) | 可移植的综合、仿真与 FPGA APR 编排 | Apache-2.0 |
| [TAPA](https://github.com/tuna/tapa) | 任务并行 HLS 到 RTL，以及软件/RTL 协同仿真 | MIT |
| [Verilator](https://github.com/verilator/verilator) | 生成 RTL 的高速 SystemVerilog 仿真与检查 | LGPL-3.0 |
| [VerilogEval](https://github.com/NVlabs/verilog-eval) | 可复现的大模型 Verilog 生成评测框架 | MIT |
| [Vitis AI](https://github.com/Xilinx/Vitis-AI) | AMD 器件上的量化、编译、运行时与部署 | Apache-2.0 |
| [Yosys](https://github.com/YosysHQ/yosys) | 开源 FPGA 流程的 RTL 综合与形式验证工具 | ISC |

### 未明确声明许可证的研究代码

- [RTLCoder](https://github.com/hkust-zhiyao/RTL-Coder)：RTLCoder 和
  OpenLLM-RTL 论文的官方代码与数据集，仓库当前未声明许可证。

## 贡献

提交 PR 前请阅读[中文贡献指南](CONTRIBUTING_CN.md)，也可查看
[英文版本](CONTRIBUTING.md)。

1. 论文仅收录 2020 年及以后发表的工作；项目应在 2020 年以后仍有实质维护。
2. 每个条目只归入一个主要岗位和一个明确的工作流。
3. 优先使用官方论文集、DOI、arXiv 和项目主仓库链接。
4. 只有明确提供许可证的仓库才能进入开源项目表，否则放入研究代码说明。
5. 论文按年份降序排列，项目在每张表中按名称排序。
6. 描述应明确指出生成、分析、检查或优化的工程对象，例如 RTL、PCB 布线、
   应力场或镜头参数。

## 许可证

本清单采用 [MIT License](LICENSE)。链接指向的论文、代码、数据集、模型和厂商
工具仍采用各自的许可证。
