# Final Project Draft 1

## Stacks:
### Introduction:

What are stacks? Stacks are a type of __list__. Like __lists__, they hold a set of data. 
However, unlike lists, stacks follow a set order of operations. There are two rules to
follow. Last In First Out (LIFO), and First In Last Out (FILO).

### Operations:

Stacks, like lists, have some operators to use. Lists use append and extend as some
basic operators, and stacks are very similar. Stacks also use append and extend,
as well as pop. Append, just like in lists, adds things to the bottom of a stack.
Pop, takes things off the top of a stack. This can also be used in lists to take
things off the end of the list.

### Example:

```python
stack = []
stack.append(1)
stack.append(2)
stack.append(3)
print('Original Stack is: ', stack)
print()
print('Popped from stack: ', stack)
print(stack.pop())
print(stack.pop())
print(stack.pop())
print('This is the stack after everything has been popped: ', stack)
# Expected output: 
# Original Stack is:  [1, 2, 3]

# Popped from stack:  [1, 2, 3]
# 3
# 2
# 1
# This is the stack after everything has been popped:  []
```
