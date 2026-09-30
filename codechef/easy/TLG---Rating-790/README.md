# TLG - Rating 790

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### The Lead Game

The game of billiards involves two players knocking 3 balls around on a green baize table. Well, there is more to it, but for our purposes this is sufficient.

The game consists of several rounds and in each round both players obtain a score, based on how well they played. Once all the rounds have been played, the total score of each player is determined by adding up the scores in all the rounds and the player with the higher total score is declared the winner.

The Siruseri Sports Club organises an annual billiards game where the top two players of Siruseri play against each other. The Manager of Siruseri Sports Club decided to add his own twist to the game by changing the rules for determining the winner. In his version, at the end of each round, the  **cumulative score**  for each player is calculated, and the leader and her current lead are found. Once all the rounds are over the player who had the maximum lead at the end of any round in the game is declared the winner.

Consider the following score sheet for a game with 5 rounds:

Round	Player 1	Player 2
1	140	82
2	89	134
3	90	110
4	112	106
5	88	90

The total scores of both players, the leader and the lead after each round for this game is given below:

Round	Player 1	Player 2	Leader	Lead
1	140	82	Player 1	58
2	229	216	Player 1	13
3	319	326	Player 2	7
4	431	432	Player 2	1
5	519	522	Player 2	3

Note that the above table contains the cumulative scores.

The winner of this game is Player 1 as he had the maximum lead (58 at the end of round 1) during the game.

Your task is to help the Manager find the winner and the winning lead. You may assume that the scores will be such that there will always be a single winner. That is, there are no ties.

Input

The first line of the input will contain a single integer N (N ≤ 10000) indicating the number of rounds in the game. Lines 2,3,...,N+1 describe the scores of the two players in the N rounds. Line i+1 contains two integer Si and Ti, the scores of the Player 1 and 2 respectively, in round i. You may assume that 1 ≤ Si ≤ 1000 and 1 ≤ Ti ≤ 1000.

Output

Your output must consist of a single line containing two integers W and L, where W is 1 or 2 and indicates the winner and L is the maximum lead attained by the winner.

### Sample 1:
Input
Output

```
5
140 82
89 134
90 110
112 106
88 90
```

```
1 58
```

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-30T18:13:56.922Z  

```c_cpp
#include <stdio.h>

int main() {
    // your code goes here
    int n, x, y, z, p = 0;
    scanf("%d", & n);
    int cumsum1 = 0, cumsum2 = 0, maxlead = 0;
    while (n--)
    {
        scanf("%d%d", & x, & y);
        cumsum1 = cumsum1 + x;
        cumsum2 = cumsum2 + y;
        if (cumsum1 > cumsum2)
        {
            z = cumsum1 - cumsum2;

        }
        else
        {
            z = cumsum2 - cumsum1;

        }
        if (z > maxlead)
        {
            maxlead = z;

            if (cumsum1 > cumsum2)
                p = 1;
            else
                p = 2;
        }
    }


    printf("%d %d", p, maxlead);

}
```

---

[View on CodeChef](https://www.codechef.com/problems/TLG)