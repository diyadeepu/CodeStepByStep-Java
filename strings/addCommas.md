# Problem: addCommas

Write a method named addCommas that accepts a string representing a number and returns a new string with a comma at every third position, starting from the right. For example, the call of addCommas("12345678") returns "12,345,678".

### Solution

```sql
public static String addCommas(String a){
    if (a.length()<=3){return a;}
    else {
        String b = "";
        int j = 1;
        for (int i = a.length() - 1; i>=0; i--){
            b+= a.substring (i, i+1);
            if (j%3==0 && i != 0){b+= ",";}
            j++;
        }
        a = "";
        for (int i = b.length() - 1; i>=0; i--){
            a += b.substring (i, i+1);
        }
      return a;
    }
}
```
