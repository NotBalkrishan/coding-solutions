# PRESENTS - Rating 757

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Presents for Cheffina

Chef has fallen in love with Cheffina, and wants to buy $N$ gifts for her. On reaching the gift shop, Chef got to know the following two things:

- The cost of each gift is $1$ coin.
- On the purchase of every $4^{th}$ gift, Chef gets the $5^{th}$ gift free of cost.

What is the minimum number of coins that Chef will require in order to come out of the shop carrying $N$ gifts?

### Input Format
- The first line of input will contain an integer $T$ — the number of test cases. The description of $T$ test cases follows.
- The first and only line of each test case contains an integer $N$, the number of gifts in the shop.
### Output Format

For each test case, output on a new line the minimum number of coins that Chef will require to obtain all $N$ gifts.

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq N \leq 10^9$
### Sample 1:
Input
Output

```
2
5
4
```

```
4
4
```

### Explanation:

 **Test case $1$** : After purchasing $4$ gifts, Chef will get the $5^{th}$ gift free of cost. Hence Chef only requires $4$ coins in order to get $5$ gifts.

 **Test case $2$** : Chef will require $4$ coins in order to get $4$ gifts.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T16:01:03.722Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&n);
	    if(n%5==0)
	    printf("%d\n",n-(n/4));
	    else
	    printf("%d\n", n-(n/4)+1);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/PRESENTS)