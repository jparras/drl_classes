# DRL codes
Collection of exercises and minimal DRL implementations used for teaching. All algorithms are coded using Torch. Note that these algorithms are for pedagogical purposes, and hence, they include minimal implementation tricks, as the purpose of this code is to have a clear view on how DRL codes are implemented (thus, the performance of these codes may be low compared to state-of-the-art implementations as Stable Baselines 3).

## Basic methods
The following examples and exercises correspond to some basic ideas needed to understand the basics of RL:
* [Multi-armed bandit](/basics/multi_armed_bandit.ipynb), which is devoted to implementing the epsilon-greedy algorithm, and how to use it to solve the multi-armed bandit problem.
* [Stationary distribution of an MP](/basics/stationary_distribution_MP.ipynb), which is devoted to computing the stationary distribution of a Markov Process (MP).
* [Gym interface example](/basics/cliff_gym.ipynb), which is devoted to showing how to use the Gym interface to create your own RL environments.
* [Bellman fixed point for PE](/basics/bellman_PE.ipynb), which is devoted to implementing the Bellman fixed point equations for policy evaluation (PE) in a simple MDP.
* [Bellman fixed point for PE in a Random Walk](/basics/bellman_PE_rw.ipynb), is similar to the previous code, but using a Random Walk with terminal states as the MDP.
* [Bellman random Policy Search](/basics/bellman_PS.ipynb), which is devoted to finding the optimal Bellman Policy using random search.
* [Bellman random Policy Search in the Cliff](/basics/bellman_PS_cliff.ipynb), which is similar to the previous code, but using the Cliff problem as the MDP.
* [Optimal policy using Bellman Equations](/basics/bellman_opt.ipynb), which is devoted to finding the optimal policy by solving the Bellman Equations in a simple case of discrete actions.
* [The recycling robot](/basics/recycling_robot.ipynb), which is devoted to finding the optimal policy by solving the Bellman Equations.
* [MDP simple example](/basics/two_state_example.ipynb), which is devoted to showing how to compute the basic elements of an MDP.

## Classic RL
The following examples and exercises correspond to some classic RL algorithms, including iterative methods, tabular methods, and linear function approximation methods:
* [Policy Evaluation](/classical_rl/policy_evaluation.ipynb), which is devoted to implementing the policy evaluation algorithm for a simple MDP.
* [Policy Iteration](/classical_rl/policy_iteration.ipynb), which is devoted to implementing the policy iteration algorithm for a simple MDP.
* [Value Iteration](/classical_rl/value_iteration.ipynb), which is devoted to implementing the value iteration algorithm for a simple MDP.
* [Grid World](/classical_rl/grid_world.ipynb), which is devoted to review the iterative methods (PE, PI, VI) in a Grid World problem.
* [Every-visit Monte-Carlo](/classical_rl/monte_carlo_rw.ipynb), which is devoted to implementing the every-visit Monte-Carlo algorithm for a simple MDP.
* [Off-policy Monte-Carlo via Importance Sampling](/classical_rl/monte_carlo_rw_off.ipynb), which is devoted to implementing the off-policy Monte-Carlo algorithm using Importance Sampling for a simple MDP.
* [Monte Carlo and Temporary Difference in a simple MDP](/classical_rl/mc_td_two_state.ipynb), which is an example devoted to implementing the Monte Carlo and Temporal Difference algorithms for a simple MDP.
* [Monte Carlo and Temporary Difference in the Cliff](/classical_rl/mc_td_cliff.ipynb), which is an example devoted to implementing the Monte Carlo and Temporal Difference algorithms for the Cliff.
* [Monte Carlo and Temporary Difference in a random walk](/classical_rl/mc_td_rw.ipynb), which is devoted to implementing the Monte Carlo and Temporal Difference algorithms for a random walk.
* [SARSA and Q-learning in a simple MDP](/classical_rl/sarsa_ql_two_state.ipynb), which is an example devoted to implementing the SARSA and Q-learning algorithms for a simple MDP.
* [SARSA and Q-learning in the Cliff](/classical_rl/sarsa_ql_cliff.ipynb), which is devoted to implementing the SARSA and Q-learning algorithms for the Cliff problem .
* [SARSA and Q-learning in a random walk](/classical_rl/sarsa_ql_rw.ipynb), which is devoted to implementing the SARSA and Q-learning algorithms for a random walk.
* [Feature basis for linear approximations](/classical_rl/linear_intro.ipynb), which is devoted to implementing a feature basis for a linear approximation.
* [Model-based prediction using linear approximations](/classical_rl/linear_mb.ipynb), which is devoted to implementing BPE (Bellman Projected Equation), a model-based prediction algorithm using linear approximations.
* [Model-free prediction using linear approximations](/classical_rl/lstd.ipynb), which is devoted to implementing LSTD, a model-free prediction algorithm using linear approximations.
* [Model-free control using linear approximations](/classical_rl/lspi.ipynb), which is devoted to implementing LSPI, a model-free control algorithm using linear approximations.
* [Linear approximation limits](/classical_rl/linear_limits.ipynb), which is an example devoted to showing the limits of linear approximations.

