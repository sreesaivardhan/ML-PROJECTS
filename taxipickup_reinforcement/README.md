# Taxi-v3 Reinforcement Learning Using Q-Learning  

## Overview  
This project implements **Q-Learning**, a fundamental **Reinforcement Learning** algorithm, to train an agent to navigate the **Taxi-v3** environment from **OpenAI Gym**. The agent learns to efficiently pick up and drop off passengers while maximizing rewards.  

## Reinforcement Learning Approach  
- **Environment**: `Taxi-v3` (A grid-based taxi navigation environment).  
- **Algorithm**: **Q-Learning** (A model-free RL algorithm based on the Bellman Equation).  
- **Exploration vs. Exploitation**: Uses an **epsilon-greedy policy** to balance learning new strategies vs. exploiting known rewards.  

## Steps in the Code  

### 1. Initialize Environment & Q-Table  
- Creates the **Taxi-v3** environment using **OpenAI Gym**.  
- Initializes a **Q-table** (states × actions) with zeros.  

### 2. Define Hyperparameters  
- `alpha` (Learning Rate): Controls how much newly acquired information overrides the old.  
- `gamma` (Discount Factor): Determines the importance of future rewards.  
- `epsilon` (Exploration Rate): Starts high to encourage exploration, then gradually decays.  

### 3. Training the Agent with Q-Learning  
- Runs **10,000 episodes**, where the agent:  
  - Selects actions using an **epsilon-greedy policy**.  
  - Updates the **Q-values** using the **Bellman equation**:  
    \[
    Q(s, a) = (1 - \alpha) \cdot Q(s, a) + \alpha \cdot (r + \gamma \cdot \max Q(s', a'))
    \]
  - Gradually reduces `epsilon` to shift from exploration to exploitation.  

### 4. Testing the Trained Agent  
- Runs **5 test episodes** where the agent follows the optimal learned policy.  
- The agent **renders the environment** to visually show the taxi navigating the grid.  
- The episode terminates when the passenger is successfully dropped off.  

## Technologies Used  
- Python  
- OpenAI Gym (Reinforcement Learning Environment)  
- NumPy (Efficient Array Operations)  

## How to Run  
1. Install dependencies:  
   ```bash
   pip install gym numpy
