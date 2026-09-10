# INSTAGRAM - Rating 408

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Instagram

Chef categorises an instagram account as  *spam*, if, the  *following*  count of the account is more than $10$ times the count of  *followers*.

Given the  *following*  and  *follower*  count of an account as $X$ and $Y$ respectively, find whether it is a  *spam*  account.

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case consists of two space-separated integers $X$ and $Y$ — the following and follower count of an account, respectively.
### Output Format

For each test case, output on a new line, `YES`, if the account is  *spam*  and `NO` otherwise.

You may print each character of the string in uppercase or lowercase. For example, the strings `YES`, `yes`, `Yes` and `yES` are identical.

### Constraints
- $1 \leq T \leq 100$
- $1 \leq X, Y \leq 100$
### Sample 1:
Input
Output

```
4
1 10
10 1
11 1
97 7

```

```
NO
NO
YES
YES

```

### Explanation:

 **Test case $1$:**  The following count is $1$ while the follower count is $10$. Since the following count is not more than $10$ times the follower count, the account is not spam.

 **Test case $2$:**  The following count is $10$ while the follower count is $1$. Since the following count is not  **more**  than $10$ times the follower count, the account is not spam.

 **Test case $3$:**  The following count is $11$ while the follower count is $1$. Since the following count is more than $10$ times the follower count, the account is spam.

 **Test case $4$:**  The following count is $97$ while the follower count is $7$. Since the following count is more than $10$ times the follower count, the account is spam.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-10T16:49:16.817Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y;
	scanf("%d",&t);
	for(int i=1;i<=t;i++)
	{
	    scanf("%d%d", &x,&y);
	    if(x>=(y+10))
	    printf("Yes\n");
	    else
	    printf("No\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/INSTAGRAM)