# Problem: NameGame

Write a console program in a class named NameGame that prints the following rhyme about the person's first and last name. You may assume that the user types a string with exactly one space.

```sql
What is your name? Fifty Cent
Fifty, Fifty, bo-Bifty
Banana-fana fo-Fifty
Fee-fi-mo-Mifty
FIFTY!

Cent, Cent, bo-Bent
Banana-fana fo-Fent
Fee-fi-mo-Ment
CENT!
```

### Solution

```sql
import java.util.*;
public class NameGame 
 {
  public static void main(String[] args) 
  {
   Scanner console = new Scanner (System.in);
   System.out.print("What is your name? ");
   String firstName = console.next();
   String lastName = console.next();
   System.out.println(firstName + ", " + firstName + ", bo-B" + firstName.substring(1));
   System.out.println("Banana-fana fo-F" + firstName.substring(1));
   System.out.println("Fee-fi-mo-M" + firstName.substring(1));
   System.out.println(firstName.toUpperCase() + "!");
   System.out.println();
   System.out.println(lastName + ", " + lastName + ", bo-B" + lastName.substring(1));
   System.out.println("Banana-fana fo-F" + lastName.substring(1));
   System.out.println("Fee-fi-mo-M" + lastName.substring(1));
   System.out.println(lastName.toUpperCase() + "!");
  }
}
```
