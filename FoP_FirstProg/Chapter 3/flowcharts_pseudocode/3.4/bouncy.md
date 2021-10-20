# Program: bouncy.py

## Project 3.4

This program calculates the total distance a ball travels as it bounces given: the initial height of the ball. its bounciness index. the number of times the ball is allowed to continue bouncing

### Flowchart

---

```flow
st=>start: Start
e=>end: End
op4=>inputoutput: Enter the height from which the ball is dropped:
Enter the bounciness index of the ball:
Enter the number of times the ball is allowed to continue bouncing:
op10=>operation: distance = 0
cond13=>condition: for eachPass in range(bounces)
op24=>operation: distance += height
height *= bounciness
distance += height
sub32=>inputoutput: Total distance traveled is: X units.

st->op4
op4->op10
op10->cond13
cond13(yes)->op24
op24(left)->cond13
cond13(no)->sub32->e
```
