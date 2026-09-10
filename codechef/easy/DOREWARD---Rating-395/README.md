# DOREWARD - Rating 395

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Donation Rewards

On the occasion of World Blood Donor Day, Chef has organized an event to reward regular blood donars in Chefland.

- If the donor has made less than or equal to $3$ donations, they receive a BRONZE donor badge.
- If the donor has made more than $3$ but less than equal to $6$ donations, they receive a SILVER donor badge.
- If the donor has made more than $6$ donations, they receive a GOLD donor badge.

Given that a person has made $X$ donations, find the badge they receive.

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case contains an integer $X$, denoting the number of blood donations the person has made.
### Output Format

For each test case, output on a new line:

- BRONZE, if the person has made less than or equal to $3$ donations;
- SILVER, if the person has made more than $3$ but less than equal to $6$ donations;
- GOLD, if the person has made more than $6$ donations.

Each character can be printed in uppercase or lowercase. For example, `GOLD`, `gold`, `Gold`, and `gOlD` are considered identical.

### Constraints
- $1 \leq T \leq 100$
- $1 \leq X \leq 10$
### Sample 1:
Input
Output

```
4
1
3
5
7

```

```
BRONZE
BRONZE
SILVER
GOLD
```

### Explanation:

 **Test case $1$:**  The person has made less than equal to $3$ donations. Thus they receive bronze badge.

 **Test case $2$:**  The person has made less than equal to $3$ donations. Thus they receive bronze badge.

 **Test case $3$:**  The person has made more than $3$ but less than equal to $6$ donations. Thus they receive silver badge.

 **Test case $4$:**  The person has made more than $6$ donations. Thus they receive gold badge.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-10T11:21:20.952Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d", &t);
	for(int i=1;i<=t;i++)
	{
	    scanf("%d", &x);
	    if(x<=3)
	    printf("Bronze\n");
	    else if(x>3&&x<=6)
	    printf("Silver\n");
	    else
	    printf("Gold\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/DOREWARD)