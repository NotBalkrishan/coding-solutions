# SNDMAX - Rating 300

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Second Max of Three Numbers
### Problem Statement

Write a program that accepts sets of three numbers, and prints the  *second-maximum number*  among the three.

### Input
- First line contains the number of triples, N.
- The next N lines which follow each have three space separated integers.
### Output

For each of the  **N**  triples, output one new line which contains the second-maximum integer among the three.

### Constraints
- 1 ≤ N ≤ 6
- 1 ≤ every integer ≤ 10000
- The three integers in a single triplet are all distinct. That is, no two of them are equal.
### Sample 1:
Input
Output

```
3
1 2 3
10 15 5
100 999 500
```

```
2
10
500
```

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-07T02:38:17.827Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int n,x,y,z;
	scanf("%d",&n);
	while(n--)
	{
	    scanf("%d%d%d", &x,&y,&z);
	    if((x<y && x>z)||(x>y && x<z))
	    {
	        printf("%d\n", x);
	    }
	    else if((y>x && y<z)||(y<x && y>z))
	    {
	        printf("%d\n",y);
	    }
	    else 
	    printf("%d\n",z);
	    
	}
}


```

---

[View on CodeChef](https://www.codechef.com/problems/SNDMAX)