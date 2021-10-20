# Program: guess.py

## Project 3.3

The computer guesses the user's number using the minimum\nnumber of attempts and prevents cheating by the user.

### Flowchart

---

```flow
st=>start: Start
e=>end: End
op4=>operation: import math
op6=>inputoutput: Enter the smaller number
Enter the larger number
op12=>operation: count = 0
op10=>operation: maxGuesses = round(math.log(((larger - smaller) + 1), 2))
cond15=>condition: while True
op66=>operation: count += 1
sub68=>inputoutput: output smaller  & larger
op70=>operation: (smaller + larger) // 2)
sub72=>inputoutput: Your number is ?
op74=>inputoutput: Enter =, <, or >: ')
cond77=>condition: if (answer == '=')
sub81=>inputoutput: Hooray, I've got it in X tries!
sub83=>subroutine: break
cond88=>condition: if (count == maxGuesses)
sub92=>inputoutput: I'm out of guesses, and you cheated!
sub94=>subroutine: break
cond99=>condition: if (answer == '<')
op103=>operation: larger = (yourNumber - 1)
op107=>operation: smaller = (yourNumber + 1)

st->op4
op4->op6
op6->op10
op10->op12
op12->cond15
cond15(yes)->op66
op66->sub68
sub68->op70
op70->sub72
sub72->op74
op74->cond77
cond77(yes)->sub81
sub81->sub83->e
cond77(no)->cond88
cond88(yes)->sub92
sub92->sub94->e
cond88(no)->cond99
cond99(yes)->op103
op103(right)->cond15
cond99(no)->op107
op107(right)->cond15
```
