# WATERREQ - Rating 351

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Water Requirement

Finally, after purchasing a water cooler during the April long challenge, Chef noticed that his water cooler requires $2$ liters of water to cool for  **one**  hour.

How much water (in liters) would be required by the cooler to cool for $N$ hours?

### Input Format
- The first line of input will contain an integer $T$ — the number of test cases. The description of $T$ test cases follows.
- The first and only line of each test case contains an integer $N$, as described in the problem statement.
### Output Format

For each test case, output the number of liters of water required by the water cooler to cool for $N$ hours.

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq N \leq 1000$
### Sample 1:
Input
Output

```
2
1
2
```

```
2
4

```

### Explanation:

 **Test case $1$** : As mentioned in the problem statement, $2$ liters of water is required by the water cooler to cool for $1$ hour.

 **Test case $2$** : $4$ liters of water is required by the water cooler to cool for $2$ hours.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-08T14:26:34.788Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n;
	scanf("%d",&t);
	while(t--)
	{   
	    scanf("%d",&n);
	    printf("%d\n",(2)*n);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/WATERREQ)