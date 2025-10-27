---
python:
  - python
  - code
  - documentation
  - comment
datee: '2025-10-27T18:14:42.445Z'
---
## Program 4.1 Brick volume

```python
# Compute the volume of a brick, given its dimensions
# Compute the base area from the width and length


# Input: the width, a positive float in any distance unit
width = 2

# Input: the length, a positive float in the same unit
length = 3

area = width * length
print('The base area is', area)

# Compute the volume from the base area and height

# Input: the height, a positive float in the same unit
height = 4

# Output: the volume, in cubic distance units
volume = area * height
print('The volume is', volume)


```


* * *

## Program 4.3 Restaurant bill

```python
# Compute total bill for given party size

# Input: the bill, in any currency, before any surcharges
bill = 10

# Input: the people, in the pary, a positive integer
people = 4

# Input: the service charge, a percentage
charge = 0.1

### Output: the total bill, in the same currency
##if people > 6:
##    total = bill + bill * charge
##else:
##    total = bill
##
##print('The total bill is', total)


# Output: the total bill, in the same currency
# Alternative
if people <= 6:
    total = bill
else:
    total = bill + bill * charge

print('The total bill is', total)
```


* * *

## Program 4.5  Grade system with multiple cases

```python
# Print the grade, given the marks

# Input: marks, an integer from 0 to 100
marks = 52

# Output: the grade, a string
if marks < 40:
    grade = 'fail'
elif marks <= 60:
    grade = 'pass'
elif  marks < 80:
    grade = 'merit'
else: # marks>= 80
    grade = 'distinction'

print('The grade is', grade)
```


* * *

## Program 4.7 Outstanding mortgage

```python
# Generate the monthly outstanding mortgage

# Input: anual interest rate, a floating-point percentage
rate = 0.05

# Input: monthly payment, a positive integer in a currency
payment = 200

# Input/ output: mortgage, a positive number, same currency
mortgage = 1000

# Output: month, a positive number, number of month
month = 1

print('Current outstanding mortgage:', mortgage)
while  (mortgage > 0):
    interest = mortgage * rate / 12
    mortgage = mortgage + interest - payment
    if mortgage <=0:
        print('Mortgage is paid-off in', month, 'months')
    else: 
        print('Outstanding mortgage:', mortgage, 'after', month, 'month(s)')
    month = month +1
```
