# CHEFBOTTLE - Rating 660

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

_Description not available._

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-20T04:22:57.651Z  

```c_cpp
#include <stdio.h>

int main() {
    // your code goes here
    int t, n;
    
    scanf("%d",&t);
    while (t>0)
    {
        scanf("%d",&n);
        char s[n];
        for(int i=0;i<n;i++)
        {
            scanf(" %c ", &s[i]);
            
            if(s[i]=='A')
            {s[i]='T';}
            
            else if(s[i]=='T')
            {s[i]='A';}
            
            else if(s[i]=='C')
            {s[i]='G';}
            
            else if(s[i]=='G')
            {s[i]='C';}
            
            printf("%c",s[i]);
            
            

        }
        printf("\n");
        t--;
    }
}
```

---

[View on CodeChef](https://www.codechef.com/problems/CHEFBOTTLE)