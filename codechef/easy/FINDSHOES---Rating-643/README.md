# FINDSHOES - Rating 643

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-18T11:36:41.262Z  

```c_cpp
#include <stdio.h>

int main() {
        // your code goes here
        int t, x, y;
        scanf("%d", & t);
        while (t--)
        {
            scanf("%d%d", & x, & y);
            if (x > y)
            {
                if (x < (2 * y))
                    printf("0\n");
                else 
                printf("%d\n", x/(2*y));

            }
            else
            printf("0\n");
        }
}
```

---

[View on CodeChef](https://www.codechef.com/problems/FINDSHOES)