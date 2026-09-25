# MOZZ - Rating 745

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T14:10:24.118Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,x,y;
	scanf("%d",&t);
	while(t--)
	{
	    int count=0;
	    scanf("%d%d%d%d",&x,&y,&a,&b);
	    if(x!=a && x!=b)
	    count++;
	    if(y!=a && y!=b)
	    count++;
	    
	    printf("%d\n", count);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/MOZZ)