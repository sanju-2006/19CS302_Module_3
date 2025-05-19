# EX 15 C program that reads a one-dimensional array of integers and replaces all even elements with 'E'.
## DATE: 19/05/25
## AIM:
To write a C program that reads a one-dimensional array of integers and replaces all even elements with 'E'.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4. Check for error
5. Run & Display the output

## Program:
```
/*
Program that reads a one-dimensional array of integers and replaces all even elements with 'E'.
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

int main() {
    int arr[100], n, i;
    scanf("%d", &n);
    printf("Enter %d integer elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("Modified array:\n");
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", arr[i]);
    }

    printf("\n");
    return 0;
}

## Output:
10 15 22 7 8
Modified array:
E 15 E 7 E


## Result:
Thus the program was executed and the output was verified successfully.
