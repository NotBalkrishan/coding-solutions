# MANGOES - Rating 481

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-12T09:15:59.997Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,w,x,y,z;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d%d",&w,&x,&y,&z);
	    printf("%d\n",(w+((x-y)*z)));
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/MANGOES)