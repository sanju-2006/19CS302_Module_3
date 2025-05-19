# EX 11 C Program to convert a given decimal value to binary using function without arguments with return type.
## DATE: 19/15/25
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

// Function to get decimal input from user and return the decimal value
int getDecimal() {
    int num;
    printf("Enter a decimal number: ");
    scanf("%d", &num);
    return num;
}

// Function to convert and print binary equivalent
void convertToBinary(int num) {
    int binary[32];
    int i = 0;

    if (num == 0) {
        printf("Binary: 0\n");
        return;
    }

    while (num > 0) {
        binary[i] = num % 2;
        num = num / 2;
        i++;
    }

    printf("Binary: ");
    for (int j = i - 1; j >= 0; j--) {
        printf("%d", binary[j]);
    }
    printf("\n");
}

int main() {
    int decimal = getDecimal(); // Call the function with no arguments, get return value
    convertToBinary(decimal);   // Convert to binary
    return 0;
}


## Output:

Enter a decimal number: 25
Binary: 11001


## Result:
Thus the program was executed and the output was verified successfully.
