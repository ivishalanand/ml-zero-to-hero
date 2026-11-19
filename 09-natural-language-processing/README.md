# 9. Natural Language Processing

Natural language processing (NLP) is about getting computers to work with human language: reading it, sorting it, translating it and writing it. Computers only understand numbers, so most of NLP is clever ways to turn words into numbers that keep their meaning. It powers search, spam filters, translation and chatbots.

## Key concepts

- tokenization
- bag of words and TF-IDF
- word embeddings (word2vec)
- RNN and LSTM
- text classification
- pretrained models (Hugging Face)

## Resources

Work through these from top to bottom. You don't need to finish every one: stop when the idea clicks, then do the mini-project.

| Title | Type | Level | Why it's good |
|---|---|---|--- |
| [NLP Course For You: Word Embeddings (Lena Voita)](https://lena-voita.github.io/nlp_course/word_embeddings.html) | Article | Beginner | Beautifully illustrated lesson from one-hot vectors to word2vec, with small interactive bits. |
| [AI-For-Beginners: Text Representation notebook](https://github.com/microsoft/AI-For-Beginners/blob/main/lessons/5-NLP/13-TextRep/TextRepresentationPyTorch.ipynb) | Notebook | Beginner | Tokenization, bag of words and TF-IDF in one short PyTorch notebook. |
| [Advanced NLP with spaCy (free interactive course)](https://course.spacy.io/en/) | Course | Beginner | Run code exercises in the browser with no sign-up; despite the name, chapter 1 is beginner level. |
| [StatQuest: Word Embedding and Word2Vec](https://www.youtube.com/watch?v=viZrOnJclY0) | Video | Beginner | Clear, short explanation of how words become vectors. |
| [TensorFlow Embedding Projector](https://projector.tensorflow.org/) | Interactive | Beginner | Fly through real word vectors in 3D and search for a word's nearest neighbours. |
| [StatQuest: Recurrent Neural Networks](https://www.youtube.com/watch?v=AsNTP8Kwu80) | Video | Beginner | Simple worked example of how a network reads a sequence one step at a time. |
| [Understanding LSTM Networks (colah)](https://colah.github.io/posts/2015-08-Understanding-LSTMs/) | Article | Beginner | The famous diagram-by-diagram explanation of LSTM gates. |
| [pytorch-sentiment-analysis: notebooks 1 and 2](https://github.com/bentrevett/pytorch-sentiment-analysis/blob/main/1%20-%20Neural%20Bag%20of%20Words.ipynb) | Notebook | Beginner | Movie review classifier built first with bag of words, then with an RNN. |
| [Hugging Face LLM Course: Chapter 1](https://huggingface.co/learn/llm-course/chapter1/1) | Course | Beginner | Free, no login; use pretrained models in three lines with `pipeline`. [Colab notebook](https://github.com/huggingface/notebooks/blob/main/course/en/chapter1/section3.ipynb). |
| [karpathy/minbpe: build your own tokenizer exercise](https://github.com/karpathy/minbpe/blob/master/exercise.md) | Practice | Intermediate | Four-step guided exercise to write the BPE tokenizer GPT uses, with reference code. |

## Mini-project

Build a movie review sentiment classifier on the **IMDB Large Movie Review** dataset ([`stanfordnlp/imdb`](https://huggingface.co/datasets/stanfordnlp/imdb), 50,000 reviews). First use scikit-learn's `TfidfVectorizer` plus logistic regression as a baseline (see [text feature extraction docs](https://scikit-learn.org/stable/modules/feature_extraction.html)), then try a Hugging Face `pipeline("sentiment-analysis")` on the same test reviews and compare accuracy.

## Want more?

[StatQuest: LSTM](https://www.youtube.com/watch?v=YCzL96nL7j0) · [The Illustrated Word2vec](https://jalammar.github.io/illustrated-word2vec/) · [Tiktokenizer](https://tiktokenizer.vercel.app/) (interactive tokenizer) · [Karpathy: Let's build the GPT Tokenizer](https://www.youtube.com/watch?v=zduSFxRajkE) · [Stanford CS224N Winter 2021 playlist](https://www.youtube.com/playlist?list=PLoROMvodv4rOSH4v6133s9LFPRHjEmbmJ) (intermediate) · [Jurafsky and Martin, Speech and Language Processing (free book)](https://web.stanford.edu/~jurafsky/slp3/) · [NLTK book](https://www.nltk.org/book/) · [fastbook: 10 NLP](https://github.com/fastai/fastbook/blob/master/10_nlp.ipynb) · [handson-ml3: 16 NLP with RNNs and attention](https://github.com/ageron/handson-ml3/blob/main/16_nlp_with_rnns_and_attention.ipynb) · [nn-zero-to-hero: makemore notebooks](https://github.com/karpathy/nn-zero-to-hero/tree/master/lectures/makemore) · [yandexdataschool/nlp_course](https://github.com/yandexdataschool/nlp_course) (10,799 stars, intermediate)

---

[← Reinforcement Learning](../08-reinforcement-learning/) · [All topics](../README.md) · [Transformers →](../10-transformers/)
