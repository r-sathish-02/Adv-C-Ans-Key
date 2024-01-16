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
    Ravikumar 4202500

  </td>
</tr>
<tr>
  <td>QA408</td>
  <td>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/f41de59e-05ae-438a-9c51-30893aa434f2">
    <h4>Ans:</h4>
    101 e
    
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
    
#include <stdio.h>

int main() {<br>
    int numerator1, denominator1, numerator2, denominator2, resultNumerator, resultDenominator;

    // Input for the first fraction
    printf("Enter the numerator and denominator of the first fraction separated by space: ");
    scanf("%d %d", &numerator1, &denominator1);

    // Input for the second fraction
    printf("Enter the numerator and denominator of the second fraction separated by space: ");
    scanf("%d %d", &numerator2, &denominator2);

    // Check if denominators are not zero
    if (denominator1 == 0 || denominator2 == 0) {
        printf("Error: Denominator cannot be zero.\n");
        return 1; // Exit with an error code
    }

    // Calculate the sum of the fractions
    resultNumerator = numerator1 * denominator2 + numerator2 * denominator1;
    resultDenominator = denominator1 * denominator2;

    // Output the result
    printf("The sum of the fractions %d/%d and %d/%d is: %d/%d\n",
           numerator1, denominator1, numerator2, denominator2, resultNumerator, resultDenominator);

    return 0; 
}

  </td>
</tr>
<tr>
  <td>
    QA502
  </td>
  <td>
    <h5>Write a program to find the ASCII value of character ‘R’ ?</h5>
    <h4>Ans:</h4>

#include <stdio.h>

int main() {<br>
   char character = 'R';<br>
  int ascii_value = character; <br> 

   printf("The ASCII value of '%c' is %d\n", character, ascii_value);<br>

   return 0;<br>
  }<br>

  </td>
</tr>
<tr>
  <td>QA503</td>
  <td>
    <h5>Define Conditional Operator with an example?</h5>
    <h4>Ans:</h4>
The conditional operator (also known as the ternary operator) is a concise way to express an if-else statement in a single line of code. It's often used to assign a value to a variable based on a condition.<br>

•syntax:<br>

condition ? expression1 : expression2<br>

•Example:<br>

int age = 25;<br>
char *category = (age >= 18) ? "Adult" : "Minor";<br>
printf("You are categorized as: %s\n", category);  <br>
  </td>
</tr>
<tr>
  <td>QA504</td>
  <td>
    <h5>Write a C program to search an element in an array ?</h5>
    <h4>Ans:</h4>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/2464d1d8-0440-480a-8c3d-8f37371e278b">

  </td>
</tr>
<tr>
  <td>QA505</td>
  <td>
    <h5>Write the difference between argc and argv arguments in main()</h5>
    <h4>Ans:</h4>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/d803d367-68c6-49a6-99f5-ac0093568710">
    
  </td>
</tr>
<tr>
  <td>QA506</td>
  <td>
    <h5>write a c program to copy a  string  into another string without using strcpy() using for loop.</h5>
    <h4>Ans:</h4>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/dba67b4a-a9b6-4cc6-a4d2-a9d15d664cbf">

  </td>
</tr>
<tr>
  <td>QA507</td>
  <td>
    write a Program to compare two strings without using strcmp(). <br>
input: saveetha cse <br>
output: strings are not same<br>
    <h4>Ans:</h4>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/f8e9bae3-a1b4-40ba-94e5-5cd12b5068cd">
  </td>
</tr>
<tr>
  <td>QA508</td>
  <td>
    write a Program To Convert The String 'Saveetha' To Uppercase<br>
Output: Upper Case String Is :SAVEETHA<br>
    <h4>Ans:</h4>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/451c6e01-17dc-4196-a833-fa51274e43ce">

  </td>
</tr>
<tr>
  <td>QA509</td>
  <td>
    write a Program To Convert The String 'SAVEETHA' To Lowercase <br>
Output: Lower Case String Is :saveetha<br>
    <h4>Ans:</h4>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/8c69afb0-1842-45b0-9ecc-efc55c53bf48">

  </td>
