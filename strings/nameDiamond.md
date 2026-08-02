# Problem: nameDiamond

Write a method named nameDiamond that accepts a string as a parameter and prints it in a "diamond" format as shown below. For example, the call of nameDiamond("MARTY"); should print:

```sql
M
MA
MAR
MART
MARTY
 ARTY
  RTY
   TY
    Y
```

### Solution

```sql
public static void nameDiamond (String s){
    for (int i = 0; i < s.length(); i++){
        System.out.println(s.substring(0, i+1));
    }
    for (int j = 0; j < s.length(); j++){
        for (int a = 0; a <= j; a++){System.out.print(" ");}
        System.out.println(s.substring(j+1, s.length()));
    }
}
```
