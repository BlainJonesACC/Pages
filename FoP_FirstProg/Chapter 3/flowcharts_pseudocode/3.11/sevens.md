# Program: sevens.py

## Project 3.11

Simulate the game of lucky sevens until all funds are depleted.

1) Rules:
       roll two dice
       if the sum equals 7, win \$4, else lose \$1
2) The input is:
       the amount of money the user is prepared to lose
3) Computations:
       use a random number generator to simulate rolling the dice
       loop until the funds are depleted
       count the number of rolls
       keep track of the maximum amount
4) The outputs are:
       the number of rolls it takes to deplete the funds
       the maximum amount

### Flowchart

---

```flow
st=>start: Start
e=>end: End
op4=>operation: import random
op6=>inputoutput: How many dollars do you have?
op8=>operation: Initialize variables
maxDollars = dollars
countAtMax = 0
count = 0
cond15=>condition: while (dollars > 0)
op50=>operation: count += 1
die1 = random.randint(1, 6)
die2 = random.randint(1, 6)
cond57=>condition: if ((die1 + die2) == 7)
op61=>operation: dollars += 4
cond69=>condition: if (dollars > maxDollars)
op73=>operation: maxDollars = dollars
countAtMax = count
op65=>operation: dollars -= 1
sub82=>inputoutput: You are broke after X rolls.
You should have quit after Y rolls when you had $Z.

st->op4
op4->op6
op6->op8
op8->cond15
cond15(yes)->op50
op50->cond57
cond57(yes)->op61
op61->cond69
cond69(yes)->op73
op73(left)->cond15
cond69(no)->cond15
cond57(no)->op65
op65->cond69
cond15(no)->sub82->e
```

### Starter Code

```python
"""
Program: sevens.py
Project 3.11

Simulate the game of lucky sevens until all funds are depleted.

1) Rules:
       roll two dice
       if the sum equals 7, win $4, else lose $1
2) The input is:
       the amount of money the user is prepared to lose 
3) Computations:
       use a random number generator to simulate rolling the dice
       loop until the funds are depleted 
       count the number of rolls
       keep track of the maximum amount
4) The outputs are:
       the number of rolls it takes to deplete the funds
       the maximum amount 

"""
# import module 

# Request the input

# Initialize variables

# Loop until the money is gone

    # Roll the dice

    #Calculate the winnings or losses

    #If this is a new maximum, remember it


# Display the results
```
