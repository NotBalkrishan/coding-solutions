# WGHTS - Rating 697

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Weights

Chef is playing with weights. He has an object weighing $W$ units. He also has three weights each of $X, Y,$ and $Z$ units respectively. Help him determine whether he can measure the  **exact**  weight of the object with one or more of these weights.

If it is possible to measure the weight of object with one or more of these weights, print `YES`, otherwise print `NO`.

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case consists of single line containing a four positive integers $W, X, Y,$ and $Z$.
### Output Format

For each test case, output on a new line `YES` if it is possible to measure the weight of object with one or more of these weights, otherwise print `NO`.

You may print each character of the string in either uppercase or lowercase (for example, the strings `yes`, `YES`, `Yes`, and `yeS` will all be treated as identical).

### Constraints
- $1 \leq T \leq 10^4$
- $1 \leq W, X, Y, Z \leq 10^5$
### Sample 1:
Input
Output

```
4
5 2 1 6
7 9 7 2
20 8 10 12
20 10 11 12

```

```
NO
YES
YES
NO

```

### Explanation:

 **Test Case $1$:**  It is not possible to measure $5$ units using any combination of given weights.

 **Test Case $2$:**  Chef can use the second weight of $7$ units to measure the object exactly.

 **Test Case $3$:**  Chef can use combination of first and third weights to measure $8+12=20$ units.

 **Test Case $4$:**  Chef cannot measure $20$ units of weight using any combination of given weights.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-22T13:48:23.165Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,w,x,y,z;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d%d",&w,&x,&y,&z);
	    if(w==x)
	    printf("Yes\n");
	    else if(w==y)
	    printf("Yes\n");
	    else if(w==z)
	    printf("Yes\n");
	    else if(w==(x+y))
	    printf("Yes\n");
	    else if(w==(x+z))
	    printf("Yes\n");
	    else if(w==(y+z))
	    printf("Yes\n");
	    else if(w==(x+y+z))
	    printf("Yes\n");
	    else
	    printf("No\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/WGHTS)