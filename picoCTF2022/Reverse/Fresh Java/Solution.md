# Fresh Java

The challenge is the following,
___
Задача заключается в следующем,

![image](https://user-images.githubusercontent.com/60939699/160281884-6dad4ce5-bb68-449d-825e-c3d5fe92e3cf.png)

Where we are given a file in **Java** and a hint that we should use a decompiler. We search the Internet, open an online service and give our file there, after which we get the following result.
___
Где нам дается файл на **Java** и подсказка, что мы должны импользовать декомпилятор. Ищем в интернете, открываем онлайн сервис и отдаем туда наш файл, после чего получаем следующий результат.

``` lang-java
import java.util.Scanner;
public class KeygenMe
{
    public static void main(final String[] array) {
        final Scanner scanner = new Scanner(System.in);
        System.out.println("Enter key:");
        final String nextLine = scanner.nextLine();
        if (nextLine.length() != 34) {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(33) != '}') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(32) != '4') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(31) != 'a') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(30) != '6') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(29) != 'e') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(28) != 'd') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(27) != '3') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(26) != 'c') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(25) != '0') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(24) != '_') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(23) != 'd') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(22) != '3') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(21) != 'r') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(20) != '1') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(19) != 'u') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(18) != 'q') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(17) != '3') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(16) != 'r') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(15) != '_') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(14) != 'g') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(13) != 'n') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(12) != '1') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(11) != 'l') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(10) != '0') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(9) != '0') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(8) != '7') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(7) != '{') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(6) != 'F') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(5) != 'T') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(4) != 'C') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(3) != 'o') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(2) != 'c') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(1) != 'i') {
            System.out.println("Invalid key");
            return;
        }
        if (nextLine.charAt(0) != 'p') {
            System.out.println("Invalid key");
            return;
        }
        System.out.println("Valid key");
    }
}
```

After studying it, it becomes clear that checks for the flag are written here in the code, we collect all the characters with which the comparison is made and get the key.
___
Изучив становится понятно, что здесь в коде прописаны проверки на флаг, собираем все символы с которыми производится сравнение и получаем ключ.
