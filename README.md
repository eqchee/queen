# Queens Puzzle



## About The Project

The queens puzzle is the problem of placing chess queens on a chessboard so that no two queens threaten each other. This algorithm has been designed to determine the number of ways to place 10 to 12 queens on a 14 x 14 chessboard given the positions of 4 to 2 queens respectively.

A naive algorithm would be computationally expensive as it would effectively involve placing 12 queens on a 12x12 chessboard, ie. 1.03E+17 possible arrangements. Constraint programming can be used to help reduce the number of possibilities to consider.  

1. Since there can only be one queen in each row,  this would help to reduce the number of possibilities to 12^12, ie. 8.92E+12
2. If permutation of the columns for the remaining queens is considered, this would further reduce the number of possibilities to 12!, ie. 4.79E+8
3. A check can be done to ensure there is no diagonal attack from the previously placed queens as the permutation is being generated. This will help to stop fully generating permutations that would not work and further reduce the possibilities to consider.  

