# 8. Reinforcement Learning

Reinforcement learning is how a program learns by trial and error, like training a dog with treats. An "agent" takes actions in an "environment", gets rewards or penalties, and slowly works out which actions pay off in the long run. It is the method behind game-playing AIs like AlphaGo and is widely used in robotics.

## Key concepts

- agent, environment, state, action, reward
- Markov decision process (MDP)
- policy and value function
- exploration vs. exploitation (epsilon-greedy)
- Q-learning and DQN
- policy gradients

## Resources

Work through these from top to bottom. You don't need to finish every one: stop when the idea clicks, then do the mini-project.

| Title | Type | Level | Why it's good |
|---|---|---|--- |
| [StatQuest: Reinforcement Learning, Essential Concepts](https://www.youtube.com/watch?v=Z-T0iJEXiwM) | Video | Beginner | Gentle, jargon-free first look at agents, rewards and policies. |
| [Hugging Face Deep RL Course: Unit 1](https://huggingface.co/learn/deep-rl-course/unit1/introduction) | Course | Beginner | Best free beginner RL course; readable without an account, with quizzes and Colab labs. |
| [REINFORCEjs: GridWorld TD demo](https://cs.stanford.edu/people/karpathy/reinforcejs/gridworld_td.html) | Interactive | Beginner | Watch Q-values and the policy update live on a grid you can edit. |
| [Gymnasium: Training an Agent (Blackjack Q-learning)](https://gymnasium.farama.org/introduction/train_agent/) | Article | Beginner | Official walkthrough of the Gymnasium loop and a full tabular Q-learning agent. |
| [deep-rl-class: Unit 2 notebook (Q-learning on FrozenLake and Taxi)](https://github.com/huggingface/deep-rl-class/blob/main/notebooks/unit2/unit2.ipynb) | Notebook | Beginner | Code Q-learning from scratch in Colab, step by step. |
| [ML-For-Beginners: Q-Learning lesson notebook](https://github.com/microsoft/ML-For-Beginners/blob/main/8-Reinforcement/1-QLearning/notebook.ipynb) | Notebook | Beginner | Friendly "Peter and the Wolf" grid world with a lesson, assignment and solution. |
| [David Silver: Introduction to RL (DeepMind x UCL)](https://www.youtube.com/playlist?list=PLqYmG7hTraZDM-OYHWgPebj2MfCFzFObQ) | Video | Intermediate | The classic university lecture series; watch lectures 1 to 5 for MDPs to Q-learning. |
| [PyTorch: DQN tutorial on CartPole](https://docs.pytorch.org/tutorials/intermediate/reinforcement_q_learning.html) | Notebook | Intermediate | Short, complete DQN with replay buffer and target network, runnable in Colab. |
| [deep-rl-class: Unit 4 notebook (policy gradient / REINFORCE)](https://github.com/huggingface/deep-rl-class/blob/main/notebooks/unit4/unit4.ipynb) | Notebook | Intermediate | Implements REINFORCE in PyTorch on CartPole; first step beyond value methods. |
| [dennybritz/reinforcement-learning: Q-Learning exercise](https://github.com/dennybritz/reinforcement-learning/blob/master/TD/Q-Learning.ipynb) | Practice | Intermediate | Empty-function exercises with matching solution notebooks. Uses the older Gym API. |

Note: the Hugging Face course can be read and run without signing in; a free Hugging Face account is only needed to upload models and earn the certificate.

## Mini-project

Teach an agent to cross the ice in **`FrozenLake-v1`** from Gymnasium ([environment docs](https://gymnasium.farama.org/environments/toy_text/frozen_lake/)). Write tabular Q-learning with epsilon-greedy exploration, plot reward per episode, then turn on `is_slippery=True` and see how the learned policy changes. Stretch: reuse the same code on [`Taxi-v3`](https://gymnasium.farama.org/environments/toy_text/taxi/).

## Want more?

[Sutton and Barto, RL: An Introduction (free book)](http://incompleteideas.net/book/the-book-2nd.html) · [Mutual Information: RL By the Book playlist](https://www.youtube.com/playlist?list=PLzvYlJMoZ02Dxtwe-MmH4nOB5jYlMGBjr) · [OpenAI Spinning Up: Key Concepts](https://spinningup.openai.com/en/latest/spinningup/rl_intro.html) · [Karpathy: Pong from Pixels](https://karpathy.github.io/2016/05/31/rl/) (policy gradients) · [Pieter Abbeel: Foundations of Deep RL](https://www.youtube.com/playlist?list=PLwRJQ4m4UJjNymuBM9RdmB3Z9N5-0IlY0) · [CleanRL single-file dqn.py](https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn.py) (10,705 stars) · [Stable-Baselines3 quickstart](https://stable-baselines3.readthedocs.io/en/master/guide/quickstart.html) · [d2l.ai: Q-Learning](https://d2l.ai/chapter_reinforcement-learning/qlearning.html) · [handson-ml3: 18 reinforcement learning](https://github.com/ageron/handson-ml3/blob/main/18_reinforcement_learning.ipynb)

---

[← Neural Networks](../07-neural-networks/) · [All topics](../README.md) · [Natural Language Processing →](../09-natural-language-processing/)
