# Problem: stutter

Write a method named stutter that accepts a string parameter returns a new string replacing each of its characters with two consecutive copies of that character. For example, a call of stutter("hello") would return "hheelllloo".

### Solution

```sql
public static String stutter (String s1){
    String a = "";
    for (int i = 0; i < s1.length(); i++){
        a+= s1.substring (i, i + 1);
        a+= s1.substring (i, i + 1);
    }
    return a;
}
```
