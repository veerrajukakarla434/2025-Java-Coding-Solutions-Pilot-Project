# String Tokens program with Java HackerRank Solutions

![image](https://github.com/user-attachments/assets/fc00bc6d-28b8-4c19-826c-d7a63b78b90b)

```java
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        /* Enter your code here. Read input from STDIN. Print output to STDOUT. Your class should be named Solution. */
        
       Scanner scan = new Scanner(System.in);
       String s = scan.nextLine();
       String[] tokens = s.split("[^A-Za-z]+");
       List<String> filtered = new ArrayList<>();
        
        for (String token : tokens) {
            if (!token.isEmpty()) {
                filtered.add(token);
            }
        }
        
        System.out.println(filtered.size());
        for (String token : filtered) {
            System.out.println(token);
        }
        
        scan.close();
    }
}

```

![image](https://github.com/user-attachments/assets/83669060-dd6f-4090-aa8c-dd175008f860)

