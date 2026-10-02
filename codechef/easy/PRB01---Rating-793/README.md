# PRB01 - Rating 793

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-10-02T14:56:31.369Z  

```c_cpp
#include <stdio.h>

int main()
{
    // your code goes here
    int t, n;
    scanf("%d", & t);
    
    while (t--)
    {
        scanf("%d", & n);
        int count1 = 0, count2 = 0;
        char a[20];
        for (int i = 0; i < n; i++)
        {
            scanf("%s", & a);
            if(strcmp(a,"START38"))
            count2++;
            if(strcmp(a,"LTIME108"))
            count1++;
        }
        printf("%d %d \n",count1,count2);

    }

}
```

---

[View on CodeChef](https://www.codechef.com/problems/PRB01)