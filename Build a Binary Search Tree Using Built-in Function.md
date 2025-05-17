# Ex. No: 15B - Build a Binary Search Tree Using Built-in Function

## AIM:
To write a Python program to build a binary search tree using a built-in function.

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

## PROGRAM:

```
from binarytree import Node
def _build_bst_from_sorted_values(sorted_values):
    if len(sorted_values)==0:
        return None
    mid_index=len(sorted_values)//2
    root=Node(sorted_values[mid_index])
    root.left=_build_bst_from_sorted_values(sorted_values[:mid_index])
    root.right=_build_bst_from_sorted_values(sorted_values[mid_index+1:])
    return (root)
def delete_BST(val):
    global x
    if val in x:
        x.remove(val)
        tree=_build_bst_from_sorted_values(sorted(x))
    else:
        return False
    return tree
def display(T):
    for i in T.values:
        print(i,'-->',end="")
x=[3,2,4,1]
print("BST before deletion:")
t=_build_bst_from_sorted_values(sorted(x))
display(t)
s=int(input())
print("\nBST after deletion:")
t1=delete_BST(s)
display(t1)
```

## OUTPUT
![Screenshot 2025-05-17 140531](https://github.com/user-attachments/assets/89aa319a-5f73-4f95-9180-25d7daa78137)

## RESULT
Thus the  Python program to build a binary search tree using a built-in function has been implemented and executed successfully.
