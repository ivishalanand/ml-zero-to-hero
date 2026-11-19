# 7. Neural Networks

A neural network is a stack of simple math units ("neurons") that learns patterns from examples instead of following hand-written rules. You show it data, measure how wrong it is, and nudge its numbers to be a little less wrong, thousands of times. Almost everything in modern AI, from image recognition to ChatGPT, is built on this one idea.

## Key concepts

- perceptron and layers (MLP)
- activation functions (ReLU, sigmoid)
- loss function
- backpropagation
- gradient descent and optimizers (SGD, Adam)
- convolution (CNNs)

## Resources

Work through these from top to bottom. You don't need to finish every one: stop when the idea clicks, then do the mini-project.

| Title | Type | Level | Why it's good |
|---|---|---|--- |
| [3Blue1Brown: Neural Networks series](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi) | Video | Beginner | The best visual intuition for layers, gradient descent and backpropagation. Start here. |
| [TensorFlow Playground](https://playground.tensorflow.org/) | Interactive | Beginner | Train a tiny network in the browser and watch layers and activations change the result. |
| [Karpathy: building micrograd (video)](https://www.youtube.com/watch?v=VMj-3S1tku0) | Video | Beginner | Builds backpropagation from scratch in plain Python, one line at a time. |
| [nn-zero-to-hero: micrograd lecture notebooks](https://github.com/karpathy/nn-zero-to-hero/tree/master/lectures/micrograd) | Notebook | Beginner | The exact notebooks from the video above, so you can code along. |
| [karpathy/micrograd: demo.ipynb](https://github.com/karpathy/micrograd/blob/master/demo.ipynb) | Repo | Beginner | A whole autograd engine and MLP in about 150 lines you can read in one sitting. |
| [PyTorch: Learn the Basics](https://docs.pytorch.org/tutorials/beginner/basics/intro.html) | Course | Beginner | Official short path: tensors, datasets, model, autograd, optimizer, saving. |
| [Learn PyTorch: 02 Neural Network Classification](https://github.com/mrdbourke/pytorch-deep-learning/blob/main/02_pytorch_classification.ipynb) | Notebook | Beginner | Hands-on PyTorch MLP with clear plots of why non-linear activations matter. |
| [fastbook: 04 MNIST basics](https://github.com/fastai/fastbook/blob/master/04_mnist_basics.ipynb) | Notebook | Beginner | Builds a digit classifier from pixels up, explaining SGD in plain language. |
| [CNN Explainer](https://poloclub.github.io/cnn-explainer/) | Interactive | Beginner | Click through a live CNN to see convolution, ReLU and pooling on real images. |
| [Learn PyTorch: 02 classification exercises](https://github.com/mrdbourke/pytorch-deep-learning/blob/main/extras/exercises/02_pytorch_classification_exercises.ipynb) | Practice | Beginner | Fill-in-the-blank exercise notebook with solutions available in the same repo. |

## Mini-project

Build a clothing classifier on **Fashion-MNIST** ([dataset](https://huggingface.co/datasets/zalando-datasets/fashion_mnist), also built into `torchvision.datasets.FashionMNIST`). Start with a 2-layer MLP in PyTorch, get above 85% test accuracy, then swap SGD for Adam and add one convolution layer and compare the three results in a small table.

## Want more?

[StatQuest Neural Networks playlist](https://www.youtube.com/playlist?list=PLblh5JKOoLUIxGDQs4LFFD--41Vzf-ME1) · [Nielsen, Neural Networks and Deep Learning ch.1](http://neuralnetworksanddeeplearning.com/chap1.html) · [MLU-Explain: Neural Networks](https://mlu-explain.github.io/neural-networks/) (interactive) · [Distill: Why Momentum Really Works](https://distill.pub/2017/momentum/) (optimizers, intermediate) · [d2l.ai: Multilayer Perceptrons](https://d2l.ai/chapter_multilayer-perceptrons/index.html) · [handson-ml3: 10 neural nets with Keras](https://github.com/ageron/handson-ml3/blob/main/10_neural_nets_with_keras.ipynb) · [AI-For-Beginners: Perceptron notebook](https://github.com/microsoft/AI-For-Beginners/blob/main/lessons/3-NeuralNetworks/03-Perceptron/Perceptron.ipynb)

---

[← Hyperparameter Tuning](../06-hyperparameter-tuning/) · [All topics](../README.md) · [Reinforcement Learning →](../08-reinforcement-learning/)
