# ELECTN - Rating 594

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-17T17:19:12.375Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&x,&a,&b);
	    if(((a*1)+(b*2))>=x)
	    printf("qualify\n");
	    else
	    printf("notqualify\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/ELECTN)