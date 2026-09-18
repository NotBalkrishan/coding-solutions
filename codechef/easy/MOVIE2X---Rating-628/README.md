# MOVIE2X - Rating 628

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Watching Movies at 2x

Chef started watching a movie that runs for a total of $X$ minutes.

Chef has decided to watch the first $Y$ minutes of the movie at  **twice**  the usual speed as he was warned by his friends that the movie gets interesting only after the first $Y$ minutes.

How long will Chef spend watching the movie in  **total** ?

 **Note:**  It is guaranteed that $Y$ is  **even**.

### Input Format
- The first line contains two space separated integers $X, Y$ - as per the problem statement.
### Output Format
- Print in a single line, an integer denoting the total number of minutes that Chef spends in watching the movie.
### Constraints
- $1 \leq X, Y \leq 1000$
- $Y$ is an even integer.
### Subtasks

 **Subtask #1 (100 points):**  original constraints

### Sample 1:
Input
Output

```
100 20
```

```
90
```

### Explanation:

For the first $Y = 20$ minutes, Chef watches at twice the usual speed, so the total amount of time spent to watch this portion of the movie is $\frac{Y}{2} = 10$ minutes.

For the remaining $X - Y = 80$ minutes, Chef watches at the usual speed, so it takes him $80$ minutes to watch the remaining portion of the movie.

In total, Chef spends $10 + 80 = 90$ minutes watching the entire movie.

### Sample 2:
Input
Output

```
50 24
```

```
38
```

### Explanation:

For the first $Y = 24$ minutes, Chef watches at twice the usual speed, so the total amount of time spent to watch this portion of the movie is $\frac{Y}{2} = 12$ minutes.

For the remaining $X - Y = 26$ minutes, Chef watches at the usual speed, so it takes him $26$ minutes to watch the remaining portion of the movie.

In total, Chef spends $12 + 26 = 38$ minutes watching the entire movie.

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-18T11:18:19.500Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int x,y;
	scanf("%d%d",&x,&y);
	int z=x-y;
	printf("%d\n",(y/2)+z);

}


```

---

[View on CodeChef](https://www.codechef.com/problems/MOVIE2X)