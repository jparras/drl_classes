# DRL codes
Minimal DRL implementations used for teaching. All algorithms are coded using Torch. Note that these algorithms are for pedagogical purposes, and hence, they include minimal implementation tricks, as the purpose of this code is to have a clear view on how DRL codes are implemented (thus, the performance of these codes may be low compared to state-of-the-art implementations as Stable Baselines 3).

## Basic methods
The codes in this section correspond to some basic ideas needed to understand the basics of RL:
* [Multi-armed bandit](/basics/multi_armed_bandit.ipynb), which is devoted to implementing the epsilon-greedy algorithm, and how to use it to solve the multi-armed bandit problem.
* [Stationary distribution of an MP](/basics/stationary_distribution_MP.ipynb), which is devoted to computing the stationary distribution of a Markov Process (MP).
* [Bellman fixed point for PE](/basics/bellman_PE.ipynb), which is devoted to implementing the Bellman fixed point equations for policy evaluation (PE) in a simple MDP.
* [Bellman fixed point for PE in a Random Walk](/basics/bellman_PE_rw.ipynb), is similar to the previous code, but using a Random Walk with terminal states as the MDP.
* [Bellman random Policy Search](/basics/bellman_PS.ipynb), which is devoted to finding the optimal Bellman Policy using random search.
* [Optimal policy using Bellman Equations](/basics/bellman_opt.ipynb), which is devoted to finding the optimal policy by solving the Bellman Equations in a simple case of discrete actions.
* [The recycling robot](/basics/recycling_robot.ipynb), which is devoted to finding the optimal policy by solving the Bellman Equations.

## Classic RL

## Model-free DRL
The algorithms implemented for model-free DRL are the following (all tested on the Cartpole problem):
* [DDQN](/model_free/DDQN_cartpole.ipynb) (Double Deep Q-Networks)
* [VPG](/model_free/VPG_cartpole.ipynb) (Vanilla Policy Gradient)
* [A2C](/model_free/A2C_cartpole.ipynb) (Advantage Actor Critic)
* [TRPO](/model_free/TRPO_cartpole.ipynb) (Trust Region Policy Optimization, note that in this case, we use the implementation of Stable Baselines 3 instead of providing an implementation to show a state-of-the-art library)
* [DDPG](/model_free/DDPG_cartpole.ipynb) (Deep Deterministic Policy Gradient)

## Model-based DRL
For model-based DRL, the only implemented code is [AlphaZero](/model_based/AlphaZero.ipynb) (tested on tic-tac-toe).

## REIL students guide

| Exercise | Link | Observations |
|----------| ----------- | ----------- |
| 2.1      | [Multi-armed bandit](/basics/multi_armed_bandit.ipynb)       | Exercise to be completed by the student |
| 3.2      | [Stationary distribution of an MP](/basics/stationary_distribution_MP.ipynb)       | Exercise to be completed by the student |
| 3.3      | [Bellman fixed point for PE](/basics/bellman_PE.ipynb)       | Exercise to be completed by the student |
| 3.4      | [Bellman fixed point for PE in a Random Walk](/basics/bellman_PE_rw.ipynb)       | Exercise to be completed by the student |
| 3.5      | [Bellman random Policy Search](/basics/bellman_PS.ipynb)       | Exercise to be completed by the student |
| 3.6      | [Optimal policy using Bellman Equations](/basics/bellman_opt.ipynb)       | Exercise to be completed by the student |
| 3.7      | [The recycling robot](/basics/recycling_robot.ipynb)       | Exercise to be completed by the student |

# Execution in Google Colab

The recommended way of executing these codes is to use Google Colab. The simplest way of doing that is to navigate to the code you want to execute, and then replace `github.com` in the URL by `githubtocolab.com`.

A second option is to go to Colab, and in the Open options, select Github and add this repository.

And finally, you can also download the code and execute it in your own machine, by installing all required dependencies.

# More websites

If you are interested in DRL and want to keep on learning, it might be worthy checking the following resources:

* [Spinning up in DRL](https://spinningup.openai.com/en/latest/) is an OpenAI webpage devoted to give an in-depth introduction to DRL, as well as a set of papers to learn more advanced topics. Their documentation is well-written, and their [code](https://github.com/openai/spinningup) is also available and worth checking.
* [CleanRL](https://github.com/vwxyzjn/cleanrl) is a project that has developed several implementations of DRL algorithms in a single file, in order to facilitate understanding. Their documentation is nice, and it is a code repository worth checking.
* [Stable Baselines 3](https://github.com/DLR-RM/stable-baselines3) is a high-quality implementation of most DRL algorithms, that is highly recommended if you want to use state-of-the-art implementations of the most popular DRL algorithms. They are a solid alternative to [OpenAI Baselines](https://github.com/openai/baselines).
