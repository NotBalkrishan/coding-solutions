# BULLET - Rating 649

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-19T09:24:27.298Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    if(x%3==0)
	    printf("Normal\n");
	    else if(x%3==1)
	    printf("Huge\n");
	    else
	    printf("Small\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/BULLET)