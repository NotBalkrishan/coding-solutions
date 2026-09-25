# REACHFAST - Rating 777

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T21:56:43.761Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n,k,x;
	scanf("%d",&t);
	while(t--)
	{
	    int count=0;
	    scanf("%d%d",&n,&k);
	    for(int i=1;i<=n;i++)
	    {
	        scanf("%d",&x);
	        if((k+x)%7==0)
	        {
	            count++;
	        }
	        
	    }
	    printf("%d\n",count);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/REACHFAST)