# Program: sum.py

## Project 3.9

Computes the sum and average of a series of input numbers.

### Flowchart

---

```flow
st=>start: Start
e=>end: End
op4=>operation: theSum = 0
op6=>operation: count = 0
cond9=>condition: while True
op31=>inputoutput: number = input('Enter a number or press Enter to quit: ')
cond34=>operation: break if  (number == '')
op44=>operation: theSum += float(number)
op46=>operation: count += 1
sub50=>inputoutput: print('The sum is', theSum)
cond53=>inputoutput: print('The average is', (theSum / count)) if  (count > 0)

st->op4
op4->op6
op6->cond9
cond9(yes)->op31
op31->cond34
cond34->op44
op44->op46
op46(left)->cond9
cond9(no)->sub50
sub50->cond53
```
