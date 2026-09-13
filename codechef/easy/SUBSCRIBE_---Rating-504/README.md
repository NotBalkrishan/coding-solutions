# SUBSCRIBE_ - Rating 504

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Subscriptions

A new TV streaming service was recently started in Chefland called the Chef-TV.

A group of $N$ friends in Chefland want to buy Chef-TV subscriptions. We know that $6$ people can share one Chef-TV subscription. Also, the cost of one Chef-TV subscription is $X$ rupees. Determine the minimum total cost that the group of $N$ friends will incur so that everyone in the group is able to use Chef-TV.

### Input Format
- The first line contains a single integer $T$ — the number of test cases. Then the test cases follow.
- The first and only line of each test case contains two integers $N$ and $X$ — the size of the group of friends and the cost of one subscription.
### Output Format

For each test case, output the minimum total cost that the group will incur so that everyone in the group is able to use Chef-TV.

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq N \leq 100$
- $1 \le X \le 1000$
### Sample 1:
Input
Output

```
3
1 100
12 250
16 135

```

```
100
500
405

```

### Explanation:
- Test case 1: There is only one person in the group. Therefore he will have to buy $1$ subscription. Therefore the total cost incurred is $100$.
- Test case 2: There are $12$ people in the group. Therefore they will have to buy $2$ subscriptions. Therefore the total cost incurred is $500$.
- Test case 3: There are $16$ people in the group. Therefore they will have to buy $3$ subscriptions. Therefore the total cost incurred is $405$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-13T17:45:41.351Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d",&n,&x);
	    if(1<=n &&n<=6)
	    printf("%d\n",x);
	    else if(n>6 && n<=12)
	    printf("%d\n",x*2);
	    else
	    printf("%d\n",x*3);
	}
}


```

---

[View on CodeChef](https://www.codechef.com/problems/SUBSCRIBE_)