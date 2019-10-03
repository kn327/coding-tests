# Shares Ancestor

In computer science, a tree is a widely used abstract data type (ADT)—or data structure implementing this ADT—that simulates a hierarchical tree structure, with a root value and subtrees of children with a parent node, represented as a set of linked nodes.

An example of this would be a computer's file/folder structure.

You are passed an array of child-parent pairs which represents the tree:
```javascript
var flat = [
    [5, 3], [6, 8], [7, 8], [7, 9], [4, 5], [4, 6], [1, 6], [1, 7], [2, 7]
];
```
The above array represents the below tree.
```
  3      8    9
  |     / \  /
  5    6   7
   \  / \ / \
    4    1   2
```


Challenge:
Write a function that can accepts the above 'flat' array, and two nodes, and returns 'true' if the nodes share an ancestor or 'false' if the nodes do not share an ancestor.

Note: In the above tree, 3 does not have any ancestors, so even though 3 is a parent of 5, they do not share an ancestor.

```javascript
sharesAncestor(flat, 4, 2) => true
sharesAncestor(flat, 5, 2) => false
sharesAncestor(flat, 1, 2) => true
sharesAncestor(flat, 7, 9) => false
```
