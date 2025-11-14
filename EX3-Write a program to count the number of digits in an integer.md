# EX3 Write a program to count the number of digits in an integer.
## DATE: 22/08/2025
## AIM:
To write a java program to count the number of digits in an integer.
## Algorithm

1.Start the program.

2.Read an integer from the user.

3.Define a recursive function countDigits() that counts digits by dividing the number by 10 each time.

4.Base condition: if the number is 0, return 0.

5.Recursive step: return 1 + countDigits(number / 10).

6.Display the total count of digits.

7.Stop the program.
  

## Program:
```
Program to to count the number of digits in an integer
Developed by: Shriram S
RegisterNumber: 212222240098 
```
```py
import java.util.Scanner;

public class CountDigitsRecursive {
    static int countDigits(int n) {
        if (n == 0)
            return 0;
        return 1 + countDigits(n / 10);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter an integer: ");
        int n = sc.nextInt();
        if (n == 0)
            System.out.println("Number of digits: 1");
        else
            System.out.println("Number of digits: " + countDigits(Math.abs(n)));
        sc.close();
    }
}
```

## Output:


<img width="341" height="158" alt="Screenshot 2025-11-13 140952" src="https://github.com/user-attachments/assets/ce3a49e9-4f98-4b49-8aac-da86361752dc" />

## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
