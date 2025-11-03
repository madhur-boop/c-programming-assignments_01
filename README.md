# c-programming-assignments_01
there are 5 questions and their answers are as well upload on this repos

//que.01:- what do you mean by array give one example of array and how you can declare an array ?
/* Answer:
An array is a collection of elements of the same data type, stored in contiguous memory locations.
It allows us to store multiple values in a single variable name instead of creating separate variables for each value.

For example, if we want to store the marks of 5 students, instead of creating 5 separate variables, we can use one array.

Example:

int marks[5] = {80, 75, 90, 85, 70};


Here,

int → data type (integer)

marks → name of array

[5] → size of array (it can store 5 integers)

{80, 75, 90, 85, 70} → elements of the array

Array Declaration Syntax:

data_type array_name[size];


Example:

float numbers[10];


This declares an array named numbers which can store 10 float values */


/* que.02:-  What do you mean by functions? Write the types of functions and give one example in code of each type
Answer:
A function is a block of code that performs a specific task.
It helps to divide a large program into smaller, manageable parts, making the code easy to read, reuse, and debug.

In C language, a function is defined only once but can be used (called) many times in the program.

Types of Functions in C:

Functions are mainly of two types:

Library Functions (Predefined Functions)

User-defined Functions

1. Library Functions

These are built-in functions provided by C libraries.
They perform common tasks like input/output, mathematical calculations, etc.

Examples: printf(), scanf(), sqrt(), strlen(), etc.

Example Code:

#include <stdio.h>
#include <math.h>

int main() {
    double num = 16, result;
    result = sqrt(num); // using library function
    printf("Square root of %.0lf = %.2lf", num, result);
    return 0;
}

2. User-defined Functions

These are functions created by the user to perform a specific task.

Example Code:

#include <stdio.h>

// function declaration
void greet() {
    printf("Hello, welcome to C programming!");
}

int main() {
    greet(); // function call
    return 0;
}


Explanation:

void greet() → user-defined function

greet(); → function call inside main()

In short:

Type	Description	Example:-
Library Function	Already defined in C libraries	printf(), sqrt()
User-defined Function	Defined by user as per need	void greet() */


/*que.03:- . What do you mean by Pointers ? Write a code how you can initialise the pointer. 

Answer:
A pointer is a special variable that stores the memory address of another variable.
Instead of storing a value directly, a pointer holds the location where the value is stored in memory.

Pointers are very useful for dynamic memory allocation, arrays, functions, and structures.

Pointer Declaration and Initialization Syntax:
data_type *pointer_name;
pointer_name = &variable_name;


* → used to declare a pointer

& → address-of operator (used to get the memory address of a variable)

Example Code:
#include <stdio.h>

int main() {
    int num = 10;        // normal variable
    int *ptr;            // pointer declaration
    ptr = &num;          // pointer initialization

    printf("Value of num = %d\n", num);
    printf("Address of num = %p\n", &num);
    printf("Value stored in pointer ptr = %p\n", ptr);
    printf("Value pointed by ptr = %d\n", *ptr);

    return 0;
}


Explanation:

int *ptr; → declares a pointer to an integer.

ptr = &num; → stores the address of num in ptr.

*ptr → gives the value stored at that memory address (called dereferencing).

