# Trees
is a the data structure representaional gragh
# Traversals
There are two categories of traversals when it comes to trees:
- Depth First: where we prioritize going through the depth (height) of the tree first.(uses a stack)
- Breadth First: Breadth first traversal iterates through the tree by going through each level of the tree node-by-node(uses a queue)

Here are three methods for depth first traversal:

* Pre-order: `root >> left >> right`
* In-order: `left >> root >> right`
* Post-order: `left >> right >> root`
 **Depth First Example:**
![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/tree-example.png)


- Pre-order: `A, B, D, E, C, F`
- In-order: `D, B, E, A, F, C`
- Post-order: `D, E, B, F, C, A`

 **Breadth First Example:**
![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/tree-example.png)
Output: `A, B, C, D, E, F`

# Binary Trees
 Trees can have any number of children per node, but Binary Trees restrict the number of children to two
 There is no specific sorting order for a binary tree
 # Binary Search Trees BST
 In a BST, nodes are organized in a manner where all values that are **smaller** than the root are placed to the **left**, and all values that are **larger** than the root are placed to the **right**.
*that helps in searching the BST*,because all you do is compare the node you are searching for against the root of the tree or sub-tree
