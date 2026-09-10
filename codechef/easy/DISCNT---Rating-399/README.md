# DISCNT - Rating 399

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-10T11:27:29.919Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y;
	scanf("%d", &t);
	for(int i=1;i<=t;i++)
	{
	    scanf("%d%d",&x,&y);
	    if(x>y)
	    printf("second\n");
	    else if(x<y)
	    printf("first\n");
	    else
	    printf("any\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/DISCNT)