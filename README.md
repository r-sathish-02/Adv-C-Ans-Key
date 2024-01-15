<div align='center'>

  # ADVANCED C PROGRAMMING ANSWER KEY
  </div>

<div align='center'>
  
  ## PART-A
  </div>
<table>
  <tr>
    <td>
      QA101
    </td>
    <td>
      <h5>Compare the for, while loop and do-while.</h5><h4>Ans:</h4>
      <h5>for loop:</h5>

• Initialization is executed once, before the loop starts.<br>
• Condition is checked. If true, the loop body executes.<br>
• Increment/decrement is executed after each iteration.<br>
• Steps 2-3 repeat until the condition is false.<br>
<h5>while loop:</h5>

• Condition is checked. If true, the loop body executes.<br>
• Steps 1-2 repeat until the condition is false.<br>

<h5>do-while loop:</h5>

• The loop body executes at least once.<br>
• Condition is checked. If true, the loop body executes again.<br>
• Steps 2-3 repeat until the condition is false.<br>
</td>

  </tr>
<tr>
  <td>
    QA102
  </td>
  <td>
    <h5> Write a program to initialize the value as 7680 & display the value on the monitor.</h5>
    <h4>Ans:</h4>
#include <stdio.h>
  
int main()<br>
{<br>
    int value = 7680;<br>
    printf("The value is: %d\n", value);<br>
    return 0;<br>
}<br>


  </td>
</tr>
<tr>
  <td>
    QA103
  </td>
  <td>
    <h5>Illustrate the C Programming Structure.</h5>
    <h4>Ans:</h4>
    Structures are user-defined data types that allow you to group variables of different types under a single name. They provide a way to organize and manage related data as a single unit, making code more readable and maintainable.<br>
  </td>
  
</tr>
<tr>
  <td>
    QA104
  </td>
  <td>
    Produce the output for the following C program<br>
    
#include <stdio.h>

int main()<br>
{<br>
  int number=1;<br>
  for(;number<10;)<br>
  {<br>
    printf("%d",number);<br>
    number++;<br>
  }<br>
return 0;<br>
}<br>
<h4>Ans:</h4>
123456789
  </td>
</tr>
<tr>
  <td>
    QA105
  </td>
  <td>
   <h5> List the unconditional/special control statements in C programming language</h5>
    <h4>Ans:</h4>
    1. goto statement:<br>

2. break statement:<br>

3. continue statement:<br>

4. return statement:<br>
  </td>
</tr>
<tr>
  <td>
    QA106
  </td>
  <td>
    <h5>write a program to find minimum between -300,-400,500 numbers using conditional operator?</h5>
    <h4>Ans:</h4>
    
#include <stdio.h>

int main()<br>
{<br>
  int num1 = -300;<br>
  int num2 = -400;<br>
  int num3 = 500;<br>

  int minimum = (num1 < num2) ? (num1 < num3 ? num1 : num3) : (num2 < num3 ? num2 : num3);<br>

  printf("The minimum number is: %d\n", minimum);<br>

  return 0;<br>
}<br>

  </td>
</tr>
<tr>
  <td>
    QA107
  </td>
  <td>
    <h5>Write a C program to perform the basic left and right shift operation for 22 integer number.</h5>
    <h4>Ans:</h4>
    
#include <stdio.h>

int main()<br>
{<br>
    int num = 22;<br>
    int left_shifted, right_shifted;<br>
    left_shifted = num << 2;<br>
    printf("Left shift by 2 bits: %d\n", left_shifted);<br>
    right_shifted = num >> 3;<br>
    printf("Right shift by 3 bits: %d\n", right_shifted);<br>
    return 0;<br>
}<br>

  </td>
</tr>
<tr>
  <td>
    QA108
  </td>
  <td>
    <h5>Write a program to find product of two fraction values.</h5>
    <h4>Ans:</h4>
    
#include <stdio.h>

int main()<br>
{<br>
int num1, denom1, num2, denom2, product_num, product_denom;<br>

printf("Enter the first fraction (numerator denominator): ");<br>
scanf("%d %d", &num1, &denom1);<br>

printf("Enter the second fraction (numerator denominator): ");<br>
scanf("%d %d", &num2, &denom2);<br>

// Calculate the product of the numerators and denominators<br>
product_num = num1 * num2;<br>
product_denom = denom1 * denom2;<br>

 // Simplify the fraction if possible<br>
int gcd = find_gcd(product_num, product_denom);<br>
 product_num /= gcd;<br>
 product_denom /= gcd;<br>

printf("The product of the fractions is: %d/%d\n", product_num, product_denom);<br>

 return 0;<br>
}<br>

