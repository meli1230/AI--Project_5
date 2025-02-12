# **Pacman Reinforcement Learning**
This project explores **Reinforcement Learning (RL)** techniques, allowing Pacman to learn optimal strategies through interaction with its environment.

## **License**
This project is for educational purposes and follows the **Berkeley AI Pacman Project** framework. <br/>
Please note that the project has been solved in teams of 2:
- Melisa Marian's work is marked under `@Author: Melisa Marian`
- Iulia Ana Anca's work is marked under `#Iulia Anca`

## **Overview**
This project applies **Markov Decision Processes (MDPs)** and **Reinforcement Learning** techniques to train Pacman using **Value Iteration, Q-Learning, and Approximate Q-Learning**.

### **Implemented Algorithms**
- **Value Iteration:** Computes optimal policies using Bellman updates
- **Q-Learning:** A model-free RL algorithm that learns from experience
- **Epsilon-Greedy Policy:** Balances exploration and exploitation in decision-making
- **Approximate Q-Learning:** Uses feature-based representations to generalize learning

## **How to Run the Reinforcement Learning Agents**
Test different RL strategies by running:

- **Value Iteration Agent:**
  ```bash
  python gridworld.py -a value -i 100
  ```
- **Q-Learning Agent in Gridworld:**
  ```bash
  python gridworld.py -a q -k 100
  ```
- **Pacman Q-Learning Agent:**
  ```bash
  python pacman.py -p PacmanQAgent -x 2000 -n 2010 -l smallGrid
  ```
- **Approximate Q-Learning Agent:**
  ```bash
  python pacman.py -p ApproximateQAgent -a extractor=SimpleExtractor -x 50 -n 60 -l mediumGrid
  ```

- Use `-h` for a list of available options:
  ```bash
  python pacman.py -h
  ```
  
- Run the autograder to test the given implementation:
```bash
python autograder.py
```

## **File Structure**
- **`valueIterationAgents.py`** – Implements Value Iteration for solving MDPs
- **`qlearningAgents.py`** – Implements Q-Learning and Approximate Q-Learning
- **`analysis.py`** – Stores answers to theoretical questions
- **`gridworld.py`** – Implements Gridworld simulation
- **`pacman.py`** – Main game engine
- **`util.py`** – Helper functions for RL algorithms
