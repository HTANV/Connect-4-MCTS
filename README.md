# Connect-4-MCTS

![GitHub stars](https://img.shields.io/github/stars/HTANV/Connect-4-MCTS?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/HTANV/Connect-4-MCTS?style=for-the-badge)
![GitHub last commit](https://img.shields.io/github/last-commit/HTANV/Connect-4-MCTS?style=for-the-badge)
![GitHub issues](https://img.shields.io/github/issues/HTANV/Connect-4-MCTS?style=for-the-badge)
![GitHub language Python](https://img.shields.io/github/languages/top/HTANV/Connect-4-MCTS?style=for-the-badge&logo=python)

## Overview

**Connect-4-MCTS** is a Monte Carlo Tree Search (MCTS)-based implementation of the classic **Connect Four** game with an AI agent capable of smart decision-making.  
This repository was developed as part of an **Artificial Intelligence coursework/assignment**, exploring search algorithms in game playing.

The project demonstrates how MCTS can be applied to build a strong AI opponent in a deterministic, turn-based game without requiring handcrafted heuristics.:contentReference[oaicite:0]{index=0}

---

## What It Does

- 🔹 Implements the **Connect Four** game environment on a standard **7×6 board**.
- 🔹 Uses **Monte Carlo Tree Search (MCTS)** to explore future moves and make decisions.
- 🔹 Provides a playable interface to test your agent against the MCTS AI.
- 🔹 Easy to experiment with different simulation parameters for the AI.

This approach allows the AI to estimate winning chances by simulating many future playouts and picking the move with the most promising results.:contentReference[oaicite:1]{index=1}

---

## Features

### Gameplay
- Two-player Connect Four game logic
- Human vs AI or AI vs AI format
- Grid state management and win detection

### AI with Monte Carlo Tree Search
- MCTS implementation with selection, expansion, simulation, and backpropagation phases
- No need for hardcoded heuristics
- Balances exploration and exploitation

---

## Repository Contents

```
Connect-4-MCTS/
├── connect4.py        # Core game mechanics
├── mcts.py            # MCTS algorithm implementation
├── mcts_ai.py         # AI that uses MCTS to select moves
├── main.py            # Game entry point & loop
├── **init**.py
├── .gitattributes
└── README.md

```

---

## Built With

- **Python 3.x** — core language  
- **MCTS (Monte Carlo Tree Search)** — decision-making AI  
- Standard Python modules (no heavy dependencies)

The repository is primarily Python and focused on algorithm logic rather than rendering or graphics.:contentReference[oaicite:2]{index=2}

---

## How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/HTANV/Connect-4-MCTS.git
   cd Connect-4-MCTS
   ```

2. **Run the main program:**
   ```bash
   python main.py
   ```

3. Start playing against the AI or watch two MCTS agents play.

---

## Monte Carlo Tree Search (MCTS) — Brief

MCTS is a game-playing search algorithm that:

1. **Selects** promising nodes in the game tree
2. **Expands** new moves
3. **Simulates** random playouts
4. **Backpropagates** outcomes to update move values

The algorithm improves estimates by balancing exploration of unknown moves and exploitation of high-value ones.([Monte Carlo Tree Search Connect Four][1])

---

## Configuration & Tuning

You can experiment with different MCTS parameters:

| Parameter            | Description                          |
| -------------------- | ------------------------------------ |
| Simulation count     | Number of simulated games per move   |
| Exploration constant | Balances exploration vs exploitation |

Tweaking these values lets you adjust how “deep” or “aggressive” the AI plays.

---

## Contribution

This repo is student-project oriented, but improvements are welcome:

* Better game interface
* Parameterized MCTS
* Alpha-Beta or Minimax comparison
* Visualization of play tree

---

## Acknowledgements

Connect Four is a classic solved board game often used to study AI techniques like MCTS. This repo applies those concepts in an educational implementation context.([GitHub][3])
