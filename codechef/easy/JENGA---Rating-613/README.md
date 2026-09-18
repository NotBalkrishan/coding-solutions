# JENGA - Rating 613

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Jenga Night

Chef hosts a party for his birthday. There are $N$ people at the party. All these $N$ people decide to play Jenga.

There are $X$ Jenga tiles available. In one round, all the players pick $1$ tile each and place it in the tower.
The game is  *valid*  if:

- All the players have a tile in each round;
- All the tiles are used at the end.

Given $N$ and $X$, find whether the game is  *valid*.

### Input Format
- First line will contain $T$, the number of test cases. Then the test cases follow.
- Each test case contains a single line of input, containing two space-separated integers $N$ and $X$ representing the number of people at the party and the number of available tiles respectively.
### Output Format

For each test case, output in a single line $\texttt{YES}$ if the game is valid, else output $\texttt{NO}$.

You may print each character of the string in uppercase or lowercase (for example, the strings $\texttt{YeS}$, $\texttt{yEs}$, $\texttt{yes}$ and $\texttt{YES}$ will all be treated as identical).

### Constraints
- $1 \leq T \leq 10^4$
- $1 \leq N, X \leq 1000$
### Sample 1:
Input
Output

```
3
3 3
4 2
2 4

```

```
YES
NO
YES

```

### Explanation:

 **Test case $1$:**  The game will last for $1$ round after which the tiles will finish.

 **Test case $2$:**  There are not enough Jenga tiles for everyone to place.

 **Test case $3$:**  The game will last for $2$ rounds as after round $2$ all Jenga tiles are used.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-18T11:05:40.740Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d",&n,&x);
	    if(x>=n)
	    {
	        if(x%n==0)
	        printf("Yes\n");
	        
	    }
	    
	    else
	    printf("No\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/JENGA)