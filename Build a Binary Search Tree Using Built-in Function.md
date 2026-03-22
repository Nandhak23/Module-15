# Ex. No: 15B - Build a Binary Search Tree Using Built-in Function

## AIM:
To write a Python program to build a binary search tree using a built-in function.

---

## ALGORITHM:

1. **Start the program.**
2. Define `_build_bst_from_sorted_values(sorted_values)` to recursively build a binary search tree (BST) from a sorted list.
3. Define `left_subtree(l)` to print the left subtree of the BST.
4. Take user input for the number of elements and store the values in a list `a`.
5. Sort the list and pass it to `_build_bst_from_sorted_values()` to construct the BST.
6. Print the postorder traversal of the BST.
7. Call `left_subtree(l)` to print the left subtree.
8. Check whether the tree is a binary search tree using the `is_bst` property.
9. **End the program.**

---

## PROGRAM:

```python
from binarytree import Node
root=Node(1)
root.left=Node(2)
root.right=Node(3)
root.left.left=Node(5)
root.left.right=Node(6)
print("Binary tree: ")
for i in (root.values):
    print(i,"-->",end="")
print("\nLeft Subtree: ")
for i in (root[1].values):
    print(i,"-->",end="")
```

## OUTPUT
<img width="1182" height="260" alt="image" src="https://github.com/user-attachments/assets/a7867d36-ea9a-48a0-80ad-5a9da8527897" />

## RESULT
Therefore, the output is the example to write a Python program to build a binary search tree using a built-in function.
