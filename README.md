# Pirate Agent Pathfinding with Deep Q-Learning

## Reflection

### Work Done on the Project

**Provided Code**: I was given an incomplete Python script that included the maze definition (an 8x8 numpy array), visualization functions, game logic, a neural network model builder, and a partial Q-training function with pseudocode for the training loop.  The `TreasureMaze` and `GameExperience` classes were also provided, handling the environment and experience replay, respectively.

**Code Created**: I completed the `qtrain` function by implementing the deep Q learning algorithm based on the provided pseudocode. This involved:
- Initializing the training loop for up to 1500 epochs.
- Randomly selecting a starting cell and resetting the maze.
- Implementing an epsilon greedy policy for action selection.
- Executing actions, storing episodes in the experience replay buffer, and training the neural network with a batch of fifty experiences.
- Updating win history, calculating win rate, and adjusting epsilon when the win rate exceeded 0.9.
- Logging training metrics and stopping when a 100% win rate was achieved.


### Connection to Computer Science

**What Do Computer Scientists Do and Why Does It Matter?**  
Computer scientists design, develop, and analyze algorithms and systems to solve complex problems efficiently, from optimizing navigation in games to advancing medical diagnostics in the health industry.  Their work matters because it drives technological innovation, improves quality of life, and addresses global challenges like climate modeling or cybersecurity.

**How Do I Approach a Problem as a Computer Scientist?**  
As a computer scientist, I approach problems systematically.  I define the problem (pathfinding to the treasure), break it into components (state representation, action selection, learning), use appropriate tools (deep Q learning, neural networks), and iterate through design, implementation, and testing.

**What Are My Ethical Responsibilities to the End User and the Organization?**  
My ethical responsibilities include ensuring the agent performs reliably without misleading users.  I must also consider fairness in game design, ensuring the AI doesn’t make the game unfairly difficult for human players.  Transparency is key.  Documenting the algorithm’s limitations helps manage user expectations.
