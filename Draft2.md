# Final Project Draft 2

## Sets:
### Introduction:

Sets are like __lists__ and __stacks__, but unlike those, sets can store 
unique data types. They don't have any particular order, but they can only contain
unique bits of data. Sets work not only with numbers, but with strings as well
shown in example 2. Sets also automatically sort themselves because they cannot
contain duplicates.

### Operations:
Since sets are similar to lists, one would think that you can still use the same 
append, extend, pop, and other operations just like lists and stacks. 
However, they cannot use these operations because sets cannot be changed once
created. If you want something different in a set, you must create a whole new
set. They are created using the inbuilt "set" function. Curly braces can also
be used to enclose items within a set.

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

### Example 2:

```python
set2 = set()
print(set2)

set2 = set(['Jeff', 'Marsh'])
print(set2)

set2 = set(['Jeff', 'Jeff', 'Marsh', 'Marsh'])
print(set2)

# Expected output:
# set()
# {'Marsh', 'Jeff'}
# {'Marsh', 'Jeff'}
```