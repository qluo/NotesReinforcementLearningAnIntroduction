## Introduction

1.1 Reinforcement Learning (RL)

  * RL is learning what to do - how to map situations to actions - so as to maximize a **numerical reward signal**.
  * Two characteristics: (1) trial-and-error search; (2) delayed reward.
  * RL is trying to maximize a reward signal instead of trying to find hidden structure.
  * RL explicitly considers whole problem of a goal-directed agent interacting with an uncertain environment.
  * RL starts wtih a complete, interactive, goal-seeking agent.
  
1.2 Examples
  * All examples involve **interaction** between an active decision-making agent and its enviroment, within which the agent seeks to achieve a **goal** despite *uncertainty* about its environment.
  
1.3 Elements of RL
  * Four main subelements of RL system:
    * **policy** 
      * defines the learning agent's way of behaving at a given time 
      * mapping from perceived states of the environment to actions to be taken when in those states
      * may be a simple function or lookup table or search process
      * core of a RL agent
    * **reward signal**
      * defines the goal in a RL problem
      * agent's sole objective is to maximize the total reward it receives over the long run
      * primary basis for altering the policy
      * may be stochastic functions of the states and the actions taken
    * **value function**
      * specifies what is good in the long run
      * the value of a state is the total amount of reward an agent can expect to accumulate over the future, starting from that state
      * indicates the long-term desirablility of states after taking into account the states that are likely to follow, and the rewards available in those states
      * Rewards are in a sense primary, whereas values, as predictions of rewards, are secondary
      * seek actions that bring about states of highest value, not highest reward
      * most important component of almost all RL algorithms is a method for efficiently estimating values
    * **model of environment** (optional)
      * allows inferences to be made about how the environment will behave
      * *model-based* methods vs *model-free* methods
      * modern RL spans the spectrum from low-level, trial-and-error learning to high-level, deliberative planning
      
1.4 Limitations and Scope
  * heavily relies on the concept of state -- Markov decision processes
  * RL methods in this book are structured around estimating value functions, but not strictly necessary to do so to solve RL problems
  
1.5 An Extended Example: Tic-Tac-Toe
  * Key features of RL methods:
    * emphasis on learning while interacting with an environment
    * clear goal, and correct behavior requires planning or foresight that takes into account delayed effects of one's choices
    
1.6 Summary
  * RL is a computational approach to understanding and automating goal-directed learning and decision making
  * RL uses the formal framework of Markov decision processes to define the interaction between a learning agent and it's environment in terms of states, actions, and rewards
  * The concepts of value and value function are key to most of the RL methods in this book.
  
1.7 Early history of RL
  
