# EX 26 C program demonstrating a self-referential structure where an employee has a pointer to their manager.

## AIM:

To write a C program to demonstrate a self-referential structure where an employee has a pointer to their manager.

## Algorithm

Start.

Create a structure and data member using pointer.

Prompt the user to enter a value.

Print the structure values.

End.

## Program:

#include <stdio.h>

#include <stdlib.h>

struct Employee {

 int empID;
 
 char name[50];
 
 struct Employee *manager; };

int main() {

 struct Employee *emp1, *emp2, *emp3;
 
 emp1 = (struct Employee*)malloc(sizeof(struct Employee));
 
 emp2 = (struct Employee*)malloc(sizeof(struct Employee));
 
 emp3 = (struct Employee*)malloc(sizeof(struct Employee));
 
 emp1->empID = 1;
 
 snprintf(emp1->name, sizeof(emp1->name), "John Doe");
 
 emp1->manager = NULL; 
 
 emp2->empID = 2;
 
 snprintf(emp2->name, sizeof(emp2->name), "Alice Smith");
 
 emp2->manager = emp1; 
 
 emp3->empID = 3;
 
 snprintf(emp3->name, sizeof(emp3->name), "Bob Brown");
 
 emp3->manager = emp1; 
 
 printf("Employee 1: %s (ID: %d), Manager: %s\n", emp1->name, emp1->empID, (emp1->manager == 

NULL) ? "None" : emp1->manager->name);

 printf("Employee 2: %s (ID: %d), Manager: %s\n", emp2->name, emp2->empID, emp2->manager->name);
 
 printf("Employee 3: %s (ID: %d), Manager: %s\n", emp3->name, emp3->empID, emp3->manager->name);
 
 free(emp1);
 
 free(emp2);
 
 free(emp3);
 
 return 0;

}

## Output:

![Screenshot 2025-05-26 130805](https://github.com/user-attachments/assets/0dbd4fa2-b122-4a9c-b6d3-8d5ef23c2e4b)


## Result:

Thus the program was executed and the output was verified successfully.
