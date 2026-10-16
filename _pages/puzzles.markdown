---
layout: page
title: Research Puzzles
permalink: /puzzles/
published: true
---

These are the questions I have been puzzling over lately. Each of them opens up more research questions than I can work through on my own, so if any of them interests you, please [reach out](/contact/). I would love to discuss the details.

### Benchmarking multimodal LLMs through a linguistic lens

Linguistic benchmarks for language models, including minimal-pair suites like [ZhoBLiMP](https://github.com/sjtu-compling/ZhoBLiMP), are almost entirely text-based. But multimodal LLMs now take in speech, images, and video, and much of language lives outside of text: tone and prosody, sign and gesture, and the grounding of words in what we see. How should we benchmark what these models know about language in modalities other than text?

Sign languages are the case I keep coming back to, after working as a TA for two sign-language courses taught by [Rachel Mayberry](https://linguistics.ucsd.edu/people/faculty/profiles/rachel-mayberry.html). They are full natural languages whose grammar is spread across the hands, face, and body, and models of them have only recently become good enough to test. A new minimal-pair benchmark for American Sign Language models ([Karabüklü et al., 2026](https://arxiv.org/abs/2604.27232)) finds that a state-of-the-art translation model relies on the hands and often misses information carried by the face and body. What would a ZhoBLiMP-style benchmark of sign language grammar look like, and what would it take for a model to pass it?

### What makes a construction learnable?

Children learn English passives after actives, and so do language models trained on English ([Leong & Linzen, 2026](https://doi.org/10.1016/j.jml.2026.104751)). Is that because passives are rarer, or because they are morphologically marked? Māori offers a test: there, passives are more frequent than actives and arguably the base form. In course projects, I trained language models on Māori with passive or active forms filtered out, and on English with the share of passives varied from 0 to 100%. I would like to know where the balance between frequency and markedness tips, and whether it tips the same way for children.

### Reverse-engineering "human-specific" cognition with language models

Many cognitive processes have long been thought to be specific to humans. I am interested in using language models to reverse-engineer these processes, and in what the results can tell us about theories of human cognition. One example is the critical period for language: people first exposed to a language late, including deaf signers who first meet sign language late in childhood, rarely reach native-like command of it ([Mayberry & Kluender, 2018](https://doi.org/10.1017/S1366728917000724)), while language models trained the usual way show no such limit ([Constantinescu et al., 2024](https://arxiv.org/abs/2407.19325)).

### Looking ahead

I am also excited to take my research in a more hard-core direction by interfacing it with clinical neural data.
