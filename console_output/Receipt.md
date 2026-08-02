# Problem: Receipt

The following console program is redundant. Rewrite it to use variables and expressions so that calculations are not repeated.

### Solution

The following code below is the corrected version, not the original version of code provided in the problem with errors.

```sql
public class Receipt {
    public static void main(String[] args) {
        // Compute total owed, assuming 8% tax and 15% tip
        int money = (38 + 40 + 30);
        double tax = (.08);
        double tip = (.15);
        System.out.println("Subtotal: " + (money));
        System.out.println("Tax: " + (money) * tax);
        System.out.println("Tip: " + (money) * tip);
        System.out.println("Total: " + (money + (money) * tax + (money) * tip));
    }
}
```
