# TIMELY - Rating 279

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Reach on Time

Chef has recently moved into an apartment. It takes $30$ minutes for Chef to reach office from the apartment.

Chef left for the office $X$ minutes before Chef was supposed to reach. Determine whether or not Chef will be able to reach on time.

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case consists of a single integer $X$.
### Output Format

For each test case, output `YES` if Chef will reach on time, `NO` otherwise.

The output is case-insensitive. Thus, the strings `YES`, `yes`, `yeS`, and `Yes` are all considered the same.

### Constraints
- $1 \leq T \leq 60$
- $1 \leq X \leq 60$
### Sample 1:
Input
Output

```
6
30
60
14
29
31
42

```

```
YES
YES
NO
NO
YES
YES

```

### Explanation:

 **Test case 1:**  Chef leaves $30$ minutes before he is supposed to reach, so he will reach the office exactly on time since it takes $30$ minutes to commute.

 **Test case 2:**  Chef will reach $30$ minutes early.

 **Test case 3:**  Chef will reach 16 minutes late.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-05T17:06:57.985Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d", &t);
	while (t--)
	{
	    scanf("%d", &x);
	    if(x>=30)
	    printf("YES \n");
	    else
	    printf("NO \n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/TIMELY)