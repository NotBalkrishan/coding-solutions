# DPOLY - Rating 793

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Degree of Polynomial

In mathematics, the degree of polynomials in one variable is the highest power of the variable in the algebraic expression with non-zero coefficient.

Chef has a polynomial in one variable $x$ with $N$ terms. The polynomial looks like $A_0\cdot x^0 + A_1\cdot x^1 + \ldots + A_{N-2}\cdot x^{N-2} + A_{N-1}\cdot x^{N-1}$ where $A_{i-1}$ denotes the coefficient of the $i^{th}$ term $x^{i-1}$ for all $(1\le i\le N)$.

Find the degree of the polynomial.

 **Note:**  It is guaranteed that there exists  **at least**  one term with non-zero coefficient.

### Input Format
- First line will contain $T$, number of test cases. Then the test cases follow.
- First line of each test case contains of a single integer $N$ - the number of terms in the polynomial.
- Second line of each test case contains of $N$ space-separated integers - the $i^{th}$ integer $A_{i-1}$ corresponds to the coefficient of $x^{i-1}$.
### Output Format

For each test case, output in a single line, the degree of the polynomial.

### Constraints
- $1 \leq T \leq 100$
- $1 \leq N \leq 1000$
- $-1000 \le A_i \le 1000$
- $A_i \ne 0$ for at least one $(0\le i \lt N)$.
### Sample 1:
Input
Output

```
4
1
5
2
-3 3
3
0 0 5
4
1 2 4 0

```

```
0
1
2
2
```

### Explanation:

 **Test case $1$:**  There is only one term $x^0$ with coefficient $5$. Thus, we are given a constant polynomial and the degree is $0$.

 **Test case $2$:**  The polynomial is $-3\cdot x^0 + 3\cdot x^1 = -3 + 3\cdot x$. Thus, the highest power of $x$ with non-zero coefficient is $1$.

 **Test case $3$:**  The polynomial is $0\cdot x^0 + 0\cdot x^1 + 5\cdot x^2= 0+0 + 5\cdot x^2$. Thus, the highest power of $x$ with non-zero coefficient is $2$.

 **Test case $4$:**  The polynomial is $1\cdot x^0 + 2\cdot x^1+ 4\cdot x^2 + 0\cdot x^3= 1 + 2\cdot x + 4\cdot x^2$. Thus, the highest power of $x$ with non-zero coefficient is $2$.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-30T18:28:20.384Z  

```c_cpp
#include <stdio.h>

int main() {
    int t, n;

    scanf("%d", &t);

    while (t--) {
        scanf("%d", &n);

        int a[n];

        for (int i = 0; i < n; i++) {
            scanf("%d", &a[i]);
        }

        for (int i = n - 1; i >= 0; i--) {
            if (a[i] != 0) {
                printf("%d\n", i);
                break;
            }
        }
    }

    return 0;
}
```

---

[View on CodeChef](https://www.codechef.com/problems/DPOLY)