</tr>
<tr>
  <td>QA510</td>
  <td>
    <h5>write a program to find the ASCII value of *.</h5>
    <h4>Ans:</h4>
    <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/13a8264a-8771-4e5f-b161-821fa1441ae7">

  </td>
</tr>
</table>

<div align='center'>
  
  ## PART-B
  </div>
<table>
  <tr>
    <td>QB101 (b)</td>
    <td>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/8ab7c51c-6fe3-4a47-87f5-a04efeb11e3a">
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/0f3cf5c7-e1c4-4aef-bcd9-6578cf808508">

   </td>
  </tr>
  <tr>
    <td>QB102 (b)</td>
    <td>
      <h5>Write a C program to calculate the area of a square(side*side) and perimeter of a square(4*side)</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/0f908f7b-15f3-430c-af72-09812e630271">

 </td>
  </tr>
  <tr>
    <td>QB103 (a)</td>
    <td>
      <h5>Build a C program to print leap years in given range from 1900 to 1999?</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/8e4f476b-970e-4174-a1db-75076838edca">

   </td>
  </tr>
  <tr>
    <td>QB104 (a)</td>
    <td>
      <h5>Write a C program to read the student marks and print the which class he/she got? marks>=70 print FIRST CLASS WITH DISTINCTION 60>= marks <70 print FIRST CLASS 50>= marks <60 print SECOND CLASS 40>= marks <50 print THIRD CLASS marks<40 print U r Failed...Better luck next time</h5>
        <h4>Ans:</h4>
        <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/c422e93f-87d3-408e-93d4-580bacfa744e">

   </td>
        
  </tr>
  <tr>
    <td>QB105 (a)</td>
    <td>
      <h5>Write a C program to input number from the user and check whether the number is even or odd using a SWITCH CASE.</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/d7f969e6-9a60-4f14-85fd-403ba837d843">

  </td>
  </tr>
  <tr>
    <td>QB201 (b)</td>
    <td>
      <h5>Write Program to print odd numbers in reverse order, range from M to N (including M and N values) using functions.</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/d2449f83-c0be-4fcf-bf8d-f51adf01552b">

 </td>
  </tr>
  <tr>
    <td>QB202 (a)</td>
    <td>
      <h5>Write  a C program to swap two numbers using pointers without using 3rd variable ?.</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/8368c547-a615-44b4-be33-28b7fc71ad46">

</td>
  </tr>
  <tr>
    <td>QB203 (b)</td>
    <td>
      <h5>Write a C program to display the factorial of a number using recursive function</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/0fb43c07-8866-4a6c-b9b1-71c0c81f954a">
    </td>
  </tr>
  <tr>
    <td>QB204 (a)</td>
    <td>
      <h5>Write a C program for Multiplication and Division of two numbers using functions (Without argument and with return type)</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/fc11c801-8b39-4fc2-8dfb-84643c1a1826">
    </td>
  </tr>
  <tr>
    <td>QB205 (a)</td>
    <td>
      <h5>Write a C program for finding the factorial of a given number using function without return type with arguments.</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/8dff20a5-8bf9-4ea7-9da1-e637c58e0168">

  </td>
  </tr>
  <tr>
    <td>QB301 (a)</td>
    <td>
      <h5>Write a C Program to find largest and second largest elements in the given array Using sorting. </h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/60c66b9a-dd73-4983-b017-c310da4edce3">
   </td>
  </tr>
  <tr>
    <td>QB302 (a)</td>
    <td>
      <h5>Write a C Program to get the 6 subject marks from the user using array and display the average of the student in float. Also write the output for this program.</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/42c372d2-af66-4ae5-a24a-af61e5dca2bd">

  </td>
  </tr>
  <tr>
    <td>QB303 (a)</td>
    <td>
      Write a C Program to arrange the following values 16, 14, 21, 61, 22 in ascending order using bubble sorting technique.<br>
Before bubble sorting the elements are:<br>
16 14 21 61 22 <br>
After bubble sorting the elements are:<br>
14 16 21 22 61<br>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/6e37fff0-697f-4ca3-b97f-20286f3e39a4">

