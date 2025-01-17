<div align="center">

# Bayesian Optimization for Iterative Learning (BOIL)


[![Paper](http://img.shields.io/badge/paper-arxiv.2006.07593-B31B1B.svg)](https://arxiv.org/pdf/1909.09593.pdf)
</div>

# Introduction
The performance of deep (reinforcement) learning systems crucially depends on the choice of hyperparameters. Their tuning is notoriously expensive, typically requiring an iterative training process to run for numerous steps to convergence. Traditional tuning algorithms only consider the final performance of hyperparameters acquired after many expensive iterations and ignore intermediate information from earlier training steps. In this paper, we present a Bayesian optimization (BO) approach which exploits the iterative structure of learning algorithms for efficient hyperparameter tuning. We propose to learn an evaluation function compressing learning progress at any stage of the training process into a single numeric score according to both training success and stability. Our BO framework is then balancing the benefit of assessing a hyperparameter setting over additional training steps against their computation cost. We further increase model efficiency by selectively including scores from different training steps for any evaluated hyperparameter set. We demonstrate the efficiency of our algorithm by tuning hyperparameters for the training of deep reinforcement learning agents and convolutional
neural networks. Our algorithm outperforms all existing baselines in identifying optimal hyperparameters in minimal time.


# Visualization
```
demo_plot_BOIL_2d.ipynb
```
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1npEC6F7tjGXiW5nrc7qEc68PNAWf2QQd#scrollTo=t9JbeFHQA7gj)

# Running the algorithms in tuning deep reinforcement learning algorithm
```
demo_BOIL_A2C_Reacher.ipynb 		... for running BOIL on A2C with Reacher-v2
demo_BOIL_A2C_InvertedPendulum.ipynb	... for running BOIL on A2C with InvertedPendulum-v2
demo_BOIL_DDQN_CartPole.ipynb		... for running BOIL on DDQN with CartPole-v0
```
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1wcyCSDhoVGh_AcX3FJRj6gFrk55C9LnO#scrollTo=HGCZqXSvQGIP)


# Dependencies
```
* numpy >= 1.10.0
* scipy==1.4.1
* matplotlib>=3.1.0
* tensorflow==2.8.0
* tensorflow-probability==0.16.0
* sobol-seq>=0.2.0
* gym>=0.5
* scikit-learn >= 1.0.2
* tqdm>=4.64.0
* tabulate>=0.8.7
* mujoco (optional)
```

# Paper and Presentation

* Visit [PDF](https://papers.nips.cc/paper/2020/file/69eba34671b3ef1ef38ee85caae6b2a1-Paper.pdf)
* Video at [Slideslive](https://slideslive.com/38936372/bayesian-optimization-for-iterative-learning?ref=search-presentations-bayesian+optimization+iterative+learning)


# Reference
```
Vu Nguyen, Sebastian Schulze, Michael A. Osborne.  "Bayesian Optimization for Iterative Learning." Advances in Neural Information Processing Systems (NeurIPS), 2020.
```
