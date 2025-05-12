# EX 12 C program to check whether the given number is prime or not using function without return type and with arguments.
## DATE:
## AIM:
To write a C program to check whether the given number is prime or not using function without return type and with arguments.

## Algorithm
1.Start
2.Declare a function checkPrime(int num) to check for prime number
3.In main(), declare variable n and read its value using scanf
4.Call the function checkPrime(n)
5.In checkPrime(), check if num is less than or equal to 1 → not prime
6.Use a loop from 2 to num/2 to check for divisibility
7.If divisible, print not prime; else, print prime — End



## Program:
```
/*
C program to check whether the given number is prime or not using function without return type and with arguments.
Developed by: Sasi Kumar B
RegisterNumber:  212223060252
*/
#include <stdio.h>

void checkPrime(int num) {
    int i, isPrime = 1;

    if (num <= 1) {
        printf("%d is not a prime number.\n", num);
        return;
    }

    for (i = 2; i <= num / 2; i++) {
        if (num % i == 0) {
            isPrime = 0;
            break;
        }
    }

    if (isPrime)
        printf("%d is a prime number.\n", num);
    else
        printf("%d is not a prime number.\n", num);
}

int main() {
    int n;
    printf("Enter a number: ");
    scanf("%d", &n);
    checkPrime(n);
    return 0;
}

```

## Output:

![image](https://github.com/user-attachments/assets/98100f2f-b31f-47b0-9ebd-8e4b73bd1720)


## Result:
Thus the program was executed and the output was verified successfully.
