# Problem: squaredArray

Write a variable declaration and for loop necessary to create and initialize an integer array named squares that contains the following values:

```sql
0 1 4 9 16 25 36 49 64 81 100
```

### Solution

```sql
int [] squares = new int[11];
for (int i = 0; i <=10; i++){squares[i] = i*i;}
```
