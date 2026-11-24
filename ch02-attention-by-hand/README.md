# Chapter 2 · Attention by hand

The rows from chapter 1 start **talking to each other**. You'll run one real GPT-2 attention head (layer 0, head 4) on
**"The cat sat on"** step by step in plain numpy: first the LayerNorm that comes right before it, then queries, keys and values, the `[1, 4, 4]` score table, dividing by 8, the causal mask,
softmax, and the weighted mix. Every step is checked against GPT-2's own numbers. Then the same head on a real **TinyStories** batch
`[8, 64]`, and **TinyGPT** gets its first attention head. Needs **Setup** and the **chapter 1 toolkit** (1.14).

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gotherohit/llm-scratch/blob/main/ch02-attention-by-hand/llm_scratch_ch02.ipynb)

`llm_scratch_ch02.ipynb` is the series notebook up to and including this chapter: Setup + chapters 1-2.

- **Episode:** coming soon
- **Deep dives:** – ([playlist](https://www.youtube.com/playlist?list=PLA-j4gq1nHi4))
- **Article:** coming soon

[← all chapters](../README.md)
