# FLOW018 - Rating 760

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Small Factorial

Write a program to find the factorial value of any number entered by the user.

### Input Format

The first line contains an integer  **T**, the total number of testcases. Then  **T**  lines follow, each line contains an integer  **N**.

### Output Format

For each test case, display the factorial of the given number  **N**  in a new line.

### Constraints
- 1 ≤ T ≤ 1000
- 0 ≤ N ≤ 20
### Sample 1:
Input
Output

```
3 
3 
4
5

```

```
6
24
120

```

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T16:09:12.617Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n;
	scanf("%d",&t);
	while(t--)
	{
	    int fact=1;
	    scanf("%d",&n);
	    for(int i=1;i<=n;i++)
	    {
	        fact=fact*i;
	    }
	    
	    printf("%d\n", fact);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/FLOW018)