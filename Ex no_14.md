# EX 14 C program to delete first element in an array.
## DATE: 19/05/25
## AIM:
To write a C program to delete first element in an array.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output

## Program:
```
/*
Program to delete first element in an array.
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

int main() {
    int arr[100], n, i;

    // Read the size of the array

    scanf("%d", &n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Deleting the first element by shifting elements left
    for(i = 0; i < n - 1; i++) {
        arr[i] = arr[i + 1];
    }

    n--; // Decrease the size after deletion

    // Print the updated array
    printf("Array after deleting the first element:\n");
    for(i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }

    printf("\n");
    return 0;
}

## Output:
10 20 30 40 50
Array after deleting the first element:
20 30 40 50


## Result:
Thus the program was executed and the output was verified successfully.