// Function to find the greatest common divisor (GCD)<br>
int find_gcd(int a, int b)<br>
{<br>
    while (b != 0) {<br>
        int temp = b;<br>
        b = a % b;<br>
        a = temp;<br>
    }<br>
    return a;<br>
}<br>

  </td>
</tr>
<tr>
  <td>
    QA109
  </td>
  <td>
    <h5>write a  program to convert temperature 90.50 degree celsius to Fahrenheit?</h5>
    <h4>Ans:</h4>
    
#include <stdio.h>

int main()<br>
{<br>
  float celsius = 90.50;<br>
  float fahrenheit = (celsius * 9/5) + 32;<br>
  printf("%0.2f degrees Celsius is equal to %0.2f degrees Fahrenheit.\n", celsius, fahrenheit);<br>
  return 0;<br>
}<br>

  </td>
</tr>
<tr>
  <td>
    QA110
  </td>
  <td>
    <h5>Write a program to find perimeter of square</h5>
    <h4>Ans:</h4>
    
#include <stdio.h>

int main()<br>
{<br>
    int side;<br>
    scanf("%d", &side);<br>
    int perimeter = 4 * side;<br>
    printf("The perimeter of the square is: %d\n", perimeter);<br>
    return 0;<br>
}<br>

  </td>
</tr>
<tr>
  <td>
    QA201
  </td>
  <td>
    <h5>Elaborate the purpose of using functions in C?</h5>
    <h4>Ans:</h4>
    1. Code Reusability<br>
    2. Modularity<br>
    3. Abstraction<br>
    4. Code Testing<br>
    5. Collaboration<br>
    6. Problem Decomposition<br>
  </td>
</tr>
<tr>
  <td>
    QA202
  </td>
  <td>
    <h5>Discuss the types of arguments passing in C.</h5>
    <h4>Ans:</h4>
    <h4>1. Call by Value:</h4>When a function is called by value, copies of the actual arguments are passed to the function's formal parameters.<br>
    <h4>2. Call by Reference:</h4>In call by reference, the addresses of the actual arguments are passed to the function's formal parameters.<br>

  </td>
</tr>
<tr>
  <td>
    QA203
  </td>
  <td>
    <h5>Compare the pointer and pointer to pointer variable with suitable example.</h5>
    <h4>Ans:</h4>
    <h4>Pointer:</h4>

• A variable that stores the memory address of another variable.<br>
• It's declared using the * operator: int *ptr;<br>
• It points to the first byte of the variable it refers to.<br>
<h4>Pointer to Pointer:</h4>

• A variable that stores the address of another pointer variable.<br>
• It's declared using two * operators: int **ptrptr;<br>
• It points to the memory location where another pointer is stored.<br>
  </td>
</tr>
<tr>
  <td>
    QA204
  </td>
  <td>
    <h5>Write a C program to print the address of variable, pointer and pointer value.(Assume “i” is variable and “p” is pointer )</h5>
    <h4>Ans:</h4>
    
#include <stdio.h>

int main()<br>
{<br>
    int i = 10; <br>
    int *p = &i;    <br>
    printf("Address of variable i: %p\n", &i);<br>
    printf("Address of pointer p: %p\n", &p);<br>
    printf("Value of pointer p (address of i): %p\n", p);<br>
    printf("Value stored at the address pointed to by p: %d\n", *p);<br>
    return 0;<br>
}<br>

  </td>
</tr>
<tr>
  <td>
    QA205
  </td>
  <td>
    <h5>Write a C Program for pointer arithmetic of any type.</h5>
    <h4>Ans:</h4>
    
#include <stdio.h>

int main() {<br>
  // Declare a pointer of any type (modify as needed)<br>
  double *ptr;<br>
  
  // Allocate memory for 5 elements of the chosen type<br>
  
  ptr = (double *)malloc(5 * sizeof(double));             // Adjust sizeof for different types<br>
  
  // Initialize the elements using pointer arithmetic<br>
  
  for (int i = 0; i < 5; i++) {<br>
    *(ptr + i) = i * 2.5;                                // Assign values using pointer offset<br>
  }<br>

  // Print the elements using pointer arithmetic<br>
  
  for (int i = 0; i < 5; i++) {<br>
      printf("Element %d: %.1f\n", i, *(ptr + i));        // Access values using pointer offset<br>
  }<br>

  // Free the allocated memory<br>
  
  free(ptr);<br>

  return 0;<br>
  }<br>

  </td>
</tr>
<tr>
  <td>QA206</td>
  <td>
    <h5>Write a C program for Multiplication of two numbers using functions (With argument and with return type)</h5>
    <h4>Ans:</h4>
    
#include <stdio.h>

