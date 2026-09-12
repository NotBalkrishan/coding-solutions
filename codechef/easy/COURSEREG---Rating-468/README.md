# COURSEREG - Rating 468

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-12T08:58:00.983Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y,z;
	scanf("%d",&t);
	for(int i=1;i<=t;i++)
	{
	    scanf("%d%d%d",&x,&y,&z);
	    if((z*24*60)>=(x*y))
	    printf("yes\n");
	    else
	    printf("No\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/COURSEREG)