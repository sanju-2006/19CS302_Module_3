# EX 11 C Program to convert a given decimal value to binary using function without arguments with return type.
## DATE: 19/05/25
## AIM:
To write a C Program to convert a given decimal value to binary using function without arguments with return type.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output
## Program:
```
/*
Program to C Program to convert a given decimal value to binary using function without arguments with return type.
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

// Function without arguments, but with return type
int getDecimal() {
    int n;
    printf("Enter a decimal number: ");
    scanf("%d", &n);
    return n;
}

int main() {
    int num = getDecimal();  // Calling the function and storing the return value

    int binary[32];
    int i = 0;

    // Edge case for 0
    if (num == 0) {
        printf("Binary: 0\n");
        return 0;
    }

    // Decimal to Binary Conversion
    while (num > 0) {
        binary[i] = num % 2;
        num = num / 2;
        i++;
    }

    // Displaying binary in reverse
    printf("Binary: ");
    for (int j = i - 1; j >= 0; j--) {
        printf("%d", binary[j]);
    }
    printf("\n");

    return 0;
}

## Output:
Enter a decimal number: 10
Binary: 1010



## Result:
Thus the program was executed and the output was verified successfully.
