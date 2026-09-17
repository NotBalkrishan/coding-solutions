# NEARESTEXIT - Rating 585

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Nearest Exit

There are two exits in a bus with $100$ seats:

- First exit is located beside seat number $1$.
- Second exit is located beside seat number $100$.

Seats are arranged in a straight line from $1$ to $100$ with equal spacing between any $2$ adjacent seats.

A passenger prefers to choose the nearest exit while leaving the bus.

Determine the exit taken by passenger sitting on seat $X$.

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case consists a single integer $X$, denoting the seat number.
### Output Format

For each test case, output `LEFT` if the passenger chooses the exit beside seat $1$, `RIGHT` otherwise.

You may print each character of the string in uppercase or lowercase (for example, the strings `LEFT`, `lEft`, `left`, and `lEFT` will all be treated as identical).

### Constraints
- $1 \leq T \leq 100$
- $1 \leq X \leq 100$
### Sample 1:
Input
Output

```
6
1
50
100
30
51
73

```

```
LEFT
LEFT
RIGHT
LEFT
RIGHT
RIGHT

```

### Explanation:

 **Test case $1$:**  The exit is located beside seat $1$. Hence, the passenger can take this exit without moving to any other seat.

 **Test case $2$:**  To take exit at seat $1$, the passenger needs to move $49$ seats. However, to take the exit at seat $100$, the passenger needs to move $50$ seats. Thus, exit at seat $1$ is closer.

 **Test case $3$:**  The exit is located beside seat $100$. Hence, the passenger can take this exit without moving to any other seat.

 **Test case $4$:**  To take exit at seat $1$, the passenger needs to move $29$ seats. However, to take the exit at seat $100$, the passenger needs to move $70$ seats. Thus, exit at seat $1$ is closer.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-17T17:01:30.905Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&x);
	    if(1<=x && x<=50)
	    printf("left\n");
	    else
	    printf("right\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/NEARESTEXIT)