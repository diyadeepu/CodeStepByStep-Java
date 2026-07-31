# Problem: computeAverage

Write a method named computeAverage that computes and returns the mean of all elements in an array of integers. For example, if an array named a contains [1, -2, 4, -4, 9, -6, 16, -8, 25, -10], then the call of computeAverage(a) should return 2.5.

Constraints: You may assume that the array contains at least one element. Your method should not modify the elements of the array.

```sql
public static double computeAverage(int [] arr)
{
 double sum = 0.0;
 double finalValue = 0.0;
 for (int i : arr)
 {
  sum += i; 
  finalValue = sum/arr.length;
 }
 return finalValue;
}
```
