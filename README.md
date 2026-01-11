# Optimization of Last-Mile Logistics via Vehicle Routing Problem (MILP)

## Overview

This project addresses the optimization of last-mile delivery systems using advanced operations research techniques. We model the delivery problem as a **Vehicle Routing Problem (VRP)** and solve it using a **Mixed-Integer Linear Programming (MILP)** formulation implemented with Constraint Programming and Guided Local Search.

## Problem Statement

Last-mile delivery is a critical and costly component of logistics operations. This project focuses on optimizing pharmaceutical distribution routes to minimize the number of vehicles required while satisfying all delivery constraints.

## Repository Structure

- **[main/](main/)** - Contains all code implementations (Jupyter notebooks)
  - `all_days.ipynb` - Multi-day optimization implementation
  - `RVP.ipynb` - Single-day Vehicle Routing Problem solver
  - `Optim&Pess.ipynb` - Optimistic vs Pessimistic scenario comparison
  - `README.md` - Setup instructions and hyperparameters

- **[data/](data/)** - Contains all datasets used in the experiments
  - `all-days/` - Multi-day operation data (9 days)
    - Distance matrices (Excel format)
    - Order data (CSV format)
    - Time matrices for most-likely scenarios
  - `one-day/` - Single-day operation data
    - Distance and time matrices (CSV format)
    - Order data

## Getting Started

### Prerequisites

Install the required dependencies:

```bash
pip install ortools
```

### Usage

1. Navigate to the `main/` directory
2. Open the desired Jupyter notebook:
   - For single-day optimization: `RVP.ipynb`
   - For multi-day optimization: `all_days.ipynb`
   - For scenario comparison: `Optim&Pess.ipynb`
3. Run the cells to execute the optimization

Refer to `main/README.md` for detailed hyperparameter configuration.

## Dataset

- **Source**: Real-world pharmaceutical distribution data
- **Scope**: Multi-day operational planning
- **Scenarios**: 
  - Single-day optimization
  - Multi-day optimization
  - Variable demand scenarios (optimistic, pessimistic, most-likely)

## Methodology

### Approach
- **Problem Formulation**: Mixed-Integer Linear Program (MILP)
- **Solution Method**: Constraint Programming with Guided Local Search
- **Solver**: Google OR-Tools (chosen due to the NP-hard complexity of VRP)

### Key Features
- Fleet size minimization objective
- Constraint satisfaction for all delivery requirements
- Scalable solution approach for real-world problem sizes

## Results

Our computational experiments, spanning **nine days of operation**, demonstrated:

- **High Efficiency**: The solver consistently found highly efficient solutions
- **Fleet Optimization**: Required only **3 to 4 vehicles** from the available fleet
- **Successful Objective Achievement**: Fleet reduction was successfully prioritized through the minimization objective while satisfying all given constraints

## Documentation

For detailed methodology, analysis, and results, please refer to the [Final Report](Report_final.pdf).

## Technologies Used

- **Google OR-Tools**: Constraint programming and optimization solver
- **Mixed-Integer Linear Programming (MILP)**: Problem formulation approach
- **Guided Local Search**: Metaheuristic for improving solution quality

---

*This project demonstrates the practical application of operations research techniques to real-world logistics optimization challenges.*
