# FLOW007 - Rating 588

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Reverse The Number

Given an Integer  **N**, write a program to reverse it.

### Input

The first line contains an integer  **T**, total number of testcases. Then follow  **T**  lines, each line contains an integer  **N**.

### Output

For each test case, display the reverse of the given number  **N**, in a new line.

### Constraints
- 1 ≤ T ≤ 1000
- 1 ≤ N ≤ 1000000
### Sample 1:
Input
Output

```
4
12345
31203
2123
2300
```

```
54321
30213
3212
32
```

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-17T17:10:10.251Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&n);
	    int sum=0;
	    while(n!=0)
	    {
	        x=n%10;
	        n=n/10;
	        sum=sum*10+x;
	    }
	    printf("%d\n",sum);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/FLOW007)