# OFFICE - Rating 532

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Chef in his Office

Recently Chef joined a new company. In this company, the employees have to work for $X$ hours each day from Monday to Thursday. Also, in this company, Friday is called Chill Day — employees only have to work for $Y$ hours $(Y \lt X)$ on Friday. Saturdays and Sundays are holidays.

Determine the total number of working hours in one week.

### Input Format
- The first line contains a single integer $T$ — the number of test cases. Then the test cases follow.
- The first and only line of each test case contains two space-separated integers $X$ and $Y$ — the number of working hours on each day from Monday to Thursday and the number of working hours on Friday respectively.
### Output Format

For each test case, output the total number of working hours in one week.

### Constraints
- $1 \leq T \leq 100$
- $2 \leq X \leq 12$
- $1 \le Y \lt X$
### Sample 1:
Input
Output

```
3
10 5
12 2
8 7

```

```
45
50
39

```

### Explanation:

 **Test case $1$:**  The total number of working hours in a week are: $10 \texttt{(Monday)} + 10 \texttt{(Tuesday)} + 10 \texttt{(Wednesday)} + 10 \texttt{(Thursday)} + 5 \texttt{(Friday)} = 45$

 **Test Case 2:**  The total number of working hours in a week are: $12 \texttt{(Monday)} + 12 \texttt{(Tuesday)} + 12 \texttt{(Wednesday)} + 12 \texttt{(Thursday)} + 2 \texttt{(Friday)} = 50$

 **Test Case 3:**  The total number of working hours in a week are: $8 \texttt{(Monday)} + 8 \texttt{(Tuesday)} + 8 \texttt{(Wednesday)} + 8 \texttt{(Thursday)} + 7 \texttt{(Friday)} = 39$

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-14T08:39:39.618Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d",&x,&y);
	    printf("%d\n", (x*4)+y);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/OFFICE)