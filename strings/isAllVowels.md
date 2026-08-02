# Problem: isAllVowels

Write a method named isAllVowels that returns whether a string consists entirely of vowels (a, e, i, o, or u, case-insensitively). For example, isAllVowels("eiEIo") should return true while isAllVowels("banana") should return false.

For this problem, you may assume that a working solution already exists to the previous problem, isVowel, and you may call it in your solution.

### Solution

```sql
public static boolean isAllVowels(String a){
    boolean b = true;
    for (int i = 0; i <= a.length()-1; i++){
        if (a.substring(i, i+1).equals("a") || a.substring(i, i+1).equals("A") || a.substring(i, i+1).equals("e") || a.substring(i, i+1).equals("E") || a.substring(i, i+1).equals("i") || a.substring(i, i+1).equals("I") || a.substring(i, i+1).equals("o") || a.substring(i, i+1).equals("O") || a.substring(i, i+1).equals("u") || a.substring(i, i+1).equals("U")){
            b = true;}
        else {
        return false;}
    }
    return b;
}
```
