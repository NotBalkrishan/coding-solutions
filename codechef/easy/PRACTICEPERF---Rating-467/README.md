# PRACTICEPERF - Rating 467

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Practice makes us perfect

Most programmers will tell you that one of the ways to improve your performance in competitive programming is to practice a lot of problems.

Our Chef took the above advice very seriously and decided to set a target for himself.

- Chef decides to solve at least $10$ problems every week for $4$ weeks.

Given the number of problems he actually solved in each week over $4$ weeks as $P_1, P_2, P_3,$ and $P_4$, output the number of weeks in which Chef met his target.

### Input Format

There is a single line of input, with $4$ integers $P_1, P_2, P_3,$ and $P_4$. These are the number of problems solved by Chef in each of the $4$ weeks.

### Output Format

Output a single integer in a single line - the number of weeks in which Chef solved  **at least**  $10$ problems.

### Constraints
- $1 \leq P_1, P_2, P_3, P_4 \leq 100$
### Sample 1:
Input
Output

```
12 15 8 10

```

```
3

```

### Explanation:

Chef solved at least $10$ problems in the first, second and fourth weeks. He failed to solve at least $10$ problems in the third week. Hence, the number of weeks in which Chef met his target is $3$.

### Sample 2:
Input
Output

```
2 3 1 10

```

```
1

```

### Explanation:

Chef solved at least $10$ problems in the fourth week. He failed to solve at least $10$ problems in all the other three weeks. Hence, the number of weeks in which Chef met his target is $1$.

### Sample 3:
Input
Output

```
12 100 99 11

```

```
4

```

### Explanation:

Chef solved at least $10$ problems in all the four weeks. Hence, the number of weeks in which Chef met his target is $4$.

### Sample 4:
Input
Output

```
1 1 1 1

```

```
0

```

### Explanation:

Chef was not able to solve at least $10$ problems in any of the four weeks. Hence, the number of weeks in which Chef met his target is $0$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-12T08:55:22.114Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int a,b,c,d;
	scanf("%d%d%d%d", &a,&b,&c,&d);
	int ans=0;
	if(a>=10)
	ans++;
	if(b>=10)
	ans++;
	if(c>=10)
	ans++;
	if(d>=10)
	ans++;
	printf("%d",ans);
	

}


```

---

[View on CodeChef](https://www.codechef.com/problems/PRACTICEPERF)