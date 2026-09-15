# CREDCOINS - Rating 539

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### CRED Coins

For each bill you pay using CRED, you earn $X$ CRED coins.
At CodeChef store, each bag is worth $100$ CRED coins.

Chef pays $Y$ number of bills using CRED. Find the  **maximum**  number of bags he can get from the CodeChef store.

### Input Format
- First line will contain $T$, number of test cases. Then the test cases follow.
- Each test case contains of a single line of input, two integers $X$ and $Y$.
### Output Format

For each test case, output in a single line - the  **maximum**  number of bags Chef can get from the CodeChef store.

### Constraints
- $1 \leq T \leq 100$
- $1 \leq X,Y \leq 1000$
### Subtasks
- Subtask 1 (100 points): Original constraints.
### Sample 1:
Input
Output

```
3
10 10
20 4
70 7
```

```
1
0
4
```

### Explanation:

 **Test Case $1$:**  For each bill payment, one receives $10$ CRED coins. Chef pays $10$ bills using CRED. Thus, he receives $100$ CRED coins. Chef can get $1$ bag from the CodeChef store using these coins.

 **Test Case $2$:**  For each bill payment, one receives $20$ CRED coins. Chef pays $4$ bills using CRED. Thus, he receives $80$ CRED coins. Chef cannot get any bag from the CodeChef store using these coins.

 **Test Case $3$:**  For each bill payment, one receives $70$ CRED coins. Chef pays $7$ bills using CRED. Thus, he receives $490$ CRED coins. Chef can get at most $4$ bags from the CodeChef store using these coins.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-15T10:57:55.823Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d",&x,&y);
	    int z=x*y;
	    printf("%d\n", z/100);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/CREDCOINS)