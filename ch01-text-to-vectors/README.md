# Chapter 1 · Text → numbers → vectors

You'll turn **"The cat sat on"** into the exact table of numbers GPT-2 sends into its first layer, using plain numpy:
token IDs, the embedding table, positions, batches, and how the lookup works as math. Then you do the same on the real dataset we'll
train on later, **TinyStories**: tokenize it, save it as `train.bin` / `val.bin`, and cut real training batches. Needs only **Setup**.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gotherohit/llm-scratch/blob/main/ch01-text-to-vectors/llm_scratch_ch01.ipynb)

`llm_scratch_ch01.ipynb` is the series notebook up to and including this chapter: Setup + chapter 1.

- **Episode:** coming soon
- **Article:** coming soon

[← all chapters](../README.md)
