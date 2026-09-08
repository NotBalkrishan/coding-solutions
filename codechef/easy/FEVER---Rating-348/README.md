# FEVER - Rating 348

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Fever

Chef is not feeling well today. He measured his body temperature using a thermometer and it came out to be $X$ °F.

A person is said to have fever if his body temperature is  **strictly greater**  than $98$ °F.

Determine if Chef has fever or not.

### Input Format
- The first line contains a single integer $T$ — the number of test cases. Then the test cases follow.
- The first and only line of each test case contains one integer $X$ - the body temperature of Chef in °F.
### Output Format

For each test case, output `YES` if Chef has fever. Otherwise, output `NO`.

You may print each character of `YES` and `NO` in uppercase or lowercase (for example, `yes`, `yEs`, `Yes` will be considered identical).

### Constraints
- $1 \le T \le 10$
- $94 \le X \le 103$
### Sample 1:
Input
Output

```
3
98
100
96

```

```
NO
YES
NO

```

### Explanation:

 **Test Case 1** : Since $X = 98$ is not greater than $98$, Chef does not have fever.

 **Test Case 2** : Since $X = 100$ is greater than $98$, Chef has fever.

 **Test Case 3** : Since $X = 96$ is not greater than $98$, Chef does not have fever.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-08T14:11:26.932Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    (x>98)?printf("Yes\n"):printf("No\n");
	}
}


```

---

[View on CodeChef](https://www.codechef.com/problems/FEVER)