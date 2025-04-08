#  Build a Binary Tree with Float Values

## Aim
To create a binary tree using Python where the root, left, and right nodes hold float values. Values are taken from the user and stored in a list before building the tree.

## Procedure
1. Define a `Node` class with attributes for value, left child, and right child.
2. Accept three float values from the user and store them in a list.
3. Use these values to create a binary tree:
   - First value → root
   - Second value → left child
   - Third value → right child
4. Print the list of node values used to build the tree.

## Python Program
```python
class Node:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

# Step 1: Get float inputs from the user
values = []
for i in range(3):
    val = float(input(f"Enter value {i+1} (float): "))
    values.append(val)

# Step 2: Build the binary tree
root = Node(values[0])
root.left = Node(values[1])
root.right = Node(values[2])

# Step 3: Print the list of node values
print("List of node values in the binary tree:", values)
```
## Output:
![image](https://github.com/user-attachments/assets/1b82011c-1dda-4392-b4c6-1b24197ca709)

## Result:
The program accepts three float values from the user, builds a binary tree with those values, and prints the list of node values.
