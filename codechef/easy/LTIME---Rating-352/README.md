# LTIME - Rating 352

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Lunchtime

Chef has his lunch only between $1$ pm and $4$ pm (both inclusive).

Given that the current time is $X$ pm, find out whether it is  *lunchtime*  for Chef.

### Input Format
- The first line of input will contain a single integer $T$, the number of test cases. Then the test cases follow.
- Each test case contains a single line of input, containing one integer $X$.
### Output Format

For each test case, print in a single line $\texttt{YES}$ if it is lunchtime for Chef. Otherwise, print $\texttt{NO}$.

You may print each character of the string in either uppercase or lowercase (for example, the strings $\texttt{YeS}$, $\texttt{yEs}$, $\texttt{yes}$ and $\texttt{YES}$ will all be treated as identical).

### Constraints
- $1 \leq T \leq 12$
- $1 \leq X \leq 12$
### Sample 1:
Input
Output

```
3
1
7
3
```

```
YES
NO
YES
```

### Explanation:

 **Test case $1$:**  Lunchtime is between $1$ pm and $4$ pm (both inclusive). Since $1$ pm lies within lunchtime, the answer is $\texttt{YES}$.

 **Test case $2$:**  Lunchtime is between $1$ pm and $4$ pm (both inclusive). Since $7$ pm lies outside lunchtime, the answer is $\texttt{NO}$.

 **Test case $3$:**  Lunchtime is between $1$ pm and $4$ pm (both inclusive). Since $3$ pm lies within lunchtime, the answer is $\texttt{YES}$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-08T17:37:12.055Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    (x>=1&&x<=4)?printf("Yes\n"):printf("no\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/LTIME)