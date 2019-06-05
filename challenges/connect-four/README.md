# Connect Four

Challenge:
Given a list of moves, write a function that will determine the winner and the winning move.

<details>
    <summary>What is Connect Four?</summary>
    <p>
A Connect Four window consists of a 7 x 6 grid of empty circles. Players switch after each move. Each move drops a token in one of the 7 top slots which falls to the bottommost available slot. A win is when there are four tokens of the same color in a row horizontally, diagonally, or vertically.
    </p>
    <img src="https://www3.nd.edu/~pbui/teaching/cdt.30010.fa16/static/img/connect4.png" />
</details>

```
var MOVES = [
  1, 3,
  2, 4,
  6, 5,
  6, 2,
  4, 3,
  5, 3,
  3, 4,
  3, 5,
  6, 3,
  5, 2
];

var BOARD = [
    [1], // 1
    [1, 2, 2], // 2
    [2, 2, 2, 1, 1, 2], // 3
    [2, 1, 2], // 4
    [2, 1, 2, 1], // 5
    [1, 1, 1], // 6
    [], // 7
];
```
