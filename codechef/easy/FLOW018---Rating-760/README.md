# FLOW018 - Rating 760

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Small Factorial

Write a program to find the factorial value of any number entered by the user.

### Input Format

The first line contains an integer  **T**, the total number of testcases. Then  **T**  lines follow, each line contains an integer  **N**.

### Output Format

For each test case, display the factorial of the given number  **N**  in a new line.

### Constraints
- 1 ≤ T ≤ 1000
- 0 ≤ N ≤ 20
### Sample 1:
Input
Output

```
3 
3 
4
5

```

```
6
24
120

```

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-10-18T07:37:05.782Z  

```c_cpp
#include <stdio.h>

int main()
{
    int t, n, i, j;
    unsigned long long fact;

    scanf("%d", &t);

    for (i = 0; i < t; i++)
    {
        scanf("%d", &n);

        fact = 1;

        for (j = 1; j <= n; j++)
        {
            fact = fact * j;
        }

        printf("%llu\n", fact);
    }

    return 0;
}
```

---

[View on CodeChef](https://www.codechef.com/problems/FLOW018)