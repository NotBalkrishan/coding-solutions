# FSQRT - Rating 668

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Finding Square Roots

 *In olden days finding square roots seemed to be difficult but nowadays it can be easily done using in-built functions available across many languages* .

Assume that you happen to hear the above words and you want to give a try in finding the square root of any given integer using in-built functions. So here's your chance.

### Input

The first line of the input contains an integer T, the number of test cases. T lines follow. Each line contains an integer N whose square root needs to be computed.

### Output

For each line of the input, output the square root of the input integer, rounded down to the nearest integer, in a new line.

### Constraints

1<=T<=20
1<=N<=10000

### Sample 1:
Input
Output

```
3
10
5
10000
```

```
3
2
100
```

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-21T06:40:35.188Z  

```c_cpp
#include <stdio.h>

#include <math.h>

int main() {
    // your code goes here
    int t, x;
    scanf("%d", & t);
    while (t--)
    {
        scanf("%d", & x);
        float z=pow(x,0.5);
        printf("%.f\n",z);
    }

}
```

---

[View on CodeChef](https://www.codechef.com/problems/FSQRT)