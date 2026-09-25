# CHEFRACES - Rating 745

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Chef and Races

The National Championships are starting soon. There are $4$ race categories, numbered from $1$ to $4$, that Chef is interested in. Chef is participating in exactly $2$ of these categories.

Chef has an arch-rival who is, unfortunately, the only person participating who is better than Chef, i.e, Chef can't defeat the arch-rival in any of the four race categories but can defeat anyone else. Chef's arch-rival is also participating in exactly $2$ of the four categories.

Chef hopes to not fall into the same categories as that of the arch-rival.

Given $X, Y, A, B$ where $X, Y$ are the races that Chef participates in, and $A, B$ are the races that Chef's arch-rival participates in, find the  **maximum**  number of gold medals (first place) that Chef can win.

### Input Format
- The first line of input contains an integer $T$, denoting the number of testcases. The description of $T$ testcases follows.
- Each testcase consists of a single line containing four space-separated integers — the values of $X, Y, A$, and $B$ respectively.
### Output Format
- For each testcase, print a single line containing one integer — the maximum number of gold medals that Chef can win.
### Constraints
- $1 \leq T \leq 144$
- $1 \leq X, Y, A, B \leq 4$
- $X \neq Y$
- $A \neq B$
### Subtasks

 **Subtask #1 (100 points):**  Original constraints

### Sample 1:
Input
Output

```
3
4 3 1 2
4 2 1 2
2 1 1 2
```

```
2
1
0
```

### Explanation:

 **Test case $1$:**  Chef participates in the races $4, 3$, whereas Chef's rival participates in $1, 2$. As Chef's only rival does not participate in any of the races that Chef takes part in, Chef can win the gold medal in both of the races, thus the answer is $2$.

 **Test case $2$:**  Chef participates in the races $4, 2$, whereas Chef's rival participates in $1, 2$. Chef cannot win race $2$ as Chef will be beaten by the arch-rival, however Chef can win the gold medal for race $4$. Thus the answer is $1$.

 **Test case $3$:**  Chef participates in the races $2, 1$, whereas Chef's rival participates in $1, 2$. Chef will be beaten by the arch-rival in both races, thus the answer is $0$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T14:10:20.778Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,x,y;
	scanf("%d",&t);
	while(t--)
	{
	    int count=0;
	    scanf("%d%d%d%d",&x,&y,&a,&b);
	    if(x!=a && x!=b)
	    count++;
	    if(y!=a && y!=b)
	    count++;
	    
	    printf("%d\n", count);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/CHEFRACES)