</td>
  </tr>
  <tr>
    <td>QB304 (a)</td>
    <td>
      <h5>Create  a C program to read n elements as input and print the elements of an array present on odd position</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/3ec17ff5-c739-45c0-9999-35e315607b09">

 </td>
  </tr>
  <tr>
    <td>QB305 (a)</td>
    <td>
      <h5>Write  a C program to read the elements of the n x n matrix and print the last element of the matrix</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/047a3cb2-bc10-42d3-8889-e9c2736cd9a6">
 </td>
  </tr>
  <tr>
    <td>QB401 (a)</td>
    <td>
      <h5>Build a C Program for Single Linked List with Create () and DisplayReverse () operations.</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/211fb522-3bad-40f6-b419-2dd23a53768d">

</td>
  </tr>
  <tr>
    <td>QB402 (a)</td>
    <td>
      <h5>Create a C Program for Single Linked List with Delete () and Display () operations.</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/9af93c75-5983-43bb-af21-c8f61d52e6f0">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/aab87e37-42bc-4f00-84a8-0c124d33bd6a">


 </td>
  </tr>
  <tr>
    <td>QB403 (b)</td>
    <td>
      <h5>Implement a C Program for Double Linked List with Delete () and Display () operations.</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/3f655a9a-9a68-4f54-9d48-eca4ad0e8ada"><br>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/bb84a0ee-0dc5-40d9-a0ec-2d4411eff4be">

 </td>
  </tr>
  <tr>
    <td>QB404 (b)</td>
    <td>
      <h5>Build a C Program for Single Linked List with all operations</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/47db3c14-beff-4de2-856a-ed7b145657b1">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/be082867-cec3-474a-b815-ebd2515cf0fe">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/a50aca8b-df77-4910-9af5-ec5638c1cfe9">
  </td>
  </tr>
  <tr>
    <td>QB405 (b)</td>
    <td>
      <h5>Build a C Program for Double Linked List with all operations</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/ba202e21-cfeb-4648-8cd6-952f0de8e7c9">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/c8a55de7-892a-4818-b146-c0248f5d8430">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/9a1f363c-03c1-44d3-8888-c1ca8cc5705a">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/9f57d845-84ab-4109-af1e-553a39ec0d4d">

  </td>
  </tr>
  <tr>
    <td>QB501 (b)</td>
    <td>
      <h5>Write a C program to read temperature in centigrade and display a suitable message according to temperature state below : Temp < 0 then Freezing weather, Temp 0-20 then Very Cold weather, Temp 20-30 then Cold weather, Temp 30-40 then Normal in Temp, Temp 40-50 then Its Hot, Temp >=50 then Its Very Hot</h5>
        <h4>Ans:</h4>
        <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/a1bf6b3e-1666-4b62-9913-07dcd88c8035">

 </td>
  </tr>
  <tr>
    <td>QB502 (a)</td>
    <td>
      <h5>Write a C program to read the wind speed in kph and display a suitable message according to the wind speed state below.(use ELSE-IF ladder) * Strong breeze at 39-49 kph (25-31 mph)  * Moderate gale at 50-61 kph (32-38 mph)  * Fresh gale at 62-74 kph (39-46 mph)  * Strong gale at < 98 kph</h5>
        <h4>Ans:</h4>
        <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/9bcb6981-26dc-4c3c-b0eb-ab15ec4c1fe0">

   </td>
  </tr>
  <tr>
    <td>QB503 (a)</td>
    <td>
      <h5>Write a c program to count total number of negative elements in an array</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/ff2b7030-c544-4f1f-a515-511eb97a17da">

  </td>
  </tr>
  <tr>
    <td>QB504 (b)</td>
    <td>
      <h5>Write a C Program to take two numbers as input from the user and then calculating the following with nested if statement. 1. check whether the number are equal or not. 2.  find the largest of two numbers</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/6fa71b7f-ab3c-48f0-b7a6-df59fa0e3699">
  </td>
  </tr>
  <tr>
    <td>QB505 (a)</td>
    <td>
      <h5>Write  a C program to read the elements of the n x n matrix and print the elements of last row of the matrix</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/fcc2f209-7b4f-4414-b1fd-82630099f8b4">
