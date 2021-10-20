# Program: tidbit.py

## Project 1.5

Print a payment schedule for a loan to purchase a computer.

Input
   purchase price

Constants
   annual interest rate = 12%
   downpayment = 10% of purchase price
   monthly payment = 5% of purchase price

### Flowchart

---

```flow
st=>start: Start
e=>end: End
op4=>operation: ANNUAL_RATE = 0.12
op6=>operation: MONTHLY_RATE = (ANNUAL_RATE / 12)
op8=>operation: purchasePrice = float(input('Enter the puchase price: '))
op10=>operation: downPayment = (purchasePrice * 0.1)
op12=>operation: purchasePrice = (purchasePrice - downPayment)
op14=>operation: monthlyPayment = (0.05 * purchasePrice)
op16=>operation: month = 1
op18=>operation: balance = purchasePrice
sub20=>subroutine: print('Month  Starting Balance  Interest to Pay  Principal to Pay  Payment  Ending Balance')
cond23=>condition: while (balance > 0)
cond53=>condition: if (monthlyPayment > balance)
op57=>operation: monthlyPayment = balance
op59=>operation: interest = 0
op66=>operation: principal = (monthlyPayment - interest)
op68=>operation: remaining = (balance - principal)
sub70=>subroutine: print(('%2d%15.2f%15.2f%17.2f%17.2f%17.2f' % (month, balance, interest, principal, monthlyPayment, remaining)))
op72=>operation: balance = remaining
op74=>operation: month += 1
op63=>operation: interest = (balance * MONTHLY_RATE)

st->op4
op4->op6
op6->op8
op8->op10
op10->op12
op12->op14
op14->op16
op16->op18
op18->sub20
sub20->cond23
cond23(yes)->cond53
cond53(yes)->op57
op57->op59
op59->op66
op66->op68
op68->sub70
sub70->op72
op72->op74
op74(left)->cond23
cond53(no)->op63
op63->op66
```
