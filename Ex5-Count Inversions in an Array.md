# Ex5 Count Inversions in an Array
## DATE: 29/08/2025
## AIM:
To write a Java program  to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j


## Algorithm

1. Start the program.
2. Read the number of elements `n` and the array elements.
3. Initialize a variable `count = 0` to store the number of inversions.
4. Use two nested loops:

   * Outer loop: `i` from `0` to `n-2`
   * Inner loop: `j` from `i+1` to `n-1`
   * If `arr[i] > arr[j]`, increment `count` by 1.
5. Display the value of `count` as the total number of inversions.
6. Stop the program.


## Program:
```
Program to count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j
Developed by: Shriram S
Register Number: 212222240098
```
```py
import java.util.Scanner;

public class CountInversions {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        int n = sc.nextInt();
        int[] arr = new int[n];
        
        for(int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
        
        int inversions = countInversions(arr, n);
        System.out.println(inversions);
    }
    
    static int countInversions(int[] arr, int n) {
        int count = 0;
        for(int i = 0; i < n - 1; i++) {
            for(int j = i + 1; j < n; j++) {
                if(arr[i] > arr[j]) {
                    count++;
                }
            }
        }
        return count;
    }
}

```

## Output:

<img width="957" height="447" alt="image" src="https://github.com/user-attachments/assets/3edb6918-d9c2-430e-9244-36a72ec19997" />


## Result:
Thus the Java program to to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < jis implemented successfully.
