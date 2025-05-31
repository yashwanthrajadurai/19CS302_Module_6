# EX 30 C program to add two integer elements in an array using realloc() and that array already has three elements.

## AIM:

To write a C program to add two integer elements in an array using realloc() and that array already has three elements.

## Algorithm

Start.

Declare array size

Initialize array elements using malloc()

Update array size using realloc()

Print the result.

End.  

## Program:

#include <stdio.h>

#include <stdlib.h>

int main() {

 int *arr, size, i;
 
 size = 3;
 
 arr = (int *)malloc(size * sizeof(int)); 
 
 for (i = 0; i < size; i++) {
 
 arr[i] = i * 10; }
 
 printf("Original array:\n");
 
 for (i = 0; i < size; i++) {
 
 printf("%d ", arr[i]);

 }
 
 printf("\n");
 
 size *= 2;
 
 arr = (int *)realloc(arr, size * sizeof(int)); 
 
 for (i = size / 2; i < size; i++) {
 
 arr[i] = i * 10;

printf("Updated array:\n");

 for (i = 0; i < size; i++) {
 
 printf("%d ", arr[i]);
 
 }
 }

## Output:

![Screenshot 2025-05-26 131625](https://github.com/user-attachments/assets/26740c34-cd5d-403a-8ca8-f3117086777c)


## Result:

Thus the program was executed and the output was verified successfully.
