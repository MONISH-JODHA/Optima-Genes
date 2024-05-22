# Optima-Genes
Genetic algorithms emulate natural selection, where the most suitable individuals in a population reproduce, passing on their genetic traits. The fitness of individuals depends on their performance, such as reaching a target. Genetic algorithms iteratively optimize solutions by guiding evolution toward greater efficiency.


# Genetic Algorithm Simulation with p5.js

This project demonstrates a simple implementation of a genetic algorithm using the p5.js library. The simulation involves a population of "rockets" that evolve over time to reach a target point on the canvas. Each rocket has a DNA sequence that influences its movement, and the population evolves to become more efficient at reaching the target through processes of selection, crossover, and mutation.

## Table of Contents
- [Introduction](#introduction)
- [How It Works](#how-it-works)
  - [Population](#population)
  - [DNA](#dna)
  - [Rocket](#rocket)
  - [Fitness](#fitness)
  - [Selection](#selection)
  - [Crossover](#crossover)
  - [Mutation](#mutation)
- [Setup](#setup)
- [Usage](#usage)
- [License](#license)

## Introduction

Genetic algorithms are optimization techniques inspired by the process of natural selection. This project uses a genetic algorithm to optimize the path of rockets trying to reach a target point. Over successive generations, the rockets' paths improve as the algorithm selects the most successful individuals to reproduce.

## How It Works

### Population

The population consists of multiple rockets, each with a unique DNA sequence. The population evolves over time, with each rocket being evaluated based on its performance (how close it gets to the target).

### DNA

DNA is represented as an array of vectors. Each vector applies a force to the rocket at each frame, influencing its movement. The DNA sequence determines the rocket's behavior.

### Rocket

Each rocket has:
- Position
- Velocity
- Acceleration
- DNA sequence

The rocket's movement is influenced by its DNA, and its performance is evaluated based on how close it gets to the target.

### Fitness

Fitness is a measure of how well a rocket performs. It is calculated based on the distance from the rocket to the target. Rockets that reach the target or get closer to it have higher fitness scores.

### Selection

Selection involves choosing the most fit individuals to reproduce. The mating pool is created based on the fitness of each rocket, with more fit rockets having a higher chance of being selected.

### Crossover

Crossover combines the DNA of two parents to create a child. This process involves taking a portion of DNA from each parent to produce a new DNA sequence for the child.

### Mutation

Mutation introduces random changes to the DNA sequence, ensuring genetic diversity. This prevents the population from stagnating and helps explore a wider range of solutions.

## Setup

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/genetic-algorithm-p5js.git
   cd genetic-algorithm-p5js
   ```

2. **Include p5.js:**
   Ensure that you have an internet connection to load p5.js from a CDN, or download and include p5.js in your project directory.

## Usage

1. **Open `index.html` in a web browser:**
   This will start the simulation and display the rockets evolving over time.

2. **Observe the simulation:**
   - The target is displayed as a small ellipse on the canvas.
   - Rockets are represented as rectangles that try to reach the target.
   - Over successive generations, you should see the rockets getting better at reaching the target.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.



