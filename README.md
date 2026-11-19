# Atomic-Scale Pairwise Simulation

An atomic-scale, pairwise N-body classical physics simulation of (almost) all fundamental forces, developed in the [Godot Engine](https://godotengine.org/).

This project is the first instalment in a series of simulations exploring the behaviour of matter at increasingly small scales. The long-term objective is to develop an accurate, computationally powerful model capable of exploring the underlying interactions and emergent behaviours of subatomic particles.

The project was originally developed as part of my Extended Project Qualification (EPQ). Consequently, a number of design and implementation decisions were made with the available development time and practical feasibility in mind.

## Project Roadmap

This simulation represents the first stage of a broader project. Future developments are intended to include:

1. **Classical Field Simulation (WIP):** A Python-based successor to this project, focusing on field-based simulations. It aims to improve computational efficiency, accuracy and scalability through additional computational resources and the use of external tools.

2. **Non-Classical Subatomic Simulation (Unconfirmed):** A fundamentally different approach, moving beyond classical mechanics towards a model based more closely on the Standard Model of particle physics and the interactions governing subatomic matter.

## Current Implementation

The simulation currently initialises with 50 protons and 50 neutrons, randomly distributed within a small region centred around the camera.

At present, meaningful interaction with the simulation requires using Godot's built-in editor functionality, including manually dragging and repositioning particles within the 3D environment.

This is neither a particularly practical nor an intended method of interacting with the simulation. A dedicated interface for particle manipulation, configuration and experimentation is therefore a planned feature for a future release.

## Operation, Features and Functionality

### Force Calculations

The simulation uses pairwise force calculations between particles. Individual force vectors are calculated for each interaction and summed to determine the resultant force acting on each particle, which is subsequently used to calculate its motion.

The forces currently represented are:

- **Electromagnetism:** Modelled using the Lorentz force.
- **Residual Nuclear Force:** Approximated using the Yukawa potential.
- **Gravity:** Modelled using an energy-based approximation of universal gravitation.

Future iterations are intended to incorporate more sophisticated hadronic interactions.

### Simulation Controls

The simulation includes controls for manipulating the passage, direction and speed of simulated time.

| Key                        | Function                            |
| -------------------------- | ----------------------------------- |
| \<kbd>↑\</kbd> Up Arrow    | Increase simulation speed           |
| \<kbd>↓\</kbd> Down Arrow  | Decrease simulation speed           |
| \<kbd>←\</kbd> Left Arrow  | Switch from forward to reverse time |
| \<kbd>→\</kbd> Right Arrow | Switch from reverse to forward time |
| \<kbd>Space\</kbd>         | Pause / resume simulation           |

*Note: Larger simulation time steps reduce numerical accuracy. Reverse-time functionality is currently experimental and should not be considered physically reliable.*

### Camera Controls

The simulation uses a first-person camera, allowing the user to navigate and observe the particle system in 3D space.

| Input                                                       | Function              |
| ----------------------------------------------------------- | --------------------- |
| Mouse Movement                                              | Look around           |
| \<kbd>W\</kbd> \<kbd>A\</kbd> \<kbd>S\</kbd> \<kbd>D\</kbd> | Move horizontally     |
| \<kbd>Shift\</kbd>                                          | Rise                  |
| \<kbd>Ctrl\</kbd>                                           | Descend               |
| \<kbd>Esc\</kbd>                                            | Release mouse control |

### Emergent Behaviour

Two particularly significant emergent behaviours observed during development have been:

- **Nuclei Formation:** The emergence of bound nucleon structures through the interactions represented in the simulation.
- **Nucleon Drip:** The separation and emission of individual nucleons from larger nuclear structures.

These behaviours are particularly interesting as they emerge from the underlying particle interactions rather than being explicitly prescribed.

## Inspiration and Further Reading

This project was inspired in part by [particle.js](https://github.com/andre-nepomuceno/particle.js) by Andre Nepomuceno.

Its approach to particle-based simulation helped inform the structure and visual direction of this project. It is also an impressive and visually interesting piece of work in its own right.

The underlying physics and accompanying project report draw heavily on Professor David Tong's lecture notes for the CERN Summer School.

## Development Status

While I'm enthusiastic about beginning work on the next iteration, there is still a considerable amount of work to be done here. I intend to make at least one more release before moving on to the next project.

### Planned Improvements

- [ ] Code cleanup and refactoring
- [ ] Optimisation of pairwise calculations
- [ ] Fix and validate reverse-time functionality
