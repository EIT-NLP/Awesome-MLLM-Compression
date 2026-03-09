<h1 align="center" id="awesome">
Awesome MLLM Compression
</h1>

<div align="center">

This repository contains a regularly updated paper list for **MLLM Compression**.

[![TechRxiv](https://img.shields.io/badge/TechRxiv-DOI-b31b1b)](https://www.techrxiv.org/doi/full/10.36227/techrxiv.177220375.55495124/v1)
[![Awesome](https://img.shields.io/badge/Awesome-List-8A2BE2)](https://github.com/sindresorhus/awesome)
[![License](https://img.shields.io/badge/License-MIT-007ec6)](https://opensource.org/license/MIT)
[![Contributions](https://img.shields.io/badge/Contributions-Welcome-2ea44f)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/pulls)
![Last Commit](https://img.shields.io/github/last-commit/EIT-NLP/Awesome-MLLM-Compression?color=6e7781)

</div>

> <strong> From Data to Model: A Survey of the Compression Lifecycle in MLLMs </strong>
>
> <a href="https://harrisonwu42.github.io/" rel="nofollow">Hao Wu</a><sup>\*,1</sup>, 
<a href="https://scholar.google.com/citations?user=Amv2QE8AAAAJ" rel="nofollow">Junlong Tong</a><sup>\*,1,2</sup>, 
<a href="https://scholar.google.com/citations?user=WP9E-ogAAAAJ" rel="nofollow">Xudong Wang</a><sup>1</sup>,
Yang Tan</a><sup>3</sup>, 
<a href="https://scholar.google.com/citations?user=56aEgJ0AAAAJ" rel="nofollow">Changyu Zeng</a><sup>1</sup>, 
<a href="https://scholar.google.com/citations?user=lJ-GGU8AAAAJ" rel="nofollow">Anastasia Antsiferova</a><sup>1</sup>, 
<a href="https://chin-gyou.github.io/" rel="nofollow">Xiaoyu Shen</a><sup>†,1</sup> 
>
> <sup>1</sup>Institute of Digital Twin, Eastern Institute of Technology, Ningbo
>
> <sup>2</sup>Shanghai Jiao Tong University, <sup>3</sup>Southeast University, <sup>4</sup>Innopolis University 
>
> <sup>\*</sup> Core Contribution, <sup>†</sup> Corresponding Author.
>
> Contact: haowu.ai.research@gmail.com, xyshen@eitech.edu.cn

If you find our paper of this resource helpful, please consider cite:
```bibtex
@article{Wu_2026,
    title={From Data to Model: A Survey of the Compression Lifecycle in MLLMs},
    url={http://dx.doi.org/10.36227/techrxiv.177220375.55495124/v1},
    DOI={10.36227/techrxiv.177220375.55495124/v1},
    publisher={Institute of Electrical and Electronics Engineers (IEEE)},
    author={Wu, Hao and Tong, Junlong and Wang, Xudong and Tan, Yang and Zeng, Changyu and Antsiferova, Anastasia and Shen, Xiaoyu},
    year={2026},
    month=feb 
}
```

<!-- 🔥 📚 👀 🌟 ✨ ✒️ 🎯 📄 🙏 ✉️ 🤗 🌐 🚀 🔔 💡 🔧 ⭐️ 📋 -->


> [!IMPORTANT]
> We actively maintain this repository and welcome community contributions.
> If you would like to:
> 
> - Add newly released MLLM compression papers  
> - Propose refinements to our taxonomy  
> - Correct or update existing entries  
> - Discuss classification or methodology  
> 
> Please submit a [pull request](https://github.com/EIT-NLP/Awesome-MLLM-Compression/pulls) or contact the authors.


## 🔥News <a id="news"></a>

- **[2026.02.27]** The preprint is now published! 



## 💡 Highlights <a id="highlights"></a>

- **Lifecycle perspective for MLLM compression**: We introduce a **Data-to-Model view** that organizes compression methods according to where compression occurs in the MLLM pipeline, including the Input, Encoder, Projector, and LLM stages.
- **Five fundamental compression operations**: We distill existing methods into five fundamental operations: **Dropping**, **Aggregation**, **Encoding**, **Resampling**, and **Skipping**, providing a unified abstraction for analyzing compression strategies.
- **Joint compression across efficiency dimensions**:  We advocate jointly considering **token compression**, **operation compression**, and **KV cache compression** as complementary strategies for improving the efficiency of MLLMs.
- **Cross-level compression coordination**: We advocate that coordinated compression across multiple pipeline levels provides a more effective way to balance efficiency and model performance.
- **Beyond efficiency-oriented compression**: We argue that compression should not be viewed solely as an efficiency technique, but also as a design principle that can reshape representations, architectures, and multimodal processing in MLLMs.


## 📚 Contents <a id="contents"></a>

- [News](#news): Latest updates, news, and announcements.
- [Highlights](#highlights): Core insights and perspectives that this survey aims to emphasize.
- [Tag Description](#tag): Brief explanation of tags in this repository.
- [Libraries](#lib): A collection of MLLM compression papers compiled in this repository.
- [License](#license): License information for this repository.
- [Acknowledgments](#acknowledgments): Credits to projects and contributors that inspired or supported this work.
- [Contact](#contact): Contact information for questions, feedback, or collaboration.
- [Related Projects](#projects): Research projects from our group ([EIT-NLP](https://idt.eitech.edu.cn/nlp/)) related to MLLM compression.


## 📋 Tag Description <a id="tag"></a>

- ![Preprint](https://img.shields.io/badge/Preprint-Paper-b31b1b) for preprint papers.
- ![PDF](https://img.shields.io/badge/PDF-Paper-1f6feb) for conference or journal papers.
- ![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github) for GitHub repositories.
- ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) for research areas (primarily categorized by modality).
- ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) for compression positions (i.e., Input, Encoder, Projector, LLM)
- ![Op](https://img.shields.io/badge/Op-Dropping-2f9e44) for compression operation types (i.e., Dropping, Aggregation, Encoding, Resampling, Skipping)
- ![Mech](https://img.shields.io/badge/Mech-Attention--based-c2416c) for specific compression mechanisms (the third level in our taxonomy).
- ![Target](https://img.shields.io/badge/Target-Token-0d9488) for compression dimensions (i.e., Token Compression, Operation Compression, KV Cache Compression)
- ![Cost](https://img.shields.io/badge/Cost-Training--Free-8b5e3c) for training cost (i.e., Training-Free, Retraining, Post-Training).

## 🌟 Libraries <a id="lib"></a>

🔔 Please check out the papers by selecting the sub-area you are interested in. Within each sub-area, papers are organized according to our compression taxonomy. On this main page, only related surveys and papers released in the past six months are shown.

- [Awesome MLLM Compression](#awesome)
  - [Image LLM (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/image-llm.md)
  - [Video LLM (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/video-llm.md)
  - [Audio LLM (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/audio-llm.md)
  - [3D LLM (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/3d-llm.md)
  - [Omni LLM (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/omni-llm.md)
  - [Vision Encoder (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/vision-encoder.md)
  - [Audio Encoder (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/audio-encoder.md)
  - [3D Encoder (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/3d-encoder.md)

### Survey
| Title & Authors & Links | Date | Taxonomy | Highlight |
|---|---|---|---|
| [![Preprint](https://img.shields.io/badge/TechRxiv-DOI-b31b1b)](https://www.techrxiv.org/users/1031130/articles/1390890-from-data-to-model-a-survey-of-the-compression-lifecycle-in-mllms) [![GitHub](https://img.shields.io/badge/GitHub-Awesome--MLLM--Compression-white?logo=github)](https://github.com/EIT-NLP/Awesome-MLLM-Compression) <br> **From Data to Model: A Survey of the Compression Lifecycle in MLLMs** <br> Hao Wu, Junlong Tong, Xudong Wang, Yang Tan, Changyu Zeng, Anastasia Antsiferova, Xiaoyu Shen| 26.2.27| Compression position & <br> Compression operation & <br> Mechanisim| Compression Lifecycle |
| [![Preprint](https://img.shields.io/badge/arXiv-2601.20742-b31b1b)](https://arxiv.org/abs/2601.20742)<br>**Compression Tells Intelligence: Visual Coding, Visual Token Technology, and the Unification** <br> Xin Jin, Jinming Liu, Yuntao Wei, Junyan Lin, Zhicheng Wang, Jianguo Huang, Xudong Yang, Yanxiao Liu, Wenjun Zeng| 26.01.28 | Codec & <br> Token Technology| Compression <br> as Intelligence |
| [![Preprint](https://img.shields.io/badge/TechRxiv-DOI-b31b1b)](https://www.techrxiv.org/users/1031130/articles/1390890-from-data-to-model-a-survey-of-the-compression-lifecycle-in-mllms) [![GitHub](https://img.shields.io/badge/GitHub-MLLM--Token--Compression-white?logo=github)](https://github.com/yaolinli/MLLM-Token-Compression) <br> **Towards Efficient Multimodal Large Language Models: A Survey on Token Compression** <br> Linli Yao, Long Xing, Yang Shi, Sida Li, Yuanxin Liu, Yuhao Dong, Yi-Fan Zhang, Lei Li, Qingxiu Dong, Xiaoyi Dong, Qidong Huang, Haotian Wang, Feng Wu, Yuanxing Zhang, Pengfei Wan, Zhouchen Lin, Xu Sun| 26.01.12 | Compression Position & <br> Mechanisim | - |
| ![PDF](https://img.shields.io/badge/ISCAS-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2508.13460-b31b1b)](https://arxiv.org/abs/2508.13460)<br>**Revisiting MLLM Token Technology through the Lens of Classical Visual Coding** <br> Jinming Liu, Junyan Lin, Yuntao Wei, Kele Shao, Keda Tao, Jianguo Huang, Xudong Yang, Zhibo Chen, Huan Wang, Xin Jin| 25.08.19| Codec & <br> Token Technology | - |
| ![PDF](https://img.shields.io/badge/TMLR-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2507.20198-b31b1b)](https://arxiv.org/abs/2507.20198v5) [![GitHub](https://img.shields.io/badge/GitHub-Awesome--Multimodal--Token--Compression-white?logo=github)](https://github.com/cokeshao/Awesome-Multimodal-Token-Compression)  <br >**A Survey of Token Compression for Efficient Multimodal Large Language Models** <br> Kele Shao, Keda Tao, Kejia Zhang, Sicheng Feng, Mu Cai, Yuzhang Shang, Haoxuan You, Can Qin, Yang Sui, Huan Wang | 25.07.27 | Modality & <br> Mechanisim | Modality-centric|
| [![Preprint](https://img.shields.io/badge/arXiv-2505.18227-b31b1b)](https://arxiv.org/abs/2505.18227) [![GitHub](https://img.shields.io/badge/GitHub-Awesome--Collection--Token--Reduction-white?logo=github)](https://github.com/ZLKong/Awesome-Collection-Token-Reduction) <br> **Token Reduction Should Go Beyond Efficiency in Generative Models -- From Vision, Language to Multimodality** <br> Zhenglun Kong, Yize Li, Fanhu Zeng, Lei Xin, Shvat Messica, Xue Lin, Pu Zhao, Manolis Kellis, Hao Tang, Marinka Zitnik| 25.05.23 | TODO | Compression<br>Beyond Efficiency |




### Recent Papers (Last 6 Months)

<!-- Image -->
<details open>
<summary><b>Image (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/ICLR-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2602.23699-b31b1b)](https://arxiv.org/abs/2602.23699) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/EIT-NLP/HiDrop) <br> **HiDrop: Hierarchical Vision Token Reduction in MLLMs via Late Injection, Concave Pyramid Pruning, and Early Exit** <br> Hao Wu, Yingqi Fan, Jinyang Dai, Junlong Tong, Yunpu Ma, Xiaoyu Shen | ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Retraining-8b5e3c)  ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Op](https://img.shields.io/badge/Op-Skip-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Depth--wise-c2416c)  <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) ![Target](https://img.shields.io/badge/Target-Operation-0d9488)|
| ![PDF](https://img.shields.io/badge/CVPR-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2602.23734-b31b1b)](https://arxiv.org/abs/2602.23699) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/EIT-NLP/UTPTrack) <br> **UTPTrack: Towards Simple and Unified Token Pruning for Visual Tracking** <br> Hao Wu, Xudong Wang, Jialiang Zhang, Junlong Tong, Xinghao Chen, Junyan Lin, Yunpu Ma, Xiaoyu Shen | ![Area](https://img.shields.io/badge/Area-Vision--Encoder-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Retraining-8b5e3c) ![Level](https://img.shields.io/badge/Level-Encoder-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488)| 


</details>

<!-- Video -->
<details open>
<summary><b>Video (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>


<!-- Audio -->
<details open>
<summary><b>Audio (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>


<!-- 3D -->
<details open>
<summary><b>3D (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>


<!-- Omni -->
<details open>
<summary><b>Omni (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>


### Published in Recent Conferences (Last 12 months)


<!-- CVPR 2026 -->
<details open>
<summary><b>CVPR 2026 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/CVPR-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2602.23734-b31b1b)](https://arxiv.org/abs/2602.23699) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/EIT-NLP/UTPTrack) <br> **UTPTrack: Towards Simple and Unified Token Pruning for Visual Tracking** <br> Hao Wu, Xudong Wang, Jialiang Zhang, Junlong Tong, Xinghao Chen, Junyan Lin, Yunpu Ma, Xiaoyu Shen | ![Area](https://img.shields.io/badge/Area-Vision--Encoder-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Retraining-8b5e3c) ![Level](https://img.shields.io/badge/Level-Encoder-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488)| 


</details>



<!-- ICLR 2026 -->
<details open>
<summary><b>ICLR 2026 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/ICLR-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2602.23699-b31b1b)](https://arxiv.org/abs/2602.23699) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/EIT-NLP/HiDrop) <br> **HiDrop: Hierarchical Vision Token Reduction in MLLMs via Late Injection, Concave Pyramid Pruning, and Early Exit** <br> Hao Wu, Yingqi Fan, Jinyang Dai, Junlong Tong, Yunpu Ma, Xiaoyu Shen | ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Retraining-8b5e3c)  ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Op](https://img.shields.io/badge/Op-Skip-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Depth--wise-c2416c)  <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) ![Target](https://img.shields.io/badge/Target-Operation-0d9488)|



</details>


<!-- EMNLP 2025 -->
<details open>
<summary><b>EMNLP 2025 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>


<!-- NeurIPS 2025 -->
<details open>
<summary><b>NeurIPS 2025 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>


<!-- ICCV 2025 -->
<details open>
<summary><b>ICCV 2025 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>



<!-- ICML 2025 -->
<details open>
<summary><b>ICML 2025 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>



<!-- ICML 2025 -->
<details open>
<summary><b>ACL 2025 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>



## 📄 License <a id="license"></a>

This project is released under the [MIT](https://opensource.org/license/MIT) License.


## 🙏 Acknowledgments <a id="acknowledgments"></a>

This repository is inspired by [Awesome-Multimodal-Token-Compression](https://github.com/cokeshao/Awesome-Multimodal-Token-Compression), [Awesome-Latent-CoT](https://github.com/EIT-NLP/Awesome-Latent-CoT), and [Awesome-Efficient-LLM](https://github.com/horseee/Awesome-Efficient-LLM).


<!-- ## 🧑‍💻 Contributors <a id="contributor"></a>
Thanks to these contributors for this excellent work ! -->

## ✉️ Contact <a id="contact"></a>

For questions, suggestions, or collaboration opportunities, please feel free to reach out:

- **Hao Wu**: haowu.ai.research@gmail.com
- **Xiaoyu Shen**: xyshen@eitech.edu.cn

## 🌐 Related Projects (ours) <a id="projects"></a>
- Vision Encoder
  - [CVPR 26] [UTPTrack: Towards Simple and Unified Token Pruning for Visual Tracking](https://github.com/EIT-NLP/UTPTrack)
- ImageLLM
  - [EMNLP 25] [VisiPruner: Decoding Discontinuous Cross-Modal Dynamics for Efficient Multimodal LLMs](https://github.com/EIT-NLP/VisiPruner)
  - [ICLR 26] [HiDrop: Hierarchical Vision Token Reduction in MLLMs via Late Injection, Concave Pyramid Pruning, and Early Exit](https://github.com/EIT-NLP/HiDrop)
  - [Preprint] [ViCA: Efficient Multimodal LLMs with Vision-Only Cross-Attention
](https://arxiv.org/abs/2602.07574)