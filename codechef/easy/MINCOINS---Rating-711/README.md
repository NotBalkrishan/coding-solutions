# MINCOINS - Rating 711

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Minimum number of coins

Chef has infinite coins in denominations of rupees $5$ and rupees $10$.

Find the  **minimum**  number of coins Chef needs, to pay  **exactly**  $X$ rupees. If it is impossible to pay $X$ rupees in denominations of rupees $5$ and $10$ only, print $-1$.

### Input Format
- First line will contain $T$, number of test cases. Then the test cases follow.
- Each test case contains of a single integer $X$.
### Output Format

For each test case, print a single integer - the  **minimum**  number of coins Chef needs, to pay  **exactly**  $X$ rupees. If it is impossible to pay $X$ rupees in denominations of rupees $5$ and $10$ only, print $-1$.

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq X \leq 1000$
### Subtasks
- Subtask 1 (100 points): Original constraints.
### Sample 1:
Input
Output

```
3
50
15
8

```

```
5
2
-1

```

### Explanation:

 **Test Case $1$:**  Chef would require at least $5$ coins to pay $50$ rupees. All these coins would be of rupees $10$.

 **Test Case $2$:**  Chef would require at least $2$ coins to pay $15$ rupees. Out of these, $1$ coin would be of rupees $10$ and $1$ coin would be of rupees $5$.

 **Test Case $3$:**  Chef cannot pay exactly $8$ rupees in denominations of rupees $5$ and $10$ only.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-22T14:10:20.934Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    int z=x/10;
	    if(x%5==0)
	    {
	        if(x%10==0)
	        printf("%d\n",(x/10));
	        else
	        {
	            x=x%10;
	            printf("%d\n",(x/5)+z);
	        }
	    }
	    else
	    printf("-1\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/MINCOINS)