# SUGARCANE - Rating 562

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-15T18:30:55.517Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,x,y;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d%d",&a,&b,&x,&y);
	    if((a*b)<=(x*y))
	    printf("YES\n");
	    else
	    printf("NO\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/SUGARCANE)