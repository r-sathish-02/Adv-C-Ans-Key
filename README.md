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
    Each index starts from 0.<br><br>
    diagram<br>
   <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/81318bbe-842b-44fa-be87-c4fba583432d">

  </td>
</tr>
<tr>
  <td>QA303</td>
  <td>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/39cf63fb-267e-4597-a8d6-f3353f63b2bd">
     <h4>Ans:</h4>
    Found element 30 at position 2
  </td>
</tr>
<tr>
  <td>QA304</td>
  <td>
    <h5>List any two sorting techniques and searching techniques.</h5>
        <h4>Ans:</h4>

<h4>Sorting Techniques:</h4>
Bubble Sort<br>
Merge Sort
    
<h4>Searching Techniques:</h4>
Linear Search<br>
Binary Search

  </td>
</tr>
<tr>
  <td>QA305</td>
  <td>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/6a349744-f4ae-4bbf-b81d-bcfc9d3c92e2">
        <h4>Ans:</h4>
The length of the name is 30
  </td>
</tr>
<tr>
  <td>QA306</td>
  <td>
    <h4>Create  a C program to read n number of elements and print the first element of the array (integer).</h4>
    <h4>Ans:</h4>
    
#include <stdio.h>

int main() {<br>
   int n, i;<br>
  int array[100];<br>
  scanf("%d", &n);<br>

  for (i = 0; i < n; i++) {<br>
      scanf("%d", &array[i]);<br>    }<br>

  printf("The first element of the array is: %d\n", array[0]); <br>

   return 0;<br>}<br>
  </td>
</tr>
<tr>
  <td>QA307</td>
  <td>
    <h5>Create  a C program to read n elements as input and print the second element of the array (integer).</h5>
    <h4>Ans:</h4>
    
  #include <stdio.h>

int main() {<br>
  int n, i;<br>
   int array[100];<br>

   scanf("%d", &n);<br>


  for (i = 0; i < n; i++) {<br>
      scanf("%d", &array[i]);<br>
  }<br>

  printf("The second element of the array is: %d\n", array[1]);<br>

  return 0;<br>
  }<br>

  </td>
</tr>
<tr>
  <td>QA308</td>
  <td>
    <h5>Create  a C program to read n elements as input and print the last element of the array (integer)</h5>
    <h4>Ans:</h4>
    
  #include <stdio.h>

int main() {<br>
  int n, i;<br>
   int array[100];<br>

   scanf("%d", &n);<br>


  for (i = 0; i < n; i++) {<br>
      scanf("%d", &array[i]);<br>
  }<br>

  printf("The second element of the array is: %d\n", array[n-1]);<br>

  return 0;<br>
  }<br>
  </td>
</tr>
<tr>
  <td>QA309</td>
  <td>
    <h5>Create  a C program to read n elements as input and print the elements of the array (character).</h5>
    <h4>Ans:</h4>
    
#include <stdio.h>

