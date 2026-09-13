# WATERCOOLER2 - Rating 798

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### The Cooler Dilemma 2

The summer is at its peak in Chefland. Chef is planning to purchase a water cooler to keep his room cool. He has two options available:

- Rent a cooler at the cost of $X$ coins per month.
- Purchase a cooler for $Y$ coins.

Chef wonders what is the  **maximum**  number of months for which he can rent the cooler such that the cost of renting is  **strictly less**  than the cost of purchasing it.

### Input Format
- The first line of input will contain an integer $T$ — the number of test cases. The description of $T$ test cases follows.
- The first and only line of each test case contains two integers $X$ and $Y$, as described in the problem statement.
### Output Format

For each test case, output the  **maximum**  number of months for which he can rent the cooler such that the cost of renting is  **strictly less**  than the cost of purchasing it.

If Chef should not rent a cooler at all, output $0$.

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq X, Y \leq 10^9$
### Sample 1:
Input
Output

```
2
5 12
5 5
```

```
2
0
```

### Explanation:

 **Test case $1$** : Cost of renting the cooler $= 5$ coins per month. Cost of purchasing the cooler $= 12$ coins. So, Chef can rent the cooler for $2$ months at the cost of $10$ coins, which is  **strictly less**  than $12$ coins.

 **Test case $2$** : Cost of renting the cooler $= 5$ coins per month. Cost of purchasing the cooler $= 5$ coins. If Chef rents the cooler for $1$ month, it will cost $5$ coins, which is  **not strictly less**  than the cost of purchasing it. So, Chef should not rent the cooler.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-13T17:33:04.752Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	
	int t,x,y,m;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d",&x,&y);
	    if(x<y)
	    printf("%d\n", y/x);
	    else 
	    printf("0\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/WATERCOOLER2)