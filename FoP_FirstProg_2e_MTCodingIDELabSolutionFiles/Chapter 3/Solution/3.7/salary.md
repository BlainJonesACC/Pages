# Program: salary.py

## Project 3.7

Compute a school district's salary schedule.

Inputs
   starting salary
   annual percentage increase
   number of years for which to print the schedule

Outputs
    Two columns containing the year and the salary
    after the increase.

### Flowchart

---

```flow
st=>start: Start
e=>end: End
op4=>inputoutput: Enter the starting salary: $
Enter the annual % increase: 
Enter the number of years: 
op6=>inputoutput: Year    Salary
---------------
op12=>operation: multiplier = (1 + (increase / 100))
nextSal = startSal
cond17=>condition: for year in range(1, (years + 1))
sub26=>inputoutput: print(('%2d%12.2f' % (year, nextSal)))
op28=>operation: nextSal *= multiplier

st->op4
op4->op6
op6->op12
op12->cond17
cond17(yes)->sub26
sub26->op28
op28(left)->cond17
```
