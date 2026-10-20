---
layout: post
title:  "Findings of the first ChineseBabyLM Challenge"
date:   2026-07-12 12:00:00 -0700
---

The overview paper for the [first ChineseBabyLM Challenge](https://arxiv.org/abs/2607.10745), a shared task at NLPCC 2026 that I co-organized, is now on arXiv. Like the English BabyLM Challenge, it asks how well language models can do when trained from scratch on a developmentally plausible amount of data: here, no more than 102M Mandarin Chinese words ([training corpus](https://huggingface.co/datasets/chinese-babylm-org/babylm-zho-100M)).

Models were scored on three tracks:

- **Natural language understanding:** zero-shot minimal pairs from ZhoBLiMP and XCOMPS-ZH, plus fine-tuning on CLUE tasks.
- **Hanzi:** knowledge of character structure and pronunciation (pinyin), tested with minimal pairs.
- **Cognitive modeling:** how well model representations predict fMRI responses to Mandarin Chinese text.

Eighteen teams submitted 28 models. The winning team used DeBERTa-v2 with an extra pinyin-prediction objective, and encoder-only models (BERT and DeBERTa-v2) took 13 of the 18 ranked spots. This differs from the English BabyLM Challenge, where hybrid causal–masked models such as GPT-BERT did well. The winning team found that adding a GPT-BERT-style causal branch lowered their scores, which they attribute to our evaluation being fully bidirectional.

As an organizer, I helped verify the code for a GPT-BERT baseline. The [evaluation pipeline](https://github.com/SiyuanSong2004/chinese-babylm-eval-pipeline) is open source. ZhoBLiMP, which I helped build at Shanghai Jiao Tong University, is one of the NLU tasks.
