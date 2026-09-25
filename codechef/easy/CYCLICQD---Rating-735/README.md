# CYCLICQD - Rating 735

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Cyclic Quadrilateral

You are given the sizes of angles of a simple quadrilateral (in degrees) $A$, $B$, $C$ and $D$, in some order along its perimeter. Determine whether the quadrilateral is cyclic.

Note: A quadrilateral is cyclic if and only if the sum of opposite angles is $180^{\circ}$.

### Input
- The first line of the input contains a single integer $T$ denoting the number of test cases. The description of $T$ test cases follows.
- The first and only line of each test case contains four space-separated integers $A$, $B$, $C$ and $D$.
### Output

Print a single line containing the string `"YES"` if the given quadrilateral is cyclic or `"NO"` if it is not (without quotes).

You may print each character of the string in uppercase or lowercase (for example, the strings "yEs", "yes", "Yes" and "YES" will all be treated as identical).

### Constraints
- $1 \leq T \leq 10^4$
- $1 \leq A, B, C, D \leq 357$
- $A + B + C + D = 360$
### Sample 1:
Input
Output

```
3
10 20 30 300
10 20 170 160
179 1 179 1
```

```
NO
YES
NO
```

### Explanation:

 **Example case 1:**  The sum of two opposite angles $A + C = 10^{\circ} + 30^{\circ} \neq 180^{\circ}$.

 **Example case 2:**  The sum of two opposite angles $A + C = 10^{\circ} + 170^{\circ} = 180^{\circ}$ and $B + D = 20^{\circ} + 160^{\circ} = 180^{\circ}$.

 **Example case 3:**  The sum of two opposite angles $B + D = 1^{\circ} + 1^{\circ} \neq 180^{\circ}$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T02:58:21.208Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,c,d;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d%d",&a,&b,&c,&d);
	    if(((a+c)==180) && ((b+d)==180))
	    printf("YEs\n");
	    else 
	    printf("No\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/CYCLICQD)