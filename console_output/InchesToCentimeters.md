# Problem: InchesToCentimeters

Write an interactive console program in a class named InchesToCentimeters that prompts the user to read in two input values: a number of feet, followed on a separate line by a number of inches. The program should convert this amount to centimeters. Here is a sample run of the program (user input is shown like this):

```sql
This program converts feet and inches to centimeters.
Enter number of feet: 5
Enter number of inches: 11
5ft 11in = 180.34cm
```

### Solution

```sql
import java.util.*;
public class InchesToCentimeters {
    public static void main(String[] args) {
        System.out.println("This program converts feet and inches to centimeters.");
        Scanner console = new Scanner (System.in);
        System.out.print("Enter number of feet: ");
        int feet = console.nextInt();
        System.out.print("Enter number of inches: ");
        int inch = console.nextInt();
        double centimeter = 2.54 *(12*feet+inch);
        System.out.println(feet+"ft "+inch+"in = "+ centimeter + "cm");
    }
}
```
