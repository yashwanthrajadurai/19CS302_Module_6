# EX 29 C program to create two float variables using calloc() and find minimum among them.

## AIM:

To write a C program to create two float variables using calloc() and find minimum among them.

## Algorithm

Start.

Initialize two variables value of calloc().

Prompt the user to enter values.

Read the values using scanf.

Find minimum and print result

End.  

## Program:

#include <stdio.h>

#include <stdlib.h>

int main() {

 int *num1, *num2, minimum;
 
 num1 = (int *)calloc(1, sizeof(int));
 
 num2 = (int *)calloc(1, sizeof(int));
 
 num1= 5.8 , num2 = 6.5;
 
 minimum = (*num1 < *num2) ? *num1 : *num2;
 
 printf("%d\n", minimum);
 
 free(num1);
 
 free(num2);


## Output:

![Screenshot 2025-05-26 131432](https://github.com/user-attachments/assets/c21084d0-d182-43d5-a824-ed0361668cc6)


## Result:

Thus the program was executed and the output was verified successfully.
