# Word Puzzle

Challenge:
Given a dictionary of words, implement a function that will take a puzzle and will return the number of all <i>non-distinct</i> occurrences of a words found in the array, horizontally, vertically, or diagonally, <b>and</b> also the reverse in each direction.

The idea here is to get a sense of your coding style. Don’t worry about producing the ideal solution regarding memory usage or performance as the solution won’t be graded on efficiency, but rather on correctness and completeness. It should, however be capable of scaling to puzzles with dimensions such as 4x4, 6x9, 9x9.

```
var DICTIONARY = ["OX","CAT","TOY","AT","DOG","CATAPULT","T"];
```

```
var exampleInput1 = [
    ["C", "A", "T"],
    ["X", "Z", "T"],
    ["Y", "O", "T"],
];
```
< expected output: 8 (AT, AT, CAT, OX, TOY, T, T, T)

```
var exampleInput2 = [
    ["C", "A", "T", "A", "P", "U", "L", "T"],
    ["X", "Z", "T", "T", "O", "Y", "O", "O"],
    ["Y", "O", "T", "O", "X", "T", "X", "X"],
];
```
< expected output: 22
