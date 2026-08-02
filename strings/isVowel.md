# Problem: isVowel

Write a method named isVowel that returns whether a string is a vowel (a single-letter string containing a, e, i, o, or u, case-insensitively).

### Solution

```sql
public static boolean isVowel (String one)
{
 if (one == "a" || one.toUpperCase() == "A")
 {
  return true;
 }
 else if (one == "e" || one.toUpperCase() == "E")
 {
  return true;
 }
 else if (one == "i" || one.toUpperCase() == "I")
 {
  return true;
 }
 else if (one == "o" || one.toUpperCase() == "O")
 {
  return true;
 }
 else if (one == "u" || one.toUpperCase() == "U")
 {
  return true;
 }
 else
 {
  return false;
 }
}
```
