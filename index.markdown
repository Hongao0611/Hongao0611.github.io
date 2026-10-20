---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<style>
    .float-left {
        float: left;
        margin: 0 15px 15px 0;
        width: 20%;
        height: auto;
    }
</style>

<img src="/assets/images/mypic.jpg" alt="Photo of Hongao Zhu" class="float-left">

I am Hongao Zhu (IPA: /xʊŋ35 ɑʊ35/ /ʈʂu55/, Mandarin: 朱虹翱, pinyin: ZHŪ HÓNG ÁO). [CV] · [Google Scholar] · [GitHub]

I study what makes language easy or hard for people, and use that to evaluate language models. I model human reading with language-model surprisal in English and Chinese, including why larger models can fit human reading *worse* ([ACL Findings 2025](https://aclanthology.org/2025.findings-acl.91/); [EMNLP 2026](https://arxiv.org/abs/2505.12196); [preprint](https://arxiv.org/abs/2610.04898)). I also build controlled tests of what models know ([ZhoBLiMP], TACL 2026), and I check model judgments against human ones: in our [annotation study](https://arxiv.org/abs/2605.17205), the best LLM agreed with human annotators at κ = .79, against a human ceiling of .87. Lately I've been asking how we can tell whether a language model communicates in ways people actually understand.

I am a second-year PhD student in computational linguistics at UC San Diego, advised by [Alex Warstadt] in the LeM🍋N Lab. Before that, I studied at Shanghai Jiao Tong University with [Hai Hu], and since 2024 I have worked with [William Schuler] at Ohio State. I also co-organized the first [ChineseBabyLM Challenge].

### Selected work

- [A Systematic Analysis of the Predictive Power of LM Surprisal in Reading Chinese](https://arxiv.org/abs/2610.04898) · preprint, 2026 (first author) · Surprisal predicts Chinese reading times, but whether bigger models predict better depends on the corpus.
- [Vectors from Larger Language Models Predict Human Reading Time and fMRI Data More Poorly when Dimensionality Expansion is Controlled](https://arxiv.org/abs/2505.12196) · EMNLP 2026 · Controlling for dimensionality, larger models predict reading times and fMRI worse, and the benefit of training vanishes at a few billion parameters on most datasets.
- [The Inverse Scaling Effect of Pre-Trained Language Model Surprisal Is Not Due to Data Leakage](https://aclanthology.org/2025.findings-acl.91/) · Findings of ACL 2025 · Models trained on leakage-free data still show larger models fitting reading times worse.
- [LLMs for Automatic Annotation of Mandarin Narrative Transcripts](https://arxiv.org/abs/2605.17205) · preprint, 2026 (co-first author) · The best LLM agreed with human annotators at κ = .794 (human–human: .872) and cut annotation time by 65%.
- [A Systematic Assessment of Language Models with Linguistic Minimal Pairs in Chinese](https://aclanthology.org/2026.tacl-1.34/) (ZhoBLiMP) · TACL 2026 · 118 paradigms across 15 phenomena; anaphora, quantifiers, and ellipsis stay hard even for 32B-parameter models.

**Tools:** [captain-nemo](https://github.com/Hongao0611/captain-nemo), for running large batches of GPU jobs on the Nautilus (NRP) Kubernetes cluster (MIT license).

**I'm looking for a research internship for summer 2027**, especially on how people understand and interact with language models, on model evaluation, or on computational psycholinguistics. See the [Contact] page.

Curious what I have been thinking about lately? My [recent research puzzles] start with when a language model communicates in a way people understand, and also cover benchmarking sign language and what makes a construction learnable. To know more about me and my research, please visit the [About] page.

[About]: /about/
[Contact]: /contact/
[recent research puzzles]: /puzzles/
[CV]: /assets/pdf/CV.pdf
[Google Scholar]: https://scholar.google.com/citations?user=FHqFfM8AAAAJ&hl=en
[GitHub]: https://github.com/Hongao0611
[Alex Warstadt]: https://alexwarstadt.github.io
[Hai Hu]: http://huhailinguist.github.io/
[William Schuler]: https://www.asc.ohio-state.edu/schuler.77
[ZhoBLiMP]: https://aclanthology.org/2026.tacl-1.34/
[ChineseBabyLM Challenge]: {% post_url 2026-07-12-ChineseBabyLM %}