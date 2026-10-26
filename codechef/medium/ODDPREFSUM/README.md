# ODDPREFSUM

![Difficulty](https://img.shields.io/badge/Difficulty-Medium-yellow)

## Problem

### All Odd Prefix Sums

You are given an array $A$ of size $N$. Can the array be rearranged such that all the (non-empty) prefixes of the array has an odd sum?

Formally, does there exist a rearrangement array $B$ of the array $A$ such that $B_1 + B_2 + \ldots + B_i$ is odd for every $1 \le i \le N$. Output $\text{Yes}$ if it is possible and $\text{No}$ otherwise.

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case consists of multiple lines of input. The first line of each test case contains a single integer $N$ - the size of the array. The second line contains $N$ integers - $A_1, A_2, \ldots, A_N$.
### Output Format

For each test case, output $\text{Yes}$ if it is possible to rearrange the array $A$ to make all prefix sums be odd, and $\text{No}$ otherwise.

It is allowed to print each character in either case, for example, $\text{YES}$, $\text{yes}$ and $\text{yEs}$ will all be accepted.

### Constraints
- $1 \le T \le 100$
- $1 \le N \le 100$
- $1 \le A_i \le 100$
### Sample 1:
Input
Output

```
3
1
1
2
2 4
3
2 1 2

```

```
Yes
No
Yes

```

### Explanation:

 **Test Case 1**  : The given array $A$ is already good because the only prefix sum is $1$, which is odd.

 **Test Case 2**  : The given array $A$ has $2$ even prefix sums. There exists no good rearrangement of the array.

 **Test Case 3**  : We can rearrange to $[1, 2, 2]$ which has prefix sums $1, 3, 5$, all of which are odd.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-10-26T08:26:30.697Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&n);
	    int a['n'];
	    int sum=0;
	    for(int i=0;i<n;i++)
	    {
	        sum=sum+a[i];
	    }
	    
	    if(sum%2!=0)
	    printf("no\n");
	    else
	    printf("yes\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/ODDPREFSUM)