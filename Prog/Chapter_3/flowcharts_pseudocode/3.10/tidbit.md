# Project 3.10

## Program: tidbit.py

The credit plan at TidBit Computer Store specifies a 10% down payment and an annual interest rate of 12%. Monthly payments are 5% of the listed purchase price, minus the down payment.

Write a program that takes the purchase price as input. The program should display a table, with appropriate headers, of a payment schedule for the lifetime of the loan. Each row of the table should contain the following items:

1. The month number (beginning with 1)
2. The current total balance owed
3. The interest owed for that month
4. The amount of principal owed for that month
5. The payment for that month
6. The balance remaining after payment
7. The amount of interest for a month is equal to balance × rate / 12.

The amount of principal for a month is equal to the monthly payment minus the interest owed.

### Example Input Output

An example of the program input and output is shown below:

```text
Enter the purchase price: 200

Month  Starting Balance  Interest to Pay  Principal to Pay  Payment  Ending Balance
 1         180.00           1.80             7.20             9.00           172.80
 2         172.80           1.73             7.27             9.00           165.53
 3         165.53           1.66             7.34             9.00           158.18
 4         158.18           1.58             7.42             9.00           150.77
 5         150.77           1.51             7.49             9.00           143.27
 6         143.27           1.43             7.57             9.00           135.71
 7         135.71           1.36             7.64             9.00           128.06
 8         128.06           1.28             7.72             9.00           120.34
 9         120.34           1.20             7.80             9.00           112.55
10         112.55           1.13             7.87             9.00           104.67
11         104.67           1.05             7.95             9.00            96.72
12          96.72           0.97             8.03             9.00            88.69
13          88.69           0.89             8.11             9.00            80.57
14          80.57           0.81             8.19             9.00            72.38
15          72.38           0.72             8.28             9.00            64.10
16          64.10           0.64             8.36             9.00            55.74
17          55.74           0.56             8.44             9.00            47.30
18          47.30           0.47             8.53             9.00            38.77
19          38.77           0.39             8.61             9.00            30.16
20          30.16           0.30             8.70             9.00            21.46
21          21.46           0.21             8.79             9.00            12.68
22          12.68           0.13             8.87             9.00             3.80
23           3.80           0.00             3.80             3.80             0.00
```
---

### Flowchart

![tidbit flowchart](tidbit.flowchart.svg)

---

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
