# Basic Data Types

Data types are the building blocks of the Deci language. They are the elements the language accepts and understands.

### Numbers

* Without units ⇒ `4`, `4.31`, `1,432,567.33`, `4.5e12`, `15%`, `1/3`
* With units:
  * simple with suffix ⇒ `10 seconds`, `10.5 EUR`, `10 kg`
  * simple with prefix ⇒ `€10.5`, `GBP 123.5`
  * composed ⇒ `5 m^2`, `80 km/hour`, `10 g/m^2`, `32 USD/month/person`

#### Units

Deci understands that some units express a basic quantity \(e.g. length\), and knows how to convert between units of that same quantity \(e.g. meters and centimeters\).

### Dates and time

* Year ⇒ `Y2020`
* Month ⇒ `2020/01` `2020/Jan`
* Month, for which deci assumes the current year ⇒ `January`
* Day ⇒ `2020/01/21` `2020-01-21`
* Day ⇒ `2020-January-21` `2020/January/21` `2020-Jan-21` `2020/Jan/21`
* Specific hour of a day ⇒ `2020/01/21 10`
* Specific minute of a day ⇒ `2020/01/21 10:34`
* Specific second of a day ⇒ `2020-01-21 20:34:10`

### Ranges and Sequences

#### Ranges

Ranges are a continuous interval of values occurring between two points, which includes the last point.

You can define a range as follows:

Ascending:

* `[1 through 10]`
* `[1..10]`

Descending:

* `[10 through 1]`
* `[10..1]`

#### Sequences

Sequences are a discrete sequence of values within a range. They can be expressed by defining the range and the step between values:

* `[1..10 by 1]` ⇒ `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`
* `[1 through 10 by 1]` ⇒ `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`

Alternatively, you can create a sequence by giving Deci an example of how it should work:

* `[1, 3..9]` ⇒ `[1, 3, 5, 7, 9]`

You can also transform a range into a sequence by applying the `by` operator:

```text
range = [0 through 10]
sequence = range by 2
sequence = [0, 2, 4, 6, 8, 10]
```

#### Time sequences

As the name implies, time sequences are a sequence of time points within a time range.

You can define a time sequence like this:

Ascending:

* `[2021-10 through 2022-03 by month]`
* `[2021-10..2022-03 by month]`

Descending:

* `[from December to January]`

Or, similarly to numeric sequences, by using the `by` operator in a time range:

```text
time_range = [2020 through 2030]
time_sequence = time_range by month 
time_sequence = [2021-01, 2021-02, ..., 2030-01]
```

