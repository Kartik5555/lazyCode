#### Name: Simple Array Sum
#### Language: C++
#### Platform: Hacker Rank
#### Question: https://www.hackerrank.com/challenges/simple-array-sum/problem

#### Question Statement

Given an array of integers, find the sum of its elements.

For example, if the array ar = [1, 2, 3], 1 + 2 + 3 = 6, so return 6.
ar = an array of integers

Input Format

The first line contains an integer, n , denoting the size of the array.
The second line contains n space-separated integers representing the array's elements.

Constraints

0 < n, ar[i] <= 1000

Output Format

Print the sum of the array's elements as a single integer.
</hr>

#### Solution:
```
#include <iostream>
using namespace std;
int main()
{
    int n, sum=0;
    cin >> n;
    int ar[n];
    for (int i = 0; i < n; i++)
    {
        cin >> ar[i];
    }
    for (int i = 0; i < n; i++)
    {
        sum = sum + ar[i];
    }
    cout<<sum;
    return 0;
}
```
