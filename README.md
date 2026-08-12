# Awesome AI Engineering Agents

[English](README.md) | [简体中文](README_CN.md)

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![Updated](https://img.shields.io/badge/updated-2026--08-blue)
![License](https://img.shields.io/github/license/whut09/Awesome-AI-Engineering-Agents)

## Why This List

Foundation models have already made rapid progress in text generation, image
and video creation, and software development. General-purpose coding agents
and work assistants such as **Codex**, **OpenHands**, and **WorkBuddy** can now
complete or substantially accelerate many workflows in these areas. Their
impact is highly visible in software and digital-content jobs, but adoption is
less uniform in engineering roles that depend on domain physics, specialized
EDA/CAD tools, proprietary data, formal verification, manufacturing
constraints, and responsibility for physical products.

This repository looks at that gap from the perspective of an intelligent
hardware company. It focuses on four roles where foundation models and agents
are still moving from research prototypes into practical workflows:
**optical engineering**, **electronics and hardware design**, **structural and
CAD engineering**, and **FPGA engineering**. The list covers work such as lens
design, optical simulation, schematic generation, PCB placement and routing,
drawing review, structural and stress analysis, topology and wall-thickness
optimization, RTL generation, verification, HLS, synthesis, timing closure,
and FPGA place-and-route.

Our goal is not only to collect resources, but also to track how AI penetrates
these engineering positions over time: which tasks have reliable agents and
open implementations, which remain research problems, and where human
engineering judgment is still essential. The collection therefore prioritizes
**2020+** papers and actively maintained open-source projects, organized by
concrete engineering workflow rather than by model family.

> [!NOTE]
> An open-source project must publish an explicit license. Paper code or
> datasets without a declared license are listed separately and are not called
> open source. Always check bundled models, datasets, and vendor EULAs.

> [!IMPORTANT]
> This is an engineering-agent stack, not an AI-model-only list. Deterministic
> CAD/EDA tools, optical simulators, solvers, linters, formal engines,
> synthesizers, and place-and-route systems are in scope whenever an agent can
> invoke them to create, analyze, simulate, verify, optimize, or deliver an
> engineering artifact. Native AI/agent projects and conventional toolchain
> components are listed separately so their roles remain clear.

Canonical upstream repositories are preferred over forks and mirrors. A fork
is listed separately only when it contains material, maintained changes that
are relevant to engineering agents.

## Contents

- [Optical Engineering](#optical-engineering)
- [Hardware and PCB Design](#hardware-and-pcb-design)
- [Structural and CAD Engineering](#structural-and-cad-engineering)
- [FPGA Engineering](#fpga-engineering)
- [Contributing](#contributing)
- [License](#license)

## Optical Engineering

### Design, Simulation, and Inverse Design Papers

| Year | Venue | Paper | Workflow |
|:---:|:---:|:---|:---|
| 2026 | arXiv | [OptiAgent: A Physics-Driven Agentic Framework for Automated Optical Design](https://arxiv.org/abs/2602.23761) | Agentic optical design |
| 2025 | DATE | [MAPS: Multi-Fidelity AI-Augmented Photonic Simulation and Inverse Design Infrastructure](https://arxiv.org/abs/2503.01046) | Photonic simulation and inverse design |
| 2024 | Advanced Engineering Informatics | [Artificial intelligence in optical lens design](https://doi.org/10.1007/s10462-024-10842-y) | Lens-design survey |
| 2024 | arXiv | [TorchOptics: An open-source Python library for differentiable Fourier optics](https://arxiv.org/abs/2411.18591) | Differentiable wave optics |
| 2024 | Nature Communications | [Curriculum learning for ab initio deep learned refractive optics](https://doi.org/10.1038/s41467-024-50835-7) | Automatic lens design |
| 2023 | ASPLOS | [LightRidge: An End-to-end Agile Design Framework for Diffractive Optical Neural Networks](https://doi.org/10.1145/3623278.3624757) | Diffractive optical neural networks |
| 2020 | TOG | [Neural Holography with Camera-in-the-loop Training](https://doi.org/10.1145/3414685.3417802) | Hologram generation and calibration |
| 2020 | CVPR | [Deep Optics for Single-Shot High-Dynamic-Range Imaging](https://doi.org/10.1109/CVPR42600.2020.00145) | Learned optical coding |

### Agentic Optical Design Papers

| Year | Paper | Workflow |
|:---:|:---|:---|
| 2026 | [OptiAgent: End-to-End Optimization Modeling via Multi-Agent Iterative Refinement](https://arxiv.org/abs/2607.05346) | Multi-agent optimization modeling |
| 2026 | [OPTIAGENT: A Physics-Driven Agentic Framework for Automated Optical Design](https://arxiv.org/abs/2602.23761) | Physics-validated optical design agent |

### Open-Source Projects

| Project | Engineering use | License |
|:---|:---|:---:|
| [DeepLens](https://github.com/vccimaging/DeepLens) | Differentiable geometric optics and automatic lens design | Apache-2.0 |
| [DeepTrack 2.0](https://github.com/softmatterlab/DeepTrack2) | Microscopy, particle tracking, and optical characterization | MIT |
| [diffractsim](https://github.com/rafael-fuente/diffractsim) | Differentiable diffraction simulation | MPL-2.0 |
| [Dolphindes](https://github.com/physical-design-bounds/dolphindes) | Bounds and optimization for photonic inverse design | MIT |
| [MAPS](https://github.com/ScopeX-ASU/MAPS) | Multi-fidelity AI photonic simulation and inverse design | MIT |
| [pinn-shaper](https://github.com/rafael-fuente/pinn-shaper) | PINN-based flat-optics beam shaping | MPL-2.0 |
| [TorchOptics](https://github.com/matthewfilipovich/torchoptics) | PyTorch Fourier-optics simulation and optimization | MIT |
| [waveprop](https://github.com/ebezzam/waveprop) | Free-space propagation and holography models | MIT |

### Agent Toolchain Components

These libraries provide deterministic simulation, propagation, ray-tracing,
and analysis capabilities that an optical agent can call and validate against.

| Project | Agent role | Interface | License |
|:---|:---|:---:|:---:|
| [HCIPy](https://github.com/ehpor/hcipy) | Optical propagation and high-contrast imaging simulation | Python | MIT |
| [POPPY](https://github.com/spacetelescope/poppy) | Physical-optics propagation and point-spread-function analysis | Python | BSD-3-Clause |
| [prysm](https://github.com/brandondube/prysm) | Physical optics, phase retrieval, aberration analysis, and ray tracing | Python | MIT |
| [ray-optics](https://github.com/ricktu288/ray-optics) | Scriptable geometric-optics scene construction and ray simulation | Web / JavaScript | Apache-2.0 |

## Hardware and PCB Design

This track covers IC/SoC physical design, analog layout, PCB schematic and
routing, design-rule checking, thermal analysis, and drawing review. FPGA RTL
generation and implementation are in [FPGA Engineering](#fpga-engineering).

### Schematic, PCB, and CAD Generation Papers

| Year | Venue | Paper | Workflow |
|:---:|:---:|:---|:---|
| 2026 | arXiv | [SchGen: PCB Schematic Generation with Semantic-Grounded Code Representations](https://arxiv.org/abs/2605.30345) | Schematic generation |
| 2026 | arXiv | [PCBSchemaGen: Constraint-Guided Schematic Design via LLM](https://arxiv.org/abs/2602.00510) | Constraint-guided schematic design |
| 2026 | ICLR | [PCB-Bench: Benchmarking LLMs for Printed Circuit Board Placement and Routing](https://jdzhu19.github.io/publication/conference_2026iclr_li/conference_2026ICLR_Li.pdf) | PCB placement and routing benchmark |
| 2024 | IEEE | [AI-Optimized Placement and Routing for PCB Design](https://ieeexplore.ieee.org/document/10568665) | PCB placement and routing |
| 2024 | arXiv | [LLM4EDA: Emerging Progress in Large Language Models for Electronic Design Automation](https://arxiv.org/abs/2401.12224) | EDA survey |
| 2024 | arXiv | [CadVLM: Bridging Language and Vision in the Generation of Parametric CAD](https://arxiv.org/abs/2409.17457) | Drawing and CAD understanding |
| 2023 | TCAD | [TRouter: Thermal-driven PCB Routing via Non-Local Crisscross Attention Networks](https://ieeexplore.ieee.org/abstract/document/10042057) | Thermal-aware routing |
| 2023 | ASP-DAC | [DPRoute: Deep Learning Framework for Package Routing](https://doi.org/10.1145/3566097.3567902) | Package and board routing |
| 2023 | NeurIPS Workshop | [CAD-LLM: Large Language Model for CAD Generation](https://neurips.cc/virtual/2023/75064) | Text-to-CAD |
| 2022 | DAC | [Automated Accelerator Optimization Aided by Graph Neural Networks](https://doi.org/10.1145/3489517.3530409) | Hardware design-space exploration |
| 2022 | ML4CAD | [A Thermal Machine Learning Solver for Chip Simulation](https://doi.org/10.1145/3551901.3556484) | Thermal simulation |
| 2021 | NeurIPS | [On Joint Learning for Solving Placement and Routing in Chip Design](https://proceedings.neurips.cc/paper/2021/file/898aef0932f6aaecda27aba8e9903991-Paper.pdf) | Joint placement and routing |
| 2021 | DAC | [AutoSVA: Democratizing Formal Verification of RTL Module Interactions](https://doi.org/10.1109/DAC18074.2021.9586118) | Design review and formal checks |
| 2020 | ICCAD | [A Customized Graph Neural Network Model for Guiding Analog IC Placement](https://doi.org/10.1145/3400302.3415624) | Analog placement |

### Agentic EDA and Hardware Papers

| Year | Paper | Workflow |
|:---:|:---|:---|
| 2026 | [ZhuLong: Execution-Grounded LLM Agent for EDA Scripting with Offline API Self-Exploration](https://arxiv.org/abs/2608.07925) | EDA scripting agent |
| 2026 | [EDATracer: An Agentic Framework for Large-Scale EDA Artifact Analysis](https://arxiv.org/abs/2608.04032) | EDA artifact review |
| 2026 | [Can AI Agents Really Complete RTL-to-GDS? Lessons from Benchmarking Tool-Interactive EDA Workflows](https://arxiv.org/abs/2607.17528) | End-to-end RTL-to-GDS agents |
| 2026 | [SABLE: An NDA-Safe Closed-Loop LLM Framework for Analog Circuit Optimization in Industrial EDA Flows](https://arxiv.org/abs/2607.03701) | Analog circuit optimization |
| 2025 | [AutoEDA: Enabling EDA Flow Automation through Microservice-Based LLM Agents](https://arxiv.org/abs/2508.01012) | EDA flow orchestration |
| 2025 | [JARVIS: A Multi-Agent Code Assistant for High-Quality EDA Script Generation](https://arxiv.org/abs/2505.14978) | EDA script generation |
| 2024 | [Agentic-HLS: An Agentic Reasoning Based High-Level Synthesis System Using Large Language Models](https://arxiv.org/abs/2412.01604) | HLS code and directive generation |
| 2024 | [EDA-Aware RTL Generation with Large Language Models](https://arxiv.org/abs/2412.04485) | RTL generation with synthesis feedback |
| 2024 | [Automatically Improving LLM-based Verilog Generation using EDA Tool Feedback](https://arxiv.org/abs/2411.11856) | Tool-grounded Verilog repair |
| 2024 | [IICPilot: An Intelligent Integrated Circuit Backend Design Framework Using Open EDA](https://arxiv.org/abs/2407.12576) | Backend design automation |
| 2024 | [Ask-EDA: A Design Assistant Empowered by LLM, Hybrid RAG and Abbreviation De-hallucination](https://arxiv.org/abs/2406.06575) | EDA design assistant |
| 2023 | [ChatEDA: A Large Language Model Powered Autonomous Agent for EDA](https://arxiv.org/abs/2308.10204) | Autonomous EDA assistant |

### Open-Source Projects

| Project | Engineering use | License |
|:---|:---|:---:|
| [ALIGN](https://github.com/ALIGN-analoglayout/ALIGN-public) | Analog schematic-to-layout automation | BSD-3-Clause |
| [CircuitLM](https://github.com/Khandakar227/circuitlm) | Multi-agent natural-language-to-schematic generation | MIT |
| [DeepPCB KiCad plugin](https://github.com/instadeepai/deeppcb-kicad-plugin) | AI-assisted PCB layout workflows in KiCad | Apache-2.0 |
| [DREAMPlace](https://github.com/limbo018/DREAMPlace) | GPU-accelerated placement optimization | BSD-3-Clause |
| [KiCad](https://github.com/KiCad/kicad-source-mirror) | Schematic capture, PCB layout, DRC, and 3D inspection foundation | GPL-3.0 |
| [KiCad Copilot](https://github.com/biosshot/kicad-copilot) | LLM assistant for KiCad projects | MIT |
| [KiCad MCP](https://github.com/lamaalrajih/kicad-mcp) | Agent access to KiCad schematics, boards, footprints, and design checks | MIT |
| [MAGICAL](https://github.com/magical-eda/MAGICAL) | Machine-learning-assisted analog layout | BSD-3-Clause |
| [OpenLane](https://github.com/The-OpenROAD-Project/OpenLane) | Automated RTL-to-GDS design flow | Apache-2.0 |
| [OpenROAD](https://github.com/The-OpenROAD-Project/OpenROAD) | Placement, routing, timing, and physical-design automation | BSD-3-Clause |
| [PCBFlow](https://github.com/NijoP/pcbflow) | Programmatic PCB generation and layout | MIT |
| [SchGen](https://github.com/microsoft/SchGen) | Semantic-grounded-code PCB schematic generation | MIT |

### Agent Toolchain Components

| Project | Agent role | Interface | License |
|:---|:---|:---:|:---:|
| [eda-agent](https://github.com/salitronic/eda-agent) | Agent-controlled Altium, KiCad, and EasyEDA Pro schematic/PCB editing, review, audits, placement, and panelization | MCP / EDA APIs | Apache-2.0 |
| [freerouting](https://github.com/freerouting/freerouting) | PCB autorouting backend for DSN/SES-based board workflows | CLI / GUI | GPL-3.0 |
| [KLayout](https://github.com/KLayout/klayout) | Scriptable GDS/OASIS layout viewing, editing, DRC, and extraction | Python / Ruby / GUI | GPL-3.0 |
| [LibrePCB](https://github.com/LibrePCB/LibrePCB) | Schematic capture, PCB layout, library management, and manufacturing export | GUI / CLI | GPL-3.0 |
| [OpenSTA](https://github.com/The-OpenROAD-Project/OpenSTA) | Static timing analysis and timing-report feedback for chip-design agents | Tcl / CLI | GPL-3.0 |
| [SKiDL](https://github.com/devbisme/skidl) | Programmatic circuit and netlist generation with electrical-rule checks | Python | MIT |

### Datasets and Code with Unclear Licensing

- [CircuitNet](https://circuitnet.github.io/) — EDA datasets for
  congestion, timing, power, and IR-drop prediction. The repository does not
  currently expose a standard software license; verify terms before reuse.
- [PCBSchemaGen](https://github.com/Sthyao/PCBSchemaGen) — research code for the
  2026 schematic-generation paper; no explicit repository license was found.
- [Pro-CAD](https://github.com/BoYuanVisionary/Pro-CAD) — official code for
  proactive requirements clarification and text-to-CAD generation; no explicit
  repository license was found.

### New PCB Agent and Multimodal Benchmark Papers

| Year | Paper | Workflow |
|:---:|:---|:---|
| 2026 | [OmniRouting: A Semantic-Coupled Multimodal Benchmark for Constraint-Aware Spatial Reasoning in PCB Routing](https://arxiv.org/abs/2608.04434) | PCB routing reasoning |
| 2026 | [PCBWorld: A Benchmark Environment for Engine-Grounded PCB Design Automation](https://arxiv.org/abs/2607.05915) | Tool-interactive PCB agents |
| 2026 | [OmniLayout: A Schematic-Coupled Multimodal Benchmark for Constraint-Aware Geometric Reasoning in PCB Layout](https://arxiv.org/abs/2607.03261) | PCB layout reasoning |
| 2026 | [PCB-QA: Evaluating LLMs over the First Printed Circuit Board Design Question-Answer Dataset](https://arxiv.org/abs/2606.23704) | PCB design knowledge evaluation |
| 2026 | [OmniSch: A Multimodal PCB Schematic Benchmark for Structured Diagram Visual Reasoning](https://arxiv.org/abs/2604.00270) | Schematic review and reasoning |
| 2026 | [HWE-Bench: Can Language Models Perform Board-level Schematic Designs?](https://arxiv.org/abs/2603.18102) | Board-level schematic benchmark |
| 2026 | [CircuitLM: A Multi-Agent LLM-Aided Design Framework for Generating Circuit Schematics from Natural Language Prompts](https://arxiv.org/abs/2601.04505) | Multi-agent schematic generation |
| 2025 | [EEschematic: Multimodal-LLM Based AI Agent for Schematic Generation of Analog Circuit](https://arxiv.org/abs/2510.17002) | Analog schematic agent |
| 2024 | [Schemato: An LLM for Netlist-to-Schematic Conversion](https://arxiv.org/abs/2411.13899) | Netlist-to-schematic conversion |
| 2024 | [AmpAgent: An LLM-based Multi-Agent System for Multi-stage Amplifier Schematic Design](https://arxiv.org/abs/2409.14739) | Amplifier schematic design |

### Commercial EDA Signals

These proprietary systems are tracked as evidence of industry adoption, not as
open-source recommendations. Vendor claims should be validated independently.

| Product | Engineering workflow | Status |
|:---|:---|:---:|
| [Cadence AuraStack AI Super Agent](https://www.cadence.com/en_US/home/tools/pcb-design-and-analysis/aurastack-ai-super-agent.html) | PCB and advanced-package planning, constraints, implementation, DFM, and multiphysics orchestration | Announced |
| [Siemens Fuse EDA AI Agent](https://news.siemens.com/en-us/siemens-fuse-eda-ai-agent/) | Semiconductor, 3D-IC, and PCB design, verification, and sign-off workflows | Production |
| [Synopsys AgentEngineer](https://www.synopsys.com/ai/agentic-ai.html) | RTL, lint, testbench, and verification workflows | Production |

## Structural and CAD Engineering

The structural track includes generative CAD, topology and thickness-aware
design, load/stress prediction, finite-element surrogates, physics-informed
simulation, and drawing/BIM review.

### Agentic CAD and Structural Design Papers

| Year | Paper | Workflow |
|:---:|:---|:---|
| 2026 | [RA-CAD: Learning Post-Execution Critique for State-Aware Text-to-CAD Generation](https://arxiv.org/abs/2608.05714) | State-aware CAD repair |
| 2026 | [TraceCAD: Trace-Guided Repair for Agentic CAD Generation](https://arxiv.org/abs/2608.03062) | Execution-trace CAD repair |
| 2026 | [CADIR: A Cross-Backend Editable Intermediate Representation for Agentic CAD Generation](https://arxiv.org/abs/2608.00891) | Cross-CAD-backend generation |
| 2026 | [ArtisanCAD: An Industrial-Level CAD Agent with Expert-Grounded Knowledge Distillation](https://arxiv.org/abs/2607.05750) | Industrial CAD agent |
| 2026 | [ASSEMCAD: Production-Ready CAD Assembly Generation from Natural Language](https://arxiv.org/abs/2607.05123) | Assembly generation with mating constraints |
| 2026 | [AgentsCAD: Automated Design for Manufacturing of FDM Parts via Multi-Agent LLM Reasoning and Geometric Feature Recognition](https://arxiv.org/abs/2607.02448) | Design for additive manufacturing |
| 2026 | [Embodied CAD: Solver-Grounded LLM Agents for Parametric B-Rep Assembly Modeling](https://arxiv.org/abs/2606.31252) | Parametric assembly modeling |
| 2026 | [IterCAD: An Iterative Multimodal Agent for Visually-Grounded CAD Generation and Editing](https://arxiv.org/abs/2606.13368) | CAD generation and editing |
| 2026 | [Physics-in-the-Loop: A Hybrid Agentic Architecture for Validated CAD Engineering Design](https://arxiv.org/abs/2605.19717) | Physics-validated CAD design |
| 2026 | [Self-Improving CAD Generation Agents with Finite Element Analysis as Feedback](https://arxiv.org/abs/2605.17448) | FEA-in-the-loop CAD optimization |
| 2026 | [Zero-to-CAD: Agentic Synthesis of Interpretable CAD Programs at Million-Scale Without Real Data](https://arxiv.org/abs/2604.24479) | Large-scale CAD program synthesis |
| 2026 | [ArtiCAD: Articulated CAD Assembly Design via Multi-Agent Code Generation](https://arxiv.org/abs/2604.10992) | Articulated assembly design |
| 2026 | [TOOLCAD: Exploring Tool-Using Large Language Models in Text-to-CAD Generation with Reinforcement Learning](https://arxiv.org/abs/2604.07960) | Tool-using text-to-CAD agent |
| 2026 | [CADSmith: Multi-Agent CAD Generation with Programmatic Geometric Validation](https://arxiv.org/abs/2603.26512) | Geometry-validated CAD generation |
| 2026 | [Clarify Before You Draw: Proactive Agents for Robust Text-to-CAD Generation](https://arxiv.org/abs/2602.03045) | Interactive requirements clarification |
| 2025 | [CADDesigner: Conceptual CAD Model Generation with a General-Purpose Agent](https://arxiv.org/abs/2508.01031) | Conceptual CAD generation |
| 2025 | [cadrille: Multi-modal CAD Reconstruction with Reinforcement Learning](https://arxiv.org/abs/2505.22914) | CAD reconstruction from images, point clouds, and text |
| 2025 | [CAD-Llama: Leveraging Large Language Models for Computer-Aided Design Parametric 3D Model Generation](https://arxiv.org/abs/2505.04481) | Parametric CAD command generation |
| 2025 | [From Idea to CAD: A Language Model-Driven Multi-Agent System for Collaborative Design](https://arxiv.org/abs/2503.04417) | Collaborative CAD design |
| 2024 | [CAD-Assistant: Tool-Augmented VLLMs as Generic CAD Task Solvers](https://arxiv.org/abs/2412.13810) | General CAD task assistant |
| 2024 | [Text2CAD: Generating Sequential CAD Models from Beginner-to-Expert Level Text Prompts](https://arxiv.org/abs/2409.17106) | Text-to-parametric-CAD generation |

### Parametric CAD Generation and Reconstruction Papers

| Year | Paper | Workflow |
|:---:|:---|:---|
| 2026 | [CADENA: Stepwise CAD Reverse Engineering](https://arxiv.org/abs/2608.00799) | Stepwise mesh-to-parametric-CAD reconstruction |
| 2026 | [HierCAD: Hierarchical Text-to-CAD Design via Structure Alignment and Parameter Grounding](https://arxiv.org/abs/2607.11339) | Hierarchical text-to-CAD generation |
| 2026 | [SOV-CAD: Stepwise Orthographic Views Guided CAD Modeling Sequence Reconstruction](https://arxiv.org/abs/2607.04119) | Orthographic-view-to-CAD-sequence reconstruction |
| 2026 | [UniCAD: A Unified Benchmark and Universal Model for Multi-Modal Multi-Task CAD](https://arxiv.org/abs/2606.05058) | Multimodal CAD generation and understanding |
| 2026 | [CADFit: Precise Mesh-to-CAD Program Generation with Hybrid Optimization](https://arxiv.org/abs/2605.01171) | Editable CAD program recovery from meshes |
| 2026 | [CADReasoner: Iterative Program Editing for CAD Reverse Engineering](https://arxiv.org/abs/2603.29847) | Iterative CAD program reconstruction and repair |
| 2026 | [GIFT: Bootstrapping Image-to-CAD Program Synthesis via Geometric Feedback](https://arxiv.org/abs/2603.27448) | Geometry-grounded image-to-CAD synthesis |
| 2026 | [Towards High-Fidelity CAD Generation via LLM-Driven Program Generation and Text-Based B-Rep Primitive Grounding](https://arxiv.org/abs/2603.11831) | Text-to-CAD with B-Rep primitive grounding |
| 2026 | [DreamCAD: Scaling Multi-modal CAD Generation using Differentiable Parametric Surfaces](https://arxiv.org/abs/2603.05607) | Editable B-Rep generation from multimodal input |
| 2026 | [STEP-LLM: Generating CAD STEP Models from Natural Language with Large Language Models](https://arxiv.org/abs/2601.12641) | Natural-language-to-STEP generation |
| 2025 | [From Intent to Execution: Multimodal Chain-of-Thought Reinforcement Learning for Precise CAD Code Generation](https://arxiv.org/abs/2508.10118) | Precise multimodal CAD code generation |
| 2025 | [CAD-Coder: An Open-Source Vision-Language Model for Computer-Aided Design Code Generation](https://arxiv.org/abs/2505.14646) | Image-to-CAD code generation |
| 2025 | [Text-to-CadQuery: A New Paradigm for CAD Generation with Scalable Large Model Capabilities](https://arxiv.org/abs/2505.06507) | Text-to-CadQuery program generation |
| 2024 | [TransCAD: A Hierarchical Transformer for CAD Sequence Inference from Point Clouds](https://arxiv.org/abs/2407.12702) | Point-cloud-to-CAD-sequence reconstruction |
| 2021 | [DeepCAD: A Deep Generative Network for Computer-Aided Design Models](https://arxiv.org/abs/2105.09492) | CAD command-sequence generation baseline |

### Papers

| Year | Venue | Paper | Workflow |
|:---:|:---:|:---|:---|
| 2026 | arXiv | [Developing Large Language Model for BIM-based Design with Domain Knowledge](https://arxiv.org/abs/2602.20812) | BIM design assistant |
| 2025 | arXiv | [Optimize Any Topology: A Foundation Model for Shape- and Resolution-Agnostic Topology Optimization](https://arxiv.org/abs/2510.23667) | Foundation model for topology optimization |
| 2025 | arXiv | [Generative Topology Optimization: Exploring Diverse Solutions in Engineering Design](https://arxiv.org/abs/2502.13174) | Diverse generative design |
| 2025 | NeurIPS | [GeoCAD: Local Geometry-Controllable CAD Generation with Large Language Models](https://arxiv.org/abs/2505.21877) | Parametric CAD generation |
| 2024 | arXiv | [Structural Design Through Reinforcement Learning](https://arxiv.org/abs/2407.07288) | Structural member/layout design |
| 2024 | arXiv | [Multi-scale Topology Optimization using Neural Networks](https://arxiv.org/abs/2404.08708) | Multi-scale topology optimization |
| 2024 | arXiv | [A Dual Physics-Informed Neural Network for Topology Optimization](https://arxiv.org/abs/2410.14342) | Physics-constrained optimization |
| 2024 | arXiv | [NITO: Neural Implicit Fields for Resolution-free Topology Optimization](https://arxiv.org/abs/2402.05073) | Resolution-free topology |
| 2023 | FEAD | [A Finite-Element-Informed Neural Network for Parametric Simulation in Structural Mechanics](https://doi.org/10.1016/j.finel.2022.103904) | Load and response surrogate |
| 2023 | NeurIPS Workshop | [TopologyGAN: Topology Optimization Using Generative Adversarial Networks](https://arxiv.org/abs/2003.04685) | Generative topology optimization |
| 2022 | SMO | [Deep Learning Accelerated Topology Optimization with Inherent Control of Image Quality](https://doi.org/10.1007/s00158-022-03433-4) | Fast topology generation |
| 2022 | SMO | [Accelerated Topology Optimization Design of 3D Structures Based on Deep Learning](https://doi.org/10.1007/s00158-022-03194-0) | 3D structural design |
| 2021 | Nature Machine Intelligence | [Learning Nonlinear Operators via DeepONet](https://doi.org/10.1038/s42256-021-00302-5) | Simulation surrogate and operator learning |

### CAD Benchmarks and Reality Checks

| Year | Benchmark | What it tests |
|:---:|:---|:---|
| 2026 | [Text2CAD-Bench: A Benchmark for LLM-based Text-to-Parametric CAD Generation](https://arxiv.org/abs/2605.18430) | Text-to-CAD generation from simple parts to complex topology |
| 2026 | [MUSE: Benchmarking Manufacturable, Functional, and Assemblable Text-to-CAD Generation](https://arxiv.org/abs/2605.28579) | Manufacturability, functionality, and assemblability of generated B-Rep parts |
| 2026 | [CADBench: A Multimodal Benchmark for AI-Assisted CAD Program Generation](https://arxiv.org/abs/2605.10873) | CAD program generation across increasing geometric complexity |
| 2026 | [BenchCAD: A Comprehensive, Industry-Standard Benchmark for Programmatic CAD](https://arxiv.org/abs/2605.10865) | Executability and parametric structure of industrial-style CAD programs |
| 2026 | [Text-to-CAD Evaluation with CADTests](https://arxiv.org/abs/2605.07807) | Functional requirements tested directly on generated geometry |

Visual similarity is insufficient for engineering CAD. Evaluation should also
cover execution success, editable feature history, constraints, assemblies,
manufacturability, and behavior under downstream analysis.

### Agentic CAD Projects

| Project | Engineering use | License |
|:---|:---|:---:|
| [AgentSCAD](https://github.com/Kevoyuan/AgentSCAD) | Generates and repairs OpenSCAD models with geometry and manufacturability validation | MIT |
| [CADAM](https://github.com/Adam-CAD/CADAM) | Converts text or images into editable parametric OpenSCAD, STL, and DXF artifacts | GPL-3.0 |
| [CAD Skills](https://github.com/earthtojake/text-to-cad) | Agent skills for generating, inspecting, modifying, and validating CAD/CAE/CAM artifacts | MIT |
| [FreeCAD AI](https://github.com/ghbalf/freecad-ai) | Conversational FreeCAD workbench that generates native geometry through Python | LGPL-2.1 |

### Open-Source CAD Research Projects and Datasets

| Project | Engineering use | License |
|:---|:---|:---:|
| [CAD-Coder](https://github.com/anniedoris/CAD-Coder) | Vision-language model and training code for image-to-CAD code generation | Apache-2.0 |
| [CADENA](https://github.com/zhemdi/cadena) | Stepwise reverse engineering from meshes to parametric CAD programs | MIT |
| [DeepCAD](https://github.com/ChrisWu1997/DeepCAD) | CAD command-sequence generation baseline and dataset tooling | MIT |
| [HierCAD](https://github.com/Collab-Gen/HierCAD) | Hierarchical text-to-CAD generation with parameter grounding | MIT |
| [SketchGraphs](https://github.com/PrincetonLIPS/SketchGraphs) | Dataset of 15 million CAD sketches with geometric constraint graphs | MIT |

### CAD Research Code with Restricted or Unclear Licensing

- [CADFit](https://github.com/ghadinehme/CADFit) publishes research code under
  CC BY-NC 4.0, which restricts commercial use and is not treated here as an
  open-source software license.
- [FutureCAD](https://github.com/JohanStackk/FutureCAD),
  [SOV-CAD](https://github.com/LukePhong/SOV-CAD), and
  [Text-to-CadQuery](https://github.com/Text-to-CadQuery/Text-to-CadQuery)
  provide research code but currently expose no explicit repository license.

### Open-Source Projects

| Project | Engineering use | License |
|:---|:---|:---:|
| [DeepXDE](https://github.com/lululxvi/deepxde) | PINNs and operator learning for PDE and mechanics problems | LGPL-2.1 |
| [DiffFE-Physics-Lab](https://github.com/danieleschmidt/DiffFE-Physics-Lab) | Differentiable finite elements with ML integration | MIT |
| [FEINN](https://github.com/ThangLe-duc/FEINN) | Finite-element-informed neural networks for truss, beam, and plate response | Apache-2.0 |
| [IF-TONIR](https://github.com/jbHu67/IF-TONIR) | Implicit neural representations for iteration-free topology optimization | GPL-2.0 |
| [NeuralOperator](https://github.com/neuraloperator/neuraloperator) | Neural operators for fast field and response prediction | MIT |
| [NVIDIA Warp](https://github.com/NVIDIA/warp) | Differentiable GPU simulation and optimization for mechanics | Apache-2.0 |
| [PhysicsNeMo](https://github.com/NVIDIA/physicsnemo) | Physics-informed surrogate models for structural mechanics and CFD | Apache-2.0 |
| [Text2BIM](https://github.com/dcy0577/Text2BIM) | Text-to-BIM generation and building-design prototyping | MIT |
| [TopOpt.jl](https://github.com/JuliaTopOpt/TopOpt.jl) | Differentiable topology-optimization components | MIT |

### Additional AI/ML for Structural Simulation

| Project | Engineering use | License |
|:---|:---|:---:|
| [DL4TO](https://github.com/dl4to/dl4to) | Deep learning and differentiable physics for 3D topology optimization and linear elasticity | Apache-2.0 |
| [NeuralSolver](https://github.com/thuml/Neural-Solver-Library) | Benchmark library for neural PDE solvers on regular and general geometries | MIT |
| [PINNacle](https://github.com/i207M/PINNacle) | Reproducible benchmark for physics-informed neural PDE solvers | MIT |
| [The Well](https://github.com/PolymathicAI/the_well) | Large-scale physics-simulation datasets for surrogate and foundation models | BSD-3-Clause |

### CAE and Simulation Agent Papers

| Year | Paper | Workflow |
|:---:|:---|:---|
| 2025 | [Foam-Agent 2.0: An End-to-End Composable Multi-Agent Framework for Automating CFD Simulation in OpenFOAM](https://arxiv.org/abs/2509.18178) | Composable OpenFOAM workflow automation |
| 2025 | [CFDagent: A Language-Guided, Zero-Shot Multi-Agent System for Complex Flow Simulation](https://arxiv.org/abs/2507.23693) | Autonomous CFD case generation and execution |
| 2025 | [ChatCFD: An LLM-Driven Agent for End-to-End CFD Automation with Structured Knowledge and Reasoning](https://arxiv.org/abs/2506.02019) | End-to-end CFD workflow |
| 2025 | [OpenFOAMGPT: a RAG-Augmented LLM Agent for OpenFOAM-Based Computational Fluid Dynamics](https://arxiv.org/abs/2501.06327) | OpenFOAM knowledge and case assistance |
| 2024 | [MetaOpenFOAM: an LLM-based multi-agent framework for CFD](https://arxiv.org/abs/2407.21320) | Multi-agent OpenFOAM workflow |

### Open-Source CAE Agents

| Project | Engineering use | License |
|:---|:---|:---:|
| [AutoCFD](https://github.com/YYgroup/AutoCFD) | Converts natural-language requirements into executable OpenFOAM cases with iterative correction | GPL-3.0 |
| [MetaOpenFOAM](https://github.com/Terry-cyx/MetaOpenFOAM) | Multi-agent OpenFOAM planning, case generation, execution, and result analysis | GPL-3.0 |

### Agent-Ready CAE Infrastructure

These projects are not necessarily AI models themselves. They are included
because their Python, CLI, or MCP interfaces make them practical solver,
geometry, meshing, and post-processing backends for engineering agents.

| Project | Engineering use | Interface | License |
|:---|:---|:---:|:---:|
| [build123d](https://github.com/gumyr/build123d) | Scriptable parametric solid modeling for agent-generated CAD | Python | Apache-2.0 |
| [CadQuery](https://github.com/CadQuery/cadquery) | Parametric CAD generation and STEP/STL export | Python | Apache-2.0 |
| [DOLFINx](https://github.com/FEniCS/dolfinx) | Parallel finite-element analysis and PDE solving | Python / C++ | LGPL-3.0 |
| [freecad-mcp](https://github.com/neka-nat/freecad-mcp) | Agent-controlled FreeCAD modeling, inspection, Python, and FEM workflows | MCP / Python | MIT |
| [Netgen](https://github.com/NGSolve/netgen) | Automatic tetrahedral meshing from STEP, IGES, STL, and CSG | Python / CLI | LGPL-2.1 |
| [ParaView-MCP](https://github.com/llnl/paraview_mcp) | Agent-controlled simulation visualization and post-processing | MCP / Python | BSD-3-Clause |
| [SfePy](https://github.com/sfepy/sfepy) | Scriptable structural, thermal, and multiphysics FEM | Python | BSD-3-Clause |
| [sim-cli](https://github.com/svd-ai-lab/sim-cli) | Replayable agent runtime for COMSOL, Abaqus, and Ansys simulation workflows | CLI / plugins | Apache-2.0 |
| [viznoir](https://github.com/kimimgo/viznoir) | Headless MCP visualization for VTK, CGNS, and OpenFOAM results | MCP / Python | MIT |

### Additional CAD, Meshing, and Solver Components

| Project | Agent role | Interface | License |
|:---|:---|:---:|:---:|
| [CalculiX](https://github.com/Dhondtguido/CalculiX) | Linear/nonlinear structural, thermal, and dynamic finite-element analysis | CLI / files | GPL-2.0 |
| [FreeCAD](https://github.com/FreeCAD/FreeCAD) | Parametric solid modeling, drawing, assembly, and FEM automation | Python / GUI | LGPL-2.1 |
| [MFEM](https://github.com/MFEM/mfem) | Scalable finite-element backend for structural and multiphysics workflows | C++ / Python | BSD-3-Clause |
| [meshio](https://github.com/nschloe/meshio) | Conversion between common finite-element and mesh formats | Python / CLI | MIT |
| [OpenFOAM](https://github.com/OpenFOAM/OpenFOAM-dev) | CFD and multiphysics case generation, execution, and result production | CLI / files | GPL-3.0 |
| [OpenRadioss](https://github.com/OpenRadioss/OpenRadioss) | Explicit finite-element solver for impact, crash, drop, and dynamic-event analysis | CLI / files | AGPL-3.0 |
| [PyVista](https://github.com/pyvista/pyvista) | Mesh analysis, field inspection, and 3D simulation-result validation | Python | MIT |
| [trimesh](https://github.com/mikedh/trimesh) | Mesh loading, repair, measurements, collision, and geometric validation | Python | MIT |

The agent-callability perspective and several infrastructure candidates in this
section were cross-checked against
[awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae), which maintains a
broader ranked collection of open CAE, CAD, meshing, and visualization tools.

The AI-versus-foundation distinction, maturity-oriented curation, and several
CAD-agent, simulation-agent, benchmark, and industry-signal candidates were
also cross-checked against
[Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI).

The parametric-CAD generation, reconstruction, dataset, and evaluation entries
were additionally cross-checked against the bilingual
[Awesome AI4CAD Hub](https://jin-s13.github.io/awesome-AI4CAD-hub/), whose
broader automated index is useful for discovery. Entries here were verified
against their original papers and repositories because the hub also contains
duplicates, pre-2020 work, and incomplete metadata.

### Commercial Drawing Review and Engineering Knowledge Signals

These products are proprietary and are listed only to track adoption in tasks
for which reproducible open implementations remain scarce.

| Product | Engineering workflow | Status |
|:---|:---|:---:|
| [bananaz](https://www.bananaz.ai/) | CAD, drawing, BOM, change, standards, and DFX review | Production |
| [CoLab AutoReview](https://www.colabsoftware.com/) | Automated dimensions, tolerances, standards, BOM, and DFM review | Production |
| [DraftAid](https://draftaid.io/) | Generation of fabrication drawings from 3D CAD | Production |
| [Leo AI](https://www.getleo.ai/) | Retrieval and reasoning over PLM, PDM, CAD, and technical data | Production |

> Wall-thickness checks, load-path validation, tolerance review, and drawing
> approval are emerging industrial workflows. Contributions with a reproducible
> paper, dataset, plugin, or benchmark are especially useful here.

## FPGA Engineering

RTL generation, simulation, assertion checking, HLS, quantization, synthesis,
place-and-route, timing prediction, and bitstream-oriented agent workflows.

### RTL, Verification, and HLS Papers

| Year | Venue | Paper | Workflow |
|:---:|:---:|:---|:---|
| 2026 | ASP-DAC | [LLM-Assisted Circuit Verification: A Comprehensive Survey](https://www.cse.cuhk.edu.hk/~byu/papers/C312-ASPDAC2026-Verif-slides.pdf) | Verification survey |
| 2025 | arXiv | [REvolution: An Evolutionary Framework for RTL Generation](https://arxiv.org/abs/2510.21407) | Iterative RTL generation |
| 2025 | TODAES | [High-level Synthesis Directives Design Optimization via Large Language Model](https://doi.org/10.1145/3747291) | HLS directive optimization |
| 2025 | ASP-DAC | [LLSM: LLM-enhanced Logic Synthesis Model](https://doi.org/10.1145/3658617.3697618) | Logic synthesis |
| 2025 | ASP-DAC | [AssertLLM: Generating Hardware Verification Assertions from Design Specifications](https://doi.org/10.1145/3658617.3697756) | Assertion generation |
| 2025 | arXiv | [OpenLLM-RTL: Open Dataset and Benchmark for LLM-Aided Design RTL Generation](https://arxiv.org/abs/2503.15112) | RTL benchmark |
| 2025 | ACM | [ResBench: A Resource-Aware Benchmark for LLM-Generated FPGA Designs](https://doi.org/10.1145/3728179.3728192) | FPGA resource benchmark |
| 2024 | TCAD | [RTLCoder: Fully Open-Source and Efficient LLM-Assisted RTL Code Generation](https://zhiyaoxie.github.io/files/TCAD25_RTLCoder.pdf) | RTL generation |
| 2024 | ICCAD | [OpenLLM-RTL: Open Dataset and Benchmark for LLM-Aided Design RTL Generation](https://zhiyaoxie.com/files/ICCAD24_OpenLLM.pdf) | RTL evaluation |
| 2024 | ASP-DAC | [RTLLM: An Open-Source Benchmark for Design RTL Generation with Large Language Models](https://www.aspdac.com/aspdac2024/archive/pdf/7C-1.pdf) | RTL benchmark |
| 2024 | TODAES | [Survey of Machine Learning for Software-Assisted Hardware Design Verification](https://doi.org/10.1145/3661308) | Verification survey |
| 2024 | arXiv | [Revisiting VerilogEval: Newer LLMs, In-Context Learning, and Specification-to-RTL Tasks](https://arxiv.org/abs/2408.11053) | Spec-to-RTL evaluation |
| 2023 | ICCAD | [VerilogEval: Evaluating Large Language Models for Verilog Code Generation](https://arxiv.org/abs/2309.07544) | Verilog benchmark |
| 2023 | ICCAD | [Robust GNN-based Representation Learning for HLS](https://ieeexplore.ieee.org/abstract/document/10323853) | HLS prediction |
| 2022 | DAC | [High-Level Synthesis Performance Prediction Using GNNs](https://doi.org/10.1145/3489517.3530408) | QoR prediction |
| 2021 | JMLR | [hls4ml: An Open-Source Codesign Workflow for Low-Power ML Devices](https://arxiv.org/abs/2103.05579) | ML-to-HLS |
| 2020 | FPL | [LogicNets: Co-Designed Neural Networks and Circuits for Extreme-Throughput Applications](https://arxiv.org/abs/2004.03021) | LUT-based inference |

### New FPGA and RTL Agent Papers

| Year | Paper | Workflow |
|:---:|:---|:---|
| 2026 | [HLSmith: An Expert-Guided Agentic Framework for C/C++-to-HLS Translation](https://arxiv.org/abs/2608.06791) | C/C++ to HLS translation |
| 2026 | [VPR-Evolve: Multi-Agent-Driven Algorithm Evolution for FPGA Place and Route](https://arxiv.org/abs/2607.24998) | FPGA place-and-route optimization |
| 2026 | [CHIA: An Open-Source Framework for Principled, Agentic AI-Driven Hardware/Software Co-design Research](https://arxiv.org/abs/2606.27350) | Hardware/software co-design agents |
| 2026 | [HSCO-Bench: An Agent-Driven End-to-End Hardware-Software Co-design Benchmark for Systems-on-Chip](https://arxiv.org/abs/2605.19399) | SoC co-design benchmark |
| 2026 | [Design Conductor 2.0: An Agent Builds a TurboQuant Inference Accelerator in 80 Hours](https://arxiv.org/abs/2605.05170) | Accelerator design agent |
| 2026 | [ChipCraftBrain: Validation-First RTL Generation via Multi-Agent Orchestration](https://arxiv.org/abs/2604.19856) | Multi-agent RTL generation |
| 2026 | [Dr. RTL: Autonomous Agentic RTL Optimization through Tool-Grounded Self-Improvement](https://arxiv.org/abs/2604.14989) | RTL optimization agent |
| 2026 | [VeriAgent: A Tool-Integrated Multi-Agent System with Evolving Memory for PPA-Aware RTL Code Generation](https://arxiv.org/abs/2603.17613) | PPA-aware RTL generation |
| 2026 | [LAAFD: LLM-based Agents for Accelerated FPGA Design](https://arxiv.org/abs/2602.06085) | FPGA design automation |
| 2025 | [A2H-MAS: An Algorithm-to-HLS Multi-Agent System for Automated and Reliable FPGA Implementation](https://arxiv.org/abs/2508.10904) | Algorithm-to-HLS implementation |
| 2025 | [TimelyHLS: LLM-Based Timing-Aware and Architecture-Specific FPGA HLS Optimization](https://arxiv.org/abs/2507.17962) | Timing-aware HLS optimization |

### Open-Source Projects

| Project | Engineering use | License |
|:---|:---|:---:|
| [Brevitas](https://github.com/Xilinx/brevitas) | Quantization-aware training for FPGA deployment | BSD-3-Clause |
| [CIRCT](https://github.com/llvm/circt) | MLIR-based RTL and hardware compilation infrastructure | Apache-2.0 WITH LLVM exception |
| [FINN](https://github.com/Xilinx/finn) | Dataflow compilation for quantized neural networks | BSD-3-Clause |
| [F4PGA](https://github.com/f4pga/f4pga) | Open FPGA synthesis and place-and-route flows | Apache-2.0 |
| [FPGA-Agent-skills](https://github.com/adeleempurpled290/FPGA-Agent-skills) | Guided HLS, simulation, synthesis, timing, and debug skills | GPL-2.0 |
| [hls4ml](https://github.com/fastmachinelearning/hls4ml) | Converts trained models to HLS implementations | Apache-2.0 |
| [nextpnr](https://github.com/YosysHQ/nextpnr) | FPGA place-and-route backend used by open flows | ISC |
| [SiliconCompiler](https://github.com/siliconcompiler/siliconcompiler) | Portable synthesis, simulation, and FPGA APR orchestration | Apache-2.0 |
| [TAPA](https://github.com/tuna/tapa) | Task-parallel HLS to RTL and software/RTL co-simulation | MIT |
| [Verilator](https://github.com/verilator/verilator) | Fast SystemVerilog simulation and linting for generated RTL | LGPL-3.0 |
| [VerilogEval](https://github.com/NVlabs/verilog-eval) | Reproducible LLM-to-Verilog evaluation harness | MIT |
| [Vitis AI](https://github.com/Xilinx/Vitis-AI) | Quantization, compilation, runtime, and deployment on AMD devices | Apache-2.0 |
| [Yosys](https://github.com/YosysHQ/yosys) | RTL synthesis and formal tooling for open FPGA flows | ISC |

### Agent Toolchain Components

These tools can form the executable feedback loop for an FPGA agent, from RTL
parsing and lint through simulation, formal verification, synthesis, timing,
and architecture-aware placement and routing.

| Project | Agent role | Interface | License |
|:---|:---|:---:|:---:|
| [cocotb](https://github.com/cocotb/cocotb) | Python testbench generation, simulation control, and regression checking | Python / VPI | BSD-3-Clause |
| [GHDL](https://github.com/ghdl/ghdl) | VHDL analysis, elaboration, simulation, and synthesis integration | CLI | GPL-2.0 |
| [Icarus Verilog](https://github.com/steveicarus/iverilog) | Verilog/SystemVerilog compilation and simulation | CLI | GPL-2.0 |
| [OpenPARF](https://github.com/PKU-IDEA/OpenPARF) | Large-scale heterogeneous FPGA placement and routing with a deep-learning toolkit | Python / C++ | BSD-3-Clause |
| [Surelog](https://github.com/chipsalliance/Surelog) | SystemVerilog preprocessing, parsing, elaboration, UHDM, and AST access | CLI / C++ / Python | Apache-2.0 |
| [SymbiYosys](https://github.com/YosysHQ/sby) | Orchestration of Yosys-based bounded, unbounded, and cover formal checks | CLI | ISC |
| [Verible](https://github.com/chipsalliance/verible) | SystemVerilog parsing, linting, formatting, and language-server checks | CLI / LSP | Apache-2.0 |
| [VTR](https://github.com/verilog-to-routing/vtr-verilog-to-routing) | FPGA architecture exploration and Verilog-to-routing flow with VPR | CLI | Mixed, primarily MIT |

### Research Code without an Explicit License

- [RTLCoder](https://github.com/hkust-zhiyao/RTL-Coder) — official code and
  datasets for the RTLCoder/OpenLLM-RTL papers; no repository license is
  currently declared.

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md) ([简体中文](CONTRIBUTING_CN.md))
before opening a pull request.

1. Add only 2020+ papers, or projects with meaningful 2020+ maintenance.
2. Put each item in one primary role and one concrete workflow subsection.
3. Prefer official proceedings, DOI, arXiv, and canonical repositories.
4. List a project in the open-source table only when its repository exposes an
   explicit license; otherwise use the research-code note.
5. Keep papers newest first and projects alphabetically sorted within each table.
6. Include the engineering artifact being generated, analyzed, checked, or
   optimized (for example RTL, PCB routing, stress field, or lens parameters).

## License

This list is released under the [MIT License](LICENSE). Linked papers, code,
datasets, models, and vendor tools remain under their own licenses.
