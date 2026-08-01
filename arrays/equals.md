# Problem: equals

Write a method named equals that accepts a pair of arrays of integers as parameters and returns true if the arrays contain the same elements in the same order. If the arrays are not the same length, your method should return false.

For example, if the following arrays are declared:

int[] a1 = {10, 20, 30, 40, 50, 60};
int[] a2 = {10, 20, 30, 40, 50, 60};
int[] a3 = {20, 3, 50, 10, 68};
The call equals(a1, a2) returns true but the call equals(a1, a3) returns false.


### Solution
```sql
public static boolean equals(int[]a1, int []a2){
   if (a1.length!= a2.length){return false;}
   else{for(int i = 0; i<a1.length; i++)
   if(a1[i]!= a2[i])return false;}
 return true;
}
```
