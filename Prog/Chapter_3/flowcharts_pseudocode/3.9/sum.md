# Project 3.9

## Program: sum.py

### Instructions

Edit the program provided so that it receives a series of numbers from the user and allows the user to press the enter key to indicate that he or she is finished providing inputs. After the user presses the enter key, the program should print:

1. The sum of the numbers
2. The average of the numbers

An example of the program input and output is shown below:

```text
Enter a number or press Enter to quit: 1
Enter a number or press Enter to quit: 2
Enter a number or press Enter to quit: 3
Enter a number or press Enter to quit:

The sum is 6.0
The average is 2.0
```

---

#### Flowchart

![flowchart](sum.flowchart.svg)

---

#### Starter Code

```python
"""
Program: sum.py
Project 3.9

Computes the sum and average of a series of input numbers.
"""

theSum = 0.0
data = input("Enter a number: ")
while data != "":
    number = float(data)
    theSum += number
    data = input("Enter the next number: ")
print("The sum is", theSum)

```
