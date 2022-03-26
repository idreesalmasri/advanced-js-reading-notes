## Trees
Definition
A tree is a data structure consisting of a set of linked nodes that represent a hierarchical tree structure. Each node is linked to others via parent-children relationship. The first node in the tree is the root, whereas nodes without any children are the leaves.

Each node in a tree data structure must have the following properties:

- key: The key of the node
- value: The value of the node
- parent: The parent of the node (null if there is none)
- children: An array of pointers to the node's children

The main operations of a tree data structure are:

- insert: Inserts a node as a child of the given parent node
- remove: Removes a node and its children from the tree
- find: Retrieves a given node
- preOrderTraversal: Traverses the tree by recursively traversing each node followed by its children
- postOrderTraversal: Traverses the tree by recursively traversing each node's children  followed by the node

### Traversals

An important aspect of trees is how to traverse them. Traversing a tree allows us to search for a node, print out the contents of a tree, and much more! There are two categories of traversals when it comes to trees:

- Depth First
- Breadth First

 ####  Implementing a simple tree data structure
 ``` 
class TreeNode {
  constructor(value) {
    this.value = value;
    this.descendants = [];
  }
}
```

