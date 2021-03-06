# Basic Operations

Here's a short showcase of some of the things you can do in Deci.

You can perform arithmetic calculations.

```text
2+2

4
```

If you perform more than one operation, the result section will show the outcome of the last one.

```text
2+2
6+3

9
```

When using the `+`, `-`, `=`, `>`, `<`, `>=`, `<=` and `**` signs, white spaces between values and operators are ignored, so that all of the following operations deliver the same result:

```text
2 + 2
2+2
2 +2

4
```

However, calculations with the operators `/` and `*` require white spaces.

```text
2 * (3+1)

8
```

You can use percentages.

```text
20% * 5000kg

1000kg
```

You can define variables and use them in operations. Variable names should not contain any symbols or word operators like `per`, `by`, `through` and `date`.

```text
variable=2
variable+3

5
```

```text
Salary = 2000€
Rent = 500€
FoodAndStuff = 400€
Savings = Salary - Rent - FoodAndStuff

1100 €
```

You can insert dates and times.

```text
date (2020-10-22)
2020-10-22

Oct 22nd 2020
```

You can create true or false statements.

```text
 2 > 1

True
```

