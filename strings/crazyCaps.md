# Problem: crazyCaps

Write a method named crazyCaps that accepts a string as a parameter and returns a new string with its capitalization altered such that the characters at even indexes are all in lowercase and odd indexes are all in uppercase. For example, if a variable s stores "Hey!! THERE!", the call of crazyCaps(s); should return "hEy!! tHeRe!".

### Solution

```sql
public static String crazyCaps (String s){
    String str = "";
    for (int i = 0; i < s.length(); i++){
      if (i % 2 == 0){
       str += s.substring(i, i + 1).toLowerCase();
      }
      else{
       str += s.substring(i, i + 1).toUpperCase();
      }
    }
    return str;
}
```
