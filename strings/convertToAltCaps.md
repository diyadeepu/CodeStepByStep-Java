# Problem: convertToAltCaps

Write a method named convertToAltCaps that accepts a string as a parameter and returns a version of the string where alternating letters are uppercase and lowercase, starting with the first letter in lowercase. For example, the call of convertToAltCaps("Pikachu") should return "pIkAcHu".

### Solution

```sql
public static String convertToAltCaps(String a){
    String b = "";
    int count = 0;
    for (int i = 0; i < a.length(); i++){
        if(!a.substring(i, i + 1).equals(" "))
        {
          if (count%2 == 0){
              String ab = a.substring(i, i + 1);
              b+=ab.toLowerCase();
              count++;}
          else {
              String bc = a.substring(i, i + 1).toUpperCase();
              b += bc;
              count++;
            }
        }
        else {
        b += " ";
        }
    }
    return b;
}
```
