# Find Hierarchical Parents

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
Write a function that can accepts the above 'flat' array, and returns an array with two elements, the first being an array containing all nodes with 0 parents, the second being an array contianing all nodes with only 1 parent.

```javascript
findParents(flat) => [
    [3, 8, 9], // 0 parents
    [2, 5, 6] // only 1 parent
]
```
