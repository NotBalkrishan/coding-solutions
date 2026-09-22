# SPCP2 - Rating 711

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-22T14:10:25.711Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    int z=x/10;
	    if(x%5==0)
	    {
	        if(x%10==0)
	        printf("%d\n",(x/10));
	        else
	        {
	            x=x%10;
	            printf("%d\n",(x/5)+z);
	        }
	    }
	    else
	    printf("-1\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/SPCP2)