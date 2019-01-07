# Computing Total Score

Challenge:
You are passed an array of blocks to compute the total score.

The blocks are processed as follows:
    * If a block is an integer, the score for that throw is the value of that integer
    * If a block is an "X", the score for that throw is double the value of the last integer
    * If a block is a "+", the score for that throw is the sum of the prior two throws
    * If a block is a "Z", the previous throw is thrown away (as if it never happened)

