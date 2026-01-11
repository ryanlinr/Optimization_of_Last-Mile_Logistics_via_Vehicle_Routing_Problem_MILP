# Optimization_of_Last-Mile_Logistics_via_Vehicle_Routing_Problem_MILP
We modeled a last-mile delivery system as a Vehicle Routing Problem (VRP). We used real- world pharmaceutical distribution dataset, and formulated as a Mixed-Integer Linear Program  (MILP) but solved using Constraint Programming with Guided Local Search to handle scale.
We modeled a last-mile delivery system as a Vehicle Routing Problem (VRP). We used real-
world pharmaceutical distribution dataset, and formulated as a Mixed-Integer Linear Program

(MILP) but solved using Constraint Programming with Guided Local Search to handle scale.
This was tested across single-day, multi-day, and variable demand scenarios such as: optimistic,
pessimistic, and most-likely. We used Google OR-Tools due to the NP-hard complexity of the
problem. Our computational experiments, spanning nine days of operation, demonstrated that the
solver consistently found highly efficient solutions, requiring only 3 to 4 vehicles from the
available fleet while successfully prioritizing fleet reduction through a minimization objective
with given constraints.
