# Improvement of MinMax Algorithm step by step

## For this project we have used Tic-Tac-Toe game board as an input parameter. Algorithm uses below position and start to find best move for the X or O (depending on turn). 
```
| X | O | X |
| O |   |   |
|   |   |   |
```
### Step 1
This step only contains **Pure MinMax Algorithm**. Here we have pure algorithm and helper functions like measureTime. We have added iteration count to original algorithm to see how many iterations and how much time it will take to run.

### Step 2
This step contains **Alpha-Beta Prunning Algorithm**. Here we have updated MiniMax code that we prun some branches that we know it is useless to check them. We have added iteration count to original algorithm to see how many iterations and how much time it will take to run.


### Step 3
Here we add **PreSort** logic applied to **Step2**. In this case, there’s a higher chance of cutting of nodes within the game tree since the algorithm starts with a high alpha or low beta value at the beginning of each level.

### Step 4
Here we add **Transposition Tables** to ***Step3**. Transposition tables are used to store the result of already analyzed boards. This prevents the algorithm from evaluating the same board multiple times and reading it from a memory, the transposition table, instead.

### Finally we get an optimized algorithm that is 25 times faster than classic MinMax algorithm.
![result1](https://github.com/sadighasanzade/Improved-MinMax-Algorithm/assets/59266227/64108686-64c2-4662-b893-2642731c08d1)
![result2](https://github.com/sadighasanzade/Improved-MinMax-Algorithm/assets/59266227/905be1fb-7e10-4076-a547-abcca2a91512)

