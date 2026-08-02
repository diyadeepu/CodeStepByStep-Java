# Problem: removeAll

Write a method named removeAll that accepts a string and a character as parameters, and removes all occurrences of the character. For example, the call of removeAll("Summer is here!", 'e') should return "Summr is hr!". Do not use the string replace method in your solution.

### Solution

```sql
public static String removeAll (String a, char b){
    String b1 = "" + b;
    for (int i = 0; i < a.length(); i++){
        if (a.substring (i, i + 1).equals(b1)){
            a = a.substring (0, i) + a.substring (i + 1);
            i--;
        }
    }
    return a;
}
```
