---
layout: post
title:  "ZhoBLiMP is published in TACL"
date:   2026-05-04 12:00:00 -0700
---

The final version of [ZhoBLiMP](https://aclanthology.org/2026.tacl-1.34/), the Chinese minimal-pair benchmark I helped build in Hai Hu's lab at Shanghai Jiao Tong University, is now out in *Transactions of the Association for Computational Linguistics* (vol. 14, pp. 755–771). I first wrote about it when the preprint came out in [November 2024]({% post_url 2024-11-09-ZhoBLiMP %}).

ZhoBLiMP has 118 paradigms covering 15 phenomena, from topicalization to the *Ba* construction, and comes with a suite of Chinese language models trained from scratch. The published version adds a new metric, sub-linear length normalized log-probabilities (SLLN-LP). The two sentences in a Chinese minimal pair often differ in length, which biases a direct comparison of their log-probabilities. SLLN-LP reduces this bias on ZhoBLiMP, as well as on the English BLiMP and the Japanese JBLiMP. Measured this way, anaphora, quantifiers, and ellipsis remain hard for models with up to 32B parameters.

<img src="/assets/images/zhoblimp/phenomena.png" alt="Linguistic phenomena covered in ZhoBLiMP" title="Phenomena covered in ZhoBLiMP" style="width:100%;height:auto;">

Many thanks to my co-authors.
