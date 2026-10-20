---
layout: page
title: Puzzles
permalink: /puzzles/
published: true
---

These are the questions I have been puzzling over lately. Each of them opens up more research questions than I can work through on my own, so if any of them interests you, please [reach out](/contact/). I would love to discuss the details.

### Reverse-engineering "human-specific" cognition with language models

Many cognitive processes have long been thought to be specific to humans. I am interested in using language models to reverse-engineer these processes, and in what the results can tell us about theories of human cognition. One example is the critical period for language: people first exposed to a language late, including deaf signers who first meet sign language late in childhood, rarely reach native-like command of it ([Mayberry & Kluender, 2018](https://doi.org/10.1017/S1366728917000724)), while language models trained the usual way show no such limit ([Constantinescu et al., 2024](https://arxiv.org/abs/2407.19325)).

### What makes a construction learnable, and how do we know a model has learned it?

I study learnability with controlled rearing: training language models on corpora in which a construction is removed or its frequency is changed, and seeing what they can still learn. I have done this for the Chinese *Ba* construction, for English passives (varying their share from 0 to 100%), and for Māori passives. Children learn English passives after actives, and so do language models trained on English ([Leong & Linzen, 2026](https://doi.org/10.1016/j.jml.2026.104751)). Is that because passives are rarer, or because they are morphologically marked? Māori offers a test: there, passives are more frequent than actives and arguably the base form. I would like to know where the balance between frequency and markedness tips, and whether it tips the same way for children.

But how can we know that a model really understands a phenomenon? Minimal pairs only show which of two sentences a model prefers. Open-ended generations are noisier, but potentially more informative, because they show what a model actually produces. How can we draw reliable conclusions from them, instead of confining ourselves to minimal-pair evaluations?

### How should we benchmark what vision-language models understand about sign language?

Linguistic benchmarks for language models, including minimal-pair suites like [ZhoBLiMP](https://github.com/sjtu-compling/ZhoBLiMP), are almost entirely text-based. But multimodal LLMs now take in speech, images, and video, and much of language lives outside of text: tone and prosody, sign and gesture, and the grounding of words in what we see. How should we benchmark what these models know about language in modalities other than text?

Sign languages are the case I keep coming back to, after working as a TA for two sign-language courses taught by [Rachel Mayberry](https://linguistics.ucsd.edu/people/faculty/profiles/rachel-mayberry.html). They are full natural languages whose grammar is spread across the hands, face, and body. Multimodal frontier models show "virtually no understanding" of American Sign Language ([Tanzer, 2025](https://aclanthology.org/2025.naacl-long.314/)). A new minimal-pair benchmark ([Karabüklü et al., 2026](https://arxiv.org/abs/2604.27232)) finds that even a state-of-the-art sign language translation model relies on the hands and often misses information carried by the face and body. What would a minimal-pair benchmark of sign language grammar look like for vision-language models, and what would it take for a model to pass it?

### When should a voice model take its turn?

In conversation, speakers of very different languages avoid both overlapping talk and long silences between turns ([Stivers et al., 2009](https://doi.org/10.1073/pnas.0903616106)). Voice models are moving from pipelines that split speech into turns to full-duplex models that listen and speak at the same time ([Défossez et al., 2024](https://arxiv.org/abs/2410.00037)). Yet a recent evaluation found that spoken dialogue systems sometimes do not know when to speak up, interrupt too aggressively, and rarely backchannel ([Arora et al., 2025](https://arxiv.org/abs/2503.01174)). Which cues should a voice model use to time its turns, such as syntax, prosody, or the listener's backchannels? More broadly, what can linguistics and cognitive science tell us about how people take turns, and how could those insights improve these systems? And should we judge a model's timing by how closely it matches human conversation, or by how well the conversation works for the person talking to it?

### When does a language model communicate in a way people understand?

We usually judge a model's replies by which ones people prefer. But preferring an answer is not the same as understanding it. Psycholinguistics has tools for measuring understanding, such as reading times and comprehension questions, and models of what makes text hard to process, such as surprisal. Both could be used to evaluate model replies directly. One complication: larger language models are worse models of human reading ([Oh, Zhu & Schuler, 2025](https://aclanthology.org/2025.findings-acl.91/); [Lin, Zhu & Schuler, 2026](https://arxiv.org/abs/2505.12196); [Oh & Linzen, 2025](https://arxiv.org/abs/2510.05141)). So a stronger model is not automatically a better stand-in for a human reader. Could we build simulated readers with human-like limits, such as limited memory, that predict what people will understand over a multi-turn conversation? And could we use them to make models clearer?

### Looking ahead

I am also excited to take my research in a more hard-core direction by interfacing it with clinical neural data.
