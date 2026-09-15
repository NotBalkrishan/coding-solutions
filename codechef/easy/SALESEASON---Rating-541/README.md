# SALESEASON - Rating 541

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Sale Season

It's the sale season again and Chef bought items worth a total of $X$ rupees. The sale season offer is as follows:

- if $X \le 100$, no discount.
- if $100 \lt X \le 1000$, discount is $25$ rupees.
- if $1000 \lt X \le 5000$, discount is $100$ rupees.
- if $X \gt 5000$, discount is $500$ rupees.

Find the final amount Chef needs to pay for his shopping.

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case consists of single line of input containing an integer $X$.
### Output Format

For each test case, output on a new line the final amount Chef needs to pay for his shopping.

### Constraints
- $1 \leq T \leq 100$
- $1 \leq X \leq 10000$
### Sample 1:
Input
Output

```
4
15
70
250
1000

```

```
15
70
225
975

```

### Explanation:

 **Test case $1$:**  Since $X \le 100$, there is no discount.

 **Test case $3$:**  Here, $X = 250$. Since $100 \lt 250 \le 1000$, discount is of $25$ rupees. Therefore, Chef needs to pay $250-25 = 225$ rupees.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-15T11:45:32.065Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    if(x<=100)
	    printf("%d\n",x);
	    else if(x>100 && x<=1000)
	    printf("%d\n", x-25);
	    else if(x>1000 && x>=5000)
	    printf("%d\n", x-100);
	    else
	    printf("%d\n", x-500);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/SALESEASON)