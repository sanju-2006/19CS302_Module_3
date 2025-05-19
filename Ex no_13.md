# EX 13 To write a C program to read the elements and print only the odd elements in the 2D array.
## DATE: 19/05/25
## AIM:
To write a C program to read the elements and print only the odd elements in the 2D array.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output
## Program:
```
/*
Program to read the elements and print only the odd elements in the 2D array.
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

int main() {
    int rows, cols;
    
    // Read size of the 2D array
    printf("Enter number of rows: ");
    scanf("%d", &rows);
    printf("Enter number of columns: ");
    scanf("%d", &cols);

    int arr[rows][cols];

    // Read elements into the 2D array
    printf("Enter the elements of the array:\n");
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            scanf("%d", &arr[i][j]);
        }
    }

    // Print only odd elements
    printf("Odd elements in the array:\n");
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            if (arr[i][j] % 2 != 0) {
                printf("%d ", arr[i][j]);
            }
        }
    }

    printf("\n");
    return 0;
}

## Output:
Enter number of rows: 2
Enter number of columns: 3
Enter the elements of the array:
1 2 3
4 5 6
Odd elements in the array:
1 3 5



## Result:
Thus the program was executed and the output was verified successfully.
