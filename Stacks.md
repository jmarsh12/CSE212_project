## Stacks:
### Introduction:

What are stacks? Stacks are a type of __list__. Like __lists__, they hold a set of data. 
However, unlike lists, stacks follow a set order of operations. There are two rules to
follow. Last In First Out (LIFO), and First In Last Out (FILO). One great thing about stacks
is that they are always O(1) in Big O Notation because they always pop from the end. 

![Stack of books](http://www.bristollib.com/wp-content/uploads/2020/05/stack-of-books-png-large-2.jpg)

### Operations:

Stacks, like lists, have some operators to use. Lists use append and extend as some
basic operators, and stacks are very similar. Stacks use append and pop. Append, 
just like in lists, adds things to the bottom of a stack. Pop, takes things
off the top of a stack. This can also be used in lists to take  things off 
the end of the list.

Stacks can also have specific indexes popped. The first problem below will
pop off specific indecies from the stack.

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

### Problem 1:

```python

# TODO: Make this stack pop only index 2 and print the result
stack2 = []
stack2.append(1)
stack2.append(17)
stack2.append(12)
stack2.append(57)

# Expected output:
# [1, 17, 12, 57]
# [1, 12, 57]
```

### Problem 2:

```python

# TODO: Append both numerical values and strings to the stack
#  pop only the strings off
stack3 =  []

# Expected output:
# Output should look something similar to this.

# [1, 2, Sam, John, 3, 4]
# [1, 2, 3, 4]
```
