# INCRIQ - Rating 475

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-12T09:08:38.982Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n,m,k;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&n,&m,&k);
	    if(n*10>=m)
	    printf("%d\n",m*k);
	    else
	    printf("%d\n",n*k*10);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/INCRIQ)