# Maximum element in an Array 

Hey guys👋, In this post we will be discuss the **Program to find maximum element of each column in a matrix** i.e., to find the maximum value in each column of the given matrix. Since it is considered as an important problem to solve while practicing, hence thought to share🤝 with you all.

### Problem Description

In a family, the people are arranged in rows and columns. Male persons in the families are arranged in a row and females are arranged in a column. Find the eldest women in each column. (Write a program to find the maximum element in each column of the matrix.)

> You can find the same set of problem in different way on the various coding platform.

Input Format:

The input consists of (m*n+2) integers. 

The first integer corresponds to m, the number of rows in the matrix and the second integer corresponds to n, the number of columns in the matrix. 

The remaining integers correspond to the elements in the matrix. 

The elements are read in row-wise order, the first row first, then second row and so on. 

Assume that the maximum value of m and n is 10.

Output Format:

Refer to the sample output for details.

*Sample Input:*

3

2

4 5

6 9

0 3

*Sample Output:*

6

9

### Explaination :

In this we will be discussing the Program to find maximum element of each column in a matrix i.e., to find the maximum value in each column of the given matrix. This can be achieved by simple loop and conditional statement. Initialize the max variable to first element of each column. If there is only one element present in each column of the matrix then the loop did not execute and max hold the only present value in the matrix, thus that element becomes the maximum of each column. If matrix has more than one element, than loop executes and if any element found bigger than the previously assigned value, then that element becomes the largest.

![Maximum element in matrix column.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623500802052/d8t6f2x8e.png)

### Logic to follow to come-up with the solution :

1. Declare the required sets of variables to use in the code.

2. Initialize the max variable to first element of each column.

3. If there is only one element present in each column of the matrix then the loop did not execute and max hold the only present value in the matrix, thus that element becomes the maximum of each column.

4. If matrix has more than one element, than loop executes and if any element found bigger than the previously assigned value, then that element becomes the largest.

5. At last maximum value of each column is displayed as the result output.

### Coding Time 👨‍💻
```
#include<iostream>
#include <bits/stdc++.h>
using namespace std;

void largestInColumn(int mat[10][10], int rows, int cols)
{
    for (int i = 0; i < cols; i++)
    {
     int maxm = mat[0][i];
     for (int j = 1; j < rows; j++)
     {
        if (mat[j][i] > maxm)
         maxm = mat[j][i];
        }
        cout << maxm << endl;
    }
}
int main()
{
  int n,m;
  cin>>n>>m;
  int mat[10][10];
  for(int i=0;i<n;i++)
  {
    for(int j=0;j<m;j++)
  {
    cin>>mat[i][j];
  }
  }
    largestInColumn(mat, n, m);
    return 0;
}
```
```
Input :
3
2
4 5
6 9
0 3
```
```
Output
6
9
```
Hence with the above set of logic and code you can easily understand and solve the problem to find maximum number in each column of a matrix.

Hope with this you learned and acquired some basic knowledge of C++ Programming.

Drop a Love❤ if you liked👍 this post, then share 🤝this with your friends and if anything is confusing or incorrect then let me know in the comment section.

#### Let's Connect at [Twitter](https://twitter.com/mayankp4513) | [LinkedIn](https://www.linkedin.com/in/mayank-pathak4513/)

Thanks from my side, this is Mayank, keep learning and exploring !!

Meet you in the next article......till than see ya🤚
