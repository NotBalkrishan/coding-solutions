# HELIUM3 - Rating 562

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Chef and NextGen

Chef is currently working for a secret research group called NEXTGEN. While the rest of the world is still in search of a way to utilize Helium-3 as a fuel, NEXTGEN scientists have been able to achieve 2 major milestones:

- Finding a way to make a nuclear reactor that will be able to utilize Helium-3 as a fuel
- Obtaining every bit of Helium-3 from the moon's surface

Moving forward, the project requires some government funding for completion, which comes under one condition: to prove its worth, the project should power Chefland by generating at least $A$ units of power each year for the next $B$ years.

Help Chef determine whether the group will get funded assuming that the moon has $X$ grams of Helium-3 and $1$ gram of Helium-3 can provide $Y$ units of power.

### Input Format
- The first line of input contains an integer $T$, the number of testcases. The description of $T$ test cases follows.
- Each test case consists of a single line of input, containing four space-separated integers $A, B, X, Y$ respectively.
### Output Format

For each test case print on a single line the answer — `Yes` if NEXTGEN satisfies the government's minimum requirements for funding and `No` otherwise.

You may print each character of the answer string in either uppercase or lowercase (for example, the strings `"yEs"`, `"yes"`, `"Yes"` and `"YES"` will all be treated as identical).

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq A, B, X, Y, \leq 1000$
### Subtasks

 **Subtask #1 (100 points):**  Original constraints

### Sample 1:
Input
Output

```
4
1 2 3 4
4 3 2 1
2 18 9 4
1 100 2 49
```

```
Yes
No
Yes
No
```

### Explanation:

 **Test case $1$:**  Chefland requires $A = 1$ units of power for the next $B = 2$ years. In total, the moon must be capable of providing $A \cdot B = 2$ units of power. There are in total $X = 3$ grams of Helium-3 on the moon which is capable of providing $X \cdot Y = 12$ units of power. $12 \gt 2$, so the project satisfies the minimum requirements for funding. Thus, the answer is `Yes`.

 **Test case $2$:**  The total amount of power needed by Chefland is $A \cdot B = 12$, whereas the total that can be provided by the Helium-3 present on the moon is $X \cdot Y = 2$, which is insufficient to receive funding, so the answer is `No`.

 **Test case $3$:**  The total amount of power needed by Chefland is $A \cdot B = 2 \cdot 18 = 36$, and the total that can be provided by the Helium-3 present on the moon is $X \cdot Y = 9 \cdot 4 = 36$, which is sufficient to receive funding, so the answer is `Yes`.

 **Test case $4$:**  The total amount of power needed by Chefland is $A \cdot B = 1 \cdot 100 = 100$, and the total that can be provided by the Helium-3 present on the moon is $X \cdot Y = 2 \cdot 49 = 98$, which is insufficient to receive funding, so the answer is `No`.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-15T18:30:52.532Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,x,y;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d%d",&a,&b,&x,&y);
	    if((a*b)<=(x*y))
	    printf("YES\n");
	    else
	    printf("NO\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/HELIUM3)