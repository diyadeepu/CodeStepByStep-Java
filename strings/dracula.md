# Problem: dracula

What is the value of s after the following code is finished running?

```sql
String s = "dracula";
for (int i = 0; i < s.length(); i++) {
    char a = s.charAt(0);
    String b = s.substring(1);
    s = b + a;
}
```

### Solution
Value of s: "dracula"
