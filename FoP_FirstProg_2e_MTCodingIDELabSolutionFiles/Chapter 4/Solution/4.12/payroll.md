```flow
st=>start: star
e=>end:
op2=>operation: '\nProgram: payroll.py\nProject 4.12\n\nPrint a payroll report.\n\nInput\n   A file in which each line has the form\n\n   <last name> <hourly wage> <hours worked>\n\nOutput\n   A report in tabular format.  Each line has the form\n\n   <last name> <hours worked> <total wages>\n\n'
op4=>operation: fileName = input('Enter the file name: ')
op6=>operation: inputFile = open(fileName, 'r')
sub8=>subroutine: print(('%-15s%6s%15s' % ('Name', 'Hours', 'Total Pay')))
cond11=>condition: for line in inputFile
op28=>operation: dataList = line.split()
op30=>operation: name = dataList[0]
op32=>operation: hours = int(dataList[1])
op34=>operation: payRate = float(dataList[2])
op36=>operation: totalPay = (hours * payRate)
sub38=>subroutine: print(('%-15s%6d%15.2f' % (name, hours, totalPay)))

st->op4
op4->op6
op6->sub8
sub8->cond11
cond11(yes)->op28
op28->op30
op30->op32
op32->op34
op34->op36
op36->sub38
sub38(left)->cond11
cond11(no)->end
```
