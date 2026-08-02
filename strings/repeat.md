# Problem: repeat

Write a method named repeat that accepts a string and a number of repetitions as parameters and returns the string concatenated that many times. For example, the call of repeat("hello", 3) returns "hellohellohello". If the number of repetitions is 0 or less, return an empty string.

### Solution

```sql
public static String repeat(String s1, int n){
String a = "";
for (int i = 0; i<n; i++){
    a+= s1;
}
    return a;
}
```
