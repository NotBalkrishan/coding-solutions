# SPEEDTEST - Rating 718

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Speed Limit Test

Alice is driving from her home to her office which is $A$ kilometers away and will take her $X$ hours to reach.
Bob is driving from his home to his office which is $B$ kilometers away and will take him $Y$ hours to reach.

Determine who is driving faster, else, if they are both driving at the same speed print `EQUAL`.

### Input Format
- The first line will contain $T$, the number of test cases. Then the test cases follow.
- Each test case consists of a single line of input, containing four integers $A,X,B,$ and $Y$, the distances and and the times taken by Alice and Bob respectively.
### Output Format

For each test case, if Alice is faster, print `ALICE`. Else if Bob is faster, print `BOB`. If both are equal, print `EQUAL`.

You may print each character of the string in uppercase or lowercase (for example, the strings `equal`, `equAL`, `EquAl`, and `EQUAL` will all be treated as identical).

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq A,X,B,Y \leq 1000$
### Sample 1:
Input
Output

```
3
20 6 20 5
10 3 20 6
9 1 1 1

```

```
Bob
Equal
Alice

```

### Explanation:

 **Test case $1$:**  Since Bob travels the distance between his office and house in $5$ hours, whereas Alice travels the same distance of $20$ kms in $6$ hours, `BOB` is faster.

 **Test case $2$:**  Since Alice travels the distance of $10$ km between her office and house in $3$ hours and Bob travels a distance of $20$ km in $6$ hours, they have equal speeds.

 **Test case $3$:**  Since Alice travels the distance of $9$ km between her office and house in $1$ hour and Bob travels only a distance of $1$ km in the same time, `ALICE` is faster.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-24T15:07:51.440Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t;
	float a,b,x,y;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%f%f%f%f",&a,&x,&b,&y);
	    float p=a/x;
	    float q=b/y;
	    if(p>q)
	    printf("Alice\n");
	    else if(q>p)
	    printf("Bob\n");
	    else
	    printf("Equal\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/SPEEDTEST)