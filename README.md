# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
# Step 1:
Start the program and import the required libraries.
# Step 2:
Seed the random number generator using the current time(i.e) rand(time(0));
# Step 3:
Get the number of randon number to generate.
# Step 4:
Pass the value for number of iterations and print the numbers.
# Step 5:
End the program.

# PROGRAM:
```
 #include <stdio.h>
 #include <stdlib.h>
 #include <time.h>
 int main()
 {
 int count, min, max;
 printf("Enter the number of random numbers to generate: ");
 scanf("%d", &count);
 printf("Enter the minimum value: ");
 scanf("%d", &min);
 printf("Enter the maximum value: ");
 scanf("%d", &max);
 srand(time(NULL));
 printf("Pseudorandom numbers:\n");
 for (int i = 0; i < count; i++)
{
 int random_number = (rand() % (max- min + 1)) + min;
 printf("%d\n", random_number);
 }
 return 0;
 }
```

# OUTPUT:
![ex 6](https://github.com/user-attachments/assets/59b55bee-1d08-40c4-b8e1-cd9c51e7a784)
# RESULT:
The code was executed sucessfully 
