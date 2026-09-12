# INTEST - Rating 464

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Enormous Input Test

You are given $N$ integers. Find the count of numbers divisible by $K$.

### Input Format

The input begins with two positive integers $N$, $K$. The next $N$ lines contains one positive integer each denoted by $A_i$.

### Output Format

Output a single number denoting how many integers are divisible by $K$.

### Constraints
- $1 \leq N, K \leq 10^7$
- $1 \leq A_i \leq 10^9$
### Sample 1:
Input
Output

```
7 3
1
51
966369
7
9
999996
11

```

```
4
```

### Explanation:

The integers divisible by $3$ are $51, 966369, 9,$ and $999996$. Thus, there are $4$ integers in total.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-12T08:42:08.979Z  

```c_cpp
//We have populated the solutions for the 10 easiest problems for your support.
//Click on the SUBMIT button to make a submission to this problem.
#include<stdio.h>

int main()
{
	int n,k,ans=0,i;
	scanf("%d %d",&n,&k);
	
	for(i=0;i<n;i++)
	{
		int t;
		scanf("%d",&t);
		if(t%k==0)
		{
			ans++;
		}
	}
	printf("%d",ans);
	return 0;
}


```

---

[View on CodeChef](https://www.codechef.com/problems/INTEST)