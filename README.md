# Awesome AI Engineering Agents

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![Updated](https://img.shields.io/badge/updated-2026--08-blue)
![License](https://img.shields.io/github/license/whut09/Awesome-AI-Engineering-Agents)

A focused collection of **2020+** papers and open-source projects that apply AI
to engineering work. The four tracks are optical engineering, electronics and
hardware design, structural/CAD engineering, and FPGA implementation.

本项目只保留 2020 年以后发表的论文，以及在 2020 年以后仍有实质维护或新版本的工程项目。
条目按实际工作流组织：设计、仿真、分析、审查、生成、综合与布线。基础工具只有在当前
AI 工程流程中仍然必要时保留，并在表格中注明用途和许可证。

> [!NOTE]
> An open-source project must publish an explicit license. Paper code or
> datasets without a declared license are listed separately and are not called
> open source. Always check bundled models, datasets, and vendor EULAs.

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

### Open-Source Projects

| Project | Engineering use | License |
|:---|:---|:---:|
| [DeepLens](https://github.com/singer-yang/DeepLens) | Differentiable geometric optics and automatic lens design | Apache-2.0 |
| [DeepTrack 2.0](https://github.com/softmatterlab/DeepTrack2) | Microscopy, particle tracking, and optical characterization | MIT |
| [diffractsim](https://github.com/rafael-fuente/diffractsim) | Differentiable diffraction simulation | MPL-2.0 |
| [Dolphindes](https://github.com/physical-design-bounds/dolphindes) | Bounds and optimization for photonic inverse design | MIT |
| [MAPS](https://github.com/ScopeX-ASU/MAPS) | Multi-fidelity AI photonic simulation and inverse design | MIT |
| [pinn-shaper](https://github.com/rafael-fuente/pinn-shaper) | PINN-based flat-optics beam shaping | MPL-2.0 |
| [TorchOptics](https://github.com/matthewfilipovich/torchoptics) | PyTorch Fourier-optics simulation and optimization | MIT |
| [waveprop](https://github.com/ebezzam/waveprop) | Free-space propagation and holography models | MIT |

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

### Open-Source Projects

| Project | Engineering use | License |
|:---|:---|:---:|
| [ALIGN](https://github.com/ALIGN-analoglayout/ALIGN-public) | Analog schematic-to-layout automation | BSD-3-Clause |
| [DeepPCB KiCad plugin](https://github.com/instadeepai/deeppcb-kicad-plugin) | AI-assisted PCB layout workflows in KiCad | Apache-2.0 |
| [DREAMPlace](https://github.com/limbo018/DREAMPlace) | GPU-accelerated placement optimization | BSD-3-Clause |
| [KiCad](https://github.com/KiCad/kicad-source-mirror) | Schematic capture, PCB layout, DRC, and 3D inspection foundation | GPL-3.0 |
| [KiCad Copilot](https://github.com/biosshot/kicad-copilot) | LLM assistant for KiCad projects | MIT |
| [MAGICAL](https://github.com/magical-eda/MAGICAL) | Machine-learning-assisted analog layout | BSD-3-Clause |
| [OpenLane](https://github.com/The-OpenROAD-Project/OpenLane) | Automated RTL-to-GDS design flow | Apache-2.0 |
| [OpenROAD](https://github.com/The-OpenROAD-Project/OpenROAD) | Placement, routing, timing, and physical-design automation | BSD-3-Clause |
| [PCBFlow](https://github.com/NijoP/pcbflow) | Programmatic PCB generation and layout | MIT |
| [SchGen](https://github.com/microsoft/SchGen) | Semantic-grounded-code PCB schematic generation | MIT |

### Datasets and Code with Unclear Licensing

- [CircuitNet](https://circuitnet.github.io/) — EDA datasets for
  congestion, timing, power, and IR-drop prediction. The repository does not
  currently expose a standard software license; verify terms before reuse.
- [PCBSchemaGen](https://github.com/Sthyao/PCBSchemaGen) — research code for the
  2026 schematic-generation paper; no explicit repository license was found.

## Structural and CAD Engineering

The structural track includes generative CAD, topology and thickness-aware
design, load/stress prediction, finite-element surrogates, physics-informed
simulation, and drawing/BIM review.

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

### Research Code without an Explicit License

- [RTLCoder](https://github.com/hkust-zhiyao/RTL-Coder) — official code and
  datasets for the RTLCoder/OpenLLM-RTL papers; no repository license is
  currently declared.

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

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
