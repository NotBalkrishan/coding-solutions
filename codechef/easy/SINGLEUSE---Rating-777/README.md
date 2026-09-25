# SINGLEUSE - Rating 777

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T22:01:41.762Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,k;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&a,&b,&k);
	    if(a>b)
	    {
	        int z=a-b;
	        if(z%k==0)
	        printf("%d\n",z/k);
	        else
	        printf("%d\n",(z/k)+1);
	    }
	    else
	    {
	        int z=b-a;
	        if(z%k==0)
	        printf("%d\n",z/k);
	        else
	        printf("%d\n",(z/k)+1);
	    }
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/SINGLEUSE)