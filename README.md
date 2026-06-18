# Alasx-04-AI Space Rover-Autonomy-System

A C++ autonomous space rover simulator featuring planet terrain selection, AI terrain analysis, battery management, object scanning, and real-time rover navigation using SFML.

## Overview

Alasx-04 AI Space Rover Autonomy Simulator is a C++ project that simulates an autonomous rover exploring different planets and terrain types. The project includes both a console-based mission simulation and an SFML-powered visual rover mode.

The rover can analyze terrain, select safer movement paths, manage battery usage, scan scientific objects, and provide AI-style feedback during exploration.

## Features

* Planet selection system
* Terrain-based exploration
* AI terrain analysis and scoring
* Console mission simulation
* SFML visual rover simulation
* Real-time rover movement using WASD controls
* Battery management system
* Battery warning messages
* Object scanning system
* AI-style scan feedback
* Mission objectives and mission logs
* Modular C++ file structure

## Technologies Used

* C++
* SFML
* Visual Studio
* Object-Oriented Programming
* Enums and structs
* Modular header and source files

## Simulation Modes

The program includes two simulation modes:

### 1. Console Mission Simulation

The console version allows the user to select a planet, generate terrain options, and let the rover AI evaluate the safest terrain choice.

### 2. SFML Visual Rover Simulation

The visual version opens an SFML window where the user can move the rover, explore planet-based terrain, scan objects, and monitor battery levels.

## Controls

| Key | Action             |
| --- | ------------------ |
| W   | Move Up            |
| A   | Move Left          |
| S   | Move Down          |
| D   | Move Right         |
| E   | Scan Nearby Object |

## Project Structure

```text
Alasx-04-AI-Space-Rover-Autonomy-Simulator/
│
├── main.cpp
├── Rover.h
├── Terrain.h
├── Terrain.cpp
├── Planet.h
├── Planet.cpp
├── Mission.h
├── Mission.cpp
├── AISystem.h
├── AISystem.cpp
├── RoverVisualizer.h
├── RoverVisualizer.cpp
└── README.md
```

## Core Systems

### Rover System

The rover system tracks the rover's name, battery level, movement speed, position, and operational status.

### Planet System

The planet system allows users to choose from multiple planets, each with different terrain combinations.

### Terrain System

The terrain system includes different terrain types such as rocky, sandy, icy, volcanic, glassy, windy, and cratered terrain.

### AI System

The AI system scans terrain, scores danger levels, chooses the safest route, and explains its decision.

### Visualizer System

The SFML visualizer displays the rover, planet terrain, battery bar, scan radius, and scannable objects.

## AI Feedback Examples

The rover AI provides feedback such as:

```text
Alasx-04 AI: Scan complete. Mineral Rock has been analyzed.
Alasx-04 AI: Warning. Battery is getting low.
Alasx-04 AI: Critical warning. Battery is extremely low.
Alasx-04 AI: Power failure. Rover battery depleted. Movement systems offline.
```

## How to Run

### Requirements

* Visual Studio
* C++ compiler
* SFML 2.6.2 or compatible version

### Setup

1. Download and install SFML.
2. Add the SFML `include` folder to Visual Studio's Additional Include Directories.
3. Add the SFML `lib` folder to Visual Studio's Additional Library Directories.
4. Add the required SFML `.lib` files to Linker Input.
5. Copy the required SFML `.dll` files into the same folder as the compiled `.exe`.
6. Build and run the project in Visual Studio.

## Required SFML Libraries

For Debug mode, add:

```text
sfml-graphics-d.lib
sfml-window-d.lib
sfml-system-d.lib
sfml-audio-d.lib
```

Required DLL files:

```text
sfml-graphics-d-2.dll
sfml-window-d-2.dll
sfml-system-d-2.dll
sfml-audio-d-2.dll
openal32.dll
```

## What I Learned

While building this project, I practiced:

* Structuring a C++ project across multiple files
* Using header files and source files
* Working with SFML graphics
* Handling keyboard input
* Creating visual simulations
* Designing basic AI decision logic
* Managing game/simulation state
* Implementing battery and scanning systems
* Debugging linker, include path, and dependency issues in Visual Studio

## Future Improvements

Possible future upgrades include:

* Adding rover animations
* Adding terrain collision
* Adding sound effects
* Adding text labels inside the SFML window
* Adding more planets and terrain types
* Adding more advanced AI route planning
* Connecting the rover to the OpenAI API for mission-control style reports

## Author

Created by Emmanuel Ray.

## License

This project is licensed under the MIT License.
