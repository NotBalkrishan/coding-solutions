# DOMINANT - Rating 487

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-13T05:50:33.358Z  

```c_cpp
#include <stdio.h>
int main()
{
    int t,x,y;
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d%d",&x,&y);
        if(y<=1.07*x)
        printf("YEs\n");
        else
        printf("no\n");
    }
}
```

---

[View on CodeChef](https://www.codechef.com/problems/DOMINANT)