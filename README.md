# Minesweeper AI

An AI-powered Minesweeper solver built with Python and Pygame. The project demonstrates knowledge-based reasoning by combining logical inference, constraint propagation, and probabilistic decision-making to solve the game autonomously.

## Overview

This project explores how Artificial Intelligence can reason under uncertainty using the classic Minesweeper game. Rather than relying on brute force, the AI builds a knowledge base of logical constraints derived from revealed cells and continuously updates its understanding of the board.

Using logical inference, the AI identifies cells that are guaranteed to be safe or contain mines. When deterministic reasoning is no longer sufficient, it estimates the probability of each unknown cell containing a mine and selects the move with the lowest risk.

## Features

* AI capable of solving Minesweeper autonomously
* Knowledge base for storing game constraints
* Logical inference using propositional reasoning
* Constraint propagation to infer new information
* Automatic identification of safe cells and mines
* Probabilistic move selection when no guaranteed move exists
* Interactive graphical interface built with Pygame

## Technologies Used

* Python
* Pygame
* Artificial Intelligence
* Knowledge-Based Systems
* Constraint Satisfaction
* Logical Inference
* Probabilistic Reasoning

## How It Works

The AI maintains a knowledge base containing logical sentences about the board.

For every revealed cell, it records:

* The neighboring unrevealed cells
* The number of mines among those neighbors

Using these constraints, the AI repeatedly performs logical inference to:

* Mark cells that must be safe
* Identify cells that must contain mines
* Generate new knowledge by combining existing constraints
* Eliminate redundant information through constraint propagation

When no deterministic move can be inferred, the AI estimates the probability of each unknown cell containing a mine and selects the move with the lowest estimated risk.

## Installation

### Clone the repository

```bash
git clone https://github.com/1amchampion/Minesweeper-AI.git
cd Minesweeper-AI
```

### Create a virtual environment

```bash
python -m venv venv
```

### Activate the virtual environment

**macOS/Linux**

```bash
source venv/bin/activate
```

**Windows**

```bash
venv\Scripts\activate
```

### Install dependencies

```bash
pip install pygame
```

## Running the Project

```bash
python runner.py
```

## What I Learned

This project strengthened my understanding of:

* Knowledge-based Artificial Intelligence
* Logical inference and deductive reasoning
* Constraint propagation
* State representation
* Decision-making under uncertainty
* Probability-based search strategies
* Object-oriented software design
* Building interactive graphical applications with Pygame

## Future Improvements

* Bayesian probability estimation for more accurate move selection
* Advanced constraint optimization techniques
* Performance improvements for larger boards
* Multiple AI difficulty levels
* Interactive visualization of the AI's reasoning process
* Statistical analysis of AI performance across games

## License

This project is open-source and available under the MIT License.
