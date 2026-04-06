# Mamba-VOS: Efficient Video Object Segmentation with Selective State Space Models

[![Paper Status](https://img.shields.io/badge/Paper-Accepted-brightgreen)]([Link to Paper])
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This is the official PyTorch implementation of the paper: **"Robust Vision-Language Alignment Using Multi-Modal Large Language Models for Open-Vocabulary Semantic Segmentation"**.  
Authors: Cheolhun Jang, Seok Jun Youn, Issac Kang, Junhyeong Kwon, Daehyun JI, Jun Won Choi and Nam Ik Cho  
Accepted at IEEE Access.

> **🚧 Code Coming Soon 🚧**
>
> The code used in the paper is currently being cleaned up and will be uploaded soon. Thank you for your patience!

## Abstract

> While memory-based networks have achieved remarkable accuracy in Video Object Segmentation (VOS), the inherent quadratic computational complexity of attention-based refinement remains a critical barrier to long-term inference efficiency. To overcome these structural limitations, we introduce Mamba-VOS, a novel architecture that reformulates the memory readout refinement as a unified spatiotemporal sequence modeling task. By integrating Mamba, a Selective State Space Model (SSM), our framework achieves linear complexity ($O(N)$) while maintaining data-dependent, content-aware selectivity. Unlike previous methods that force a compromise between temporal context and speed, Mamba-VOS facilitates holistic spatiotemporal modeling without the substantial computational cost of Transformers. Comprehensive experiments demonstrate that Mamba-VOS achieves a superior trade-off between accuracy and efficiency. On the challenging MOSE and LVOS datasets, our method sets a new state-of-the-art with $\mathcal{J}\&\mathcal{F}$ scores of 68.6\% and 62.6\%, respectively, outperforming existing Transformer-based and linear-attention methods. Furthermore, on standard benchmarks, Mamba-VOS matches top-tier performance, achieving 88.9\% on DAVIS-2017 and 86.1\% on YouTube-VOS. Notably, our model runs at 48.2 FPS on an NVIDIA V100 GPU, which represents a 45\% speedup over the strong baseline. Our results validate that Mamba-VOS offers a robust and highly efficient solution for next-generation video segmentation. The source code is available at https://github.com/c-jang/mamba-vos.

## Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/woori21c/dfag.git](https://github.com/c-jang/mamba-vos.git)
    cd dfag
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: The `requirements.txt` file will be uploaded along with the source code.)*

## Usage

(This section will be updated once the code is uploaded.)

#### **Training**

To train the model, run the following command:
```bash
python train.py --config [path_to_config_file]
