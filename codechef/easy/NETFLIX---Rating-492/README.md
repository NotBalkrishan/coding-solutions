# NETFLIX - Rating 492

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-13T04:38:57.021Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,c,x,y;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&c,&x,&y);
	    int z=c-x;
	    printf("%d\n",z*y);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/NETFLIX)