# Contexutal-Bandit

# Part 0: [Simple Reinforcement Learning with Tensorflow Part 0: Q-Learning with Tables and Neural Networks](https://medium.com/emergent-future/simple-reinforcement-learning-with-tensorflow-part-0-q-learning-with-tables-and-neural-networks-d195264329d0)

Unlike policy gradient methods, which attempt to learn functions which directly map an observation to an action, Q-Learning attempts to learn the value of being in a given state, and taking a specific action there


# Part 1: [Simple Reinforcement Learning in Tensorflow: Part 1 - Two-armed Bandit](https://medium.com/@awjuliani/super-simple-reinforcement-learning-tutorial-part-1-fd544fab149)

### **Two-Armed Bandit**

Different actions yield different rewards. For example, when looking for treasure in a maze, going left may lead to the treasure, whereas going right may lead to a pit of snakes.

**policy**: learn which rewards we get for each of the possible actions, and ensuring we chose the optimal ones. 
 
**value functions**: instead of learning the optimal action in a given state, the agent learns to predict how good a given state or action will be for the agent to be in.

### **Policy Gradient**

Once our agent has taken an action, it then receives a reward of either 1 or -1. With this reward, we can then make an update to our network using the policy loss equation:

`Loss = -log(π)*A`

A is advantage, and is an essential aspect of all reinforcement learning algorithms. Intuitively it corresponds to how much better an action was than some baseline. `π` is the policy. In this case, it corresponds to the chosen action’s weight.


# Part 1.5: [Simple Reinforcement Learning with Tensorflow Part 1.5: Contextual Bandits](https://medium.com/emergent-future/simple-reinforcement-learning-with-tensorflow-part-1-5-contextual-bandits-bff01d1aad9c)

There are states, but they aren’t determined by the previous states or actions. Additionally, we won’t be considering delayed rewards

![Picture](https://cdn-images-1.medium.com/max/2600/1*3NziBtrANN6UVltplxwaGA.png)

Above: Multi-armed bandit problem, where only action effect reward. Middle: Contextual bandit problem, where state and action effect reward. Bottom: Full RL problem, where action effects state, and rewards may be delayed in time.

# [Contextual Bandits and Reinforcement Learning](https://towardsdatascience.com/contextual-bandits-and-reinforcement-learning-6bdfeaece72a)
