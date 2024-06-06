# Phase Description (Actual Codes)
## Use Cases
- Code problems
- Large scale projects

## Decription
- This is the **6th phase** in the *Qualine SDLC*.
- It has three sub-phases: **Actual code**, **Testing** & **Debugging**.
- In the first sub-phase *actual code*, we write the actual codes mapped from our pseudo code we wrote in previous phase.
- In the second sub-phase *testing*, we test the code with varying types of values as input.
- And in the third sub-phase *debugging*, we debug the bugs after finding them (if any).
- When working fully digitally, consider storing all *user design* files of various versions in a folder named **"6\) Actual codes"**.

## Factorial Examples
### Actual codes:
#### Final pseudo code (previous phase):
```
ALL HEADERS

FACT(N)             //FACTORIAL FUNCTION
    INT F = 1

    FOR[2,N]I       //SQR BRACKETS MEAN FROM EXACTLY 2 TO N
        F *= I
    
    RETURN F

MAIN FUNCTION
    PRINT("ENTER A NUMBER: ")
    USER INPUT 'N'

    IF N<0:
        PRINT("PLEASE PROVIDE A WHOLE NUMBER!")
        RETURN STATEMENT
    
    ELSE IF N==0:
        PRINT("SO, FACTORIAL = 0")

    PRINT("SO, FACTORIAL = ", FACT(N))
    RETURN STATEMENT
```

#### Mapping pseudo code to actual code:
> NOTE: The code below is written using [GCC compiler](https://gcc.gnu.org/onlinedocs/libstdc++/manual/license.html) (C language).
```
#include <stdio.h>

int fact(int n)
{
    int f = 1;

    for (int i=2; i<=n; i++)
    {
        f *= i;
    }

    return f;
}

int main()
{
    printf("Enter a number: ");
    int n; scanf("%d", &n);

    if (n<0)
    {
        printf("Please provide a whole number!");

        return 0;
    }

    else if (n==0)
    {
        printf("So, factorial = 0");
    }

    printf("So, factorial = %d", fact(n));

    return 0;
}
```
- Well, that was quite easy! Probably because we chose a very easy problem.
- But *Qualine SDLC* made it quite smoother.
- Now comes **testing** & **debugging**.

### Testing (Test 1):
```
Enter a number: 5
So, factorial = 120
```

### Testing (Test 2):
> Let's check if the conditions are working as expected or not.
```
Enter a number: 0
So, factorial = 0
```

### Testing (Test 3):
> Let's check for the forbidden number as per our code (negative number).
```
Enter a number: -1
Please provide a whole number!
```
- We coded the program to accept numbers only from *semi-positive* set.
- Our code passed all test cases, doesn't look like we need any debugging.

## Note
To know how to use it in large scale projects, you will be seeing them in a future project soon, link would be provided here.
