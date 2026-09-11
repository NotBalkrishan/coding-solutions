# BROKENPHONE - Rating 451

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Broken Phone

Uttu broke his phone. He can get it repaired by spending $X$ rupees or he can buy a new phone by spending $Y$ rupees. Uttu wants to spend as little money as possible. Find out if it is better to get the phone repaired or to buy a new phone.

### Input Format
- The first line contains a single integer $T$ — the number of test cases. Then the test cases follow.
- The first and only line of each test case contains two space-separated integers $X$ and $Y$ — the cost of getting the phone repaired and the cost of buying a new phone.
### Output Format

For each test case,

- output REPAIR if it is better to get the phone repaired.
- output NEW PHONE if it is better to buy a new phone.
- output ANY if both the options have the same price.

You may print each character of `REPAIR`, `NEW PHONE` and `ANY` in uppercase or lowercase (for example, `any`, `ANy`, `Any` will be considered identical).

### Constraints
- $1 \leq T \leq 1000$
- $1 \le X, Y \le 10^4$
### Sample 1:
Input
Output

```
3
100 1000
10000 5000
3000 3000

```

```
REPAIR
NEW PHONE
ANY

```

### Explanation:

 **Test Case 1:**  It is better to get the phone repaired since $100 \lt 1000$.

 **Test Case 2:**  It is better to buy a new phone since $10000 \gt 5000$.

 **Test Case 3:**  Uttu can choose either of the two options since $3000 = 3000$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-11T13:52:37.610Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d",&x,&y);
	    if(x<y)
	    printf("Repair\n");
	    else if(x>y)
	    printf("new Phone\n");
	    else
	    printf("Any\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/BROKENPHONE)