## Model-free DRL
The following examples implement model-free DRL algorithms (all tested on the Cartpole problem):
* [DDQN](/model_free/DDQN_cartpole.ipynb) (Double Deep Q-Networks)
* [VPG](/model_free/VPG_cartpole.ipynb) (Vanilla Policy Gradient)
* [A2C](/model_free/A2C_cartpole.ipynb) (Advantage Actor Critic)
* [TRPO](/model_free/TRPO_cartpole.ipynb) (Trust Region Policy Optimization, note that in this case, we use the implementation of Stable Baselines 3 instead of providing an implementation to show a state-of-the-art library)
* [DDPG](/model_free/DDPG_cartpole.ipynb) (Deep Deterministic Policy Gradient)

## Model-based DRL
For model-based DRL, the only implemented example is [AlphaZero](/model_based/AlphaZero.ipynb) (tested on tic-tac-toe).

## PASD students guide

| Link                                                  | Observations                       |
|-------------------------------------------------------|------------------------------------|
| [Example 7.6](/basics/cliff_gym.ipynb)                | Code for the example in the slides |
| [Example 8.1](/basics/two_state_example.ipynb)        | Code for the example in the slides |
| [Example 8.3](/basics/bellman_PS_cliff.ipynb)         | Code for the example in the slides |
| [Example 8.5](/classical_rl/policy_evaluation.ipynb)  | Homework                           |
| [Example 8.6](/classical_rl/policy_iteration.ipynb)   | Homework                           |
| [Example 8.7](/classical_rl/value_iteration.ipynb)    | Homework                           |
| [Example 9.1](/classical_rl/mc_td_two_state.ipynb)    | Code for the example in the slides |
| [Example 9.2](/classical_rl/mc_td_cliff.ipynb)        | Code for the example in the slides |
| [Example 9.3](/classical_rl/sarsa_ql_two_state.ipynb) | Code for the example in the slides |
| [Example 9.4](/classical_rl/sarsa_ql_cliff.ipynb)     | Homework                           |
| [Example 9.5](/classical_rl/linear_intro.ipynb)       | Homework                           |
| [Example 9.6](/classical_rl/linear_mb.ipynb)          | Homework                           |
| [Example 9.7](/classical_rl/lstd.ipynb)               | Homework                           |
| [Example 9.8](/classical_rl/lspi.ipynb)               | Homework                           |
| [Example 9.9](/classical_rl/linear_limits.ipynb)      | Code for the example in the slides      |
| [Example 9.10](/model_free/DDQN_cartpole.ipynb)       | Code for the example in the slides |
| [Example 9.11](/model_free/VPG_cartpole.ipynb)        | Code for the example in the slides |
| [Example 9.12](/model_free/A2C_cartpole.ipynb)        | Code for the example in the slides |

## REIL students guide

| Link                                                     | Observations                            |
|----------------------------------------------------------|-----------------------------------------|
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
| [Exercise 5.2](/classical_rl/monte_carlo_rw_off.ipynb)   | Exercise to be completed by the student |
| [Exercise 5.3](/classical_rl/mc_td_rw.ipynb)             | Exercise to be completed by the student |
| [Exercise 5.4](/classical_rl/sarsa_ql_rw.ipynb)          | Exercise to be completed by the student |
| [Exercise 5.5](/classical_rl/sarsa_ql_cliff.ipynb)       | Exercise to be completed by the student |
| [Exercise 6.1](/classical_rl/linear_intro.ipynb)         | Exercise to be completed by the student |
| [Exercise 6.2](/classical_rl/linear_mb.ipynb)            | Exercise to be completed by the student |
| [Exercise 6.3](/classical_rl/lstd.ipynb)                 | Exercise to be completed by the student |
| [Exercise 6.4](/classical_rl/lspi.ipynb)                 | Exercise to be completed by the student |
| [Example 7.1](/classical_rl/linear_limits.ipynb)         | Code for the example in the slides      |
| [Example 7.2](/model_free/DDQN_cartpole.ipynb)           | Code for the example in the slides |
| [Example 7.3](/model_free/VPG_cartpole.ipynb)            | Code for the example in the slides |
| [Example 7.4](/model_free/A2C_cartpole.ipynb)            | Code for the example in the slides |
| [Example 7.5](/model_free/TRPO_cartpole.ipynb)           | Code for the example in the slides |
| [Example 7.6](/model_free/DDPG_cartpole.ipynb)           | Code for the example in the slides |
| [Example 7.7](/model_based/AlphaZero.ipynb)              | Code for the example in the slides |

# Execution in Google Colab

The recommended way of executing these codes is to use Google Colab. The simplest way of doing that is to navigate to the code you want to execute, and then replace `github.com` in the URL by `githubtocolab.com`.

A second option is to go to Colab, and in the Open options, select GitHub and add this repository.

And finally, you can also download the code and execute it in your own machine, by installing all required dependencies.

# More websites

If you are interested in DRL and want to keep on learning, it might be worthy checking the following resources:

* [Spinning up in DRL](https://spinningup.openai.com/en/latest/) is an OpenAI webpage devoted to give an in-depth introduction to DRL, as well as a set of papers to learn more advanced topics. Their documentation is well-written, and their [code](https://github.com/openai/spinningup) is also available and worth checking.
* [CleanRL](https://github.com/vwxyzjn/cleanrl) is a project that has developed several implementations of DRL algorithms in a single file, in order to facilitate understanding. Their documentation is nice, and it is a code repository worth checking.
* [Stable Baselines 3](https://github.com/DLR-RM/stable-baselines3) is a high-quality implementation of most DRL algorithms, that is highly recommended if you want to use state-of-the-art implementations of the most popular DRL algorithms. They are a solid alternative to [OpenAI Baselines](https://github.com/openai/baselines).
