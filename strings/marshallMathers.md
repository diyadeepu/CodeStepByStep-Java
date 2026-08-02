# Problem: marshallMathers

Given the following variable declarations:

```sql
// index       0123456789012345678901234
String s1   = "Snoop Dogg";
String s2   = "Marshall 'Eminem' Mathers";
String s3   = s2.substring(18);
String book = "Art & Science of Java";
```

Give the results of the following expressions. Make sure to indicate a value of the proper type (e.g. strings in " " quotes).

### Solution

- **s1.length():** 10
- **s2.length():** 25
- **s1.indexOf("o"):** 2
- **s2.indexOf("x"):** -1
- **s1.substring(6, 9):** "Dog"
- **s2.substring(21):** "hers"
- **book.substring(6, 12):** "Scienc"
- **s3.toLowerCase():** "mathers"
