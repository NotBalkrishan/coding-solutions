# MINPIZZA - Rating 546

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Minimum Pizzas

Each pizza consists of $4$ slices. There are $N$ friends and each friend needs exactly $X$ slices.

Find the  **minimum**  number of pizzas they should order to satisfy their appetite.

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case consists of two integers $N$ and $X$, the number of friends and the number of slices each friend wants respectively.
### Output Format

For each test case, output the  **minimum**  number of pizzas required.

### Constraints
- $1 \leq T \leq 100$
- $1 \leq N, X \leq 10$
### Sample 1:
Input
Output

```
4
1 5
2 6
4 3
3 5

```

```
2
3
3
4

```

### Explanation:

 **Test case $1$:**  There is only $1$ friend who requires $5$ slices. If he orders $1$ pizza, he will get only $4$ slices. Thus, at least $2$ pizzas should be ordered to have required number of slices.

 **Test case $2$:**  There are $2$ friends who require $6$ slices each. Thus, total $12$ slices are required. To get $12$ slices, they should order $3$ pizzas.

 **Test case $3$:**  There are $4$ friends who require $3$ slices each. Thus, total $12$ slices are required. To get $12$ slices, they should order $3$ pizzas.

 **Test case $4$:**  There are $3$ friends who require $5$ slices each. Thus, total $15$ slices are required. To get $15$ slices, they should order at least $4$ pizzas.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-15T11:52:04.801Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d",&n,&x);
	    if(n*x%4==0)
	    {
	        printf("%d\n",(n*x)/4);
	    }
	    else
	    {
	        printf("%d\n",((n*x)/4)+1);
	    }
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/MINPIZZA)