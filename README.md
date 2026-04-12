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

🔔 Please check out the papers by selecting the sub-area you are interested in. Within each sub-area, papers are organized according to our compression taxonomy. The main page presents all survey papers, together with major conference (i.e., ICML, NeurIPS, ICLR, CVPR, ICCV, ECCV, ACL, EMNLP, NAACL) papers from the past year and recently released papers within the last six months. Note that papers already included in the major conference papers from the past year are excluded from the recent papers.


- [Awesome MLLM Compression](#awesome)
  - Image
    - [Vision Encoder (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/vision-encoder.md)
    - [Image LLM (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/image-llm.md)
    - [Vision Decoder (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/vision-decoder.md)
  - Video
    - [Video LLM (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/video-llm.md)
  - Audio
    - [Audio Encoder](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/audio-encoder.md)
    - [Audio LLM](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/audio-llm.md)
    - [Audio Decoder](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/audio-decoder.md)
  - 3D
    - [3D Encoder](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/3d-encoder.md)
    - [3D LLM](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/3d-llm.md)
    - [3D Decoder](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/3d-decoder.md)
  - Omni
    - [Omni LLM (TODO)](https://github.com/EIT-NLP/Awesome-MLLM-Compression/blob/main/omni-llm.md)
- [Survey](#survey)
- [Recent Papers](#recent)
- [Published in Recent Conferences](#conference)

### Survey
| Title & Authors & Links | Date | Taxonomy | Highlight |
|---|---|---|---|
| ![PDF](https://img.shields.io/badge/ACL--Findings-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2604.05546-b31b1b)](https://arxiv.org/abs/2604.05546) <br> **Efficient Inference for Large Vision-Language Models: Bottlenecks, Techniques, and Prospects** <br> Jun Zhang, Yicheng Ji, Feiyang Ren, Yihang Li, Bowen Zeng, Zonghao Chen, Ke Chen, Lidan Shou, Gang Chen, Huan Li| 26.4.07| | |
| [![Preprint](https://img.shields.io/badge/TechRxiv-DOI-b31b1b)](https://www.techrxiv.org/users/1031130/articles/1390890-from-data-to-model-a-survey-of-the-compression-lifecycle-in-mllms) [![GitHub](https://img.shields.io/badge/GitHub-Awesome--MLLM--Compression-white?logo=github)](https://github.com/EIT-NLP/Awesome-MLLM-Compression) <br> **From Data to Model: A Survey of the Compression Lifecycle in MLLMs** <br> Hao Wu, Junlong Tong, Xudong Wang, Yang Tan, Changyu Zeng, Anastasia Antsiferova, Xiaoyu Shen| 26.2.27| Compression position & <br> Compression operation & <br> Mechanisim| Compression Lifecycle |
| [![Preprint](https://img.shields.io/badge/arXiv-2601.20742-b31b1b)](https://arxiv.org/abs/2601.20742)<br>**Compression Tells Intelligence: Visual Coding, Visual Token Technology, and the Unification** <br> Xin Jin, Jinming Liu, Yuntao Wei, Junyan Lin, Zhicheng Wang, Jianguo Huang, Xudong Yang, Yanxiao Liu, Wenjun Zeng| 26.01.28 | Codec & <br> Token Technology| Compression <br> as Intelligence |
| [![Preprint](https://img.shields.io/badge/TechRxiv-DOI-b31b1b)](https://www.techrxiv.org/users/1031130/articles/1390890-from-data-to-model-a-survey-of-the-compression-lifecycle-in-mllms) [![GitHub](https://img.shields.io/badge/GitHub-MLLM--Token--Compression-white?logo=github)](https://github.com/yaolinli/MLLM-Token-Compression) <br> **Towards Efficient Multimodal Large Language Models: A Survey on Token Compression** <br> Linli Yao, Long Xing, Yang Shi, Sida Li, Yuanxin Liu, Yuhao Dong, Yi-Fan Zhang, Lei Li, Qingxiu Dong, Xiaoyi Dong, Qidong Huang, Haotian Wang, Feng Wu, Yuanxing Zhang, Pengfei Wan, Zhouchen Lin, Xu Sun| 26.01.12 | Compression Position & <br> Mechanisim | - |
| ![PDF](https://img.shields.io/badge/ISCAS-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2508.13460-b31b1b)](https://arxiv.org/abs/2508.13460)<br>**Revisiting MLLM Token Technology through the Lens of Classical Visual Coding** <br> Jinming Liu, Junyan Lin, Yuntao Wei, Kele Shao, Keda Tao, Jianguo Huang, Xudong Yang, Zhibo Chen, Huan Wang, Xin Jin| 25.08.19| Codec & <br> Token Technology | - |
| ![PDF](https://img.shields.io/badge/TMLR-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2507.20198-b31b1b)](https://arxiv.org/abs/2507.20198v5) [![GitHub](https://img.shields.io/badge/GitHub-Awesome--Multimodal--Token--Compression-white?logo=github)](https://github.com/cokeshao/Awesome-Multimodal-Token-Compression)  <br >**A Survey of Token Compression for Efficient Multimodal Large Language Models** <br> Kele Shao, Keda Tao, Kejia Zhang, Sicheng Feng, Mu Cai, Yuzhang Shang, Haoxuan You, Can Qin, Yang Sui, Huan Wang | 25.07.27 | Modality & <br> Mechanisim | Modality-centric|
| [![Preprint](https://img.shields.io/badge/arXiv-2505.18227-b31b1b)](https://arxiv.org/abs/2505.18227) [![GitHub](https://img.shields.io/badge/GitHub-Awesome--Collection--Token--Reduction-white?logo=github)](https://github.com/ZLKong/Awesome-Collection-Token-Reduction) <br> **Token Reduction Should Go Beyond Efficiency in Generative Models -- From Vision, Language to Multimodality** <br> Zhenglun Kong, Yize Li, Fanhu Zeng, Lei Xin, Shvat Messica, Xue Lin, Pu Zhao, Manolis Kellis, Hao Tang, Marinka Zitnik| 25.05.23 | Compression operation | Compression<br>Beyond Efficiency |




### Recent Papers (Last 6 Months) <a id="recent"></a>

<!-- Image -->
<details open>
<summary><b>Image (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>

<!-- Video -->
<details open>
<summary><b>Video (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>


<!-- Audio -->
<details open>
<summary><b>Audio</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/ICASSP-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2511.07253-b31b1b)](https://arxiv.org/abs/2511.07253) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/umbertocappellazzo/Omni-AVSR) <br> **Omni-AVSR: Towards Unified Multimodal Speech Recognition with Large Language Models** <br> Umberto Cappellazzo, Xubo Liu, Pingchuan Ma, Stavros Petridis, Maja Pantic | ![Area](https://img.shields.io/badge/Area-Audio--LLM-6f42c1) <br> ![Area](https://img.shields.io/badge/Task-AVSR-white) | ![Cost](https://img.shields.io/badge/Cost-Re--Train-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Rule--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488)| 
| ![PDF](https://img.shields.io/badge/ICASSP-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2511.14293-b31b1b)](https://arxiv.org/abs/2511.14293) <br> **Segmentwise Pruning in Audio-Language Models** <br> Marcel Gibier, Raphaël Duroselle, Pierre Serrano, Olivier Boeffard, Jean-François Bonastre | ![Area](https://img.shields.io/badge/Area-Audio--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488)| 
| [![Preprint](https://img.shields.io/badge/arXiv-2511.20973-b31b1b)](https://arxiv.org/abs/2511.20973) <br> **Towards Audio Token Compression in Large Audio Language Models** <br> Saurabhchand Bhati, Samuel Thomas, Hilde Kuehne, Rogerio Feris, James Glass | ![Area](https://img.shields.io/badge/Area-Audio--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Post--Train-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Rule--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488)| 


</details>


<!-- 3D -->
<details open>
<summary><b>3D</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| [![Preprint](https://img.shields.io/badge/arXiv-2603.05959-b31b1b)](https://arxiv.org/abs/2603.05959) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/VAISR/OVGGT) <br> **OVGGT: O(1) Constant-Cost Streaming Visual Geometry Transformer** <br> Si-Yu Lu, Po-Ting Chen, Hui-Che Hsu, Sin-Ye Jhong, Wen-Huang Cheng, Yung-Yao Chen | ![Area](https://img.shields.io/badge/Area-3D--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Eviction-c2416c) <br> ![Target](https://img.shields.io/badge/Target-KV%20Cache-0d9488) ![Note](https://img.shields.io/badge/Note-Streaming-white)|
| ![PDF](https://img.shields.io/badge/AAAI-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2511.09883-b31b1b)](https://arxiv.org/abs/2511.09883) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/lihengzhang02/HCC-3D) <br> **HCC-3D: Hierarchical Compensatory Compression for 98% 3D Token Reduction in Vision-Language Models** <br> Liheng Zhang, Jin Wang, Hui Li, Bingfeng Zhang, Weifeng Liu | ![Area](https://img.shields.io/badge/Area-3D--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Post--Train-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Resamp-2f9e44) ![Target](https://img.shields.io/badge/Target-Token-0d9488) |

</details>


<!-- Omni -->
<details open>
<summary><b>Omni (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|



</details>


### Published in Recent Conferences (Last 12 months) <a id="conference"></a>


<!-- CVPR 2026 -->
<details open>
<summary><b>CVPR 2026 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/CVPR-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2602.23734-b31b1b)](https://arxiv.org/abs/2602.23699) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/EIT-NLP/UTPTrack) <br> **UTPTrack: Towards Simple and Unified Token Pruning for Visual Tracking** <br> Hao Wu, Xudong Wang, Jialiang Zhang, Junlong Tong, Xinghao Chen, Junyan Lin, Yunpu Ma, Xiaoyu Shen | ![Area](https://img.shields.io/badge/Area-Vision--Encoder-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Re--Train-8b5e3c) ![Level](https://img.shields.io/badge/Level-Encoder-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488)| 
| ![PDF](https://img.shields.io/badge/CVPR-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2508.13305-b31b1b)](https://arxiv.org/abs/2508.13305) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/MinhaoXiong/Prune2Drive) <br> **Prune2Drive: A Plug-and-Play Framework for Accelerating Vision-Language Models in Autonomous Driving** <br> Minhao Xiong, Zichen Wen, Zhuangcheng Gu, Xuyang Liu, Rui Zhang, Hengrui Kang, Jiabing Yang, Junyuan Zhang, Weijia Li, Conghui He, Yafei Wang, Linfeng Zhang | ![Area](https://img.shields.io/badge/Area-3D--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Div--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) |

</details>



<!-- ICLR 2026 -->
<details open>
<summary><b>ICLR 2026 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/ICLR-2026-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2602.23699-b31b1b)](https://arxiv.org/abs/2602.23699) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/EIT-NLP/HiDrop) <br> **HiDrop: Hierarchical Vision Token Reduction in MLLMs via Late Injection, Concave Pyramid Pruning, and Early Exit** <br> Hao Wu, Yingqi Fan, Jinyang Dai, Junlong Tong, Yunpu Ma, Xiaoyu Shen | ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Re--Train-8b5e3c)  ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Op](https://img.shields.io/badge/Op-Skip-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Depth--wise-c2416c)  <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) ![Target](https://img.shields.io/badge/Target-Operation-0d9488)|



</details>


<!-- EMNLP 2025 -->
<details open>
<summary><b>EMNLP 2025 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/EMNLP-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2506.02850-b31b1b)](https://arxiv.org/abs/2506.02850) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/mnyuew/METok) <br> **METok: Multi-Stage Event-based Token Compression for Efficient Long <br> Video Understanding** <br> Mengyue Wang, Shuo Chen, Kristian Kersting, Volker Tresp, Yunpu Ma | ![Area](https://img.shields.io/badge/Area-Video--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) <br> ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) <br> ![Mech](https://img.shields.io/badge/Mech-Metric--based-c2416c) ![Mech](https://img.shields.io/badge/Mech-Rule--based-c2416c) <br> ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) <br> ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) ![Target](https://img.shields.io/badge/Target-Token-0d9488) |



</details>


<!-- NeurIPS 2025 -->
<details open>
<summary><b>NeurIPS 2025 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/NeurIPS-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2503.11187-b31b1b)](https://arxiv.org/abs/2503.11187) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/LunarShen/FastVID) <br> **FastVID: Dynamic Density Pruning for Fast Video Large Language Models**  <br> Leqi Shen, Guoqiang Gong, Tao He, Yifeng Zhang, Pengzhang Liu, Sicheng Zhao, Guiguang Ding | ![Area](https://img.shields.io/badge/Area-Video--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Metric--Based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) |
| ![PDF](https://img.shields.io/badge/NeurIPS-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2503.16980-b31b1b)](https://arxiv.org/abs/2503.16980) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/Hai-chao-Zhang/VQToken) <br> **VQToken: Neural Discrete Token Representation Learning for Extreme Token <br> Reduction in Video Large Language Models** <br> Haichao Zhang, Yun Fu | ![Area](https://img.shields.io/badge/Area-Video--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Post--Train-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Metric--Based-c2416c) <br> ![Op](https://img.shields.io/badge/Op-Enc-2f9e44) ![Target](https://img.shields.io/badge/Target-Token-0d9488) |
| ![PDF](https://img.shields.io/badge/NeurIPS-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2512.06866-b31b1b)](https://arxiv.org/abs/2512.06866) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/yu-lin-li/DyToK) <br> **Less Is More, but Where? Dynamic Token Compression via LLM-Guided Keyframe Prior** <br> Yulin Li, Haokun Gui, Ziyang Fan, Junjie Wang, Bin Kang, Bin Chen, Zhuotao Tian | ![Area](https://img.shields.io/badge/Area-Video--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) |
| ![PDF](https://img.shields.io/badge/NeurIPS-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2410.17434-b31b1b)](https://arxiv.org/abs/2410.17434) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/Vision-CAIR/LongVU) <br> **LongVU: Spatiotemporal Adaptive Compression for Long Video-Language <br> Understanding** <br> Xiaoqian Shen, Yunyang Xiong, Changsheng Zhao, Lemeng Wu, Jun Chen, Chenchen Zhu, <br> Zechun Liu, Fanyi Xiao, Balakrishnan Varadarajan, Florian Bordes, Zhuang Liu, Hu Xu, <br> Hyunwoo J. Kim, Bilge Soran, Raghuraman Krishnamoorthi, Mohamed Elhoseiny, <br> Vikas Chandra | ![Area](https://img.shields.io/badge/Area-Video--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Re--Train-8b5e3c) ![Level](https://img.shields.io/badge/Level-Input-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Simi--based-c2416c) <br> ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) <br> ![Mech](https://img.shields.io/badge/Mech-Simi--based-c2416c) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Rule--Based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) |



</details>


<!-- ICCV 2025 -->
<details open>
<summary><b>ICCV 2025 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/ICCV-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2503.08101-b31b1b)](https://arxiv.org/abs/2503.08101) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/iseri27/tg_gbc) <br> **Accelerate 3D Object Detection Models via Zero-Shot Attention Key Pruning** <br> Lizhen Xu, Xiuxiu Bai, Xiaojun Jia, Jianwu Fang, Shanmin Pang | ![Area](https://img.shields.io/badge/Area-3D--Decoder-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Level](https://img.shields.io/badge/Level-Decoder-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-KV-0d9488) |
| ![PDF](https://img.shields.io/badge/ICCV-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2503.04130-b31b1b)](https://arxiv.org/abs/2503.04130) <br> **STORM: Token-Efficient Long Video Understanding for Multimodal LLMs**  <br> Jindong Jiang, Xiuyu Li, Zhijian Liu, Muyang Li, Guo Chen, Zhiqi Li, De-An Huang, Guilin Liu, <br>Zhiding Yu, Kurt Keutzer, Sungjin Ahn, Jan Kautz, Hongxu Yin, Yao Lu, Song Han, Wonmin Byeon | ![Area](https://img.shields.io/badge/Area-Video--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Re--Train-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Model--Based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) |
| ![PDF](https://img.shields.io/badge/ICCV-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2406.08085-b31b1b)](https://arxiv.org/abs/2406.08085) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/IVGSZ/Flash-VStream) <br> **Flash-VStream: Memory-Based Real-Time Understanding for Long Video Streams** <br> Haoji Zhang, Yiqin Wang, Yansong Tang, Yong Liu, Jiashi Feng, Jifeng Dai, Xiaojie Jin | ![Area](https://img.shields.io/badge/Area-Video--LLM-6f42c1) <br> ![Note](https://img.shields.io/badge/Note-Streaming-white) <br> ![Note](https://img.shields.io/badge/Note-Memory-white) | ![Cost](https://img.shields.io/badge/Cost-Post--Train-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Metric--Based-c2416c) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Simi--Based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488)  |
| ![PDF](https://img.shields.io/badge/ICCV-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2403.15388-b31b1b)](https://arxiv.org/abs/2403.15388) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/42Shawn/LLaVA-PruMerge) <br> **LLaVA-PruMerge: Adaptive Token Reduction for Efficient Large Multimodal Models** <br> Yuzhang Shang, Mu Cai, Bingxin Xu, Yong Jae Lee, Yan Yan | ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Cost](https://img.shields.io/badge/Cost-Re--Train-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Metric--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) |
| ![PDF](https://img.shields.io/badge/ICCV-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2412.13180-b31b1b)](https://arxiv.org/abs/2412.13180) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/markendo/FEATHER) <br> **Feather the Throttle: Revisiting Visual Token Pruning for Vision-Language Model Acceleration** <br> Mark Endo, Xiaohan Wang, Serena Yeung-Levy  | ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) |
| ![PDF](https://img.shields.io/badge/ICCV-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2412.01818-b31b1b)](https://arxiv.org/abs/2412.01818) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/Theia-4869/VisPruner) <br> **Beyond Text-Visual Attention: Exploiting Visual Cues for Effective <br> Token Pruning in VLMs** <br> Qizhe Zhang, Aosong Cheng, Ming Lu, Renrui Zhang, Zhiyong Zhuo, Jiajun Cao, <br> Shaobo Guo, Qi She, Shanghang Zhang  | ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) ![Mech](https://img.shields.io/badge/Mech-Sim--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) |
| ![PDF](https://img.shields.io/badge/ICCV-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2412.03248-b31b1b)](https://arxiv.org/abs/2412.03248) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/LaVi-Lab/AIM) <br> **AIM: Adaptive Inference of Multi-Modal LLMs via Token Merging and Pruning** <br> Yiwu Zhong, Zhuoming Liu, Yin Li, Liwei Wang  | ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) <br> ![Area](https://img.shields.io/badge/Area-Video--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) <br> ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) <br> ![Mech](https://img.shields.io/badge/Mech-Sim--based-c2416c)  <br> ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) <br>  ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) ![Target](https://img.shields.io/badge/Target-Token-0d9488)  |


</details>



<!-- ICML 2025 -->
<details open>
<summary><b>ICML 2025 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/ICML-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2410.04417-b31b1b)](https://arxiv.org/abs/2410.04417) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/Gumpest/SparseVLMs) <br> **SparseVLM: Visual Token Sparsification for Efficient Vision-Language <br> Model Inference** <br> Yuan Zhang, Chun-Kai Fan, Junpeng Ma, Wenzhao Zheng, Tao Huang, Kuan Cheng, <br> Denis Gudovskiy, Tomoyuki Okuno, Yohei Nakata, Kurt Keutzer, Shanghang Zhang | ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44)  ![Mech](https://img.shields.io/badge/Mech-R--Merge-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) |



</details>



<!-- ACL 2025 -->
<details open>
<summary><b>ACL 2025 (TODO)</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/ACL-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2412.16117-b31b1b)](https://arxiv.org/abs/2412.16117) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/Visual-AI/PruneVid) <br> **PruneVid: Visual Token Pruning for Efficient Video Large Language Models** <br> Xiaohu Huang, Hao Zhou, Kai Han | ![Area](https://img.shields.io/badge/Area-Video--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Rule--Based-c2416c) <br> ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) ![Op](https://img.shields.io/badge/Op-Drop-2f9e44)  <br>  ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) ![Target](https://img.shields.io/badge/Target-Token-0d9488) |
| ![PDF](https://img.shields.io/badge/ACL--findings-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2503.11315-b31b1b)](https://arxiv.org/abs/2503.11315) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/JeongHun0716/MMS-LLaMA) <br> **MMS-LLaMA: Efficient LLM-based Audio-Visual Speech Recognition with Minimal Multimodal Speech Tokens** <br> Jeong Hun Yeo, Hyeongseop Rha, Se Jin Park, Yong Man Ro | ![Area](https://img.shields.io/badge/Area-Audio--LLM-6f42c1) <br> ![Area](https://img.shields.io/badge/Task-AVSR-white) | ![Cost](https://img.shields.io/badge/Cost-Re--Train-8b5e3c) ![Level](https://img.shields.io/badge/Level-Projector-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Rule--based-c2416c) <br> ![Op](https://img.shields.io/badge/Op-Resamp-2f9e44) ![Target](https://img.shields.io/badge/Target-Token-0d9488)| 



</details>


<!-- NAACL 2025 -->
<details open>
<summary><b>NAACL 2025</b></summary>

| Title & Authors & Links | Areas | Tags |
|---|---|---|
| ![PDF](https://img.shields.io/badge/NAACL--Findings-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2503.04982-b31b1b)](https://arxiv.org/abs/2503.04982) <br> **LVLM-Compress-Bench: Benchmarking the Broader Impact of Large Vision-Language <br> Model Compression** <br> Souvik Kundu, Anahita Bhiwandiwalla, Sungduk Yu, Phillip Howard, Tiep Le, <br> Sharath Nittur Sridhar, David Cobbley, Hao Kang, Vasudev Lal | ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) | ![Target](https://img.shields.io/badge/Target-Weight-0d9488) ![Target](https://img.shields.io/badge/Target-KV--Cache-0d9488)| 
| ![PDF](https://img.shields.io/badge/NAACL-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2502.17599-b31b1b)](https://arxiv.org/abs/2502.17599) [![GitHub](https://img.shields.io/badge/GitHub-Code-white?logo=github)](https://github.com/AIoT-MLSys-Lab/MEDA) <br> **MEDA: Dynamic KV Cache Allocation for Efficient Multimodal Long-Context Inference** <br> Zhongwei Wan, Hui Shen, Xin Wang, Che Liu, Zheda Mai, Mi Zhang | ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Train--Free-8b5e3c) ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Op](https://img.shields.io/badge/Op-Agg-2f9e44) ![Mech](https://img.shields.io/badge/Mech-D--Merge-c2416c) <br> ![Target](https://img.shields.io/badge/Target-KV--Cache-0d9488)| 
| ![PDF](https://img.shields.io/badge/NAACL--findings-2025-1f6feb) [![Preprint](https://img.shields.io/badge/arXiv-2501.13652-b31b1b)](https://arxiv.org/abs/2501.13652) <br> **LVPruning: An Effective yet Simple Language-Guided Vision Token Pruning Approach <br> for Multi-modal Large Language Models** <br> Yizheng Sun, Yanze Xin, Hao Li, Jingyuan Sun, Chenghua Lin, Riza Batista-Navarro | ![Area](https://img.shields.io/badge/Area-Image--LLM-6f42c1) | ![Cost](https://img.shields.io/badge/Cost-Post--Train-8b5e3c) ![Level](https://img.shields.io/badge/Level-LLM-f59e0b) <br> ![Op](https://img.shields.io/badge/Op-Drop-2f9e44) ![Mech](https://img.shields.io/badge/Mech-Attn--based-c2416c) <br> ![Target](https://img.shields.io/badge/Target-Token-0d9488) |


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