# LLM from scratch

Open up a real language model, GPT-2 small, one step at a time: from token IDs to the next word, then how it's trained, how it
writes, and the modern variants. Every number is computed on the real model, and you write each step yourself. From chapter 1 on
we work on the real dataset we'll train on later, [TinyStories](https://huggingface.co/datasets/roneneldan/TinyStories).

This is the notebook for the **Transformers from scratch** series on the YouTube channel [MORE (@go_rohit)](https://www.youtube.com/@go_rohit).

## Chapters
Each chapter builds on the one before. Every chapter has its own folder with a notebook that goes up to that chapter: it has
every earlier chapter too, so the newest chapter's notebook has everything so far. Each episode links to its own chapter's notebook.

| # | Chapter | Notebook | Episode | Article |
|---|---|---|---|---|
| 1 | Text → numbers → vectors: token IDs, the embedding table, positions, batches, 3-D matrix multiplication, the lookup as math, and the TinyStories dataset as train.bin / val.bin | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gotherohit/llm-scratch/blob/main/ch01-text-to-vectors/llm_scratch_ch01.ipynb) · [folder](ch01-text-to-vectors) | coming soon | coming soon |

Coming next: attention by hand, one full layer, the whole model, the loss, training on a batch, backprop, the training loop, picking
the next word, batched inference, modern variants (RMSNorm, RoPE, SwiGLU, grouped-query attention) and mixture of experts.

## How to use it
1. Click **Open in Colab** for the chapter you want.
2. Choose **File → Save a copy in Drive**, so your answers are saved in your own copy.
3. Run **Setup** first, every time you open the notebook.
4. Cells marked **✏️ YOUR TURN** have blanks (`___`) for you to fill in; the cell below prints ✅ when you're right. Solutions are at
   the end of each chapter.

Each chapter ends with a **toolkit** cell that recreates its results, so you can start any chapter without your old answers.

The dataset files, and later the checkpoints, can be saved to your Google Drive (folder `transformer-scratch-yt`), so a
disconnected Colab session can pick up where it left off. Colab asks you to sign in and allow access when you switch that on.

It's a normal Jupyter notebook, so it also runs locally (`pip install numpy torch transformers matplotlib pandas pyarrow`); only the
Drive step is Colab-only.

## Sources
GPT-2 paper (Radford et al., 2019), *Attention Is All You Need* (Vaswani et al., 2017), OpenAI's
[gpt-2](https://github.com/openai/gpt-2) code, Hugging Face Transformers, Karpathy's [nanoGPT](https://github.com/karpathy/nanoGPT),
and *TinyStories* (Eldan & Li, 2023, [arXiv:2305.07759](https://arxiv.org/abs/2305.07759)).
