# TABLETS - Rating 376

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Multivitamin Tablets

The doctor prescribed Chef to take a multivitamin tablet $3$ times a day for the next $X$ days.

Chef already has $Y$ multivitamin tablets.

Determine if Chef has enough tablets for these $X$ days or not.

### Input Format
- The first line contains a single integer $T$ — the number of test cases. Then the test cases follow.
- The first and only line of each test case contains two space-separated integers $X$ and $Y$ — the number of days Chef needs to take tablets and the number of tablets Chef already has.
### Output Format

For each test case, output `YES` if Chef has enough tablets for these $X$ days. Otherwise, output `NO`.

You may print each character of `YES` and `NO` in uppercase or lowercase (for example, `yes`, `yEs`, `Yes` will be considered identical).

### Constraints
- $1 \leq T \leq 2000$
- $1 \le X \le 100$
- $0 \le Y \le 1000$
### Sample 1:
Input
Output

```
4
1 10
12 0
10 29
10 30

```

```
YES
NO
NO
YES

```

### Explanation:

 **Test Case 1:**  Chef has $10$ tablets and Chef needs $3$ tablets for $1$ day. Therefore Chef has enough tablets.

 **Test Case 2:**  Chef has $0$ tablets and Chef needs $36$ tablets for $12$ days. Therefore Chef does not have enough tablets.

 **Test Case 3:**  Chef has $29$ tablets and Chef needs $30$ tablets for $10$ days. Therefore Chef does not have enough tablets.

 **Test Case 4:**  Chef has $30$ tablets and Chef needs $30$ tablets for $10$ days. Therefore Chef has enough tablets.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-09T14:22:27.532Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y;
	scanf("%d", &t);
	for(int i=1;i<=t;i++)
	{
	    scanf("%d%d", &x,&y);
	    if(y>=x*3)
	    printf("yes\n");
	    else
	    printf("No\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/TABLETS)