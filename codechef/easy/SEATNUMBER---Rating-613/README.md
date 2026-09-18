# SEATNUMBER - Rating 613

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-green)

## Problem

### Bus Seat Numbering

There is a bus with 30 seats. The seats are numbered from 1 to 30, and the numbering is as depicted in this image.

As can be seen in the image, the bus is divided into two decks - The Lower deck, and the Upper deck, with 15 seats each. And some of the seats come as Single and some as Double. For example, Seats 1 and 2 are Double, whereas Seat 11 is a Single.

You will be given a Seat number, and your job is to classify it as one of these 4 types:

- Lower Single
- Lower Double
- Upper Single
- Upper Double
### Input Format
- The first line of input will contain a single integer $T$, denoting the number of test cases.
- Each test case consists of a single line of input which contains a single integers $N$ — the seat number.
### Output Format

For each test case, output on a new line, the type of seat.

### Constraints
- $1 \leq T \leq 100$
- $1 \leq N \leq 30$
### Sample 1:
Input
Output

```
5
6
28
16
13
10

```

```
Lower Double
Upper Single
Upper Double
Lower Single
Lower Double

```

### Explanation:

 **Testcase 1:**  The seat number 6 is in the Lower deck, and it is a Double. Hence the output is "Lower Double".

 **Testcase 2:**  The seat number 28 is in the Upper deck, and it is a Single. Hence the output is "Upper Single".

 **Testcase 3:**  The seat number 16 is in the Upper deck, and it is a Double. Hence the output is "Upper Double".

 **Testcase 4:**  The seat number 13 is in the Lower deck, and it is a Single. Hence the output is "Lower Single".

 **Testcase 5:**  The seat number 10 is in the Lower deck, and it is a Double. Hence the output is "Lower Double".

## Solution

**Language:** c_cpp  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-09-18T11:09:49.965Z  

```c_cpp
#include <stdio.h>

int main() {
	// your code goes here
	int t,n;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&n);
	    if(1<=n && n<=10)
	    printf("Lower double\n");
	    
	    else if(11<=n && n<=15)
	    printf("Lower Single\n");
	    
	    else if(16<=n && n<=25)
	    printf("Upper double\n");
	    
	    else 
	    printf("Upper Single\n");
	    
	}

}


```

---

[View on CodeChef](https://www.codechef.com/problems/SEATNUMBER)