# REACHFAST - Rating 777

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Reach fast

Chef is standing at coordinate $A$ while Chefina is standing at coordinate $B$.

In one step, Chef can increase or decrease his coordinate by  **at most**  $K$.

Determine the  **minimum**  number of steps required by Chef to reach Chefina.

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case consists of three integers $A, B,$ and $K$, the initial coordinate of Chef, the initial coordinate of Chefina and the maximum number of coordinates Chef can move in one step.
### Output Format

For each test case, output the minimum number of steps required by Chef to reach Chefina.

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq A, B \leq 100$
- $1 \leq K \leq 100$
### Sample 1:
Input
Output

```
4
10 20 3
36 36 5
50 4 100
30 4 2

```

```
4
0
1
13

```

### Explanation:

 **Test case $1$:**  In the first three steps, Chef increases his coordinate by $K = 3$. In the fourth step, Chef increases his coordinate by $1$ which is less than equal to $K$. It can be shown that this is the minimum number of steps required by Chef.

 **Test case $2$:**  Chef is already at the same coordinate as Chefina. Thus, he needs $0$ steps.

 **Test case $3$:**  Chef can use $1$ step to decrease his coordinate by $46$ which is less than $K = 100$ and reach Chefina.

 **Test case $4$:**  Chef can use $13$ steps to decrease his coordinate by $K = 2$ and reach the coordinate $30-13\cdot 2 = 4$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T22:01:31.528Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,k;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&a,&b,&k);
	    if(a>b)
	    {
	        int z=a-b;
	        if(z%k==0)
	        printf("%d\n",z/k);
	        else
	        printf("%d\n",(z/k)+1);
	    }
	    else
	    {
	        int z=b-a;
	        if(z%k==0)
	        printf("%d\n",z/k);
	        else
	        printf("%d\n",(z/k)+1);
	    }
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/REACHFAST)