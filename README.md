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