</td>
    
  </tr>
</table>

<div align='center'>
  
  ## PART-C
  </div>

  <table>
    <tr>
      <td>QC101 (b)</td>
      <td>
        Develop a C program to check whether a number is palindrome or not<br>
Sample input: 3223<br>
Sample output: 3223 is a palindrome<br><br>

Sample input: 1234<br>
Sample output: 4321 is not a palindrome<br>
<h4>Ans:</h4>
<img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/c3c3ae26-ed01-4501-a52c-3bc4a10914a3">

 </td>
    </tr>
    <tr>
      <td>QC102 (a)</td>
      <td>
        <h5>Write a C program to read temperature in centigrade and display a suitable message according to temperature state below : Temp < 0 then Freezing weather Temp 0-10 then Very Cold weather Temp 10-20 then Cold weather Temp 20-30 then Normal in Temp Temp 30-40 then Its Hot Temp >=40 then Its Very Hot</h5>
          <h4>Ans:</h4>
          <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/d78045e8-fcea-4dea-815c-3a39e51bbf0c">

</td>
  <tr>
    <td>QC201 (a)</td>
    <td>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/f3f40d46-a440-4d49-a4f6-b382608e6a23">
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/c9a7cbbf-a247-4ba8-ba45-6fdae3d8aeea">

</td>
  </tr>
  <tr>
    <td>QC202 (a)</td>
    <td>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/c504fb56-a3f1-4e15-9cf9-61cf8c5f79da">
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/bd7025c7-7cd4-4d57-8d5f-ae09344d04c8">

</td>
  </tr>
  <tr>
    <td>QC301 (a)</td>
    <td>
      <h5>Construct a program in C for Bubble Sort Technique using Arrays and explain the Sorting technique with example.</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/7964a893-04c1-48eb-899e-12f7843f2f69">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/2a2105a2-833b-47c8-8666-56fdb7b3fd6d">
</td>
  </tr>
  <tr>
    <td>QC302 (a)</td>
    <td>
      <h5>Write  a C program to read the elements of the n x n matrix and print the diagonal elements of the matrix</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/a6e70138-6843-4455-a0d1-b5eeb51a0148">
    
</td>
  </tr>
  <tr>
    <td>QC401 (b)</td>
    <td>
      <h5>Implement a C Program for Single Linked List with Create (), Insert (), Search () and Display () operations.</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/47db3c14-beff-4de2-856a-ed7b145657b1">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/be082867-cec3-474a-b815-ebd2515cf0fe">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/a50aca8b-df77-4910-9af5-ec5638c1cfe9">
</td>
  </tr>
  <tr>
    <td>QC402 (b)</td>
    <td>
      <h5>Implement a C Program for Double Linked List with Create (), Insert (), Search () and Display () operations.</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/ba202e21-cfeb-4648-8cd6-952f0de8e7c9">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/c8a55de7-892a-4818-b146-c0248f5d8430">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/9a1f363c-03c1-44d3-8888-c1ca8cc5705a">
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/9f57d845-84ab-4109-af1e-553a39ec0d4d">
   </td>
  </tr>
  <tr>
    <td>QC501 (b)</td>
    <td>
      C program to find sum of each row of a matrix please enter number of rows and columns : 3 3 <br>
Input elements of matrix: {1 2 3}   { 4 5 6}    { 7 8 9} <br>
Output: The Sum of Elements of a Rows in a Matrix:  6<br> The Sum of Elements of a Rows in a Matrix:  15<br> The Sum of Elements of a Rows in a Matrix:  24<br>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/da55b88d-e2eb-49e5-bbca-02d2a971b899">

  </td>
  </tr>
  <tr>
    <td>QC502 (a)</td>
    <td>
      <h5>Write  a C program to read the elements of the n x n matrix and check whether the diagonal elements of the matrix is divisible by 3</h5>
      <h4>Ans:</h4>
      <img src="https://github.com/r-sathish-02/Adv-C-Ans-Key/assets/118787261/f5e0b975-9370-4df4-83de-b780a87597c2">

  </td>
  </tr>
  </table>
