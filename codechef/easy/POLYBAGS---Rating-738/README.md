# POLYBAGS - Rating 738

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Too many items

Chef bought $N$ items from a shop. Although it is hard to carry all these items in hand, so Chef has to buy some polybags to store these items.

$1$ polybag can contain at most $10$ items. What is the minimum number of polybags needed by Chef?

### Input Format
- The first line will contain an integer $T$ - number of test cases. Then the test cases follow.
- The first and only line of each test case contains an integer $N$ - the number of items bought by Chef.
### Output Format

For each test case, output the minimum number of polybags required.

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq N \leq 1000$
### Sample 1:
Input
Output

```
3
20
24
99

```

```
2
3
10

```

### Explanation:

 **Test case-1:**  Chef will require $2$ polybags. Chef can fit $10$ items in the first and second polybag each.

 **Test case-2:**  Chef will require $3$ polybags. Chef can fit $10$ items in the first and second polybag each and fit the remaining $4$ items in the third polybag.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T03:00:18.853Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    if(x%10==0)
	    printf("%d\n", x/10);
	    else 
	    printf("%d\n", (x/10)+1);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/POLYBAGS)