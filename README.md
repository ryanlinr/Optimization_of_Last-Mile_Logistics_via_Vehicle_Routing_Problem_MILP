# Optimization of Last-Mile Logistics via Vehicle Routing Problem (MILP)

## 📋 Overview

This project addresses the optimization of last-mile delivery systems using advanced operations research techniques. We model the delivery problem as a **Vehicle Routing Problem (VRP)** and solve it using a **Mixed-Integer Linear Programming (MILP)** formulation implemented with Constraint Programming and Guided Local Search.

##  Problem Statement

Last-mile delivery is a critical and costly component of logistics operations. This project focuses on optimizing pharmaceutical distribution routes to minimize the number of vehicles required while satisfying all delivery constraints.

##  Dataset

- **Source**: Real-world pharmaceutical distribution data
- **Scope**: Multi-day operational planning
- **Scenarios**: 
  - Single-day optimization
  - Multi-day optimization
  - Variable demand scenarios (optimistic, pessimistic, most-likely)

##  Methodology

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
