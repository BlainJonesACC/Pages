# Program: tidbit.py

## Project 3.10

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
op4=>operation: Set Constants 
ANNUAL RATE
MONTHLY RATE 
io8=>inputoutput: Enter the purchase price:
op10=>operation: Calculate 
down payment
purchase price
op14=>operation: Calculate Monthly Payment
op16=>operation: Initialize Loop Variables
Month
Balance
io20=>inputoutput: Output schedule header
cond23=>condition: Balance > 0
cond53=>condition: Monthly Payment Balance
op57=>operation: Calculate Monthly Payment
op66=>operation: Calculate
Principal
Remaining
io70=>inputoutput: Output Month, Balance,
Interest, Principal,
Monthly Payment,
Remaining Balance
op72=>operation: Set Balance to Remaining Balance
Iterate Month
op63=>operation: Calculate Interest

st->op4
op4->io8
io8->op10
op10->op14
op14->io20
io20->op16
op16->cond23
cond23(yes, right)->cond53
cond23(no)->e
cond53(yes)->op57
op57->op66
op66->io70
io70->op72
op72(left)->cond23
cond53(no)->op63
op63->op66
```

### Starter Code

```python
"""
Program: tidbit.py
Project 1.5

Print a payment schedule for a loan to purchase a computer.

Input
   purchase price

Constants
   annual interest rate = 12%
   downpayment = 10% of purchase price
   monthly payment = 5% of purchase price
   
"""
# Set Constants


# Request input


# Calculate down payment and purchase price


# Calculate monthly payment


# Output schedule header


# Initialize loop variables

# Loop through declining balance

    # Output "Month  Starting Balance  Interest to Pay  Principal to Pay  Payment  Ending Balance" on this iteration

    # Iterate loop variables

```
