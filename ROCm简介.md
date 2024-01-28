# ROCm 简介
## 介绍
ROCm 是AMD公司对于其自己GPU的一个软件栈。 ROCm 跨越多个领域：图形处理单元上的通用计算 (GPGPU)、高性能计算 (HPC)、异构计算。它提供了多种编程模型：HIP（基于GPU内核的编程）、OpenMP/消息传递接口（MPI）（基于指令的编程）、OpenCL。

ROCm 是免费、自由和开源软件（除了 GPU 固件 blob [4] ），它根据各种许可证进行分发。 ROCm 是 Radeon 开放计算平台的缩写。

ROCm 是一个开源堆栈，主要由开源软件组成，专为图形处理单元 (GPU) 计算而设计。 ROCm 包含一系列驱动程序、开发工具和 API，支持从低级内核到最终用户应用程序的 GPU 编程。

借助 ROCm，您可以自定义 GPU 软件以满足您的特定需求。您可以在免费、开源、集成且安全的软件生态系统中开发、协作、测试和部署应用程序。 ROCm 特别适合 GPU 加速的高性能计算 (HPC)、人工智能 (AI)、科学计算和计算机辅助设计 (CAD)。

ROCm 由 AMD 的异构计算可移植接口 (HIP) 提供支持，这是一个开源软件 C++ GPU 编程环境及其相应的运行时。 HIP 允许 ROCm 开发人员通过在从专用游戏 GPU 到百亿亿级 HPC 集群的一系列平台上部署代码，在不同平台上创建便携式应用程序。

ROCm 支持 OpenMP 和 OpenCL 等编程模型，并包括所有必需的开源软件编译器、调试器和库。 ROCm 完全集成到机器学习 (ML) 框架中，例如 PyTorch 和 TensorFlow。

## 重点
本项目着重研究RoCm中的关于内核驱动以及中间件的相关驱动代码，至于应用层不会太过关心。
ROCm 项目使用的带有 KFD 的 AMDGPU 驱动程序。还包含与此基本驱动程序匹配的当前 Linux 内核
KFD ：  Kernel Fusion Driver
截至 2022 年，AMD 内核融合驱动程序 (KFD) 现已集成到这一内核模块中。 AMD 的 AMD KFD 开发是 ROCm 的一部分，属于 ROCk 项目。
* [ROCK-Kernel-Driver](https://github.com/ROCm/ROCK-Kernel-Driver)

## 参考
[What is ROCm?](https://rocm.docs.amd.com/en/latest/what-is-rocm.html)

[AMDgpu](https://en.wikipedia.org/wiki/AMDgpu_(Linux_kernel_module))
