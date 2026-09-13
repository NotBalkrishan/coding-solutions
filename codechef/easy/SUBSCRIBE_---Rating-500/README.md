# SUBSCRIBE_ - Rating 500

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-13T12:08:23.545Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,c;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&a,&b,&c);
	    if(((a+b)*0.5)>c)
	    printf("YEs\n");
	    else
	    printf("No\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/SUBSCRIBE_)