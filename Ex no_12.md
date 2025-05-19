# EX 12 C program to check whether the given number is prime or not using function without return type and with arguments.
## DATE: 19/05/25
## AIM:
To write a C program to check whether the given number is prime or not using function without return type and with arguments.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output

## Program:
```
/*
C program to check whether the given number is prime or not using function without return type and with arguments.
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

// Function without return type and with arguments
void checkPrime(int n) {
    int i, flag = 0;

    if (n <= 1) {
        printf("%d is not a prime number.\n", n);
        return;
    }

    for (i = 2; i <= n / 2; i++) {
        if (n % i == 0) {
            flag = 1;
            break;
        }
    }

    if (flag == 0)
        printf("%d is a prime number.\n", n);
    else
        printf("%d is not a prime number.\n", n);
}

int main() {
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);

    checkPrime(num);  // Calling the function with argument

    return 0;
}

## Output:
Enter a number: 17
17 is a prime number.



## Result:
Thus the program was executed and the output was verified successfully.
