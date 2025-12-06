# Snake-RL: Reinforcement Learning from Scratch 🐍

![Python](https://img.shields.io/badge/python-gray?logo=python)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy)
![Pygame](https://img.shields.io/badge/Pygame-green?logo=pygame)
![License](https://img.shields.io/badge/license-MIT-grey)

A Reinforcement Learning agent that masters the classic Snake game using **Deep Q-Learning (DQN)**. 

**Key Differentiator:** This project does **not** use ML frameworks like PyTorch or TensorFlow. The Neural Network (backpropagation, optimization, and dense layers) is implemented entirely **from scratch** using NumPy math in `nn.py`.

## 📸 Demo
<p align="center">
  <img src="https://github.com/user-attachments/assets/2cc2e69c-c9a8-4dfe-a133-8ea72ae95661" alt="Snake RL Demo" width="600">
</p>

## 🧠 Key Concepts
* **Custom ML Engine:** A raw implementation of Feed Forward networks and Gradient Descent.
* **Deep Q-Learning:** Using the custom engine to approximate Q-values.
* **Experience Replay:** Storing past game states to train the custom network in mini-batches.

## 🚀 Getting Started

### 1. Installation
Clone the repo and set up the environment:

```bash
git clone [https://github.com/Alireza2317/Snake_RL](https://github.com/Alireza2317/Snake_RL)
cd Snake_RL

# Create virtual env (Optional)
python -m venv env
source env/bin/activate  # Windows: env\Scripts\activate

# Install dependencies (Mainly Pygame & NumPy)
pip install -r requirements.txt
```
### 2. Usage
Run the main application. The agent will start with random moves and progressively learn from the custom neural net.

```bash
python app.py
```
Check configs in `app.py` to tweak hyperparameters like learning rate or epsilon decay.

## 📂 Project Structure

```
.
├── app.py          # Entry point: Orchestrates training loop and game rendering
├── agent.py        # The DQN Agent logic
├── snake.py        # The Game Environment (Pygame logic)
├── nn.py           # ⚠️ CUSTOM ENGINE: Neural Net implementation from scratch
```

## 🛠️ Tech Stack
- Language: Python
- Math Backend: NumPy (Matrix operations)
- Game Engine: Pygame
