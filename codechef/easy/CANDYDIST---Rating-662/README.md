# CANDYDIST - Rating 662

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-20T04:32:07.694Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n,x,k;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&n,&x,&k);
	    if(k>=x)
	    {
	        if((n*x)<=k)
	        printf("%d\n", n);
	        
	        else 
	        printf("%d\n", k/x);
	    }
	    
	    else
	    printf("0\n");
	    
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/CANDYDIST)