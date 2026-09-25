# MOZZ - Rating 752

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Endless Appetizers

 *Life is a like a box of of mozzarella sticks. You never know what you're gonna get, but you can predict with 100 percent accuracy that it will be a mozzarella stick.* 

Chef's colleague issued a challenge to Chef: "If you eat more than $X$ mozzarella sticks, I'll give you $30$ rupees for each extra one you eat".
For example, if $X = 5$ and Chef eats $8$ sticks, he would receive $90$ rupees because he ate $3$  *extra*  sticks.

You know that the restaurant serves $Y$ mozzarella sticks per plate.
You also know that Chef received $R$ rupees from his colleague as a result of the challenge.

What's the  **maximum**  number of plates of mozzarella sticks that Chef could have ordered?

 **Note:** 

- Chef won't order a new plate till he finishes eating all the sticks from the previous one.
- However, it's possible that Chef didn't finish all the sticks from the final plate he ordered. See the explained examples below for more clarification.
### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case consists of one line of input, containing three space-separated integers $X, Y,$ and $R$ — the lower limit on the number of sticks, the number of sticks on a single plate, and the money received by Chef.
### Output Format

For each test case, output on a new line the answer: the maximum number of plates Chef could have ordered.

### Constraints
- $1 \leq T \leq 10^4$
- $1 \leq X \leq 100$
- $1 \leq Y \leq 10$
- $0 \leq R \leq 3\cdot 10^4$
- It is guaranteed that $R$ is a multiple of $30$.
### Sample 1:
Input
Output

```
4
7 5 30
16 5 0
15 9 120
23 1 2130

```

```
2
4
3
94

```

### Explanation:

 **Test case $1$:**  Chef received $30$ rupees; meaning he ate $1$ extra stick.
Since $X = 7$, this means he must've eaten exactly $8$ sticks.
At $5$ sticks per plate, Chef would need $2$ plates to eat $8$ sticks (and two sticks from the second plate will remain uneaten).

 **Test case $2$:**  Chef received $0$ rupees. Since $X = 16$, this means he ate $\leq 16$ sticks.
The maximum he could've eaten is exactly $16$; and this would require $4$ plates since each plate has $5$ sticks.

 **Test case $3$:**  Chef received $120$ rupees, meaning he ate $4$ extra sticks.
This makes for a total of $15 + 4 = 19$ sticks, and at $9$ sticks per plate he would need $3$ plates.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T14:26:24.991Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y,r;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&x,&y,&r);
	    int z=r/30;
	    if((z+x)%y==0)
	    printf("%d\n",(z+x)/y);
	    else
	    printf("%d\n",((z+x)/y)+1);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/MOZZ)