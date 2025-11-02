# EX-NO-6-Pseudo-Random-Number

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

int main() {
    int i, n, min, max;

    srand(time(NULL));

    printf("Enter how many random numbers to generate: ");
    scanf("%d", &n);

    printf("Enter minimum value: ");
    scanf("%d", &min);

    printf("Enter maximum value: ");
    scanf("%d", &max);

    printf("Random numbers between %d and %d:\n", min, max);
    for (i = 0; i < n; i++) {
        int r = min + rand() % (max - min + 1);
        printf("%d\n", r);
    }

    return 0;
}

```
# OUTPUT:
<img width="415" height="214" alt="image" src="https://github.com/user-attachments/assets/eadcce3b-ae18-4a1d-96ad-2d23a017553a" />


# RESULT:
Thus the Pseudo random number was generated successfully.
