# Flappy Bird AI with Neural Networks and Genetic Algorithms

## Overview

This project is a C++ implementation of an AI that plays the game **Flappy Bird** using **neural networks** and **genetic algorithms**. The game loop is built using the **SFML graphics library**, and the AI is trained to play the game by simulating multiple generations using genetic algorithms with elitism. The AI learns by evolving through successive generations until it reaches an optimal strategy to keep the bird alive for as long as possible.

![flappy-footage](https://github.com/user-attachments/assets/cf9498c0-13aa-4bb1-be63-f803fc99b5da)

## Features

- **Flappy Bird Game**: A classic game loop implemented with **SFML**, where the AI controls the bird to avoid obstacles.
- **Neural Networks**: Each bird is controlled by a simple neural network, which decides whether to "flap" based on the current game state (e.g., bird's position, velocity, proximity to pipes).
- **Genetic Algorithm**: The neural networks evolve through generations using genetic algorithms. Each bird's fitness is evaluated by how long it survives in the game.
- **Elitism**: A portion of the top-performing birds are kept for the next generation, ensuring that the best traits are passed on.
- **Automatic Play**: The game plays itself by simulating the AI's evolution through multiple generations, with the birds improving over time.

## Getting Started

### Requirements

- **C++ compiler** (e.g., GCC or MSVC)
- **SFML** graphics library (version X.X or higher)

### Installation

1. Clone the repository or download the project files.
2. Install the SFML library. Follow the instructions for your platform on the [SFML website](https://www.sfml-dev.org/).
3. Open the project in your C++ IDE or use your command line to compile the project.
4. Compile and run the program.

### Controls

- The AI plays the game automatically. You can configure the population size and other parameters within the code.

### How it Works

1. **Population**: The simulation begins with a population of birds, each controlled by a randomly initialized neural network.
2. **Training**: Each bird plays the game and gets a fitness score based on how long it survives.
3. **Genetic Algorithm**: After all birds lose, a new generation is created by selecting the best-performing birds (elitism), and slightly mutating their neural networks.
4. **Repeat**: This process repeats for multiple generations, with the birds gradually improving their ability to play the game.

### Results

The game will automatically play and evolve over multiple generations. The AI will gradually improve at navigating the obstacles, with birds learning how to flap at optimal times to avoid pipes.

# The values
The corrresponding neural network values for the best fit bird (so i don't forget later) are

test.nn.bias_h = 0.991851568;
test.nn.bias_o = 0.715597987;
test.nn.weights_ih.matrix[0][0] = -0.23319190740585327;
test.nn.weights_ih.matrix[0][1] = -0.44383066892623901;
test.nn.weights_ih.matrix[0][2] = -0.71691030263900757;
test.nn.weights_ih.matrix[0][3] = -0.98840296268463135;

test.nn.weights_ih.matrix[1][0] = 0.87768185138702393;
test.nn.weights_ih.matrix[1][1] = -0.27542954683303833;
test.nn.weights_ih.matrix[1][2] = -0.91473126411437988;
test.nn.weights_ih.matrix[1][3] = -0.20780050754547119;

test.nn.weights_ih.matrix[2][0] = 0.89861750602722168;
test.nn.weights_ih.matrix[2][1] = 0.60570085048675537;
test.nn.weights_ih.matrix[2][2] = -0.29184848070144653;
test.nn.weights_ih.matrix[2][3] = 0.92809844017028809;

test.nn.weights_ih.matrix[3][0] = -0.83123266696929932;
test.nn.weights_ih.matrix[3][1] = 0.70543539524078369;
test.nn.weights_ih.matrix[3][2] = 0.85930967330932617;
test.nn.weights_ih.matrix[3][3] = 0.63939332962036133;

test.nn.weights_ih.matrix[4][0] = 0.45841848850250244;
test.nn.weights_ih.matrix[4][1] = 0.57036042213439941;
test.nn.weights_ih.matrix[4][2] = 0.092562675476074219;
test.nn.weights_ih.matrix[4][3] = -0.59471416473388672;

test.nn.weights_ih.matrix[5][0] = 0.39976191520690918;
test.nn.weights_ih.matrix[5][1] = 0.88628804683685303;
test.nn.weights_ih.matrix[5][2] = -0.51963865756988525;
test.nn.weights_ih.matrix[5][3] = -0.059785783290863037;

test.nn.weights_ho.matrix[0][0] = 0.018097519874572754;
test.nn.weights_ho.matrix[0][1] = -0.56712543964385986;
test.nn.weights_ho.matrix[0][2] = -0.32987457513809204;
test.nn.weights_ho.matrix[0][3] = 0.69170200824737549;
test.nn.weights_ho.matrix[0][4] = -0.28153324127197266;
test.nn.weights_ho.matrix[0][5] = -0.75438702106475830;
