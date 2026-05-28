# Modeling Social Behavior — Python Implementations

Python implementations of agent-based models from  
**"Modeling Social Behavior: Mathematical and Agent-Based Models of Social Dynamics and Cultural Evolution"** by Paul E. Smaldino.

The book's original code uses NetLogo. This repository reimplements every exercise in Python, with detailed comments and explanations designed for social science students learning ABM from scratch.

---

## About This Project

I'm a social psychology student working through Smaldino's book chapter by chapter. Each notebook is a full, self-contained implementation of a coding exercise, written to be readable and educational. 

**What makes these notebooks different:**
- Every line of code is commented to explain *what* it does and *why*
- Variable types (global, agent, local) are explicitly labeled throughout
- Explanations connect the code back to the social science concepts in the book

---

## Setup

All models use Python 3 and [Mesa 3.x](https://mesa.readthedocs.io/), the standard library for agent-based modeling in Python.

Install all dependencies with:

```bash
pip install -r requirements.txt
```

Then launch JupyterLab:

```bash
jupyter lab
```

---
## Repository Structure 

├── chapter_02_particles/
│   ├── ch02_particles_basic.ipynb        # Random walk, movement, collision detection
│   └── ch02_particles_flock.ipynb        # Emergent collective motion (flocking)
│
├── chapter_03_schelling/
│   └── ch03_schelling_segregation.ipynb  # Residential segregation model
│
├── chapter_04_contagion/
│   └── ch04_spontaneous_adoption.ipynb   # Spontaneous adoption (no social influence)
│
├── chapter_05_opinion_dynamics/
│   └── ch05_positive_influence.ipynb     # Opinion change through social influence
│
├── chapter_06_cooperation/
│   └── ch06_cooperation.ipynb            # Evolution of cooperation
│
├── chapter_07_coordination/
│   └── ch07_coordination.ipynb           # Coordination games and conventions
│
├── chapter_08_scientific_process/
│   └── ch08_scientific_process.ipynb     # Models of science and knowledge production
│
├── chapter_09_networks/
│   └── ch09_networks.ipynb               # Network structure and social dynamics
│
├── requirements.txt
└── README.md
```

---

## Dependencies

| Library | Purpose |
|---|---|
| `mesa >= 3.0` | Agent-based modeling framework (agents, space, data collection) |
| `numpy` | Numerical operations and random number generation |
| `matplotlib` | Plotting and visualization |
| `jupyter` | Interactive notebook environment |

---

## Notes & Conventions

- All models use **Mesa 3.x** (newer API — no separate Scheduler class)
- Notebooks are designed to run top-to-bottom without errors
- Each notebook includes a section on the **ODD protocol** (Overview, Design, Details) as described in the book
- Variable scope is always documented: `# GLOBAL variable`, `# AGENT variable`, `# LOCAL variable`

---

## Reference

Smaldino, P. E. (2023). *Modeling Social Behavior: Mathematical and Agent-Based Models of Social Dynamics and Cultural Evolution*. Princeton University Press.
