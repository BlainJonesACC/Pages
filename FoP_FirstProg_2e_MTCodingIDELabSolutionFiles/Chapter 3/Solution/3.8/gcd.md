# Program: gcd.py

## Project 3.8

Compute and print the greatest common divisor of two input
integers.

### Flowchart

---

```flow
st=>start: Start
e=>end: End
op4=>inputoutput: Enter the smaller number: 
Enter the larger number:
cond9=>condition: while (first > 0)
op20=>operation: remainder = (second % first)
second = first
first = remainder
sub28=>inputoutput: The greatest common divisor is', second

st->op4
op4->cond9
cond9(yes, right)->op20
op20(top)->cond9
cond9(no)->sub28->e
```
