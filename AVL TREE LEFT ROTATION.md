# Experiment 10(e): AVL Tree - Left Rotation

## Aim
To write a Python function `def leftRotate(self, z)` to perform the left rotation operation in an AVL Tree. Additionally, insert '7' into the existing AVL Tree and perform the necessary rotations to balance it.

---

## Algorithm

1. Define the `TreeNode` class to represent each node in the AVL Tree with:
   - Key value
   - Left and right child pointers
   - Height of the node
2. Define the `AVL_Tree` class to manage AVL Tree operations.
3. In the `insert()` method:
   - Insert the key using Binary Search Tree (BST) logic.
   - Update the height of the current node.
   - Calculate the balance factor to check if the node is unbalanced.
   - Based on balance factor and key position, perform the necessary rotations (left or right).
4. Define the `leftRotate(z)` method:
   - Let `y = z.right` and `T2 = y.left`.
   - Make `z` the left child of `y`.
   - Assign `T2` as the right child of `z`.
   - Update the heights of `z` and `y`.
   - Return `y` as the new root of the subtree.
5. Insert the key '7' using the `insert()` method. If it causes an imbalance, perform the appropriate rotation.
6. Display the AVL Tree structure after insertion and rotations using preOrder traversal.

---

## Program

```
from TreeAVL.AVL import AVL

def Construct_AVL(L):
  tree = AVL(L)
  print("Length of an AVL Tree is",tree.length_tree)

```

## OUTPUT
![image](https://github.com/user-attachments/assets/40ac664e-0ce2-4614-b965-5aecd6a630a4)

## RESULT

The left rotation operation in an AVL Tree was successfully implemented, and the insertion of key '7' triggered the appropriate rotation to maintain the tree's balance.
