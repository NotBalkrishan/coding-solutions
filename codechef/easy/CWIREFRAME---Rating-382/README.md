# CWIREFRAME - Rating 382

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-09T14:25:17.751Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y;
	scanf("%d", &t);
	while(t--)
	{
	    scanf("%d%d", &x,&y);
	    if((3*x)>=(y*2))
	    printf("%d\n", y*2);
	    else
	    printf("%d\n", x*3);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/CWIREFRAME)