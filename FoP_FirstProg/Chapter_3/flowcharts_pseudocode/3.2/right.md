# Program: right.py

## Project 3.2

Determine whether or not three input sides compose a right triangle.

### Flowchart

---

```flow
st=>start: Start
e=>end: End
op4=>inputoutput: Enter the first side
Enter the second side
Enter the third side
op10=>operation: calculate square root of side 1
calculate square root of side 2
calculate square root of side 3
cond17=>condition: Test the three
possible Pythagorean
Theorem
sub21=>inputoutput: The triangle is a right triangle.
sub25=>inputoutput: The triangle is not a right triangle.

st->op4
op4->op10
op10(right)->cond17
cond17(yes, left)->sub21
cond17(no, right)->sub25
sub21->e
sub25->e
```

---

```mermaid
flowchart
id1([Start]);
id2([End])
io4[/Enter the first side\nEnter the second side\nEnter the third side/]
op10[calculate square root of side 1\ncalculate square root of side 2\ncalculate square root of side 3]
cond17{Test the three\npossible Pythagorean\nTheorem}
sub21[/The triangle is a right triangle/]
sub25[/The triangle is not a right triangle/]

id1-->io4
io4-->op10
op10-->cond17
cond17--true-->sub21
cond17--False-->sub25
sub21-->id2
sub25-->id2
```