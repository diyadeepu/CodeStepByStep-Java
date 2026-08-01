# Problem: findRange

Write a method named findRange that accepts an array of integers as a parameter and returns the range of values contained in the array, which is equal to one more than the difference between its largest and smallest element. For example, if the largest element is 17 and the smallest is 6, the range is 12. If the largest and smallest values are the same, the range is 1.

Constraints: You may assume that the array contains at least one element (that its length is at least 1). You should not modify the contents of the array.

### Solution

```sql
public static int findRange(int [] a){
    int range = 1;
    int max = -10000;
    int min = 10000;
    for (int i = 0; i < a.length; i++){
        if (a[i] < min){
            min = a[i];
        }
        if (a[i] > max){
            max = a[i];
        }
    }
    return max-min+range;
}
```
