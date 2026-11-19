# 10. Transformers

The transformer is the neural network design behind ChatGPT, Claude, BERT and almost every modern AI model. Its key trick is "attention": for every word, the model looks at all the other words and decides which ones matter most for understanding it. That lets it read whole passages at once and train on huge amounts of text.

## Key concepts

- attention and self-attention (query, key, value)
- multi-head attention
- positional encoding
- encoder vs. decoder (BERT vs. GPT)
- next-token prediction
- pretraining and fine-tuning

## Resources

Work through these from top to bottom. You don't need to finish every one: stop when the idea clicks, then do the mini-project.

| Title | Type | Level | Why it's good |
|---|---|---|--- |
| [3Blue1Brown: Transformers, the tech behind LLMs](https://www.youtube.com/watch?v=wjZofJX0v4M) then [Attention, step-by-step](https://www.youtube.com/watch?v=eMlx5fFNoYc) | Video | Beginner | Two animated videos that make embeddings and attention click before any code. |
| [The Illustrated Transformer (Jay Alammar)](https://jalammar.github.io/illustrated-transformer/) | Article | Beginner | The standard picture-by-picture walkthrough of the full architecture. |
| [Transformer Explainer](https://poloclub.github.io/transformer-explainer/) | Interactive | Beginner | A real GPT-2 running in your browser; type text and watch attention and predictions. |
| [LLM Visualization (bbycroft)](https://bbycroft.net/llm) | Interactive | Beginner | 3D step-through of every number flowing through a tiny GPT. |
| [Karpathy: Let's build GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY) | Video | Intermediate | Two hours from an empty file to a working GPT; the best coding lecture on the topic. |
| [karpathy/ng-video-lecture (gpt.py)](https://github.com/karpathy/ng-video-lecture/blob/master/gpt.py) | Repo | Intermediate | The finished code from the video: a complete GPT in one roughly 200-line file. |
| [LLMs-from-scratch: ch03 attention notebook](https://github.com/rasbt/LLMs-from-scratch/blob/main/ch03/01_main-chapter-code/ch03.ipynb) | Notebook | Intermediate | Builds self-attention up in small steps; ch04 then assembles a full GPT. |
| [BertViz](https://github.com/jessevig/bertviz) | Repo | Intermediate | See which words attend to which in real BERT and GPT-2, with Colab notebooks. |
| [Hugging Face LLM Course: Chapter 3, fine-tuning](https://huggingface.co/learn/llm-course/chapter3/1) | Notebook | Intermediate | Fine-tune BERT on your own data. [Colab notebook](https://github.com/huggingface/notebooks/blob/main/course/en/chapter3/section3.ipynb). |
| [nanoGPT: train a character-level GPT on Shakespeare](https://github.com/karpathy/nanoGPT/tree/master/data/shakespeare_char) | Practice | Intermediate | Follow the README quick start to train your own GPT in minutes, then change the settings. |

## Mini-project

Train a tiny character-level GPT on **Tiny Shakespeare** ([raw text file](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt), about 1 MB) using `gpt.py` from the Karpathy lecture on a free Colab GPU. Get it to produce Shakespeare-like text, then swap in your own text file (song lyrics, a book from your language) and change the number of layers and heads to see what happens to the loss.

## Want more?

[StatQuest: Transformer Neural Networks](https://www.youtube.com/watch?v=zxQyTK8quyY) · [The Illustrated GPT-2](https://jalammar.github.io/illustrated-gpt2/) · [The Illustrated BERT](https://jalammar.github.io/illustrated-bert/) · [A Visual Guide to Using BERT for the First Time](https://jalammar.github.io/a-visual-guide-to-using-bert-for-the-first-time/) · [The Annotated Transformer](https://nlp.seas.harvard.edu/annotated-transformer/) (7,609 stars, intermediate) · [GPT in 60 Lines of NumPy](https://jaykmody.com/blog/gpt-from-scratch/) · [Karpathy: Intro to Large Language Models](https://www.youtube.com/watch?v=zjkBMFhNj_g) · [Karpathy: Let's reproduce GPT-2](https://www.youtube.com/watch?v=l8pRSuU81PU) (advanced) · [d2l.ai: The Transformer Architecture](https://d2l.ai/chapter_attention-mechanisms-and-transformers/transformer.html) · [LLMs-from-scratch: ch06 fine-tuning for classification](https://github.com/rasbt/LLMs-from-scratch/blob/main/ch06/01_main-chapter-code/ch06.ipynb) · [pytorch-sentiment-analysis: 4 Transformers](https://github.com/bentrevett/pytorch-sentiment-analysis/blob/main/4%20-%20Transformers.ipynb)

---

[← Natural Language Processing](../09-natural-language-processing/) · [All topics](../README.md)
