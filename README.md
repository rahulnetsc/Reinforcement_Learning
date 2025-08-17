# Reinforcement Learning

Implementations of reinforcement learning algorithms in **Python & PyTorch**. The repository is structured for modularity, and reuse.

---

## 📂 Repository Structure


### Module Functions

- **`chapters/`**  
  Contains per-chapter code, demos, and notebooks. Used to show algorithm behavior in a learning-oriented way.

- **`algos/`**  
  Core algorithm implementations, grouped by family:  
  - `bandits/` – multi-armed bandits (ε-greedy, UCB, Thompson).  
  - `tabular/` – DP, MC, TD, SARSA, Q-learning.  
  - `value_based/` – DQN and extensions.  
  - `policy_gradient/` – REINFORCE, A2C, PPO.  
  - `actor_critic/` – DDPG, TD3, SAC.

- **`common/`**  
  Reusable utilities:  
  - `nets.py` – neural network architectures.  
  - `buffers.py` – replay buffers (basic, prioritized, n-step, GAE).  
  - `schedules.py` – epsilon, learning rate, entropy schedules.  
  - `wrappers.py` – environment wrappers.  
  - `logging.py` – logging and monitoring helpers.  
  - `utils.py` – seeds, device helpers, serialization.

- **`envs/`**  
  Toy MDPs (e.g., Random Walk, Gridworld) and custom environments.  

- **`experiments/`**  
  Experiment configurations (YAML/JSON) for reproducibility.  

- **`scripts/`**  
  CLI entry points for training, evaluation, and plotting results.  

- **`tests/`**  
  Unit and integration tests for correctness (e.g., verifying Bellman backups, loss convergence).  

---

## 🚀 Quickstart

```bash
git clone https://github.com/rahulnetsc/Reinforcement_Learning.git
cd Reinforcement_Learning

python -m venv .venv
source .venv/bin/activate     # Windows: .venv\Scripts\activate
pip install -r requirements.txt

