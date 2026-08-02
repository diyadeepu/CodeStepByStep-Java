# Problem: isPalindrome

Write a method named isPalindrome that accepts a string parameter and returns true if that string is a palindrome, or false if it is not a palindrome.

For this problem, a palindrome is defined as a string that contains exactly the same sequence of characters forwards as backwards, case-insensitively. For example, "madam" or "racecar" are palindromes, so the call of isPalindrome("racecar") would return true. Spaces, punctuation, and any other characters should be treated the same as letters; so a multi-word string such as "dog god" could be a palindrome, as could a gibberish string such as "123 $$ 321". The empty string and all one-character strings are palindromes by our definition. Your code should ignore case, so a string like "Madam" or "RACEcar" would also count as palindromes.

### Solution

```sql
public static boolean isPalindrome (String word){
   word = word.toLowerCase();
   for (int i = 0; i < word.length()/2; i++){
      String part = word.substring(i,i+1);
      if (!part.equals(word.substring(word.length()-1-i,word.length()-i))){
         return false;
      }
   }
   return true;
}
```
