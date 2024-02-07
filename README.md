# Grand Prix Transportation Optimization
## Objective
The objective of this project is to find the most efficient shipping plan for Grand Prix Transportation, aiming to minimize shipping costs while ensuring that the demands of each region are met without exceeding the capacities of the plants.

## Problem Description
Grand Prix Automobile Company manufactures automobiles in three plants and ships them to four regions of the country. The plants have different capacities, and each region has specific demand requirements. The unit costs of shipping an automobile from each plant to each region are provided. The goal is to devise a shipping plan that minimizes costs while meeting demand and capacity constraints.

## Model Formulation
### Input Parameters
1. plants: Index to represent plants.
2. regions: Index to represent regions.
3. k: Capacity of each plant.
4. d: Demand of each region.
5. c: Unit shipping cost from each plant to each region.

## Decision Variables
nx: Quantity to ship from each plant to each region.
## Objective Function
The objective is to minimize the total shipping cost, calculated as the sum of the product of unit shipping costs and the quantity shipped from each plant to each region.

## Constraints
Non-Negative Shipping: Ensure that the quantity shipped from each plant to each region is non-negative.
Capacity Constraint: The total quantity shipped from each plant should not exceed its capacity.
Demand Satisfaction Constraint: The total quantity shipped to each region should meet its demand.
Implementation
The optimization model is implemented using the Gurobi optimization solver in Python.
Input parameters, decision variables, objective function, and constraints are defined and set up in the model.
The model is solved to obtain the optimal shipping plan that minimizes costs while satisfying all constraints.
Installation and Usage
Ensure that the Gurobi optimizer is installed (!pip install gurobipy).
The provided Python code can be used to set up and solve the optimization model.

## Results
After optimization, the optimal shipping plan and the corresponding objective value are obtained.

The optimal solution provides the quantity to be shipped from each plant to each region.
The total shipping cost for the optimal solution is also provided.
## Conclusion
This optimization approach helps Grand Prix Transportation in efficiently planning their shipping operations, minimizing costs while meeting demand and capacity constraints.
