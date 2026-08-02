# Problem: printBackward

Write a method named printBackward that accepts a String as its parameter and prints the characters in the opposite order. For example, a call of printBackward("hello there!"); should print the following output:

```sql
!ereht olleh
```
If the empty string is passed, no output should be produced.

### Solution

```sql
public static void printBackward(String b) {
    String a = "";
    for (int i = b.length()-1; i >=0; i--){
      a += b.substring(i, i+1);
    }
    System.out.println(a);
  }
```
