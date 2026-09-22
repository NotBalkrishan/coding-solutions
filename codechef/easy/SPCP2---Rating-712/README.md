# SPCP2 - Rating 712

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Airlines

An airline operates $X$ aircraft every day. Each aircraft can carry up to $100$ passengers.
One day, $N$ passengers would like to travel to the same destination. What is the minimum number of new planes that the airline must buy to carry all $N$ passengers?

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case consists of a single line containing two space-separated integers $X$ and $N$ — the number of aircraft the airline owns and the number of passengers travelling, respectively.
### Output Format
- For each test case, output the minimum number of planes the airline needs to purchase.
### Constraints
- $1 \leq T \leq 1000$
- $1 \leq X \leq 10^6$
- $1 \leq N \leq 10^6$
### Sample 1:
Input
Output

```
3
4 600
3 523
8 245
```

```
2
3
0
```

### Explanation:

 **Test case $1$:**  The airline needs at least $6$ planes to carry $600$ passengers. They already have $4$, so they must purchase $2$ more.

 **Test case $2$:**  The airline needs at least $6$ planes to carry $523$ passengers. They already have $3$, so they must purchase $3$ more.

 **Test case $3$:**  The airline needs at least $3$ planes to carry $245$ passengers. They already have $8$, so there's no need to purchase any more.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-22T14:32:34.424Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,n;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d",&x,&n);
	    if(n>x*100)
	    {
	        if(n%100==0)
	        printf("%d\n",(n/100)-x);
	        else
	        printf("%d\n",((n/100)+1)-x);
	    }
	    else
	    printf("0\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/SPCP2)