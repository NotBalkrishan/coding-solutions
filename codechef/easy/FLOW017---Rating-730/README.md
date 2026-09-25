# FLOW017 - Rating 730

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Second Largest

Three numbers  **A**,  **B**  and  **C**  are the inputs. Write a program to find second largest among them.

### Input Format

The first line contains an integer  **T**, the total number of testcases. Then  **T**  lines follow, each line contains three integers  **A**,  **B**  and  **C**.

### Output Format

For each test case, display the second largest among  **A**,  **B**  and  **C**, in a new line.

### Constraints
- 1 ≤ T ≤ 1000
- 1 ≤ A,B,C ≤ 1000000
### Sample 1:
Input
Output

```
3 
120 11 400
10213 312 10
10 3 450
```

```
120
312
10
```

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-25T02:53:23.253Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,a,b,c;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d%d%d",&a,&b,&c);
	    if(a>b && a<c)
	    printf("%d\n",a);
	    else if(a>c && a<b)
	    printf("%d\n",a);
	    else if(b>a && b<c)
	    printf("%d\n",b);
	    else if(b>c && b<a)
	    printf("%d\n",b);
	    else if(c>a && c<b)
	    printf("%d\n",c);
	    else if(c>b && c<a)
	    printf("%d\n",c);
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/FLOW017)