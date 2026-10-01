---
layout: page
title: Resources
permalink: /resources/
published: true
---

### Academic

**ZhoBLiMP:** a systematic assessment of language models with linguistic minimal pairs in Chinese. ZhoBLiMP is a dataset that can be used to probe Chinese linguistic knowledge in language models, especially syntax. To validate ZhoBLiMP, we trained 5 Zh-Pythia models from scratch on original Chinese data.
* **[Dataset](https://github.com/sjtu-compling/ZhoBLiMP):** ZhoBLiMP covers 118 paradigms in 15 high-level linguistic phenemena. It contains 35k minimal pairs that differ in a minimal way to demonstrate a single syntactic or semantic contrast.
* **[Models](https://huggingface.co/collections/SJTU-CL/zh-pythia-6734b40c21823ee4ea28de8f):** The parameters of the Zh-Pythia models correspond to their English counterparts (size: 14M, 70M, 160M, 410M, 1.4B).


**captain-nemo:** a toolkit for running large batches of GPU jobs on the [Nautilus (NRP)](https://nrp.ai) Kubernetes cluster without tripping its fair-use gate. It paces launches by NRP's utilization-violation budget, keeps jobs off faulty nodes, checks job manifests for setup steps that can hang, and produces an hourly health report. It ships as a skill that Claude Code and other coding agents can follow; the scripts also run on their own.
* **[Github](https://github.com/Hongao0611/captain-nemo):** code, quick start, and the lessons learned from running ~700 GPU jobs on Nautilus (MIT license).


**LanguageTesting:** A pipeline for analyzing students' performance in exams, which takes into account item facility, item discrimination, *B*-index,...
* **[Github](https://github.com/Hongao0611/LanguageTesting):** Github webpage for the tool.
* **[Binder](https://mybinder.org/v2/gh/Hongao0611/LanguageTesting.git/main?labpath=script%2Fanalysis.ipynb):** Binder example for the tool.


**RL Logistics Simulator:** we implemented a logistics simulator that handles express packages efficiently. The optimation of pricing and transportation strategy was realized with unsupervised reinforcement learning, where extreme scenarios were simulated multiple times before convergence.
* **[Github](https://github.com/Hongao0611/Data-Structure---Project-2)**
* **[PPT](/assets/pdf/ESLogistics/PPT.pdf)**
* **[Manuel](/assets/pdf/ESLogistics/AppUsage.pdf)**



### Fun
*(brewing)*