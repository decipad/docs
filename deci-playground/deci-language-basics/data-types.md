# Data Types

Data types are the building blocks of the Deci language. They are the elements the language accepts and understands.

### Numbers

`4`, `4.31`, `1,432,567.33`, `4.5e12`, `15%`, `1/3`

### Dates

* Year ⇒ `date(2020)`
* Month ⇒ `date(2020/01)` `date(2020/Jan)`
* Day ⇒ `date(2020/01/21)` `date(2020/January/21)` `date(2020/Jan/21)` `date(2020-01-21)` `date(2020-January-21)` `date(2020-Jan-21)`

### Ranges

Ranges are a continuous interval of values occurring between two points, which includes the last point.

You can define a range as follows:

Ascending:

* `[1 through 10]`
* `[1..10]`

Descending:

* `[10 through 1]`
* `[10..1]`

### Sequences

Sequences are a discrete sequence of values within a range. They can be expressed by defining the range and the step between values:

* `[1..10 by 1]` ⇒ `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`
* `[1 through 10 by 1]` ⇒ `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`

