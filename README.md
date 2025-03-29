# 🧠 Self-Driving Car Simulator with NEAT-Python

Autonomous car simulation using **NEAT (NeuroEvolution of Augmenting Topologies)** and **PyGame**. Cars learn to navigate a custom map by evolving neural networks through generations.

## 🚀 Features

- NEAT-Python integration for evolving neural networks.
- Real-time car simulation with PyGame.
- Sensor-based (radar) input for obstacle detection.
- Fitness function based on survival time and distance.
- Fullscreen visual feedback with radar rendering.
- Easily customizable with your own maps and cars.

## 🖼 Demo

> Replace this with a GIF or screenshot.

![Simulation Screenshot](assets/screenshot.png)

## 🧠 How It Works

Each car is controlled by a neural network evolved with NEAT. Inputs are distances to obstacles (from 5 radars), and outputs decide whether to turn left, right, accelerate, or decelerate.

## 🗂 Project Structure

```
📦 project/
├── main.py            # Main simulation script
├── config.txt         # NEAT configuration file
├── car.png            # Car sprite
├── map.png            # Driving map (must have white borders)
└── README.md
```

## ⚙️ Requirements

Install Python dependencies:

```bash
pip install pygame neat-python
```

## 🧪 Run the Simulation

From the project directory:

```bash
python main.py
```

## 📁 Customization

- `map.png`: Add your own track. Obstacles must be white (`(255,255,255)`).
- `car.png`: Customize your car sprite (preferably with transparent background).
- `config.txt`: Tune NEAT parameters to experiment with evolution dynamics.

## 🧠 Neural Network Inputs/Outputs

- **Inputs (5)**: Distances from 5 radars (normalized).
- **Outputs (4)**:
  1. Turn Left
  2. Turn Right
  3. Decelerate
  4. Accelerate

## 📜 Credits

- Original Concept by [Cheesy AI (YouTube)](https://www.youtube.com/c/CheesyAI)
- Optimized and extended by [NeuralNine](https://github.com/NeuralNine)

## 📄 License

This project is for educational purposes. Use freely with attribution.
