# MINCARS - Rating 608

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Minimum Cars required

A single car can accommodate at most $4$ people.

$N$ friends want to go to a restaurant for a party. Find the  **minimum**  number of cars required to accommodate all the friends.

### Input Format
- The first line contains a single integer $T$ - the number of test cases. Then the test cases follow.
- The first and only line of each test case contains an integer $N$ - denoting the number of friends.
### Output Format

For each test case, output the minimum number of cars required to accommodate all the friends.

### Constraints
- $1 \leq T \leq 1000$
- $2 \leq N \leq 1000$
### Sample 1:
Input
Output

```
4
4
2
7
98

```

```
1
1
2
25

```

### Explanation:

 **Test Case $1$:**  There are only $4$ friends and a single car can accommodate $4$ people. Thus, only $1$ car is required.

 **Test Case $2$:**  There are only $2$ friends and a single car can accommodate $4$ people. Thus, only $1$ car is required

 **Test Case $3$:**  There are $7$ friends and $2$ cars can accommodate $8$ people. Thus, $2$ cars are required.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-17T17:28:52.319Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&n);
	    if(n%4==0)
	    {
	        printf("%d\n",n/4);
	    }
	    else
	    printf("%d\n",(n/4)+1);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/MINCARS)