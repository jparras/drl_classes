# DRL codes
Minimal DRL implementations used for teaching. All algorithms are coded using Torch. Note that these algorithms are for pedagogical purposes, and hence, they include minimal implementation tricks, as the purpose of this code is to have a clear view on how DRL codes are implemented (thus, the performance of these codes may be low compared to state-of-the-art implementations as Stable Baselines 3).

The algorithms implemented for model-free DRL are the following (all tested on the Cartpole problem):
* DDQN (Double Deep Q-Networks)
* VPG (Vanilla Policy Gradient)
* A2C (Advantage Actor Critic)
* TRPO (Trust Region Policy Optimization, note that in this case, we use the implementation of Stable Baselines 3 instead of providing an implementation to show a state-of-the-art library)
* DDPG (Deep Deterministic Policy Gradient)


# Execution in Google Colab

The recommended way of executing these codes is to use Google Colab. The simplest way of doing that is to navigate to the code you want to execute, and then replace `github.com` in the URL by `githubtocolab.com`.

A second option is to go to Colab, and in the Open options, select Github and add this repository.

And finally, you can also download the code and execute it in your own machine, by installing all required dependencies.

# More websites

If you are interested in DRL and want to keep on learning, it might be worthy checking the following resources:

* [Spinning up in DRL](https://spinningup.openai.com/en/latest/) is an OpenAI webpage devoted to give an in-depth introduction to DRL, as well as a set of papers to learn more advanced topics. Their documentation is well-written, and their [code](https://github.com/openai/spinningup) is also available and worth checking.
* [CleanRL](https://github.com/vwxyzjn/cleanrl) is a project that has developed several implementations of DRL algorithms in a single file, in order to facilitate understanding. Their documentation is nice, and it is a code repository worth checking.
* [Stable Baselines 3](https://github.com/DLR-RM/stable-baselines3) is a high-quality implementation of most DRL algorithms, that is highly recommended if you want to use state-of-the-art implementations of the most popular DRL algorithms. They are a solid alternative to [OpenAI Baselines](https://github.com/openai/baselines).
