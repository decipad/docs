# Columns and Tables

### Columns

A column is a series of elements. They can be of any data type.

* `[1, 2, 3, 4]`
* `["November", "December", "January", "February"]`



You can perform operations across a column. In order to perform an operation across a column, all elements of that column must be of the same type.

```text
[1, 2, 3] + 4

[5, 6, 7]


[0, 1, 2, 3] * 2

[0, 2, 4, 6]


[0h, 1h, 2h, 3h] * [0, 1, 0, 1]

[0h, 1h, 0h, 3h] 
```

### Tables

Tables are groups of columns. A table can contain multiple columns with different data types.

You can easily create a table using the interface.

_EXAMPLE HERE_

Alternatively, you can use the language to create a table.

```text
People = {
  Names = ["Alice", "Eve", "Jen"],
  Salaries = [50000, 60000, 55000]
}
```

In order to perform operations with a column from a table, all elements of that column must be of the same type.

