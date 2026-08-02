# Problem: containsTwice

Write a method named containsTwice that accepts a string and a character as parameters and returns true if that character occurs two or more times in the string. For example, the call of containsTwice("hello", 'l') should return true because there are two 'l' characters in that string.

### Solution

```sql
public static boolean containsTwice(String a, char x){
    int count = 0;
    if(a.indexOf(x)== -1){
        return false;
    }
    if(a.indexOf(x)!= -1){
        count++;
        a = a.substring (0, a.indexOf(x)) + a.substring(a.indexOf(x)+1);
    }
    if(a.indexOf(x)!= -1){
        return true;
    }
   return false;
}
```
