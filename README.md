# Square-Matrix-Multiplication ( 5kyu)
# 21.10.2022
# перемножение квадратных матриц
# [ссылка на задание](https://www.codewars.com/kata/5263a84ffcadb968b6000513/train/java)
# код :
```java
int n =a.length;
        int[][] c =new int[n][n];

        for (int i =0;i<n;i++)
        {
            for(int j=0;j<n;j++)
            {
                for(int k=0;k<n;k++) {

                    c[i][j] += a[i][k] * b[k][j];
                }
            }
        }
        return c;
```    
 # понравивщееся   решение (автор velocerap)

``` java 
 public static int[][] matrixMultiplication(int[][] a, int[][] b) {
    int n = a.length;
    int[][] res = new int[n][n];
    for (int i = 0; i < n; i++) {
      for (int j = 0; j < n; j++) {
        for (int k = 0; k < n; k++) {
          res[i][j] += a[i][k] * b[k][j];
        }
      }
    }
    return res;
