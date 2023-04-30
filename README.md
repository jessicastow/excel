# Data Analysis in Excel
#### Excel notes taken from DataCamp's Data Analysis in Excel course


#### EXPLORING DATA

`EXACT()` function syntax
- syntax:
`=EXACT(value1, value2)`
-example: 
`=EXACT(I2, J2)`
- returns TRUE or FALSE depending on whether the cells match or not

`TRIM()` function syntax
- syntax: 
`TRIM(value)` 
- example:
`TRIM(A2)`
- removes extra spaces at the beginning and end of the cell value

`SORT()` function syntax
- syntax:
`=SORT(array, [sort)index], [sort_order])`
- example:
`=SORT(B2:B104, 1, -1)
- `sort_index`: column number to sort by
- `sort_order`: for A to Z enter `1` and for Z to A enter `-1`

Nested formulas
- nesting: using a function as part of another function
- excel exectutes them from the inside out

`FILTER()` function syntax
- syntax:
`=FILTER(range, criteria, [if_empty])
- example:
`=FILTER(C2:C104, C2:C104>1000)`

Combining `SORT()` and `FILTER()`
- syntax:
`=SORT(FILTER(range, criteria), [sort_index], [sort_order])`
- example:
`=SORT(FILTER(B2:C104, C2:C104>1000), 1, -1)`

#### Data types in Excel
- Text: strings, numbers or dates represented in a text format
- Number: numeric values
- Date: dates and times in an accepted date-time representation
- Boolean: logical or TRUE/FALSE

`TEXT()` function
- syntax:
`=TEXT(value, format)`
- example:
`=TEXT(A2, "000000000")
- change the data type so it behaves like a string
- the number of 0s represents the minimum number of characters in the id field

`VALUE()` function syntax
- syntax:
`=VALUE(text)`
- example:
`=VALUE(L2)`
- can remove $'s

`ROUND()` with `VALUE()`
- syntax:
`=ROUND(VALUE(text), decimal places)`
- example:
`=ROUND(VALUE(L2), 0)`

#### PREPARING DATA

#### ANALYSING DATA
