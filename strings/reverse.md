# Problem: reverse

Write a method named reverse that accepts a string parameter returns a new string with the characters in the opposite order. For example, A call of reverse("Pikachu") would return "uchakiP".

### Solution

```sql
public static String reverse(String b) {
    String a = "";
    for (int i = b.length() - 1; i >= 0; i--){
      a += b.substring(i, i + 1);
    }
    return a;
  }
```
