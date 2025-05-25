
AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

ALGORITHM:
Declare two integer variables to store the values of M and N.
Use the printf function to prompt the user to enter the values of M and N.
Use the scanf function to read the values of M and N from the user.
Use a loop (for or while) to iterate from M to N.
Inside the loop, check if the current number is even.
If the current number is even, print it.
Continue the loop until you have iterated through all numbers from M to N.
PROGRAM:
#include <stdio.h>
int main() {
    int M, N, i;

    scanf("%d", &M);
    scanf("%d", &N);
    for (i = M; i <= N; i++) {
        if (i % 2 == 0) {
            printf("%d ", i);
        }
    }
    printf("\n");
    return 0;
}
OUTPUT:
![image](https://github.com/user-attachments/assets/91f08241-18d4-43d6-aae4-22b583e95f58)


RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully

EX-07-Nested-loop
AIM:
Write a C program to print the given triangular pattern using loop.

ALGORITHM:
Declare a variable to store the number of rows in the triangle.
Use the printf function to prompt the user to enter the number of rows.
Use a loop (for or while) to iterate through each row.
Inside the loop, use another loop to print the desired number of asterisks for each row.
Continue the loop until you have printed the entire triangular pattern.
PROGRAM:
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    for (int i=n;i>0;i--){
        for (int j=0;j<i;j++){
            printf("*");
        }
        printf("\n");
    }
}
OUTPUT:
![image](https://github.com/user-attachments/assets/8c84cd63-d8c9-4b05-ac6d-545b54683081)


RESULT:
Thus the program to print the given triangular pattern using loop has been executed successfully

EX-08-Functions
AIM:
Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

ALGORITHM:
Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
Inside the addition & subtraction function, add & subtract the two numbers and print the result.
In the main function, declare two integer variables and read their values from the user.
Call the addition and subtraction functions, passing the two numbers as arguments.
PROGRAM:
#include <stdio.h>
void add(int a, int b) {
    int sum = a + b;
    printf("Sum = %d\n", sum);
}
void subtract(int a, int b) {
    int difference = a - b;
    printf("Difference = %d\n", difference);
}
int main() {
    int num1, num2;
    scanf("%d", &num1);
    scanf("%d", &num2);

    add(num1, num2);
    subtract(num1, num2);

    return 0;
}
OUTPUT:
![image](https://github.com/user-attachments/assets/92d5bfcb-69c5-4300-ac18-a1d5537646f0)


RESULT:
Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully

EX-09-Use For Loop
AIM:
Write a c program to find the sum of odd digits using for loop

ALGORITHM:
Declare variables to store the input number and the sum of odd digits.
Initialize the sum of odd digits to 0.
Use a for loop to iterate through each digit of the input number.
Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
If the digit is odd, add it to the sum of odd digits.
Print the sum of odd digits.
PROGRAM:
#include <stdio.h>

int main() {
    int num, digit, sum = 0, i;
    scanf("%d", &num);
    for (i = num; i > 0; i = i / 10) {
        digit = i % 10; 

        if (digit % 2 != 0) { 
            sum += digit;
        }
    }
    printf("Sum of odd digits = %d\n", sum);
    return 0;
}
OUTPUT:
![image](https://github.com/user-attachments/assets/67e60d90-b9d4-4f9c-8fee-36b2b42f9855)


RESULT:
Thus the program to find the sum of odd digits using for loop has been executed successfully.

EX – 10 - Factorial of a Number Using a Function
AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.

ALGORITHM:
Start
Declare the function fact().
In the main() function, call the fact() function.
In fact() function: a. Declare variables i, N, and fact (initialized to 1). b. Read an integer N from the user. c. Use a for loop from 1 to N: i. Multiply fact by i in each iteration. d. After the loop, print the factorial value.
End
PROGRAM:
#include <stdio.h>

int factorial() 
{
    int n, fact = 1;
    scanf("%d", &n);
    for (int i = 1; i <= n; i++)
    {
        fact *= i;
    }
    
    return fact;
}

int main() {
    printf("Factorial value is: %d\n", factorial());
    return 0;
}
OUTPUT:
![image](https://github.com/user-attachments/assets/eb8351d8-7b90-4ea4-8bd0-12644261a2e0)


RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
