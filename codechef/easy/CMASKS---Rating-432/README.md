# CMASKS - Rating 432

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Chef and Masks

Chef is shopping for masks. In the shop, he encounters $2$ types of masks:

- Disposable Masks — cost $X$ but last only $1$ day.
- Cloth Masks — cost $Y$ but last $10$ days.

Chef wants to buy masks to last him $100$ days. He will buy the masks which cost him the least. In case there is a tie in terms of cost, Chef will be eco-friendly and choose the cloth masks. Which type of mask will Chef choose?

### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases. Then the test cases follow.
- Each test case consists of a single line of input, containing two space-separated integers $X, Y$.
### Output Format

For each test case, if Chef buys the cloth masks print `CLOTH`, otherwise print `DISPOSABLE`.

You may print each character of the string in uppercase or lowercase (for example, the strings `cloth`, `clOTh`, `cLoTH`, and `CLOTH` will all be treated as identical).

### Constraints
- $1 \leq T \leq 5000$
- $1 \leq X \lt Y \leq 100$
### Sample 1:
Input
Output

```
4
10 100
9 100
88 99
1 11

```

```
Cloth
Disposable
Cloth
Disposable

```

### Explanation:

 **Test case $1$:**  The cost of the disposable masks will be $10 \cdot 100 = 1000$, while the cost of the cloth masks will be $100 \cdot 10 = 1000$. Since the price is equal and Chef is eco-friendly, Chef will buy the cloth masks.

 **Test case $2$:**  The cost of the disposable masks will be $9 \cdot 100 = 900$, while the cost of the cloth masks will be $100 \cdot 10 = 1000$. Since the price of disposable masks is less, Chef will buy the disposable masks.

 **Test case $3$:**  The cost of the disposable masks will be $88 \cdot 100 = 8800$, while the cost of the cloth masks will be $99 \cdot 10 = 990$. Since the price of the cloth masks is less, Chef will buy the cloth masks.

 **Test case $4$:**  The cost of the disposable masks will be $1 \cdot 100 = 100$, while the cost of the cloth masks will be $11 \cdot 10 = 110$. Since the price of disposable masks is less, Chef will buy the disposable masks.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-11T10:08:30.228Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,x,y;
	scanf("%d",&t);
	for(int i=1;i<=t;i++)
	{
	    scanf("%d%d",&x,&y);
	    if((x*100)>=(y*10))
	    printf("Cloth\n");
	    else
	    printf("Disposable\n");
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/CMASKS)