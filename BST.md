## Binary Search Trees And Recursion
### Introduction:

Binary search trees are comprised of different BSTs. Each BST has a subtree with another
BST. Binary search trees have a few specific properties; each BST is its own binary 
search tree. The left subtree only has values that are less than the BST key, 
whereas the right subtree only has values that are greater. Finally, no BSTs can be 
duplicated. This may seem a little confusing. To clarify, each BST has its own key, and
an associated value with that key. When you search a key, you need to have a sorted
array to perform that search. You can search the key, and if the key is found, you can
perform operations with that found key.

![BST Image](https://media.geeksforgeeks.org/wp-content/uploads/BSTSearch.png)

### Operations:

Binary search trees only have a few inherent operations. BST's make use of recursion to
refer to the previous BST when the key is found, eventually leading back up to the first
BST. This is the only way you can get out of a search tree. If I wanted to find __14__ in the
image above, I would need to use a loop to look through each direction on the tree, and their
subtrees to find __14__. Once I've found __14__, I can then return __True__ to the previous
BST (in this case __10__), which will in turn return True to the first BST (__8__).
To accomplish this, we can use [tree].right, [key] (where tree is the name of the search
tree, and key is the key associated with the desired BST.) We can also use the same principle
to search left. We do this in a loop or with if statements until we find what we're looking
for.

### Example:

```python

def search(tree, key):
    if tree is None or tree.value == key:
        return tree

    elif tree.value < key:
        return search(tree.right, key)
    
    else:
        return search(tree.left, key)
```

### Problem 1:

```python

class BST:
    def __init__(self, key):
        self.left = None
        self.right = None
        self.value = key
 
# A utility function to insert
#  a new BST with the given key
 
# TODO: Implement the insert function
def insert(tree, key):
    if tree is None:
        pass
    else:
        if tree.value == key:
           pass
        elif tree.value < key:
            pass
        else:
            pass
    pass
 
# A utility function to print tree in order
 
def inorder(tree):
    if tree:
        inorder(tree.left)
        print(tree.value)
        inorder(tree.right)
 
 
# Tree:
#    50
#  /     \
# 30     70
#  / \ / \
# 20 40 60 80
 
r = BST(50)
r = insert(r, 30)
r = insert(r, 20)
r = insert(r, 40)
r = insert(r, 70)
r = insert(r, 60)
r = insert(r, 80)
 
# Print the BST in order
inorder(r)

# Expected output:
# 20
# 30
# 40
# 50
# 60
# 70
# 80
```

### Problem 2:

```python

class BST:
    def __init__(self, key):
        self.left = None
        self.right = None
        self.value = key
 
# TODO: Implement the insert function. This is very similar to the previous problem
def insert(tree, key):
    pass 
 
def inorder(tree):
    if tree:
        inorder(tree.left)
        print(tree.value)
        inorder(tree.right)
 
# Tree:
#     7
#  /     \
# 5       3
#  / \   / \
# 13 10 20 12
 
r = BST(7)
r = insert(r, 5)
r = insert(r, 13)
r = insert(r, 10)
r = insert(r, 3)
r = insert(r, 20)
r = insert(r, 12)
 
# Print the BST in order
inorder(r)

# Expected output:
# Should be similar to this
# 13
# 5
# 10
# 7
# 20
# 3
# 12
```