# CHESSDIST - Rating 686

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-21T13:35:14.402Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y;
	scanf("%d",&t);
	for(int i=1;i<=t;i++)
	{
	    scanf("%d%d",&x,&y);
	    int z=x/y;
	    
	    if(x%y==0)
	    printf("%d\n", z);
	    else
	    printf("%d\n", z+(x-(y*z)));
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/CHESSDIST)