# Chapter 1 · Text → numbers → vectors

You'll turn **"The cat sat on"** into the exact table of numbers GPT-2 sends into its first layer, using plain numpy:
token IDs, the embedding table, positions, batches, and how the lookup works as math. Then you do the same on the real dataset we'll
train on later, **TinyStories**: tokenize it, save it as `train.bin` / `val.bin`, and cut real training batches. Last, you start
**TinyGPT**, our own model in PyTorch, which grows one piece per chapter until we train it. Needs only **Setup**.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gotherohit/llm-scratch/blob/main/ch01-text-to-vectors/llm_scratch_ch01.ipynb)

`llm_scratch_ch01.ipynb` is the series notebook up to and including this chapter: Setup + chapter 1.

- **Episode:** [watch on YouTube](https://youtu.be/IKFiXlc0k-k)
- **Deep dives:** [D1.1](https://youtu.be/25GaBn2QYW4) · D1.2 (soon) · D1.3 (soon) ([playlist](https://www.youtube.com/playlist?list=PLA-j4gq1nHi4))
- **Article:** [read](https://gotherohit.github.io/AIML/series/transformers-from-scratch/01-text-to-vectors/)

[← all chapters](../README.md)
