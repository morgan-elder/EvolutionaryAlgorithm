# Project 2

Morgan Elder</br>
Ben Vuong</br>
CS4320</br>
Spring 2023

# How to use

## Optimization Goal

The Optimization_Goal class lets the user define if the goal of a problem is to find a maximum or minimum. Then the genetic algorithm can follow steps that depend on the goal.

```python3
# define the goal of a problem
goal=Optimization_Goal.MINIMIZE

# perform an action that depends on the goal
if (goal == Optimization_Goal.MINIMIZE):
  # TODO minimize 
  pass
elif (goal == Optimization_Goal.MAXIMIZE):
  # TODO maximize
  pass
```

## Optimization Problem

Use the Problem class to identify a new class as an optimization problem. 

### Adding New Problems

1. To add a new problem, define a new subclass that inherits from the problem class
2. Problem parameters can be predefined as class variables or defined at runtime as instance variables
  - Include variables that describe the optimization goal, input dimensions, and input domain (upper/lower boundaries)
3. Each problem subclass must have a function called `objective_function` defines and returns how input data is evaluated.
  - The input should should match expected problem parameters such as input dimensions and boundaries. 

```Python3

class Problem():
  pass
  
class New_Problem(Problem):
  # TODO define problem parameters
  
  # predefined class variables
  dimensions = 2
  goal = Optimization_Goal.MAXIMIZE
  upper_bouds = [1, 44]
  
  # instance variables defined at runtime
  def __init__(self, lower_bounds):
    self.lower_bounds = lower_bounds
  
  def objective_function(X):
    result = X[0] + X[1]
    return result
  

```
