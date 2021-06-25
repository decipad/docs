# Basic Operations

Here's a short showcase of some of the things you can do in Deci.

You can perform arithmetic calculations.

```text
2+2
4
<result type: number>
```

If you perform more than one operation, the result section will show the outcome of the last one.

```text
2+2
6+3
9
<result type: number>
```

When writing formulas, white spaces between values and operators are ignored, so that all of the following operations deliver the same result:

```text
2 + 2
2+2
2 +2
4
<result type: number>
```

You can use percentages.

```text
20% of 5000kg
1000 kg
<result type: number>
```

You can define variables and use them in operations. Variable names should not contain the following reserved words: f, in, x, per, from, to, by.

```text
variable=2
variable+3
5
<result type: number>
```

```text
Salary = 2000€
Rent = 500€
FoodAndStuff = 400€
Savings = Salary - Rent - FoodAndStuff
1100 €
<result type: currency>
```

You can convert currencies.

```text
£10 in $
13.91 $
**<result type: currency>
```

You can create true or false statements.

```text
 2 > 1
**true
**<result type: boolean>
```

You can insert dates and times.

```text
date (2020-10-22)
2020-10-22
<result type: date>
```

```text
time (2020/10/10 14:00)
2020-10-10 14:00
<result type: time>
```

You can add and subtract time periods from a date or time.

```text
date1 = date (2020/10/10)
time_quantity = [3 weeks]
date2 = date1 + time_quantity
2020-10-31 
<result type: date>
```

You can define conditional expressions:

```text
if condition then value1 else value2
```

