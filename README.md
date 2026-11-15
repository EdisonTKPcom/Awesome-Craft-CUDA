<div align="center">

# Awesome Craft CUDA [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of open-source CUDA learning material, kernel libraries, tooling and portability projects.

![Tools](https://img.shields.io/badge/tools-24-6366f1?style=for-the-badge)
[![Categories](https://img.shields.io/badge/categories-4-0ea5e9?style=for-the-badge)](#contents)
[![Combined stars](https://img.shields.io/badge/combined_stars-124.5k-f59e0b?style=for-the-badge&logo=github)](#-leaderboard)
[![Stars](https://img.shields.io/github/stars/EdisonTKPcom/Awesome-Craft-CUDA?style=for-the-badge&color=22c55e)](https://github.com/EdisonTKPcom/Awesome-Craft-CUDA/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/EdisonTKPcom/Awesome-Craft-CUDA?style=for-the-badge&color=ec4899)](https://github.com/EdisonTKPcom/Awesome-Craft-CUDA/commits/main)

</div>

The NVIDIA CUDA Toolkit is proprietary. nvcc, CUDA-GDB, Nsight, cuBLAS, cuDNN and most official NVIDIA developer tools are distributed under NVIDIA's EULA, not an OSI licence. Open-source CUDA libraries often still need that toolkit to build or run. Portability projects are not automatically drop-in replacements for CUDA. This list repeats a drop-in claim only when the project's own documentation uses that wording, and then only with coverage caveats. SCALE by Spectral Compute is not listed as open source: its free licence is limited to non-commercial use.

Related lists: [Awesome Craft](https://github.com/EdisonTKPcom/Awesome-Craft), [Awesome Craft AI](https://github.com/EdisonTKPcom/Awesome-Craft-AI).

## Contents

- [Dashboard](#dashboard)
- [Learning material](#learning-material)
- [Kernel and GPU libraries](#kernel-and-gpu-libraries)
- [Tooling and samples](#tooling-and-samples)
- [Portability and other programming models](#portability-and-other-programming-models)

## Dashboard

<table>
<tr>
<td align="center"><h2>24</h2>listed projects</td>
<td align="center"><h2>4</h2>categories</td>
<td align="center"><h2>124.5k</h2>combined GitHub stars</td>
<td align="center"><h2>20.6k</h2>combined forks</td>
<td align="center"><h2>12/14</h2>pushed in the last 30 days</td>
<td align="center"><h2>6</h2>languages</td>
</tr>
</table>

Stats snapshot taken on 2026-11-15 from the GitHub API, for GitHub-hosted repositories only. Official documentation and other non-GitHub entries are listed but have no stars, forks or push dates. Star badges next to GitHub entries update live.

### 🏆 Leaderboard

<table>
<tr><th>Rank</th><th>Project</th><th>Kind</th><th align="right">Stars</th><th></th></tr>
<tr><td align="center">🥇</td><td><b>FlashAttention</b></td><td>Attention kernels</td><td align="right">25.3k</td><td><code>████████████████████</code></td></tr>
<tr><td align="center">🥈</td><td><b>Triton</b></td><td>GPU kernel language</td><td align="right">20.6k</td><td><code>████████████████</code></td></tr>
<tr><td align="center">🥉</td><td><b>ZLUDA</b></td><td>CUDA on other GPUs</td><td align="right">15.2k</td><td><code>████████████</code></td></tr>
<tr><td align="center">4</td><td><b>Apache TVM</b></td><td>ML compiler</td><td align="right">13.9k</td><td><code>███████████</code></td></tr>
<tr><td align="center">5</td><td><b>CuPy</b></td><td>Python arrays</td><td align="right">12.4k</td><td><code>██████████</code></td></tr>
<tr><td align="center">6</td><td><b>CUTLASS</b></td><td>GEMM templates</td><td align="right">10.7k</td><td><code>████████</code></td></tr>
<tr><td align="center">7</td><td><b>NVIDIA CUDA Samples</b></td><td>Official samples</td><td align="right">9.8k</td><td><code>████████</code></td></tr>
<tr><td align="center">8</td><td><b>NCCL</b></td><td>Collective comms</td><td align="right">5.2k</td><td><code>████</code></td></tr>
<tr><td align="center">9</td><td><b>ThunderKittens</b></td><td>CUDA kernel primitives</td><td align="right">3.8k</td><td><code>███</code></td></tr>
<tr><td align="center">10</td><td><b>CUDA Python</b></td><td>Python bindings</td><td align="right">3.4k</td><td><code>███</code></td></tr>
</table>


### Stars by category

```mermaid
pie showData
    title Combined GitHub stars by category
    "Learning material" : 9769
    "Kernel and GPU libraries" : 78245
    "Tooling and samples" : 0
    "Portability and other programming models" : 36512
```

### Licences

![Custom](https://img.shields.io/badge/Custom-6-64748b?style=flat-square) ![MIT](https://img.shields.io/badge/MIT-4-64748b?style=flat-square) ![Apache-2.0](https://img.shields.io/badge/Apache--2.0-3-64748b?style=flat-square) ![BSD-3-Clause](https://img.shields.io/badge/BSD--3--Clause-1-64748b?style=flat-square)

"Custom" or "None" means GitHub could not match a standard SPDX licence, often because of extra terms or an undeclared licence. Read the project licence before you use it commercially.

## Learning material

- [GPU MODE lectures](https://github.com/gpu-mode/lectures) - Lecture notes and material from the GPU MODE community, covering CUDA kernel writing and related performance topics. ![Stars](https://img.shields.io/github/stars/gpu-mode/lectures?style=flat-square&label=%E2%AD%90)
- [GPU Puzzles](https://github.com/srush/GPU-Puzzles) - A puzzle-style tutorial that teaches GPU kernel ideas through small exercises. This is a teaching repository, not a production kernel library. ![Stars](https://img.shields.io/github/stars/srush/GPU-Puzzles?style=flat-square&label=%E2%AD%90)
- [NVIDIA CUDA Samples](https://github.com/NVIDIA/cuda-samples) - Official example programs that demonstrate CUDA Toolkit features. Building and running the samples generally requires a proprietary CUDA Toolkit install. ![Stars](https://img.shields.io/github/stars/NVIDIA/cuda-samples?style=flat-square&label=%E2%AD%90)

## Kernel and GPU libraries

- [Apache TVM](https://github.com/apache/tvm) - A compiler stack for deploying machine-learning models and kernels onto a range of hardware backends, including GPUs. TVM is a compiler framework, not a CUDA source-level substitute. ![Stars](https://img.shields.io/github/stars/apache/tvm?style=flat-square&label=%E2%AD%90)
- [CCCL](https://github.com/NVIDIA/cccl) - NVIDIA CUDA C++ Core Libraries, unifying Thrust, CUB and libcu++. Component licences differ: Thrust and libcu++ use Apache-2.0 with listed exceptions, and CUB is BSD-3-Clause. Read the repository licence file for the component you use. ![Stars](https://img.shields.io/github/stars/NVIDIA/cccl?style=flat-square&label=%E2%AD%90)
- [CUDA Python](https://github.com/NVIDIA/cuda-python) - NVIDIA official Python bindings to the CUDA Toolkit. The bindings are open source; they still call into the proprietary CUDA Toolkit and driver. ![Stars](https://img.shields.io/github/stars/NVIDIA/cuda-python?style=flat-square&label=%E2%AD%90)
- [CuPy](https://github.com/cupy/cupy) - A NumPy and SciPy compatible array library that can use NVIDIA CUDA and, in supported builds, other GPU backends. This is a Python array layer, not a CUDA compiler. ![Stars](https://img.shields.io/github/stars/cupy/cupy?style=flat-square&label=%E2%AD%90)
- [CUTLASS](https://github.com/NVIDIA/cutlass) - CUDA C++ template abstractions, and related Python DSLs, for high-performance GEMM and related linear algebra on NVIDIA GPUs. ![Stars](https://img.shields.io/github/stars/NVIDIA/cutlass?style=flat-square&label=%E2%AD%90)
- [FlashAttention](https://github.com/Dao-AILab/flash-attention) - The official implementation of FlashAttention and FlashAttention-2. The README also describes ROCm backends; those backends are not implied to be complete substitutes for every CUDA build flag. ![Stars](https://img.shields.io/github/stars/Dao-AILab/flash-attention?style=flat-square&label=%E2%AD%90)
- [HipKittens](https://github.com/HazyResearch/HipKittens) - The AMD and HIP counterpart to ThunderKittens, for writing similar tile-style kernels on AMD GPUs. This is not a drop-in compile of ThunderKittens CUDA sources. ![Stars](https://img.shields.io/github/stars/HazyResearch/HipKittens?style=flat-square&label=%E2%AD%90)
- [Kokkos](https://github.com/kokkos/kokkos) - A C++ performance-portability programming model with CUDA, HIP, SYCL and other backends. Code written in Kokkos is not automatically a drop-in of existing CUDA C++. ![Stars](https://img.shields.io/github/stars/kokkos/kokkos?style=flat-square&label=%E2%AD%90)
- [NCCL](https://github.com/NVIDIA/nccl) - NVIDIA library for multi-GPU and multi-node collective communication. Most of the project is Apache-2.0, with some parts remaining under their original BSD licence. ![Stars](https://img.shields.io/github/stars/NVIDIA/nccl?style=flat-square&label=%E2%AD%90)
- [Numba](https://github.com/numba/numba) - A Python JIT compiler that includes a CUDA target for writing GPU kernels in Python. The CUDA target still depends on a CUDA toolchain when compiling for NVIDIA GPUs. ![Stars](https://img.shields.io/github/stars/numba/numba?style=flat-square&label=%E2%AD%90)
- [rocBLAS](https://github.com/ROCm/rocBLAS) - AMD BLAS implementation for ROCm, often used when porting CUDA code that called cuBLAS. This is an AMD library, not a binary replacement for cuBLAS. ![Stars](https://img.shields.io/github/stars/ROCm/rocBLAS?style=flat-square&label=%E2%AD%90)
- [ThunderKittens](https://github.com/HazyResearch/ThunderKittens) - A header-only CUDA framework of tile primitives for writing deep-learning kernels on NVIDIA GPUs. ![Stars](https://img.shields.io/github/stars/HazyResearch/ThunderKittens?style=flat-square&label=%E2%AD%90)
- [tiny-cuda-nn](https://github.com/NVlabs/tiny-cuda-nn) - A collection of fused CUDA kernels and bindings for small, fast neural networks. ![Stars](https://img.shields.io/github/stars/NVlabs/tiny-cuda-nn?style=flat-square&label=%E2%AD%90)

## Tooling and samples

- [nvbench](https://github.com/NVIDIA/nvbench) - NVIDIA C++ benchmark harness for CUDA kernels. Useful for measuring kernels you already build with the CUDA toolchain; it is not a substitute for Nsight Compute. ![Stars](https://img.shields.io/github/stars/NVIDIA/nvbench?style=flat-square&label=%E2%AD%90)

## Portability and other programming models

- [AdaptiveCpp](https://github.com/AdaptiveCpp/AdaptiveCpp) - An open SYCL compiler stack, historically known as hipSYCL or Open SYCL, targeting multiple backends. Any CUDA-like compatibility layer should be treated as experimental unless the version you use documents otherwise. ![Stars](https://img.shields.io/github/stars/AdaptiveCpp/AdaptiveCpp?style=flat-square&label=%E2%AD%90)
- [chipStar](https://github.com/CHIP-SPV/chipStar) - Compiles and runs HIP and CUDA applications on platforms that support SPIR-V, using OpenCL or Level Zero. The project documents unsupported or partial features; do not assume complete CUDA compatibility. ![Stars](https://img.shields.io/github/stars/CHIP-SPV/chipStar?style=flat-square&label=%E2%AD%90)
- [HIP and HIPIFY](https://github.com/ROCm/HIPIFY) - AMD tools for translating CUDA to HIP so code can be retargeted to ROCm. AMD porting documentation describes a porting process with manual changes and testing, not a drop-in CUDA replacement. See also the HIP runtime repository. ![Stars](https://img.shields.io/github/stars/ROCm/HIPIFY?style=flat-square&label=%E2%AD%90)
- [Intel llvm SYCL](https://github.com/intel/llvm) - Intel LLVM fork that implements SYCL and related oneAPI or DPC++ compilation. oneAPI as a product also includes proprietary or separately licensed components; this entry is the open compiler project. ![Stars](https://img.shields.io/github/stars/intel/llvm?style=flat-square&label=%E2%AD%90)
- [ROCm](https://github.com/ROCm/ROCm) - AMD open GPU software stack of compilers, runtimes and libraries with mixed licences. It is the usual home for HIP on AMD hardware, not a CUDA Toolkit substitute on NVIDIA hardware. ![Stars](https://img.shields.io/github/stars/ROCm/ROCm?style=flat-square&label=%E2%AD%90)
- [Triton](https://github.com/triton-lang/triton) - A language and compiler for writing tiled GPU kernels at a higher level than raw CUDA C++. Triton is a different programming model, not a source-compatible replacement for nvcc. ![Stars](https://img.shields.io/github/stars/triton-lang/triton?style=flat-square&label=%E2%AD%90)
- [ZLUDA](https://github.com/vosen/ZLUDA) - A project whose README describes it as a drop-in replacement for running unmodified CUDA applications on non-NVIDIA GPUs. That wording is the project's claim; it is unofficial, architecture coverage is incomplete, and it is not a licence to the CUDA Toolkit. ![Stars](https://img.shields.io/github/stars/vosen/ZLUDA?style=flat-square&label=%E2%AD%90)

## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

<div align="center">

If this list is useful, give it a ⭐ so others can find it.

</div>
