# Flappy Bird AI using NEAT Algorithm

## Project Description
This project implements an artificial intelligence that learns to play Flappy Bird using the NEAT (NeuroEvolution of Augmenting Topologies) algorithm. The AI starts with no knowledge of the game and evolves through generations to develop optimal strategies for navigating through pipes.

## Features
- 🐦 NEAT-based neural network evolution
- 🎮 Pygame visualization of the learning process
- 📊 Real-time statistics display (generation count, alive birds, score)
- 🧠 Configurable neural network parameters
- 📈 Fitness tracking and visualization

## Requirements
- Python 3.x
- Pygame
- NEAT-Python
- Graphviz (for network visualization)
- Matplotlib (for statistics plotting)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/neel212p/flappy-bird-ai.git
   cd flappy-bird-ai
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
Run the main script to start the evolution process:
```bash
python flappy_bird.py
```

### Configuration
The NEAT algorithm parameters can be adjusted in the `config-feedforward.txt` file. Key parameters include:
- Population size
- Mutation rates
- Activation functions
- Network topology settings

## How It Works
1. The algorithm starts with a population of birds with random neural networks.
2. Each bird plays the game, with its neural network making jump decisions based on:
   - Current y-position
   - Distance to top pipe
   - Distance to bottom pipe
3. Birds are rewarded for staying alive and passing pipes.
4. The best-performing birds are selected for reproduction.
5. The process repeats for multiple generations, with networks improving over time.

## Results
The AI typically learns to play effectively within 10-20 generations, achieving scores of 50+ consistently.

## Files
- `flappy_bird.py`: Main game and NEAT implementation
- `config-feedforward.txt`: NEAT configuration
- `visualize.py`: Visualization utilities
- `imgs/`: Game assets folder



## Acknowledgments
- NEAT-Python library
- Flappy Bird game concept
- Pygame community


