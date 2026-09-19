# TRANSFORM - Rating 649

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Mario and Transformation

Mario transforms each time he eats a mushroom as follows:

- If he is currently small, he turns normal.
- If he is currently normal, he turns huge.
- If he is currently huge, he turns small.

Given that Mario was initially `normal`, find his size after eating $X$ mushrooms.

### Input Format
- The first line of input will contain one integer $T$, the number of test cases. Then the test cases follow.
- Each test case contains a single line of input, containing one integer $X$.
### Output Format

For each test case, output in a single line Mario's size after eating $X$ mushrooms.

Print:

- $\texttt{NORMAL}$, if his final size is normal.
- $\texttt{HUGE}$, if his final size is huge.
- $\texttt{SMALL}$, if his final size is small.

You may print each character of the answer in either uppercase or lowercase (for example, the strings $\texttt{Huge}$, $\texttt{hUgE}$, $\texttt{huge}$ and $\texttt{HUGE}$ will all be treated as identical).

### Constraints
- $1 \leq T \leq 100$
- $1 \leq X \leq 100$
### Sample 1:
Input
Output

```
3
2
4
12
```

```
SMALL
HUGE
NORMAL
```

### Explanation:

 **Test case $1$:**  Mario's initial size is `normal`. On eating the first mushroom, he turns `huge`. On eating the second mushroom, he turns `small`.

 **Test case $2$:**  Mario's initial size is `normal`. On eating the first mushroom, he turns `huge`. On eating the second mushroom, he turns `small`. On eating the third mushroom, he turns `normal`. On eating the fourth mushroom, he turns `huge`.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-19T09:24:25.619Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    if(x%3==0)
	    printf("Normal\n");
	    else if(x%3==1)
	    printf("Huge\n");
	    else
	    printf("Small\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/TRANSFORM)