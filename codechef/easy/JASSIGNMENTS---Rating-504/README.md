# JASSIGNMENTS - Rating 504

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-14T08:26:44.352Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d",&n,&x);
	    if(n%6!=0)
	    printf("%d\n",((n/6)+1)*x);
	    else
	    printf("%d\n",(n/6)*x);
	}
}


```

---

[View on CodeChef](https://www.codechef.com/problems/JASSIGNMENTS)