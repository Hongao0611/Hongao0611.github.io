---
layout: page
title: Resources
permalink: /resources/
published: true
---

### Academic

**ZhoBLiMP:** a systematic assessment of language models with linguistic minimal pairs in Chinese. ZhoBLiMP is a dataset that can be used to probe Chinese linguistic knowledge in language models, especially syntax. To validate ZhoBLiMP, we trained 5 Zh-Pythia models from scratch on original Chinese data.
* **[Dataset](https://github.com/sjtu-compling/ZhoBLiMP):** ZhoBLiMP covers 118 paradigms in 15 high-level linguistic phenomena. It contains 35k minimal pairs that differ in a minimal way to demonstrate a single syntactic or semantic contrast.
* **[Models](https://huggingface.co/collections/SJTU-CL/zh-pythia-6734b40c21823ee4ea28de8f):** The parameters of the Zh-Pythia models correspond to their English counterparts (size: 14M, 70M, 160M, 410M, 1.4B).


**captain-nemo:** a toolkit for running large batches of GPU jobs on the [Nautilus (NRP)](https://nrp.ai) Kubernetes cluster without tripping its fair-use gate. It paces launches by NRP's utilization-violation budget, keeps jobs off faulty nodes, checks job manifests for setup steps that can hang, and produces an hourly health report. It ships as a skill that Claude Code and other coding agents can follow; the scripts also run on their own.
* **[Github](https://github.com/Hongao0611/captain-nemo):** code, quick start, and the lessons learned from running ~700 GPU jobs on Nautilus (MIT license). <!-- TODO(Hongao): verify "~700 GPU jobs"; it is not in the CV or the repo -->


**Information in Mandarin tones:** how much do segmental and pitch (F0) cues each tell us about Mandarin tone? I predicted tones from segmental features, F0 contours, or both, on 1.1M vowels from the AISHELL-1 speech corpus. F0 carried most of the information, and vowel height and rounding added a little more.
* **[Github](https://github.com/Hongao0611/LIGN211-Phonology):** data processing, F0 extraction, and the regression and neural classifiers.


**LanguageTesting:** A pipeline for analyzing students' performance in exams, which takes into account item facility, item discrimination, *B*-index,...
* **[Github](https://github.com/Hongao0611/LanguageTesting):** Github webpage for the tool.
* **[Binder](https://mybinder.org/v2/gh/Hongao0611/LanguageTesting.git/main?labpath=script%2Fanalysis.ipynb):** Binder example for the tool.


**RL Logistics Simulator:** we designed a smart logistics simulator using deep Q-learning (DQN) and Dijkstra's algorithm that can prevent 10% of the traffic jams in Black Friday events via prediction.
* **[Github](https://github.com/Hongao0611/Data-Structure---Project-2)**
* **[PPT](/assets/pdf/ESLogistics/PPT.pdf)**
* **[Manual](/assets/pdf/ESLogistics/AppUsage.pdf)**



### Fun
*(brewing)*