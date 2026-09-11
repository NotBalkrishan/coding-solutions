# MANIPULATE - Rating 427

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Ezio and Guards

Ezio can manipulate  **at most**  $X$ number of guards with the apple of eden.

Given that there are $Y$ number of guards, predict if he can safely manipulate all of them.

### Input Format
- First line will contain $T$, number of test cases. Then the test cases follow.
- Each test case contains of a single line of input, two integers $X$ and $Y$.
### Output Format

For each test case, print $\texttt{YES}$ if it is possible for Ezio to manipulate all the guards. Otherwise, print $\texttt{NO}$.

You may print each character of the string in uppercase or lowercase (for example, the strings $\texttt{YeS}$, $\texttt{yEs}$, $\texttt{yes}$ and $\texttt{YES}$ will all be treated as identical).

### Constraints
- $1 \leq T \leq 100$
- $1 \leq X, Y \leq 100$
### Sample 1:
Input
Output

```
3
5 7
6 6
9 1
```

```
NO
YES
YES
```

### Explanation:

 **Test Case $1$:**  Ezio can manipulate at most $5$ guards. Since there are $7$ guards, he cannot manipulate all of them.

 **Test Case $2$:**  Ezio can manipulate at most $6$ guards. Since there are $6$ guards, he can manipulate all of them.

 **Test Case $3$:**  Ezio can manipulate at most $9$ guards. Since there is only $1$ guard, he can manipulate the guard.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-11T10:05:55.077Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y;
	scanf("%d",&t);
	for(int i=1;i<=t;i++)
	{
	    scanf("%d%d",&x,&y);
	    if(x>=y)
	    printf("Yes\n");
	    else
	    printf("No\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/MANIPULATE)