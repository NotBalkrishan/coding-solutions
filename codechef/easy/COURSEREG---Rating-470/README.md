# COURSEREG - Rating 470

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Course Registration

There is a group of $N$ friends who wish to enroll in a course together. The course has a maximum capacity of $M$ students that can register for it. If there are $K$ other students who have already enrolled in the course, determine if it will still be possible for all the $N$ friends to do so or not.

### Input Format
- The first line contains a single integer $T$ - the number of test cases. Then the test cases follow.
- Each test case consists of a single line containing three integers $N$, $M$ and $K$ - the size of the friend group, the capacity of the course and the number of students already registered for the course.
### Output Format

For each test case, output `Yes` if it will be possible for all the $N$ friends to register for the course. Otherwise output `No`.

You may print each character of `Yes` and `No` in uppercase or lowercase (for example, `yes`, `yEs`, `YES` will be considered identical).

### Constraints
- $1 \leq T \leq 1000$
- $1 \leq N \leq M \leq 100$
- $0 \leq K \leq M$
### Sample 1:
Input
Output

```
3
2 50 27
5 40 38
100 100 0

```

```
Yes
No
Yes

```

### Explanation:

 **Test Case 1:**  The $2$ friends can enroll in the course as it has enough seats to accommodate them and the $27$ other students at the same time.

 **Test Case 2:**  The course does not have enough seats to accommodate the $5$ friends and the $38$ other students at the same time.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-12T09:01:08.373Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n,m,k;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&n,&m,&k);
	    if((m-k)>=n)
	    printf("yes\n");
	    else
	    printf("No\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/COURSEREG)