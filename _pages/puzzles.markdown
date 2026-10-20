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

I study learnability with controlled rearing: training language models on corpora in which a construction is removed or its frequency is changed, and seeing what they can still learn. I have done this for the Mandarin Chinese *Ba* construction, for English passives (varying their share from 0 to 100%), and for Māori passives. Children learn English passives after actives, and so do language models trained on English ([Leong & Linzen, 2026](https://doi.org/10.1016/j.jml.2026.104751)). Is that because passives are rarer, or because they are morphologically marked? Māori offers a test: there, passives are more frequent than actives and arguably the base form. I would like to know where the balance between frequency and markedness tips, and whether it tips the same way for children.

But how can we know that a model really understands a phenomenon? Minimal pairs only show which of two sentences a model prefers. Open-ended generations are noisier, but potentially more informative, because they show what a model actually produces. How can we draw reliable conclusions from them, instead of confining ourselves to minimal-pair evaluations?

### How should we benchmark what vision-language models understand about sign language?

Linguistic benchmarks for language models, including minimal-pair suites like [ZhoBLiMP](https://github.com/sjtu-compling/ZhoBLiMP), are almost entirely text-based. But multimodal LLMs now take in speech, images, and video, and much of language lives outside of text: tone and prosody, sign and gesture, and the grounding of words in what we see. How should we benchmark what these models know about language in modalities other than text?

Sign languages are the case I keep coming back to, after working as a TA for two sign-language courses taught by [Rachel Mayberry](https://linguistics.ucsd.edu/people/faculty/profiles/rachel-mayberry.html). They are full natural languages whose grammar is spread across the hands, face, and body. Multimodal frontier models show "virtually no understanding" of American Sign Language ([Tanzer, 2025](https://aclanthology.org/2025.naacl-long.314/)). A new minimal-pair benchmark ([Karabüklü et al., 2026](https://arxiv.org/abs/2604.27232)) finds that even a state-of-the-art sign language translation model relies on the hands and often misses information carried by the face and body. What would a minimal-pair benchmark of sign language grammar look like for vision-language models, and what would it take for a model to pass it?

### When should a voice model take its turn?

In conversation, speakers of very different languages avoid both overlapping talk and long silences between turns ([Stivers et al., 2009](https://doi.org/10.1073/pnas.0903616106)). Voice models are moving from pipelines that split speech into turns to full-duplex models that listen and speak at the same time ([Défossez et al., 2024](https://arxiv.org/abs/2410.00037)). Yet a recent evaluation found that spoken dialogue systems sometimes do not know when to speak up, interrupt too aggressively, and rarely backchannel ([Arora et al., 2025](https://arxiv.org/abs/2503.01174)). Which cues should a voice model use to time its turns, such as syntax, prosody, or the listener's backchannels? More broadly, what can linguistics and cognitive science tell us about how people take turns, and how could those insights improve these systems? And should we judge a model's timing by how closely it matches human conversation, or by how well the conversation works for the person talking to it?

### Are humans LLMs?

Language models are often called "stochastic parrots" that stitch together patterns from their training data ([Bender et al., 2021](https://doi.org/10.1145/3442188.3445922)). But how much are we shaped by our own "training": the language we have heard and read all our lives? And now that many people talk to AI assistants every day, do those conversations become part of their training too? There are early signs that they do: words that ChatGPT favors, such as *delve*, have become more frequent in people's unscripted speech ([Yakura et al., 2024](https://arxiv.org/abs/2409.01754)). The influence runs the other way too. Language models talk with people every day, and those conversations can feed into their next round of training. Will that make them more human? And how far are we from the "Singularity", the hypothetical point at which AI becomes capable of recursive self-improvement, each generation building a better successor ([Good, 1966](https://doi.org/10.1016/S0065-2458%2808%2960418-0); [Vinge, 1993](https://ntrs.nasa.gov/citations/19940022856))?

### How can we detect AI impersonation?

AI has made it easy to clone a person's voice or face, and fraudsters have noticed. In one widely reported case, a finance worker in Hong Kong paid out about US$25 million after a video call in which the "colleagues" were deepfakes ([CNN, 2024](https://www.cnn.com/2024/02/04/asia/deepfake-cfo-scam-hong-kong-intl-hnk)). How can we tell, in real time, that a call comes from an AI and not a person, and how can people protect their voices and faces from identity theft? I have worked on detecting AI-generated text ([Zhu & Lei, 2025](https://doi.org/10.1093/llc/fqaf048)); speech and video raise harder versions of the same question. There is a legal side too, which interests me as someone who minored in law at Shanghai Jiao Tong University. The US Federal Communications Commission has ruled that AI-generated voices in robocalls fall under existing rules on artificial voices, so such calls need the recipient's prior consent ([FCC, 2024](https://docs.fcc.gov/public/attachments/FCC-24-17A1.pdf)). The EU AI Act requires AI-generated content to be marked in a machine-readable way, and deepfakes to be disclosed ([EU AI Act, Art. 50](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)). What should the law require of AI systems, and how reliable must detectors be before courts and companies can rely on them?

### Looking ahead

I am also excited to take my research in a more hard-core direction by interfacing it with clinical neural data.
