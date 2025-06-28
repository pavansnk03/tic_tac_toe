# Tic-Tac-Toe Q-Learning Agents

A Python-based implementation and analysis of Q-learning agents playing Tic-Tac-Toe. This repository contains two Jupyter notebooks demonstrating both a single-agent scenario (agent vs. random opponent) and a multi-agent scenario (two Q-learning agents competing against each other).

---

## Table of Contents

1. Overview
2. Features
3. Repository Structure
4. Installation
5. Usage

   * Single-Agent Notebook
   * Multi-Agent Notebook
6. Results & Visualizations
7. Dependencies

---

## Overview

This project demonstrates how reinforcement learning—specifically Q-learning—can be applied to train agents to play Tic-Tac-Toe:

* Single-Agent Notebook: Trains one Q-learning agent against a random opponent.
* Multi-Agent Notebook: Trains two Q-learning agents that alternate play and learn from each other.

Each notebook includes training loops, exploration vs. exploitation strategies, Q-table updates, and performance visualizations.

---

## Features

* Q-Learning Implementation: Core Q-learning algorithm with learning rate, discount factor, and ε-greedy exploration.
* Training Metrics: Tracking of win/loss/draw rates, exploration decay, and Q-value stability.
* Heatmaps: Visualize learned move preferences across board positions.
* Testing Framework: Evaluate trained agents against random or another agent, reporting win/loss/draw statistics.
* Interactive Notebooks: Fully documented Jupyter notebooks allow easy experimentation with hyperparameters.

---

## Repository Structure

```
README.md
single_agent.ipynb   # Single-agent training and evaluation
multi_agent.ipynb    # Multi-agent training and evaluation
requirements.txt     # Python dependencies
```

---

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/pavansnk03/tic-tac-toe.git
   cd tic-tac-toe
   ```
2. Create and activate a virtual environment (optional but recommended):

   ```bash
   python3 -m venv venv
   source venv/bin/activate   # macOS/Linux
   venv\Scripts\activate      # Windows
   ```
3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

### Single-Agent Notebook

1. Open `single_agent.ipynb` in JupyterLab or Jupyter Notebook.
2. Adjust hyperparameters (learning rate, discount factor, episodes) at the top.
3. Run all cells to train the agent and generate plots:

   * Win/Loss/Draw rate curves
   * Exploration decay curve
   * Q-value stability curve
   * Average Q-value heatmap
4. Test the trained agent against a random opponent using the built-in test function.

### Multi-Agent Notebook

1. Open `multi_agent.ipynb`.
2. Set training episodes and exploration decay parameters.
3. Execute cells to train two agents alternately.
4. View:

   * Smoothed win/draw rate plot comparing both agents
   * Exploration decay for each agent
   * Final performance bar chart
   * Heatmaps of learned move preferences
5. Test the trained agents against each other and view results.

---

## Results & Visualizations

Each notebook outputs a series of matplotlib and seaborn plots, including:

* Training Curves: Smoothed rates for wins, losses, and draws.
* Exploration Decay: ε value vs. episodes.
* Q-Value Stability: Average change in Q-values over time.
* Heatmaps: Visualization of preferred moves based on Q-table data.
* Bar Charts: Final test performance counts.

Tip: Modify window sizes or smoothing parameters in the notebook to explore different trends.

---

## Dependencies

All dependencies are listed in `requirements.txt`. Key packages include:

* numpy
* matplotlib
* seaborn
* tqdm
* pandas (if you extend analysis)

---
