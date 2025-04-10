# EX-NO-6-Pseudo-Random-Number
## AIM:
Implementation of Pseudorandom Number Generation Using Standard library

## ALGORITHM:
Start the program and import the required libraries. Seed the random number generator using the current time(i.e) rand(time(0)); Get the number of randon number to generate. Pass the value for number of iterations and print the numbers. End the program.

## PROGRAM:
```
#include <stdio.h>

// LCG Constants
#define MULTIPLIER 1664525
#define INCREMENT 1013904223
#define MODULUS 4294967296 // 2^32

unsigned int seed = 1; // You can change this seed value

// Function to generate pseudo-random number
unsigned int pseudo_random() {
    seed = (MULTIPLIER * seed + INCREMENT) % MODULUS;
    return seed;
}

int main() {
    // Generate 10 pseudo-random numbers
    for (int i = 0; i < 10; i++) {
        printf("%u\n", pseudo_random());
    }
    return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/b29f2f9b-1f8f-422d-a4cd-9eebdd671fe4)

## RESULT:
The program for Pseudorandom Number Generation is executed successfully
