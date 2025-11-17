Write a function that checks if a given string (case insensitive) is a palindrome.

A palindrome is a word, number, phrase, or other sequence of symbols that reads the same backwards as forwards, such as madam or racecar.


```java
public class Palindrome {

    public static boolean isPalindrome(String str) {
        String cleaned = str.toLowerCase(); ////Это метод (функция), который возвращает новую строку, где все буквы превращены в маленькие.
        int left = 0;
        int right = cleaned.length() - 1; ////это метод, который возвращает количество символов в строке.

        while (left < right) {
            if (cleaned.charAt(left) != cleaned.charAt(right)) {
                return false;
            }
            left++;
            right--;
        }

        return true;
    }
}
//charAt(i) — это метод, который возвращает символ по индексу i.

```
