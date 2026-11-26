---
permalink: /
title: ""
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

# 🧑 About me

I am a first-year Ph.D. student at [Fudan University (FDU)](https://www.fudan.edu.cn/en/) and [Shanghai Innovation Institute (SII)](https://www.sii.edu.cn/), supervised by Prof. [Cewu Lu](https://www.qingyuan.sjtu.edu.cn/a/Cewu-Lu.html). I received my B.S. in Computer Science and Technology from [Harbin Institute of Technology, Shenzhen (HITSZ)](https://www.hitsz.edu.cn/). Previously, I was a Research Intern in the Qingyun Program with the [Tencent Hunyuan3D team](https://3d.hunyuan.tencent.com/), dedicated to developing next-generation efficient architectures for 3D generation. I am currently a Research Intern at [Noematrix](https://www.noematrix.ai/), building scalable world-action models trained entirely on robot-free data.

<!-- [CV](files/cv_en.pdf)   [简历](files/cv_zh.pdf) -->

My current research interests include:
- **Embodied Intelligence & Robotics**: Anything that helps scale embodied AI
- **3D Vision & Graphics**: Better 3D representation
- **Efficient AI**: Hardware-aligned efficient attention mechanisms for long-context generation
- **Generative AI**: 3D generation, video generation, and world models
  
<br>

# 🔥 News
* 2026.11: 🚀 We released [**RSI-Infra Bench (Preview)**](https://ai4ai-for-anything.github.io/blog/rsi-infra-bench/), evaluating long-horizon AI infrastructure optimization on real training workloads. [Leaderboard](https://ai4ai-for-anything.github.io/blog/rsi-infra-bench/leaderboard/)
* 2026.11: ⚡ We released a **Lite Harness update** for [**ResearchBoost-Agent**](https://github.com/DAGroup-PKU/ResearchBoost-Agent/pull/12), making in-loop evaluation lighter while keeping a separate final correctness and speed check.
* 2026.10: 🚀 We open-sourced [**ResearchBoost-Agent (RBA)**](https://github.com/DAGroup-PKU/ResearchBoost-Agent), an autonomous agent for accelerating AI training code with verified speedups. [More projects]({{ '/' | relative_url }}#projects)
* 2026.10: 🚀 We have open-sourced [**MC-Sparse**](https://github.com/dodododddo/mcsparse)!
* 2026.01:  🎉🎉 1 paper accepted to ICLR 2026 !!!
* 2025.12:  🚀 Selected as Tencent **Qingyun Program** Intern
* 2025.10:  Awarded the **National Scholarship**
* 2025.03:  Awarded the **Tat-Seng Chua Scholarship**
* 2025.03:  🎉🎉 1 paper accepted to CVPR 2025 !!!
<br>

# 💻 Experience
- **Research Intern** \| [Noematrix](https://www.noematrix.ai/) \| 10/2026 – Present, Mentored by [Wendi Chen](https://wendichen.me/)

- **Research Intern (Qingyun Program)** \| [Hunyuan3D, Tencent](https://3d.hunyuan.tencent.com/) \| 12/2025 – 09/2026, Mentored by [Zeqiang Lai](https://zeqiang-lai.github.io/)

- **Visiting Student** \| [IGL-HKUST](https://github.com/IGL-HKUST) \| 12/2024 – 09/2025, Mentored by Prof. [Yuan Liu](https://liuyuan-pal.github.io/)

- **Research Intern** \| HITSZ \| 04/2024 – 11/2024, Mentored by Prof. [Baoquan Zhang](https://zhangbq-research.github.io/) and Prof. [Yunming Ye](https://homepage.hit.edu.cn/yeyunming)
  
<br>

<span class='anchor' id='projects'></span>

# 🚀 Projects

{% include research-projects.html %}

<br>

<span class='anchor' id='publications'></span>

# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><a href='{{ "/images/foresight-forcing-stacked.svg" | relative_url }}' target="_blank" rel="noopener" aria-label="View Foresight Forcing figures at full size"><img src='{{ "/images/foresight-forcing-stacked.svg" | relative_url }}' alt="Foresight Forcing: future-point visualization from Figure 4(b), above six real-world task scenes from Figure 6" width="100%" loading="lazy"></a></div></div>
<div class='paper-box-text' markdown="1">

<a href="https://anson2333.github.io/foresight-forcing/" style="font-size: 22px; color: #483D8B; text-decoration: none">**Foresight Forcing: Learning Spatial Foresight for Robotic Manipulation**</a><br>
<span style="font-size: 18px;">Mishuo Han, Zhixuan Liang, Zhaoyuan Wan, Wendi Chen, **Jiarui Chen**, Xinkai Wang, Yue Ma, Yu Zhou, Junting Chen, Yao Mu, Jun Lv, Chuan Wen, Cewu Lu</span><br>
<span style="font-size: 18px;">[**Website**](https://anson2333.github.io/foresight-forcing/) [**Paper**](https://arxiv.org/abs/2611.30963) [**Code**](https://github.com/anson2333/ForesightForcing)</span>

<span style="font-size: 18px;">We present Foresight Forcing, a world action model that learns spatial transition queries from a frozen 3D teacher to guide robotic manipulation. The policy anticipates task-relevant geometric changes without requiring future observations or the 3D teacher at deployment.</span>

</div>
</div>

<div class='paper-box paper-box--mcsparse' id='mcsparse'><div class='paper-box-image'><div><a href="images/mcsparse-labels.svg" target="_blank" rel="noopener"><img src='images/mcsparse-labels.svg' alt="MC-Sparse: original three-frame diagonal Dense/Ours video comparisons alongside a complete mechanical beetle rendered from Ours at a near-eye-level side angle on a gray studio floor with soft shadows, with staggered Dense and Ours circular magnifications of the marked gear region. Both meshes use identical camera, material, and lighting." width="100%"></a></div></div>
<div class='paper-box-text' markdown="1">

<a href="https://dodododddo.github.io/mcsparse-project-page/" style="font-size: 22px; color: #483D8B; text-decoration: none">**MC-Sparse: Deconstructing and Closing the Dense-Sparse Attention Gap in Diffusion Transformers**</a><br>
<span style="font-size: 18px;">**Jiarui Chen**, Zeqiang Lai†, Jiangshan Wang, Ziheng Ouyang, Ye Huang, Xiangyu Yue, Cewu Lu\*, Chunchao Guo\*</span><br>
<span style="font-size: 18px;">[**Website**](https://dodododddo.github.io/mcsparse-project-page/) [**Paper**](https://arxiv.org/abs/2610.06801) [**Code**](https://github.com/dodododddo/mcsparse)</span>

<span style="font-size: 18px;"> We present MC-Sparse, a training-free, <strong>token-level</strong> sparse attention framework. We analyze three sources of the gap between dense and sparse attention and address each in turn, achieving 1.80× denoising speedup for video generation and 2.32× for 3D asset generation. </span>

</div>
</div>

<div class='paper-box' id='position-forcing'><div class='paper-box-image'><div><img src='images/position-forcing-original.png' alt="Position Forcing Figure 1: recoverable token positions and positional conditioning designs" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<a href="https://ouyangziheng.github.io/Position-Forcing-Page/" style="font-size: 22px; color: #483D8B; text-decoration: none">**Position Forcing: Self-Conditioning 3D Generation**</a><br>
<span style="font-size: 18px;">Ziheng Ouyang, Zeqiang Lai†, **Jiarui Chen**, Jiangshan Wang, Yuhao Wan, Jingbo Gong, Xiangyu Yue, Hengshuang Zhao, Qibin Hou‡, Chunchao Guo‡</span><br>
<span style="font-size: 18px;">[**Website**](https://ouyangziheng.github.io/Position-Forcing-Page/) [**Paper**](https://arxiv.org/abs/2610.10342)</span>

<span style="font-size: 18px;"> We present Position Forcing, which recovers token positions from predicted clean geometry latents and feeds them back as coarse-to-fine spatial guidance during denoising, improving single-stage 3D generation without a separate position generation stage. </span>

</div>
</div>

<div class='paper-box paper-box--compact' id='texzero'><div class='paper-box-image'><div><img src='images/texzero-teaser.png' alt="High-quality 3D textures generated by Tex-Zero" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<a href="https://arxiv.org/abs/2609.34621" style="font-size: 22px; color: #483D8B; text-decoration: none">**Does Native 3D Texture Generation Necessarily Require 3D Assets for Training?**</a><br>
<span style="font-size: 18px;">Jiangshan Wang, Zeqiang Lai†, Jiayi Guo, Xin Yang, Xin Huang, **Jiarui Chen**, Ziheng Ouyang, Chunchao Guo\*, Xiangyu Yue\*</span><br>
<span style="font-size: 18px;">[**Paper**](https://arxiv.org/abs/2609.34621) [**Project**](https://github.com/wangjiangshan0725/Tex-Zero)</span>

<span style="font-size: 18px;"> We present Tex-Zero, a native 3D texture generation framework trained solely on 2D images. By constructing 3D training samples from image patches, it generates detailed 3D textures without using real 3D assets for training. </span>

</div>
</div>

<div class='paper-box paper-box--compact'><div class='paper-box-image'><div><div class="badge">ICML 2026</div><img src='images/e-dit-teaser.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<a href="https://arxiv.org/pdf/2602.13993" style="font-size: 22px; color: #483D8B; text-decoration: none">**Elastic Diffusion Transformer**</a><br>
<span style="font-size: 18px;">Jiangshan Wang, Zeqiang Lai†, **Jiarui Chen**, Jiayi Guo, Hang Guo, Xiu Li, Xiangyu Yue\*, Chunchao Guo\*</span><br>
<span style="font-size: 18px;">[**Paper**](https://arxiv.org/pdf/2602.13993)   [**Code**](https://github.com/wangjiangshan0725/Elastic-DiT)</span>

<span style="font-size: 18px;"> We present Elastic Diffusion Transformer (E-DiT), which achieves ~2× acceleration by dynamically allocating computation (depth and width) based on sample-dependent sparsity. </span>

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICLR 2026</div><img src='images/megs-teaser.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<a href="https://megs-2.github.io/" style="font-size: 22px; color: #483D8B; text-decoration: none">**MEGS²: Memory-Efficient Gaussian Splatting via Spherical Gaussians and Unified Pruning**</a><br>
<span style="font-size: 18px;">**Jiarui Chen\***, Yikeng Chen\*, Yingshuang Zou, Ye Huang, Peng Wang, Yuan Liu†, Yujing Sun†, Wenping Wang</span><br>
<span style="font-size: 18px;">[**Website**](https://megs-2.github.io/) [**Paper**](https://arxiv.org/pdf/2509.07021)   [**Code**](https://github.com/IGL-HKUST/MEGS-2)</span>

<span style="font-size: 18px;"> We present MEGS², a novel 3DGS compression framework that shifts the focus from storage reduction to the critical bottleneck of rendering memory, enabling real-time performance on edge devices and in web browsers. </span>

</div>
</div>

<div class='paper-box paper-box--compact'><div class='paper-box-image'><div><div class="badge">CVPR 2025</div><img src='images/CDRA-teaser.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<a href="https://cvpr.thecvf.com/virtual/2025/poster/33380" style="font-size: 22px; color: #483D8B; text-decoration: none">**Sensitivity-Aware Efficient Fine-Tuning via Compact Dynamic-Rank Adaptation**</a><br>
<span style="font-size: 18px;">Tianran Chen, **Jiarui Chen**, Baoquan Zhang\*, Zhehao Yu, Shidong Chen, Rui Ye, Xutao Li, Yunming Ye</span><br>
<span style="font-size: 18px;">[**Paper**](https://cvpr.thecvf.com/virtual/2025/poster/33380)</span>

<span style="font-size: 18px;"> We present CDRA-SPT, a novel PEFT method that harnesses the complementary strengths of selection-based and reparameterization-based approaches. </span>

</div>
</div>

# 🏆 Honors and Awards

## During My Undergraduate Studies

- National Scholarship, 2025. (Top 0.2% nationwide in China & Top 0.4% in HITSZ)
- Tat-Seng Chua Scholarship, Harbin Institute of Technology, Shenzhen, 2025. (8 undergraduates per year)
- First-Prize Academic Scholarship, Harbin Institute of Technology, Shenzhen, 2024. (Top 5%)
- National Second Prize, 19th Challenge Cup Special Competition, 2024. (Team Leader)
- National First Prize, China Undergraduate Mathematical Contest in Modeling, 2023. (Top 0.5%)


