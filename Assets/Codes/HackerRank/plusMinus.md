#### Name: Plus Minus
#### Language: C
#### Platform: Hacker Rank
#### Question: https://www.hackerrank.com/challenges/plus-minus/problem

#### Question Statement
Given an array of integers, calculate the ratios of its elements that are positive, negative, and zero. Print the decimal value of each fraction on a new line with 6 places after the decimal.

Note: This challenge introduces precision problems. The test cases are scaled to six decimal places, though answers with absolute error of up to 10<sub>-4</sub> are acceptable.

Example :-

arr = [1, 1, 0, -1, -1]
There are n elements, two positive, two negative and one zero. Their ratios are 2/5 = 0.400000, 2/5 = 0.400000 and 1/5 = 0.200000 . Results are printed as:

0.400000

0.400000

0.200000

Print

Print the ratios of positive, negative and zero values in the array. Each value should be printed on a separate line with 6 digits after the decimal. The function should not return a value.

Input Format

The first line contains an integer, n, the size of the array.
The second line contains n space-separated integers that describe arr[n].

Constraints

0 < n <= 100

-100 <= arr[i] <= 100

Output Format

Print the following  lines, each to  decimals:

1. proportion of positive values
2. proportion of negative values
3. proportion of zeros

</hr>

#### Solution:
```
#include <stdio.h>
int main(){
    int i, n;
    scanf("%d", &n);
    float a[n], p=0, q=0, z=0;
    for (i = 0; i<n; i++) 
    {
        scanf("%f", &a[i]);
        if (a[i]>0) 
        {
            p++;
        }
        else if (a[i]<0) 
        {
            q++;
        }
        else 
        {
            z++;
        }
    }
    printf("%f\n%f\n%f", p/n, q/n, z/n);
    return 0;
}

```
