# SALE - Rating 778

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Get Lowest Free

Chef goes to the supermarket to buy some items. Luckily there's a sale going on under which Chef gets the following offer:

- If Chef buys $3$ items then he gets the item (out of those $3$ items) having the lowest price as free.

For e.g. if Chef bought $3$ items with the cost $6$, $2$ and $4$, then he would get the item with cost $2$ as free. So he would only have to pay the cost of the other two items which will be $6 + 4 = 10$.

Chef buys $3$ items having prices $A$, $B$ and $C$ respectively. What is the amount of money Chef needs to pay?

### Input Format
- The first line will contain an integer $T$ - number of test cases. Then the test cases follow.
- The first and only line of each test case contains three integers $A, B, C$ - the prices of the items bought by Chef.
### Output Format

For each test case, output the price paid by Chef.

### Constraints
- $1 \leq T \leq 100$
- $1 \leq A, B, C \leq 10$
### Sample 1:
Input
Output

```
3
6 2 4
3 3 3
8 4 4

```

```
10
6
12

```

### Explanation:

 **Test case-1:**  Explained in the problem statement.

 **Test case-2:**  Since all the three items have the same price, Chef will get one of them free and will have to pay the cost of the other two items which will be $3 + 3 = 6$.

 **Test case-3:**  Chef will get one of the items having price $4$ as free and will have to pay the cost of the other two items which will be $8 + 4 = 12$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T22:08:21.798Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,c;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&a,&b,&c);
	    if(a<=b && a<=c)
	    printf("%d\n",b+c);
	    else if(b<=a && b<=c)
	    printf("%d\n", a+c);
	    else
	    printf("%d\n", a+b);
	}
	

}


```

---

[View on CodeChef](https://www.codechef.com/problems/SALE)