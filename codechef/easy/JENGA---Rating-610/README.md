# JENGA - Rating 610

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-18T01:48:50.774Z  

```c_cpp
#include <stdio.h>

int main() {
    // your code goes here
    int t, n, x, y;
    scanf("%d", & t);
    while (t--)
    {
        scanf("%d%d%d", & n, & x, & y);
        if (y >= 0)
        {
            if (y > (x * n))
            {
                printf("no\n");
                continue;
            }
            else if (y % x == 0)
                printf("Yes\n");


            else
                printf("No\n");
        }
        else
            continue;




    }

}
```

---

[View on CodeChef](https://www.codechef.com/problems/JENGA)