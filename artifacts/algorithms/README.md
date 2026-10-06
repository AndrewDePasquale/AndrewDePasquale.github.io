# Algorithms and Data Structures

## CS 370 Treasure Hunt Intelligent Agent

The artifact selected for the Algorithms and Data Structures category is the Treasure Hunt Game project originally developed in CS 370: Current and Emerging Trends in Computer Science.

The project uses reinforcement learning to train an intelligent agent to navigate a maze and locate a treasure. The application demonstrates algorithmic decision making through exploration and exploitation, experience replay, neural-network training, and performance evaluation.

During CS 499, I enhanced the training process by adding a maximum step limit, training performance metrics, graphs, configurable epsilon decay, and comparison functionality. These enhancements make the agent's training behavior easier to evaluate and provide additional ways to examine the tradeoff between exploration and exploitation.

This section provides both the original artifact and the enhanced version so that the improvements made during the capstone can be reviewed.

## Artifacts

- [Initial CS 370 Treasure Hunt Intelligent Agent](TreasureHuntGame%20(Initial).zip)
- [Enhanced CS 370 Treasure Hunt Intelligent Agent](TreasureHuntGame%20(Enhanced).zip)

## Enhancement Narrative

The artifact selected for this enhancement is the Treasure Hunt Game project originally developed in CS 370: Current and Emerging Trends in Computer Science. The project uses reinforcement learning to train an intelligent agent to navigate a maze and locate a treasure. The agent evaluates its environment, selects valid actions, stores experiences and uses a neural network and experience replay to improve its decision making over time.
  
I selected this artifact because it demonstrates the use of algorithms and data structures in an artificial intelligence application. The original project uses a reinforcement learning algorithm in which the agent balances exploration and exploitation while learning from previous experiences is stored in memory. The experience replay structure stores information about previous states, actions, rewards, next states and game results so that this information can later be sampled during training.
  
For my enhancement, I expanded the training process so its behavior and performance could be evaluated more clearly. I added a maximum step limit to prevent an individual training game from continuing indefinitely. I also created a training history structure that records the epoch, win rate, number of steps, reward, loss and epsilon value. These values are visualized using graphs so that changes in the agent’s performance can be examined throughout training.
  
I also made the epsilon decay rate configurable. This allowed separate training sessions to use different decay settings while maintaining the same training structure. I added a comparison that runs independent models with separate optimizers and plots their win rates. A short functional test confirmed that both configurations execute and can be compared visually. Because the test used only one epoch for each configuration, the results are not sufficient to determine that one decay rate produces better learning performance. Instead, the comparison demonstrates an extensible approach that can be used with longer training runs to evaluate the tradeoff between exploration and exploitation.
  
This enhancement primarily supports outcome three, designing and evaluating solutions using algorithm principles and appropriate computer science practices while considering design tradeoffs. The reinforcement learning algorithm requires decisions about exploration, exploitation, training limits, experience replay and performance evaluation. Making epsilon decay configurable also provides a way to examine how different algorithm parameters influence the learning process.
  
The enhancement also supports outcome four through the use of computing tools and techniques to improve the usefulness of the original solution. TensorFlow/Keras is used for the neural network, NumPy supports numerical operations and experience data, and visualization tools are used to present training metrics. Separating training models and optimizers during the comparison also improved the structure of the experiment by ensuring that each configuration maintains its own training state. These changes are consistent with my original outcome coverage plan, so I do not currently need to change the outcomes selected for this artifact.
  
Enhancing this artifact gave me a better understanding of how reinforcement learning algorithms can be evaluated rather than simply executed. One of the most important things I learned was that the behavior of an algorithm depends on more than whether the program runs successfully. Values such as epsilon, reward, win rate and the number of steps provide information about how the agent is learning and whether changes to the algorithm are having the intended effect.
  
One challenge was managing the training process because reinforcement learning can require significant execution time. This made it important to use a maximum step limit and smaller functional tests while developing the enhancement. I also encountered challenges when creating independent training runs for the epsilon decay comparison. The model and optimizer needed to be associated with the correct training session, and TensorFlow’s function behavior required changes to the training step before separate optimizers could be used successfully. Resolving these issues helped me better understand the relationship between an algorithm’s design and the tools used to implement it.
  
The enhancement also reinforced the importance of interpreting experimental results carefully. A short training run can verify that an algorithm works, but it does not provide enough evidence to conclude that one configuration performs better than another. Longer-controlled experiments would be necessary to make that type of performance comparison. Overall, the enhancement made the original artifact easier to evaluate and expanded its ability to demonstrate algorithmic decision making, reinforcement learning and performance analysis.
