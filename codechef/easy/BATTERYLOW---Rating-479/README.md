# BATTERYLOW - Rating 479

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Battery Low

Chef's phone shows a Battery Low notification if the battery level is $15 \%$ or less.

Given that the battery level of Chef's phone is $X \%$, determine whether it would show a Battery low notification.

### Input Format
- First line will contain $T$, number of test cases. Then the test cases follow.
- Each test case contains a single line of input, an integer $X$, denoting the battery level of the phone.
### Output Format

For each test case, output in a single line $\texttt{Yes}$, if the battery level is $15 \%$ or below. Otherwise, print $\text{No}$.

You may print each character of $\texttt{Yes}$ and $\text{No}$ in uppercase or lowercase (for example, $\texttt{YeS}$, $\texttt{YES}$, $\texttt{yes}$ will be considered identical).

### Constraints
- $1 \leq T \leq 100$
- $1 \leq X \leq 100$
### Subtasks

 **Subtask #1 (100 points):**  original constraints

### Sample 1:
Input
Output

```
3
15
3
65
```

```
Yes
Yes
No
```

### Explanation:

 **Test Case 1:**  The battery level is $15$. Thus, it would show a battery low notification.

 **Test Case 2:**  The battery level is $3$, which is less than $15$. Thus, it would show a battery low notification.

 **Test Case 3:**  The battery level is $65$, which is greater than $15$. Thus, it would not show a battery low notification.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-12T09:12:09.098Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    if(x<=15)
	    printf("Yes\n");
	    else
	    printf("No\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/BATTERYLOW)