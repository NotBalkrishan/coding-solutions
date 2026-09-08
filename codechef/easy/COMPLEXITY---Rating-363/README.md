# COMPLEXITY - Rating 363

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-08T17:59:58.181Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n,x,k;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&n,&x,&k);
	    (k>=n*x)?printf("Yes\n"):printf("No\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/COMPLEXITY)