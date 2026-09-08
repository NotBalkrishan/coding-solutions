# SLEEP - Rating 348

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Sleep deprivation

A person is said to be sleep deprived if he slept  **strictly less than**  $7$ hours in a day.

Chef was only able to sleep $X$ hours yesterday. Determine if he is sleep deprived or not.

### Input Format
- The first line contains a single integer $T$ — the number of test cases. Then the test cases follow.
- The first and only line of each test case contains one integer $X$ — the number of hours Chef slept.
### Output Format

For each test case, output `YES` if Chef is sleep-deprived. Otherwise, output `NO`.

You may print each character of `YES` and `NO` in uppercase or lowercase (for example, `yes`, `yEs`, `Yes` will be considered identical).

### Constraints
- $1 \leq T \leq 20$
- $1 \le X \le 15$
### Sample 1:
Input
Output

```
3
4
7
10

```

```
YES
NO
NO

```

### Explanation:

 **Test Case 1:**  Since $4 \lt 7$, Chef is sleep deprived.

 **Test Case 2:**  Since $7 \ge 7$, Chef is not sleep deprived.

 **Test Case 3:**  Since $10 \ge 7$, Chef is not sleep deprived.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-08T14:14:01.404Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    (x<7)?printf("Yes\n"):printf("no\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/SLEEP)