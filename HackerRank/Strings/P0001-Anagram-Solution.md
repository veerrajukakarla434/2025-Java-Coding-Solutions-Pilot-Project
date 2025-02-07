# Anagram Strings program with Java HackerRank Solutions

![image](https://github.com/user-attachments/assets/e7851fa5-2c2b-4520-9be5-8febfc205caa)

```java
import java.util.Arrays;
import java.util.Scanner;

public class Anagram {

    static boolean isAnagram(String a, String b) {
        if (a.length() != b.length())
            return false;

        a = a.toLowerCase();
        b = b.toLowerCase();

        char[] Arr1 = a.toCharArray();
        char[] Arr2 = b.toCharArray();
        Arrays.sort(Arr1);
        Arrays.sort(Arr2);

        return Arrays.equals(Arr1, Arr2);
    }

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        String a = scan.next();
        String b = scan.next();
        scan.close();
        
        boolean ret = isAnagram(a, b);
        System.out.println(ret ? "Anagrams" : "Not Anagrams");
    }
}

```

![image](https://github.com/user-attachments/assets/c5641bcb-0a7c-4e87-91f6-58719c7b140c)