int multiply(int num1, int num2)<br
{<br>
    int product = num1 * num2;<br>
    return product;<br>
}<br>

int main() {<br>
  int num1, num2, result;<br>
  scanf("%d %d", &num1, &num2);<br>
  result = multiply(num1, num2);<br>

  printf("The product of %d and %d is %d\n", num1, num2, result);<br>

  return 0;<br>
}<br>


  </td>
</tr>
<tr>
  <td>
    QA207
  </td>
  <td>
    <h5>Write a C program for subtraction of two numbers using functions (With argument and without return type)</h5>
    <h4>Ans:</h4>
    
  #include <stdio.h>

void subtract(int num1, int num2) {<br>
    int difference = num1 - num2;<br>
    printf("The difference of %d and %d is %d\n", num1, num2, difference);<br>
}<br>

int main() {<br>
  int num1, num2;<br>

   scanf("%d %d", &num1, &num2);<br>

  subtract(num1, num2);<br>

  return 0;<br>
  }<br>

  </td>
</tr>
<tr>
  <td>
    QA208
  </td>
  <td>
    <h5>Write a C program for Division of two numbers using functions (With argument and without return type)</h5>
    <h4>Ans:</h4>
    
#include <stdio.h>

void divide(int num1, int num2) {<br>
    if (num2 == 0) {<br>
        printf("Error: Division by zero is not allowed.\n");<br>
    } <br>
    else {<br>
        float quotient = (float)num1 / num2; <br>
        printf("The quotient of %d and %d is %.2f\n", num1, num2, quotient);<br>
    }<br>
}<br>

int main() {<br>
  int num1, num2;<br>

   scanf("%d %d", &num1, &num2);<br>

   divide(num1, num2);<br>

   return 0;<br>
   }<br>

  </td>
</tr>
<tr>
  <td>QA209</td>
  <td>
    <h5>Write a C program for addition and subtraction a =30 and b=20 using functions</h5>
    <h4>Ans:</h4>
    
 #include <stdio.h>

int add(int a, int b) {<br>
   return a + b;<br>
}<br>

int subtract(int a, int b) {<br>
   return a - b;<br>
}<br>

int main() {<br>
   int a = 30, b = 20;<br>

   int sum = add(a, b);<br>
   printf("The sum of %d and %d is %d\n", a, b, sum);<br>

   int difference = subtract(a, b);<br>
   printf("The difference of %d and %d is %d\n", a, b, difference);<br>

   return 0;<br>
}<br>

  </td>
</tr>
<tr>
  <td>QA210</td>
  <td>
    <h5>Write a C program for Multiplication and Division of a = 50 and b =5 using functions </h5>
    <h4>Ans:</h4>
    
 #include <stdio.h>

int multiply(int a, int b) {<br>
    return a * b;<br>
}<br>

float divide(int a, int b) {<br>
    return a / b; <br>
}<br>

int main() {<br>
  int a = 50, b = 5;<br>

   int product = multiply(a, b);<br>
  printf("The product of %d and %d is %d\n", a, b, product);<br>

  float division = divide(a, b);<br>
  printf("The quotient of %d and %d is %.2f\n", a, b, quotient);<br>


  return 0;<br>
  }<br>

  </td>
</tr>
<tr>
  <td>
    QA301
  </td>
  <td>
    <h5>Illustrate the Array and how to initialize an array?</h5>
    <h4>Ans:</h4>
    Arrays:<br>

A collection of elements of the same data type, stored in contiguous memory locations.<br>
Accessed using an index, starting from 0.<br>
Represented with square brackets [] after the variable name.<br><br>
Types of Array Initialization:<br>

1.Initialization during declaration:<br>
example: int numbers[5] = {10, 20, 30, 40, 50};<br>

2.Initialization after declaration:<br>
example: <br>
float prices[3];<br>
for (int i = 0; i < 3; i++) {<br>
    prices[i] = 12.5 * (i + 1);<br>
}<br>
  </td>
</tr>
<tr>
  <td>
    QA302
  </td>
  <td>
    <h5>Determine 3-Dimentional Array and indexing with neat diagram.</h5>
    3-Dimensional Arrays:<br>
Represent a collection of elements arranged in a 3D grid-like structure, with rows, columns, and depth.<br>
Visualize as a cube of elements.<br><br>
    Declaration:<br>
    data_type array_name[rows][columns][depth];<br><br>
     Indexing:<br>
    Access elements using three indices:<br>
    array_name[row_index][column_index][depth_index]<br>
    Each index starts from 0.<br>
    ![3darray](https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/95f52000-4490-40c2-acf5-ae56713fd4eb)

  </td>
</tr>
</table>
 
