# Problem: maxValue

Write a method named maxValue that accepts an array of integers as a parameter and returns the maximum value in the array. For example, if an array named a passed stores {17, 7, -1, 26, 3, 9}, the call of maxValue(a) should return 26. You may assume that the array contains at least one element. Your method should not modify the elements of the array.

### Solution

```sql
public static int maxValue (int [] numbers)
{
// int j = 0;
 int maximum = numbers [0];
 for (int i = 1; i < numbers.length; i++)
 {
  if (numbers[i] > maximum)
  {
   maximum = numbers[i];
  }
 }
 return maximum;
}
```
