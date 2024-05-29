# Phase Description (Pseudo Codes)
## Use Cases
- Code problems
- Large scale projects

## Decription
- This is the **5th phase** in the *Qualine SDLC*.
- It has two sub-phases: **Pseudo codes** & **Algorithm improvement**.
- For various parts of the code, separate pseudo code files must be kept instead stuffing all into one.
- Though this tip can be ignored when working on small code problems.
- Keep them in a *.txt* file, because just like terminals, most text editers don't have syntax designing features.
- Later on after writing the pseudo code, we will **rewrite** it if we detect some potential bottlenecks.
- When working fully digitally, consider storing all *user design* files of various versions in a folder named **"5\) Pseudo codes"**.

## Factorial Example
### Pseudo code:

```
ALL HEADERS

FACT(N)             //FACTORIAL FUNCTION
    IF N>=1:
        RETURN (N*FACT(N-1))
    
    ELSE IF N==1:
        RETURN 1

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
- There is no hard rules to write pseudo codes, its up to the individual or their organization's standards.
- Same about the programming language.
- I personally write them completely in **UPPERCASE** in order to show them different from *actual codes*.
- And I will be using [GCC compiler](https://gcc.gnu.org/onlinedocs/libstdc++/manual/license.html) for this work.

> For our example, we noticed a bottleneck issue i.e. a *bad space complexity*.
> So, in order to solve it we can use a 
**loop** instead to save space on stack memory.

`Rewriting the pseudo code:`
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
- The procedures to detect & fix performance issues may vary.
- Larger projects can use proper methods like study of graph to analyse performance along with time & space complexity.

## Note
To know how to use it in large scale projects, you will be seeing them in a future project soon, link would be provided here.