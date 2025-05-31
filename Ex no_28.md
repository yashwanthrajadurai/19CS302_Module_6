# EX 28 C program that demonstrates the use of enum (enumeration) type to define and use named integer constants.

## AIM:

To write a C program that demonstrates the use of enum (enumeration) type to define and use named integer constants.

## Algorithm

Start.

Declare enum type

Declare all days in a week

Print result

End

## Program:

#include <stdio.h>

enum weekdays {

 Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday

};

int main() {

 enum weekdays today = Wednesday;
 
 if (today == Wednesday) {
 
 printf("Today is Wednesday.\n");
 
 }

}


## Output:

![Screenshot 2025-05-26 131241](https://github.com/user-attachments/assets/6513f9ec-8fe5-4954-a03d-96e2616f4ce9)



## Result:

Thus the program was executed and the output was verified successfully.
