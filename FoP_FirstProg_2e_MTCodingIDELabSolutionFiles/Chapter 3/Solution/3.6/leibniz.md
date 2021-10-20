# Program: leibniz.py

## Project 3.6

This program approximates the value of pi using an algorithm designed by the German mathematician Gottfried Leibniz.

The algorithm is as follows:
pi = 4 - 4 / 3 + 4 / 5 - 4 / 7 + . . .

This program allows the user to specify the number of iterations
to use in the approximation.

### Flowchart

---

```flow
st=>start: Start
e=>end: End
op4=>inputoutput: Enter the number of iterations: 
op6=>operation: pioverfour = 0
numerator = 1
denominator = 1
cond13=>condition: for count in range(iterations)
op24=>operation: pioverfour += (numerator / denominator)
numerator = (- numerator)
denominator += 2
sub32=>inputoutput: The approximation of pi is', (pioverfour * 4)

st->op4
op4->op6
op6->cond13
cond13(yes, right)->op24
op24(top)->cond13
cond13(no)->sub32->e
```
