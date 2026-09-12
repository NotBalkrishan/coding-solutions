# FLOW004 - Rating 461

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### First and Last Digit

Given an integer  **N** . Write a program to obtain the sum of the first and last digits of this number.

### Input Format

The first line contains an integer  **T**, the total number of test cases. Then follow  **T**  lines, each line contains an integer  **N**.

### Output Format

For each test case, display the sum of first and last digits of  **N**  in a new line.

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq N \leq 1000000$
### Sample 1:
Input
Output

```
3 
1234
124894
242323

```

```
5
5
5
```

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-12T08:41:16.454Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n;
	scanf("%d",&t);
	int sum=0;
	while(t>0)
	{
	    scanf("%d",&n);
	    int y=n%10;
	   while(n>=10)
	   {
	       n=n/10;
	   }
	   int z=n;
	   printf("%d\n", y+z);
	   t--;
	}
	   
	    
	

}


```

---

[View on CodeChef](https://www.codechef.com/problems/FLOW004)