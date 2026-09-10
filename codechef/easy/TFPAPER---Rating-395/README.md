# TFPAPER - Rating 395

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-10T11:21:22.953Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d", &t);
	for(int i=1;i<=t;i++)
	{
	    scanf("%d", &x);
	    if(x<=3)
	    printf("Bronze\n");
	    else if(x>3&&x<=6)
	    printf("Silver\n");
	    else
	    printf("Gold\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/TFPAPER)