# Documentation

Here is the planned program flow:
CSV file is converted into Python dictionary object first:
The `key` is the variable(x1,x2,...,xn and y or column in CSV ) and `value` contains all the datapoints(rows in CSV)

```python
# [] --> list, ()--> tuple
# this snippet is for Representaion only -- to give a general idea
input_dict{x1:(,...,),
x2(,..,),
.
.
.
xn:(,...,),
y(,..,)}
```

The `input_dict`'s value is `tuple` as input(xi) and output(y) should not be altered.
After performing data cleaning and other pre-processing the updated dictionary object is created:

```python
# [] --> list, ()--> tuple
# this snippet is for Representaion only -- to give a general idea
updated_dict{x1:(,...,),
x2(,..,),
.
.
.
xn:(,...,),
y(,..,)
outliers:[],
blanks:[] }
```

For further calculations use `updated_dict` and append it if required.

**Note**: As dictionary in `python` is _unordered_ you can access its members using name of`keys`, so name the `keys` appropriately(according to the corresponding `values`) so that everyone can easily use them.
