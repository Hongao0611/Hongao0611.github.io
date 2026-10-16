---
layout: post
title:  "New preprint: does language model surprisal predict reading times in Chinese?"
date:   2026-10-04 12:00:00 -0700
---

Our new preprint, [A Systematic Analysis of the Predictive Power of LM Surprisal in Reading Chinese](https://arxiv.org/abs/2610.04898), is on arXiv. It is joint work with Muxiaoqiao Xu, Yikang Liu, Siyuan Song, Yuxia Wang, Byung-Doh Oh, and Hai Hu.

Surprisal from language models is a reliable predictor of reading times in English, but earlier studies of Chinese found no such effect. Part of the problem is alignment: eye-tracking corpora segment Chinese text into words, language models split it into subword tokens, and the two often disagree. We propose the Shortest Matching Sequence (SMS), an alignment scheme that maps between them.

Using Chinese Pythia models (14M–1.4B parameters) trained from scratch on 30B tokens, we tested surprisal against first fixation duration, gaze duration, and total reading time in three eye-tracking corpora: GECO-CN, HKP, and MECO. We found that:

- Surprisal does predict Chinese reading times.
- Whether bigger and longer-trained models predict better depends on the corpus. They do in GECO-CN, but HKP shows inverse scaling, and so does MECO at the largest model sizes.
- In HKP, checkpoints whose surprisal stays closer to n-gram statistics are better predictors of reading.

<img src="/assets/images/surprisal/dll-across-training.png" alt="Gain in log-likelihood from adding surprisal, across training, for three Chinese eye-tracking corpora and three reading measures" title="Δllh across training" style="width:100%;height:auto;">

*How much adding surprisal improves the fit to reading times (Δllh), across training, for each corpus (columns) and reading measure (rows). Darker lines are larger models.*

The main lesson is that scaling conclusions drawn from one corpus may not hold for another.
