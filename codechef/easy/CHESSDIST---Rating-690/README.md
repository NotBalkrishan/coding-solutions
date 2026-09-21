# CHESSDIST - Rating 690

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Chessboard Distance

The Chessboard Distance for any two points $(X_1, Y_1)$ and $(X_2, Y_2)$ on a Cartesian plane is defined as $max(|X_1 - X_2|, |Y_1 - Y_2|)$.

You are given two points $(X_1, Y_1)$ and $(X_2, Y_2)$. Output their Chessboard Distance.

Note that, $|P|$ denotes the absolute value of integer $P$. For example, $|-4| = 4$ and $|7| = 7$.

### Input Format
- First line will contain $T$, the number of test cases. Then the test cases follow.
- Each test case consists of a single line of input containing $4$ space separated integers - $X_1, Y_1, X_2, Y_2$ - as defined in the problem statement.
### Output Format

For each test case, output in a single line the chessboard distance between $(X_1, Y_1)$ and $(X_2, Y_2)$

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq X_1, Y_1, X_2, Y_2 \leq 10^5$
### Subtasks

 **Subtask #1 (100 points):**  original constraints

### Sample 1:
Input
Output

```
3
2 4 5 1
5 5 5 3
1 4 3 3

```

```
3
2
2

```

### Explanation:
- In the first case, the distance between $(2, 4)$ and $(5, 1)$ is $max(|2- 5|, |4 - 1|) = max(|-3|, |3|) = 3$.
- In the second case, the distance between $(5, 5)$ and $(5, 3)$ is $max(|5- 5|, |5 - 3|) = max(|0|, |2|) = 2$.
- In the third case, the distance between $(1, 4)$ and $(3, 3)$ is $max(|1- 3|, |4 - 3|) = max(|-2|, |1|) = 2$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-21T17:50:23.981Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y,n,m;
	scanf("%d",&t);
	for(int i=1;i<=t;i++)
	{
	    scanf("%d%d%d%d",&x,&y,&n,&m);
	    if((x-n)>=(n-x))
	    {
	        if((m-y)>=(y-m))
	        {
	            if((m-y)>=(x-n))
	            printf("%d\n", (m-y));
	            else
	            printf("%d\n", (x-n));
	        }
	        else
	        {
	            if((y-m)>=(x-n))
	            printf("%d\n", (y-m));
	            else
	            printf("%d\n", (x-n));
	        }
	    }
	    else
	    {
	        if((m-y)>=(y-m))
	        {
	            if((m-y)>=(n-x))
	            printf("%d\n", (m-y));
	            else
	            printf("%d\n", (n-x));
	        }
	        else
	        {
	            if((y-m)>=(n-x))
	            printf("%d\n", (y-m));
	            else
	            printf("%d\n", (n-x));
	        }
	    }
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/CHESSDIST)