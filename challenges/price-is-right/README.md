# The Price Is Right

The price is right is a game on tv where contestants win by guessing the monetary value (price) of the prizes. There are typically four contestants and each one gets a turn to guess. Each round, the contestant that guesses closest to the price without going over wins the round.

Challenge:
Write a function that takes the price and the guesses from the contestants, and determines the winner of the round by returning the index of the winning guess.

Requirements:\
[x] If a winner is not found, return -1.\
[x] Code must be clean and optimal.\
[x] Handle all error conditions and edge cases.

Examples:
* FindWinner(20, [21, 32, 4, 12]) => 3
* FindWinner(30, [36, 67, 90]) => -1
* FindWinner(20, [21, 19, 32, 4, 12]) => 1
