## Sets:
### Introduction:

Sets are like __lists__ and __stacks__, but unlike those, sets store 
unique data types. They don't have any particular order, but they can only contain
unique bits of data. Sets work not only with numbers, but with strings as well
shown in example 2. Sets also automatically sort themselves because they cannot
contain duplicates.

![Set](https://media.geeksforgeeks.org/wp-content/uploads/Hasing-Python.png)

### Operations:
Since sets are similar to lists, one would think that you can still use the same 
append, extend, pop, and other operations just like lists and stacks. 
However, they cannot use these operations because sets cannot be changed once
created. If you want something different in a set, you must create a whole new
set. They are created using the inbuilt "set" function. Curly braces can also
be used to enclose items within a set. There is one exception to this rule; the add function.
This allows values to be added into the set separately. Problem 2 will accomplish this.

### Example:

```python

set1 = set()
print(set1)

set1 = set([1, 2, 2, 3, 4, 5, 5, 5, 5, 6, 7, 8, 9, 9, 9])

print(set1)

# Expected output:
# set()
# {1, 2, 3, 4, 5, 6, 7, 8, 9}
```

### Problem 1:

```python

# TODO: Make this set output the same thing two different ways
set2 = set()
print(set2)

set2 = set()
print(set2)

set2 = set()
print(set2)

# Expected output:
# Output should be similar to this
# set()
# {'Smith', 'John'}
# {'Smith', 'John'}
```

### Problem 2:

```python

set3 = set()
print('Original Set: ', set3)

# TODO: Add multiple elements to the set
set3.add('')

# TODO: Print the new set

```