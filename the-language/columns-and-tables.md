# Columns and Tables

### Columns

A column is a series of elements. They can be of any data type.

* `[1, 2, 3, 4]`
* `[November, December, January, February]`
* `[$1000, 250, "apple"]`

You can access elements of a column by calling them:

```text
my_column = [2, 4, 6, 8, 10]

first my_column
2
<result type: number>

second my_column
4
<result type: number>

last my_column
10
<result type: number>
```

You can append elements to a column:

```text
[1, 2, 3] + 4
[1, 2, 3, 4]
<result type: number>

"pineapples" + [2, 3, 4]
[pineapples, 2, 3, 4]
<result type: ?>
```

In order to perform an operation across a column, all elements of that column must be of the same type.

```text
[0, 1, 2, 3] * 2
[ 0, 2, 4, 6 ]
<result type: number>

**[0h, 1h, 2h, 3h] * [0, 1, 0, 1]
[ 0h, 1h, 0h, 3h ] 
<result type: time>
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

In order to perform operations with a specific column, all elements of that column must be of the same type.

