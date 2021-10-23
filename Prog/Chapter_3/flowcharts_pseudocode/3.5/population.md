# Project 3.5

## Program: population.py

### Instructions

A local biologist needs a program to predict population growth. The inputs would be:

1. The initial number of organisms, as an **int**
2. The rate of growth (a real number greater than 1), as a **float**
3. The number of hours it takes to achieve this rate, as an **int**
4. A number of hours during which the population grows, as an **int**

For example, one might start with a population of 500 organisms, a growth rate of 2, and a growth period to achieve this rate of 6 hours. Assuming that none of the organisms die, this would imply that this population would double in size every 6 hours. Thus, after allowing 6 hours for growth, we would have 1000 organisms, and after 12 hours, we would have 2000 organisms.

Write a program that takes these inputs and displays a prediction of the total population.

An example of the program input and output is shown below:

```text
Enter the initial number of organisms: 10
Enter the rate of growth [a real number > 1]: 2
Enter the number of hours to achieve the rate of growth: 2
Enter the total hours of growth: 6

The total population is 80
```

### Flowchart

---

![Population flowchart](population.flowchart.svg)

---

#### Starter Code

```python
"""
Program: population.py
Project 3.5

Predict population growth, assuming that no
organisms die.

Inputs:
   initial number of organisms
   rate of growth (a float > 1)
   the number of hours to achieve the rate
   number of hours of growth
"""

# Accept the inputs

# Calculate the number of cycles

# Calculate the population after an integral number of cycles

# Output the total population
```
