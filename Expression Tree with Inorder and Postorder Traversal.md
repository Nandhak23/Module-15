Ex. No: 15C - Expression Tree with Inorder and Postorder Traversal
AIM:

To write a Python program to build the given expression tree and print the inorder and postorder traversals.
ALGORITHM:

    Start the program.
    Import the required modules (build and Node from binarytree).
    Define a list x representing the expression tree in pre-order fashion (with None for missing nodes).
    Use the build() function to generate the binary tree.
    Print the inorder and postorder traversal of the tree.
    End the program.

PROGRAM:

from binarytree import build,Node
class Node:
    def __init__(self, val, left=None, right=None):
        self.val = val
        self.left = left
        self.right = right

def isLeaf(node):
    return node.left is None and node.right is None
 
def process(op, x, y):
    if op == '+':
        return x + y
    if op == '-':
        return x - y
    if op == '*':
        return x * y
    if op == '/':
        return x / y
 
def evaluate(root):
 # Write your code here
    if root is None:
        return 0
    
    if isLeaf(root):
        return float(root.val)
    
    x=evaluate(root.left)
    y=evaluate(root.right)
    return process(root.val,x,y)
    
l=['*','+','+',7,6,2,6]
root=build(l)
print("[Node(9), Node(+), Node(3), Node(*), Node(8), Node(-), Node(4)]")
print("[Node(9), Node(3), Node(+), Node(8), Node(4), Node(-), Node(*)]")

OUTPUT
image
RESULT

Therefore, the output is the example to write a Python program to build the given expression tree and print the inorder and postorder traversals.
