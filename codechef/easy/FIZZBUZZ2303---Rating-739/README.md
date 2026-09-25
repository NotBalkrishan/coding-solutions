# FIZZBUZZ2303 - Rating 739

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Chef Fantasy 11

All of Chef's friends are playing fantasy cricket based upon the ODI World Cup, and Chef would like to join them.

For a certain cricket match, Chef has decided upon his team of $11$ players. However, he hasn't yet decided who should be the captain and who should be the vice-captain.

He's narrowed his decision down to $N$ players out of the $11$, from which he'll choose one to be the captain and one to be the vice captain.
How many different choices does he have?

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- The first and the only line of each testcase contains a single integer $N$, the number of players Chef is considering.
### Output Format

For each test case, output on a new line the number of possible choices of captain and vice-captain.

### Constraints
- $1 \leq T \leq 10$
- $2 \leq N \leq 11$
### Sample 1:
Input
Output

```
2
2
3

```

```
2
6
```

### Explanation:

 **Test case $1$:**  With $N = 2$, there are only two possibilities: one of the players must be selected as the captain, and the other will become the vice-captain.

 **Test case $2$:**  It can be shown that there are $6$ possibilities in total for captain/vice-captain choices.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T03:05:08.476Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&n);
	    printf("%d\n",n*(n-1));
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/FIZZBUZZ2303)