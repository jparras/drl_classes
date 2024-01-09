# DRL codes
Collection of exercises and minimal DRL implementations used for teaching. All algorithms are coded using Torch. Note that these algorithms are for pedagogical purposes, and hence, they include minimal implementation tricks, as the purpose of this code is to have a clear view on how DRL codes are implemented (thus, the performance of these codes may be low compared to state-of-the-art implementations as Stable Baselines 3).

## Basic methods
The following examples and exercises correspond to some basic ideas needed to understand the basics of RL:
* [Multi-armed bandit](/basics/multi_armed_bandit.ipynb), which is devoted to implementing the epsilon-greedy algorithm, and how to use it to solve the multi-armed bandit problem.
* [Stationary distribution of an MP](/basics/stationary_distribution_MP.ipynb), which is devoted to computing the stationary distribution of a Markov Process (MP).
* [Bellman fixed point for PE](/basics/bellman_PE.ipynb), which is devoted to implementing the Bellman fixed point equations for policy evaluation (PE) in a simple MDP.
* [Bellman fixed point for PE in a Random Walk](/basics/bellman_PE_rw.ipynb), is similar to the previous code, but using a Random Walk with terminal states as the MDP.
* [Bellman random Policy Search](/basics/bellman_PS.ipynb), which is devoted to finding the optimal Bellman Policy using random search.
* [Optimal policy using Bellman Equations](/basics/bellman_opt.ipynb), which is devoted to finding the optimal policy by solving the Bellman Equations in a simple case of discrete actions.
* [The recycling robot](/basics/recycling_robot.ipynb), which is devoted to finding the optimal policy by solving the Bellman Equations.

## Classic RL
The following examples and exercises correspond to some classic RL algorithms, including iterative methods, tabular methods, and linear function approximation methods:
* [Policy Evaluation](/classical_rl/policy_evaluation.ipynb), which is devoted to implementing the policy evaluation algorithm for a simple MDP.
* [Policy Iteration](/classical_rl/policy_iteration.ipynb), which is devoted to implementing the policy iteration algorithm for a simple MDP.
* [Value Iteration](/classical_rl/value_iteration.ipynb), which is devoted to implementing the value iteration algorithm for a simple MDP.
* [Grid World](/classical_rl/grid_world.ipynb), which is devoted to review the iterative methods (PE, PI, VI) in a Grid World problem.
* [Every-visit Monte-Carlo](/classical_rl/monte_carlo_rw.ipynb), which is devoted to implementing the every-visit Monte-Carlo algorithm for a simple MDP.
* [Monte Carlo and Temporary Difference](/classical_rl/mc_td_rw.ipynb), which is devoted to implementing the Monte Carlo and Temporal Difference algorithms for a simple MDP.
* [SARSA and Q-learning](/classical_rl/sarsa_ql_rw.ipynb), which is devoted to implementing the SARSA and Q-learning algorithms for a simple MDP.
* [Cliff](/classical_rl/cliff.ipynb), which is devoted to implementing the SARSA and Q-learning algorithms for the Cliff problem .

## Model-free DRL
The following examples implement model-free DRL algorithms (all tested on the Cartpole problem):
* [DDQN](/model_free/DDQN_cartpole.ipynb) (Double Deep Q-Networks)
* [VPG](/model_free/VPG_cartpole.ipynb) (Vanilla Policy Gradient)
* [A2C](/model_free/A2C_cartpole.ipynb) (Advantage Actor Critic)
* [TRPO](/model_free/TRPO_cartpole.ipynb) (Trust Region Policy Optimization, note that in this case, we use the implementation of Stable Baselines 3 instead of providing an implementation to show a state-of-the-art library)
* [DDPG](/model_free/DDPG_cartpole.ipynb) (Deep Deterministic Policy Gradient)

## Model-based DRL
For model-based DRL, the only implemented example is [AlphaZero](/model_based/AlphaZero.ipynb) (tested on tic-tac-toe).

## REIL students guide

| Link                                                     | Observations |
|----------------------------------------------------------| ----------- |
| [Exercise 2.1](/basics/multi_armed_bandit.ipynb)         | Exercise to be completed by the student |
| [Exercise 3.2](/basics/stationary_distribution_MP.ipynb) | Exercise to be completed by the student |
| [Exercise 3.3](/basics/bellman_PE.ipynb)                 | Exercise to be completed by the student |
| [Exercise 3.4](/basics/bellman_PE_rw.ipynb)              | Exercise to be completed by the student |
| [Exercise 3.5](/basics/bellman_PS.ipynb)                 | Exercise to be completed by the student |
| [Exercise 3.6](/basics/bellman_opt.ipynb)                | Exercise to be completed by the student |
| [Exercise 3.7](/basics/recycling_robot.ipynb)            | Exercise to be completed by the student |
| [Exercise 4.1](/classical_rl/policy_evaluation.ipynb)    | Exercise to be completed by the student |
| [Exercise 4.2](/classical_rl/policy_iteration.ipynb)     | Exercise to be completed by the student |
| [Exercise 4.3](/classical_rl/value_iteration.ipynb)      | Exercise to be completed by the student |
| [Exercise 4.4](/classical_rl/grid_world.ipynb)           | Exercise to be completed by the student |
| [Exercise 5.1](/classical_rl/monte_carlo_rw.ipynb)       | Exercise to be completed by the student |
| [Exercise 5.3](/classical_rl/mc_td_rw.ipynb)             | Exercise to be completed by the student |
| [Exercise 5.4](/classical_rl/sarsa_ql_rw.ipynb)          | Exercise to be completed by the student |
| [Exercise 5.5](/classical_rl/cliff.ipynb)                | Exercise to be completed by the student |

# Execution in Google Colab

The recommended way of executing these codes is to use Google Colab. The simplest way of doing that is to navigate to the code you want to execute, and then replace `github.com` in the URL by `githubtocolab.com`.

A second option is to go to Colab, and in the Open options, select GitHub and add this repository.

And finally, you can also download the code and execute it in your own machine, by installing all required dependencies.

# More websites

If you are interested in DRL and want to keep on learning, it might be worthy checking the following resources:

* [Spinning up in DRL](https://spinningup.openai.com/en/latest/) is an OpenAI webpage devoted to give an in-depth introduction to DRL, as well as a set of papers to learn more advanced topics. Their documentation is well-written, and their [code](https://github.com/openai/spinningup) is also available and worth checking.
* [CleanRL](https://github.com/vwxyzjn/cleanrl) is a project that has developed several implementations of DRL algorithms in a single file, in order to facilitate understanding. Their documentation is nice, and it is a code repository worth checking.
* [Stable Baselines 3](https://github.com/DLR-RM/stable-baselines3) is a high-quality implementation of most DRL algorithms, that is highly recommended if you want to use state-of-the-art implementations of the most popular DRL algorithms. They are a solid alternative to [OpenAI Baselines](https://github.com/openai/baselines).
