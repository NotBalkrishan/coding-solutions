# CHEFEREN - Rating 706

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Chef Eren

Chef is a very big fan of Eren Yeager.

In the last season of Attack on Titan, there were $N$ episodes numbered from $1$ to $N$.
Each even indexed episode was $A$ minutes long and each odd indexed episode was $B$ minutes long.

Calculate the total duration (in minutes) of the last season.

### Input Format
- The first line of input contains a single integer $T$, the number of test cases.
- The first and only line of each test case contains three integers $N$, $A,$ and $B$, the number of episodes and the durations of each even-indexed and odd-indexed episodes respectively in minutes.
### Output Format

For each test case, print a single integer on a new line, the total duration of the last season in minutes.

### Constraints
- $1 \leq T \leq 100$
- $1 \leq N \leq 60$
- $1 \leq A, B \leq 60$
### Sample 1:
Input
Output

```
3
1 2 2
2 3 4
4 20 30
```

```
2
7
100
```

### Explanation:

 **Test case $1$:**  There is only one episode, so there is $1$ odd-indexed episode, and $0$ even-indexed episode. The total duration of the season $= 0\cdot A + 1\cdot B = 0\cdot 2 + 1\cdot 2 = 2$.

 **Test case $2$:**  There are two episodes with indices $\{1, 2\}$. Thus, there is $1$ odd-indexed episode $(\{1\})$, and $1$ even-indexed episode $(\{2\})$. The total duration of the season $= 1\cdot A + 1\cdot B = 1\cdot 3 + 1\cdot 4 = 7$.

 **Test case $3$** : There are four episodes with indices $\{1, 2, 3, 4\}$. Thus, there are $2$ odd-indexed episodes $(\{1, 3\})$, and $2$ even-indexed episodes $(\{2, 4\})$. The total duration of the season $= 2\cdot A + 2\cdot B = 2\cdot 20 + 2\cdot 30 = 100$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-22T14:01:03.463Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n,a,b;
	scanf("%d",&t);
	for(int i=1;i<=t;i++)
	{
	    scanf("%d%d%d",&n,&a,&b);
	    if(n%2==0)
	    printf("%d\n",(n/2)*(a+b));
	    else
	    printf("%d\n",((n/2)*a)+(((n/2)+1)*b));
	 }

}


```

---

[View on CodeChef](https://www.codechef.com/problems/CHEFEREN)