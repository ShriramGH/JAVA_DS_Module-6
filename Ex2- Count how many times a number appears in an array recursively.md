# Ex2 Count how many times a number appears in an array recursively.
## DATE: 09/08/2025
## AIM:
To write a Java program to Count how many times a number appears in an array recursively.

## Algorithm
1.Start the program.

2.Read the size of the array and input all elements into the array.

3.Read the target number whose frequency you want to count.

4.Call the recursive function countOccurrences(arr, index, target)
  If index == arr.length, return 0
  If arr[index] == target, return 1 + countOccurrences(arr, index + 1, target)
  Else return countOccurrences(arr, index + 1, target)
  
5.Display the returned count as the total number of occurrences.

6.End the program.

## Program:
```
Program Count how many times a number appears in an array recursively.
Developed by: Shriram S
Register Number: 212222240098 
```
```py
import java.util.Scanner;

public class CountOccurrences {

    public static int countOccurrences(int[] arr, int n, int target) {
        //write your code here
        if (n == 0) {
            return 0;
        }

        if (arr[n - 1] == target) {
            return 1 + countOccurrences(arr, n - 1, target);
        } else {
            return countOccurrences(arr, n - 1, target);
        }
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int size = scanner.nextInt();

        if (size <= 0) {
            System.out.println("Invalid array size. Must be positive.");
            return;
        }

        int[] arr = new int[size];
        for (int i = 0; i < size; i++) {
            arr[i] = scanner.nextInt();
        }

        int target = scanner.nextInt();

        int count = countOccurrences(arr, size, target);
        System.out.println("The number " + target + " appears " + count + " time(s) in the array.");

        scanner.close();
    }
}

```

## Output:

<img width="1027" height="611" alt="image" src="https://github.com/user-attachments/assets/6c352262-b618-42ca-895f-669f0cff5116" />


## Result:
Thus, the Java program to Count how many times a number appears in an array recursively is implemented successfully.
