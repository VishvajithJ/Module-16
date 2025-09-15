# Experiment 10(b): Balancing AVL Tree

## Aim
To write a Python program to construct an AVL tree, balance it, and print the nodes of the tree before and after balancing using the appropriate packages and built-in functions.

---

## Algorithm

1. Start the program.
2. Define `getDictTree(self)` to return the dictionary representation of the AVL tree.
3. Define `Construct_AVL(L)` to:
   - Create the AVL tree from the list `L`.
   - Print the tree before balancing.
   - Balance the tree using the `BalanceTree()` method.
   - Print the tree after balancing.
4. Create a list `L` of integers.
5. Call `Construct_AVL(L)` to build and balance the tree.
6. End the program.

---

## Program

```
from TreeAVL.AVL import AVL

def getDictTree(self):
    return self.dict_tree

def Construct_AVL(L):
    tree=AVL(L)
    
    print("AVL Tree Before Balancing\n",getDictTree(tree))
    tree.BalanceTree()
    print("AVL Tree After Balancing\n",getDictTree(tree))
L=[11,8,18,5,13,17,4,7,2]

```
## OUTPUT
![image](https://github.com/user-attachments/assets/fd32a79a-620d-4445-a4cf-05ddff23c432)

## RESULT
The Python program for constructing and balancing an AVL tree was successfully implemented. The AVL tree structure was correctly displayed before and after balancing, verifying that the BalanceTree() method effectively restructured the tree to maintain AVL balance properties.








