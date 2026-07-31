# EX-NO-6-Pseudo-Random-Number
# NAME: P.S.SABARI
# REG.NO: 212225040352
# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
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
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }return 0;
    
}
```

# OUTPUT:
<img width="1918" height="650" alt="Screenshot 2026-07-31 113208" src="https://github.com/user-attachments/assets/9ae175bc-5beb-4c88-a4d1-882f8d799fe6" />

# RESULT:
 Thus,Pseudorandom Number Generation Using Standard library is implemented successfully.
