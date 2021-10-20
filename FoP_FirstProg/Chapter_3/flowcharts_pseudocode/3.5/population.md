# Program: population.py

## Project 3.5

Predict population growth, assuming that no organisms die.

Inputs:
   initial number of organisms
   rate of growth (a float > 1)
   the number of hours to achieve the rate\n   number of hours of growth

### Flowchart

---

```flow
st=>start: Start
e=>end: End
op4=>inputoutput: Enter the initial number of organisms:
Enter the rate of growth [a real number > 1]:
Enter the number of hours to achieve the rate of growth:
Enter the total hours of growth: 
op12=>operation: cycles = (totalHours // cycleHours)
cond13=>condition: for eachPass in range(cycles)
cond15=>operation: number = (number * rate) 
sub27=>inputoutput: The total population is', int(number))

st->op4
op4->op12
op12->cond13
cond13(yes, right)->cond15
cond15(top)->cond13
cond13(no)->sub27->e
```
