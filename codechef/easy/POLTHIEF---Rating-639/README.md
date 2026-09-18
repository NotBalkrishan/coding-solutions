# POLTHIEF - Rating 639

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Police and Thief

Chef discovered that his secret recipe has been stolen. He immediately informs the police of the theft.

It is known that the policeman and thief move on the number line. You are given that:

- The initial location of the policeman on the number line is $X$ and his speed is $2$ units per second.
- The initial location of the thief on the number line is $Y$ and his speed is $1$ unit per second.

Find the  **minimum**  time (in seconds) in which the policeman can catch the thief. Note that, the policeman catches the thief as soon as their locations become equal and the thief will try to evade the policeman for as long as possible.

### Input Format
- The first line of input will contain an integer $T$ — the number of test cases. The description of $T$ test cases follows.
- The first and only line of each test case contains two integers $X$ and $Y$, as described in the problem statement.
### Output Format

For each test case, output in a single line the minimum time taken by the policeman to catch the thief.

### Constraints
- $1 \leq T \leq 1000$
- $-10^5 \leq X, Y \leq 10^5$
### Sample 1:
Input
Output

```
3
1 3
2 1
1 1
```

```
2
1
0
```

### Explanation:

 **Test case $1$** : The initial locations of the policeman and thief are $1$ and $3$ respectively. The minimum time taken by the policeman to catch the thief is $2$ seconds, and this happens when both the policeman and the thief move towards the right.

 **Test case $2$** : The initial location of the policeman and thief are $2$ and $1$ respectively. The minimum time taken by the policeman to catch the thief is $1$ second, and this happens when both the policeman and the thief move towards the left.

 **Test case $3$** : The initial locations of the policeman and thief are $1$ and $1$ respectively. Because the police is already present at the location of thief, the time taken by police to catch the thief is $0$ seconds.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-18T11:21:12.490Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d",&x,&y);
	    if(x>y)
	    {
	        printf("%d\n",(x-y)*1);
	    }
	    else
	    printf("%d\n",(y-x)*1);
	    
	}
}


```

---

[View on CodeChef](https://www.codechef.com/problems/POLTHIEF)