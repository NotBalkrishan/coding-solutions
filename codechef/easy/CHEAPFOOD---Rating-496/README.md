# CHEAPFOOD - Rating 496

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Best Coupon

Chef is ordering food online (instead of cooking) and the bill comes out to be Rs. $X$. Chef can use one of the following two coupons to avail a discount.

- Get $10$ percent off on the bill amount
- Get a flat discount of Rs. $100$ on the bill amount

What is the maximum discount Chef can avail?

### Input Format
- The first line contains a single integer $T$ - the number of test cases. Then the test cases follow.
- The first and only line of each test case contains a single integer $X$ - the bill amount before discount.
### Output Format

For each testcase, output the maximum discount Chef can avail.

### Constraints
- $1 \leq T \leq 100$
- $100 \leq X \leq 10000$
- $X$ is a multiple of $100$.
### Sample 1:
Input
Output

```
3
300
1300
1000

```

```
100
130
100

```

### Explanation:

 **Test case 1:**  Using the second coupon, Chef can get a flat discount of Rs. $100$, which is maximum.

 **Test case 2:**  Using the first coupon, Chef can get a $10$ percent discount of Rs. $130$, which is maximum.

 **Test case 3:**  No matter which coupon Chef chooses Chef will get a discount of Rs. $100$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-13T04:53:02.911Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    if(100>=x*0.01*10)
	    printf("100\n");
	    else
	    printf("%d\n",x/10);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/CHEAPFOOD)