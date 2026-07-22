# Memory Management Simulator

<p align="center">
<img alt="C++" src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge" />
  <img alt="CMake" src="https://img.shields.io/badge/CMake-064F8C?style=for-the-badge" />
  <img alt="Operating Systems" src="https://img.shields.io/badge/Operating%20Systems-374151?style=for-the-badge" />
</p>

<p align="center">
  <strong>A systems-level simulator for visualizing memory allocation, page behavior, and operating-system memory management concepts.</strong>
</p>

Memory Management provides a C++ simulation environment for studying how memory state changes over time. It includes build configuration, visual frame artifacts, and supporting documentation around requirements and implementation behavior.

## Core Capabilities

- Simulates memory-management behavior for operating-systems study.
- Uses CMake for repeatable C++ builds.
- Produces visual frame artifacts for state-by-state inspection.
- Includes requirements analysis and project summary documentation.

## Technical Architecture

The repository is structured as a C++ project with CMake build files, documentation, and generated visualization frames. The design supports both command-line experimentation and visual explanation of memory behavior.

## Architecture Diagram

```mermaid
flowchart LR
  Config["Simulation Configuration"] --> Engine["C++ Memory Simulation"]
  Engine --> States["Memory State Frames"]
  States --> PNG["PNG Frame Sequence"]
  PNG --> GIF["Animated Visualization"]
  Engine --> Metrics["Allocation and Paging Behavior"]
  Metrics --> Docs["Requirement and Analysis Documents"]

  classDef inputs fill:#FEF3C7,stroke:#D97706,color:#78350F,stroke-width:2px;
  classDef process fill:#DBEAFE,stroke:#2563EB,color:#1E3A8A,stroke-width:2px;
  classDef data fill:#DCFCE7,stroke:#16A34A,color:#14532D,stroke-width:2px;
  classDef agent fill:#F3E8FF,stroke:#9333EA,color:#581C87,stroke-width:2px;
  classDef output fill:#FFE4E6,stroke:#E11D48,color:#881337,stroke-width:2px;
  class Config,Engine,States,Docs process;
  class PNG,GIF,Metrics data;
  linkStyle default stroke:#64748B,stroke-width:2px;
```

## Technology Stack

- C++ implementation for systems simulation.
- CMake build workflow.
- Generated PNG/GIF artifacts for memory-state visualization.
- Project requirement documents for traceable implementation planning.

## Repository Structure

- `CMakeLists.txt` - Build configuration.
- `memory.gif` - Rendered memory-management visualization.
- `frames/png` - Generated frame sequence.
- `PROJECT_REQUIREMENTS_ANALYSIS.md` - Requirements analysis.
- `REQUIREMENTS_SUMMARY.md` - Requirement summary.

## Getting Started

```bash
cmake -S . -B build
cmake --build build
```

```bash
./build/Memory-Management
```

## Professional Context

This project demonstrates C++ systems programming, OS concept modeling, and visual technical communication.
