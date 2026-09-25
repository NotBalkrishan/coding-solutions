# PASSORFAIL - Rating 730

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T02:53:24.747Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,c;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&a,&b,&c);
	    if(a>b && a<c)
	    printf("%d\n",a);
	    else if(a>c && a<b)
	    printf("%d\n",a);
	    else if(b>a && b<c)
	    printf("%d\n",b);
	    else if(b>c && b<a)
	    printf("%d\n",b);
	    else if(c>a && c<b)
	    printf("%d\n",c);
	    else if(c>b && c<a)
	    printf("%d\n",c);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/PASSORFAIL)