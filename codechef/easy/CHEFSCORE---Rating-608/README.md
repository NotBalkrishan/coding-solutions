# CHEFSCORE - Rating 608

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-17T17:28:53.393Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&n);
	    if(n%4==0)
	    {
	        printf("%d\n",n/4);
	    }
	    else
	    printf("%d\n",(n/4)+1);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/CHEFSCORE)