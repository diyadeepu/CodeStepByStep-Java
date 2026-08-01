# Problem: getPercentEven

Write a method named getPercentEven that accepts an array of integers as a parameter and returns the percentage of the integers in the array that are even numbers. For example, if an array a stores {6, 4, 9, 11, 5}, then your method should return 40.0 representing 40% even numbers. If the array contains no even elements or is empty, return 0.0. Do not modify the array passed in.

### Solution

```sql
public static double getPercentEven (int [] array)
{
 double evenCount = 0.0;
 if (array.length == 0)
 {
  return 0.0;
 }
 for (int i : array)
 {
  if (i % 2 == 0)
  {
   evenCount += 1.0;
  }
 }
 double percent = evenCount / array.length;
 double totalPercent = percent * 100;
 return totalPercent;
}
```
