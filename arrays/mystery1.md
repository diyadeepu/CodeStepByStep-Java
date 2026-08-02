# Problem: mystery1

What are the values of the elements in array a1 after the following code executes?

```sql
public static void mystery1(int[] a1, int[] a2) {
    for (int i = 0; i < a1.length; i++) {
        a1[i] += a2[a2.length - i - 1];
    }
}
int[] a1 = {1, 3, 5, 7, 9};
int[] a2 = {1, 4, 9, 16, 25};
mystery1(a1, a2);
```

### Solution
1. a1[0]: 26
2. a1[1]: 19
3. a1[2]: 14
4. a1[3]: 11
5. a1[4]: 10
