# Problem: productOfOthers

Write a method named productOfOthers that accepts an array of integers a as its parameter and returns a new array where each element at index i stores the product of all elements in a excluding a[i]. For example, if the array a stores {1, 4, 3, 4, 2}, the call of productOfOthers(a) should return {96, 24, 32, 24, 48}.

You may assume that the product of all elements in the array is within the domain of integers (type int).

### Solution

```sql
public static int [] productOfOthers(int [] a){
  int product = 1;
  int zero = 1;
  int [] array = new int[a.length];
  for (int i = 0; i < a.length; i++){
      if (a[i] == 0){product=product;
       zero = 0;}
    else{product *= a[i];}
  }
  for (int i = 0; i < a.length; i++){
      if (a[i] == 0)
          array[i]=product;
      else if(a[i] != 0 && zero == 0){array[i] =0;}
      else{array[i] = product/a[i];}
  }
  return array;
}
```
