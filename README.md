# Awesome AI Engineering Agents

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![Last Commit](https://img.shields.io/github/last-commit/whut09/Awesome-AI-Engineering-Agents)
![License](https://img.shields.io/github/license/whut09/Awesome-AI-Engineering-Agents)

A curated list of papers and open-source projects that apply artificial
intelligence to four engineering roles: **optical engineering**, **hardware
engineering**, **structural design**, and **FPGA engineering**.

本项目收集 AI 在光学、硬件、结构设计与 FPGA 四类工程岗位中的代表性论文和开源项目。
它关注能够参与建模、仿真、优化、生成设计、验证或部署的实际方法与工具，而不是泛化的
AI 新闻或产品列表。

> [!NOTE]
> A repository is listed as open source only when it publishes an explicit
> license. Always verify the current license and third-party asset terms before
> commercial use.

## Contents

- [Optical Engineering](#optical-engineering)
- [Hardware Engineering](#hardware-engineering)
- [Structural Design](#structural-design)
- [FPGA Engineering](#fpga-engineering)
- [Contributing](#contributing)
- [License](#license)

## Optical Engineering

AI-assisted lens and optical-system design, differentiable wave propagation,
computational imaging, holography, and photonic neural networks.

### Papers

| Year | Venue | Paper | Focus |
|:---:|:---:|:---|:---|
| 2024 | Nature Communications | [Curriculum learning for ab initio deep learned refractive optics](https://doi.org/10.1038/s41467-024-50835-7) | Automatic lens design |
| 2024 | arXiv | [TorchOptics: An open-source Python library for differentiable Fourier optics](https://arxiv.org/abs/2411.18591) | Differentiable optics |
| 2023 | ASPLOS | [LightRidge: An End-to-end Agile Design Framework for Diffractive Optical Neural Networks](https://doi.org/10.1145/3623278.3624757) | Diffractive optical neural networks |
| 2021 | Nature | [Parallel convolutional processing using an integrated photonic tensor core](https://doi.org/10.1038/s41586-020-03070-1) | Optical AI accelerator |
| 2020 | TOG | [Neural Holography with Camera-in-the-loop Training](https://doi.org/10.1145/3414685.3417802) | Learned hologram generation |
| 2020 | CVPR | [Deep Optics for Single-Shot High-Dynamic-Range Imaging](https://doi.org/10.1109/CVPR42600.2020.00145) | Learned optical coding |
| 2018 | Science | [All-optical machine learning using diffractive deep neural networks](https://doi.org/10.1126/science.aat8084) | Diffractive optical computing |
| 2018 | TOG | [End-to-end optimization of optics and image processing for achromatic extended depth of field and super-resolution imaging](https://doi.org/10.1145/3197517.3201333) | Joint optics and image processing |

### Open-Source Projects

| Project | What it provides | Stack | License |
|:---|:---|:---:|:---:|
| [DeepLens](https://github.com/singer-yang/DeepLens) | Differentiable geometric optics and automatic lens design | Python / PyTorch | Apache-2.0 |
| [DeepTrack 2.0](https://github.com/softmatterlab/DeepTrack2) | Deep learning for microscopy, particle tracking, and optical characterization | Python / TensorFlow | MIT |
| [diffractsim](https://github.com/rafael-fuente/diffractsim) | GPU-accelerated diffraction simulation with differentiable backends | Python / JAX | MPL-2.0 |
| [TorchOptics](https://github.com/matthewfilipovich/torchoptics) | Differentiable Fourier-optics simulation for PyTorch | Python / PyTorch | MIT |
| [waveprop](https://github.com/ebezzam/waveprop) | Differentiable free-space wave propagation and holography models | Python / PyTorch | MIT |

## Hardware Engineering

AI accelerator architecture, design-space exploration, performance and energy
modeling, and hardware-aware neural-network optimization. FPGA-specific work is
kept in the [FPGA Engineering](#fpga-engineering) section.

### Papers

| Year | Venue | Paper | Focus |
|:---:|:---:|:---|:---|
| 2020 | ICLR | [Once-for-All: Train One Network and Specialize it for Efficient Deployment](https://openreview.net/forum?id=HylxE1HKwS) | Hardware-aware specialization |
| 2019 | MICRO | [Understanding Reuse, Performance, and Hardware Cost of DNN Dataflow](https://doi.org/10.1145/3352460.3358252) | Accelerator dataflow modeling |
| 2019 | ISPASS | [Timeloop: A Systematic Approach to DNN Accelerator Evaluation](https://doi.org/10.1109/ISPASS.2019.00042) | Architecture exploration |
| 2019 | ICLR | [ProxylessNAS: Direct Neural Architecture Search on Target Task and Hardware](https://openreview.net/forum?id=HylVB3AqYm) | Hardware-aware NAS |
| 2019 | CVPR | [HAQ: Hardware-Aware Automated Quantization with Mixed Precision](https://openaccess.thecvf.com/content_CVPR_2019/html/Wang_HAQ_Hardware-Aware_Automated_Quantization_With_Mixed_Precision_CVPR_2019_paper.html) | Hardware-aware quantization |
| 2017 | ISCA | [In-Datacenter Performance Analysis of a Tensor Processing Unit](https://doi.org/10.1145/3079856.3080246) | AI accelerator architecture |
| 2016 | ISCA | [Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks](https://doi.org/10.1109/ISCA.2016.40) | Spatial accelerator dataflow |

### Open-Source Projects

| Project | What it provides | Stack | License |
|:---|:---|:---:|:---:|
| [Apache TVM](https://github.com/apache/tvm) | ML compiler with target-aware scheduling and hardware backends | C++ / Python | Apache-2.0 |
| [gem5](https://github.com/gem5/gem5) | Modular computer-architecture simulator used for AI hardware research | C++ / Python | BSD-3-Clause |
| [Gemmini](https://github.com/ucb-bar/gemmini) | Generator for full-system DNN accelerators based on RISC-V | Scala / Chisel | BSD-3-Clause |
| [MAESTRO](https://github.com/maestro-project/maestro) | Analytical cost model for DNN dataflows and mappings | C++ | MIT |
| [ProxylessNAS](https://github.com/mit-han-lab/ProxylessNAS) | Reference implementation of hardware-aware neural architecture search | Python / PyTorch | MIT |
| [Timeloop](https://github.com/NVlabs/timeloop) | DNN accelerator mapping and design-space exploration | C++ / Python | BSD-3-Clause |

## Structural Design

AI for topology optimization, structural response prediction, surrogate
modeling, physics-informed learning, and generative engineering design.

### Papers

| Year | Venue | Paper | Focus |
|:---:|:---:|:---|:---|
| 2022 | Structures | [Machine learning for structural engineering: A state-of-the-art review](https://doi.org/10.1016/j.istruc.2022.02.003) | Survey |
| 2021 | Nature Machine Intelligence | [Learning nonlinear operators via DeepONet based on the universal approximation theorem of operators](https://doi.org/10.1038/s42256-021-00302-5) | Structural surrogate modeling |
| 2020 | CMAME | [Physics-informed neural networks for high-speed flows](https://doi.org/10.1016/j.cma.2019.112789) | Physics-constrained simulation |
| 2020 | NeurIPS Workshop | [TopologyGAN: Topology Optimization Using Generative Adversarial Networks Based on Physical Fields Over the Initial Domain](https://arxiv.org/abs/2003.04685) | Generative topology optimization |
| 2019 | JCP | [Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations](https://doi.org/10.1016/j.jcp.2018.10.045) | Physics-informed learning |
| 2019 | Russian Numerical Analysis and Mathematical Modelling | [Neural networks for topology optimization](https://doi.org/10.1515/rnam-2019-0018) | Fast topology prediction |
| 2018 | arXiv | [3D Topology Optimization using Convolutional Neural Networks](https://arxiv.org/abs/1808.07440) | 3D structural generation |

### Open-Source Projects

| Project | What it provides | Stack | License |
|:---|:---|:---:|:---:|
| [DeepXDE](https://github.com/lululxvi/deepxde) | PINNs and operator learning for forward and inverse PDE problems | Python | LGPL-2.1 |
| [JAX-SSO](https://github.com/GaoyuanWu/JaxSSO) | Differentiable structural analysis and optimization | Python / JAX | MIT |
| [NeuralOperator](https://github.com/neuraloperator/neuraloperator) | Fourier and other neural operators for surrogate simulation | Python / PyTorch | MIT |
| [OptNet](https://github.com/locuslab/optnet) | Differentiable optimization layers for learned design pipelines | Python / PyTorch | Apache-2.0 |
| [PhysicsNeMo](https://github.com/NVIDIA/physicsnemo) | Physics-informed and data-driven models for engineering simulation | Python / PyTorch | Apache-2.0 |
| [TopOpt.jl](https://github.com/JuliaTopOpt/TopOpt.jl) | Differentiable topology optimization building blocks | Julia | MIT |

## FPGA Engineering

Quantized neural networks, FPGA inference accelerators, high-level synthesis,
dataflow compilation, and deployment toolchains.

### Papers

| Year | Venue | Paper | Focus |
|:---:|:---:|:---|:---|
| 2025 | arXiv | [A Survey on LUT-Based Deep Neural Networks Implemented in FPGAs](https://arxiv.org/abs/2506.07367) | Survey |
| 2021 | arXiv | [hls4ml: An Open-Source Codesign Workflow to Empower Scientific Low-Power Machine Learning Devices](https://arxiv.org/abs/2103.05579) | ML-to-HLS workflow |
| 2020 | FPL | [LogicNets: Co-Designed Neural Networks and Circuits for Extreme-Throughput Applications](https://arxiv.org/abs/2004.03021) | LUT-based neural inference |
| 2019 | FCCM | [LUTNet: Rethinking Inference in FPGA Soft Logic](https://doi.org/10.1109/FCCM.2019.00014) | Learned FPGA LUT operators |
| 2018 | TRETS | [FINN-R: An End-to-End Deep-Learning Framework for Fast Exploration of Quantized Neural Networks](https://doi.org/10.1145/3242897) | QNN design-space exploration |
| 2017 | FPGA | [FINN: A Framework for Fast, Scalable Binarized Neural Network Inference](https://doi.org/10.1145/3020078.3021744) | Binary neural networks on FPGA |
| 2016 | MICRO | [DNNWeaver: From High-Level Deep Network Models to FPGA Acceleration](https://cseweb.ucsd.edu/~hadi/doc/paper/2016-cogarch-dnn_weaver.pdf) | Accelerator generation |

### Open-Source Projects

| Project | What it provides | Stack | License |
|:---|:---|:---:|:---:|
| [Brevitas](https://github.com/Xilinx/brevitas) | Quantization-aware training frontend used by FINN and other accelerators | Python / PyTorch | BSD-3-Clause |
| [FINN](https://github.com/Xilinx/finn) | End-to-end dataflow compiler for quantized neural networks on AMD/Xilinx FPGAs | Python / HLS / RTL | BSD-3-Clause |
| [fpgaConvNet](https://github.com/AlexMontgomerie/fpgaconvnet-hls) | Streaming CNN accelerator generation and performance modeling | Python / HLS | GPL-3.0 |
| [HeteroCL](https://github.com/cornell-zhang/heterocl) | Hardware-oriented DSL and compiler for customizable ML accelerators | Python / C++ | Apache-2.0 |
| [hls4ml](https://github.com/fastmachinelearning/hls4ml) | Converts trained ML models into FPGA-oriented HLS implementations | Python / C++ HLS | Apache-2.0 |
| [Vitis AI](https://github.com/Xilinx/Vitis-AI) | Quantization, compilation, runtime, and model examples for AMD devices | Python / C++ | Apache-2.0 |

## Contributing

Contributions are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md)
before opening a pull request. In short:

1. Add resources to exactly one primary engineering role.
2. Prefer peer-reviewed papers and official paper or DOI links.
3. List only repositories with an explicit license in open-source tables.
4. Keep papers in descending publication-year order and projects alphabetical.
5. Explain the engineering workflow improved by the resource.

## License

Released under the [MIT License](LICENSE). Linked papers, code, datasets, and
other third-party resources remain under their respective licenses.