int main() {<br>
   int i, n;<br>
   char array[100]; <br>

   scanf("%d", &n);<br>

  for (i = 0; i < n; i++) {<br>
      scanf(" %c", &array[i]);  <br>

  for (i = 0; i < n; i++) {<br>
      printf("%c ", array[i]);<br>
  }<br>
  printf("\n");<br>

  return 0;<br>
  }<br>

  </td>
</tr>
<tr>
  <td>QA310</td>
  <td>
    <h5>Write a program in C to read n number of values in an array and display it in reverse order.</h5>
    <h4>Ans:</h4>
    
  #include <stdio.h>

int main() {<br>
int n, i;<br>
  int array[100];<br>
  scanf("%d", &n);<br>

  for (i = 0; i < n; i++) {<br>
      scanf("%d", &array[i]);<br>
  }<br>

  for (i = n - 1; i >= 0; i--) { <br>
      printf("%d ", array[i]);<br>
  }<br>
  printf("\n");<br>
   return 0;<br>
   }<br>
  </td>
</tr>
<tr>
  <td>QA401</td>
  <td>
    <h5>Define structure with an example</h5>
    <h4>Ans:</h4>
    In C programming, a structure is a user-defined composite data type that groups variables of different data types under a single name. It's used to represent a collection of related data items as a single unit, making code more organized and easier to manage.<br>
    <h5>Example:</h5>
    
 #include <stdio.h>

struct Student {<br>
  int roll_no;<br>
  char name[50];<br>
   float marks;<br>
  };<br>

int main() {<br>
   struct Student s1 = {123, "Alice", 85.5};  <br>
  printf("Roll Number: %d\n", s1.roll_no);<br>
  printf("Name: %s\n", s1.name);<br>
  printf("Marks: %.2f\n", s1.marks);<br>

   return 0;<br>
}<br>

  </td>
</tr>
<tr>
  <td>QA402</td>
  <td>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/06426072-c04d-4397-8d71-d66b6a029913">
    <h4>Ans:</h4>
    Ravikumar 1981
  </td>
</tr>
<tr>
  <td>QA403</td>
  <td>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/d6665881-c3a5-4ad7-955a-8a5d4bb647a6">
   <h4>Ans:</h4> 
    101 Saveetha
  </td>
</tr>
<tr>
  <td>QA404</td>
  <td>
    <h5>Define self referenced structure with an example?</h5>
    <h4>Ans:</h4> 
    A self-referenced structure, also known as a self-referential structure, is a structure that contains a pointer to a variable of the same structure type. This creates a recursive relationship, allowing the structure to refer to itself.<br>
<h5>Example:</h5>
    
#include<stdio.h>

struct person<br>
{<br>

int id;  <br>
float height;<br>
};<br>

int main()<br>
{<br>
   struct person *personPtr, person1;<br>
    personPtr=&person1;<br>
    printf("Displaying:\n");<br>
    scanf("%d%f",&personPtr->id,&personPtr->height);<br>
    printf("id: %d\nheight: %f",personPtr->id,personPtr->height);<br>
}<br>
  </td>
</tr>
<tr>
  <td>QA405</td>
  <td>
    <h5>Compare the Single Linked List and Double Linked List.</h5>
    <h4>Ans:</h4> 
• Single Linked List: Contains nodes with data and a single link pointing to the next node. Nodes cannot be accessed from the end.<br>
• Double Linked List: Contains nodes with data, a link to the next node, and a link to the previous node. Access is possible from both ends.
  </td>
</tr>
<tr>
  <td>QA406</td>
  <td>
    <h5>Define union with an example</h5>
    <h4>Ans:</h4>
    In C programming, a union is a user-defined data type that allows storing different data types in the same memory location, but only one member can hold a value at a time. This means that all members share the same memory space, and the size of the union is equal to the size of its largest member.<br>
    <h5>Example:</h5>
    
#include <stdio.h>

union Data {<br>
   int i;<br>
   float f;<br>
   char str[20];<br>
  };<br>
int main() {<br>
   union Data data;<br>

   data.i = 10; <br>
   printf("Integer value: %d\n", data.i);<br>
   data.f = 3.14; <br>
   printf("Float value: %f\n", data.f);<br>

   strcpy(data.str, "Hello"); <br>
  printf("String value: %s\n", data.str);<br>

  return 0;<br>
  }<br>

  </td>
</tr>
<tr>
  <td>QA407</td>
  <td>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/9488c2f4-7cdf-41e6-8a04-1a88e4b46ea4">
    <h4>Ans:</h4>
    Error

  </td>
</tr>
<tr>
  <td>QA408</td>
  <td>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/f41de59e-05ae-438a-9c51-30893aa434f2">
    <h4>Ans:</h4>
    Error
    
  </td>
</tr>
<tr>
  <td>QA409</td>
  <td>
    <h5>Compare the structure and union.</h5>
    <h4>Ans:</h4>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/4ed19f8e-59b6-4782-a88f-291397010fd5">

  </td>
</tr>
<tr>
  <td>QA410</td>
  <td>
    <h5>Compare structure and self-referenced structure with an example?</h5>
    <h4>Ans:</h4>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/825f971b-363e-4947-a504-2fd819e40f0f">
  </td>
</tr>
<tr>
  <td>QA501</td>
  <td>
    <h5>Write a program to find sum of two fraction values</h5>
    <h4>Ans:</h4>
    <img src:"https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/d83e82a2-da69-4293-a959-81128b14de26">
  </td>
</tr>
</table>

