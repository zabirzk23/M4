# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int a = 44, b = 3, c;
    c = a << b;
    printf("%d", c);
    return 0;
}
```
## OUTPUT

![Screenshot 2025-05-17 143449](https://github.com/user-attachments/assets/94f7fd3d-c120-4600-9d4a-481be862d6b2)


## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int a, b;
    scanf("%d%d", &a, &b);
    if(a == b)
        printf("Equal");
    else
        printf("Not Equal");
    return 0;
}
```

## OUTPUT

![Screenshot 2025-05-17 143648](https://github.com/user-attachments/assets/1154b0a0-1ae1-4ae8-a2ad-1af8a398e60b)

![Screenshot 2025-05-17 143706](https://github.com/user-attachments/assets/2b606373-67f4-4df1-81db-1f9519c258d4)


## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM

```

#include <stdio.h>
#include <ctype.h>

int main() {
    char s[100];
    int i;
    scanf("%s", s);
    for(i = 0; s[i] != '\0'; i++)
        s[i] = tolower(s[i]);
    printf("%s", s);
    return 0;
}

```

## OUTPUT

![Screenshot 2025-05-17 143947](https://github.com/user-attachments/assets/3755031e-fbd8-406a-9277-341814a21a25)


## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM

```

#include <stdio.h>

int main() {
    char s[100];
    int i = 0, c = 1;
    fgets(s, sizeof(s), stdin);
    do {
        if(s[i] == ' ' && s[i+1] != ' ' && s[i+1] != '\0' && s[i+1] != '\n')
            c++;
        i++;
    } while(s[i] != '\0' && s[i] != '\n');
    printf("%d", c);
    return 0;
}

```

## OUTPUT

![Screenshot 2025-05-17 144342](https://github.com/user-attachments/assets/05e93dfe-c565-475c-ab98-cc668c69d7e7)


## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM

```

#include <stdio.h>

int main() {
    char s1[100], s2[100];
    int i = 0, f = 0;
    fgets(s1, sizeof(s1), stdin);
    fgets(s2, sizeof(s2), stdin);
    while(s1[i] != '\0' && s2[i] != '\0') {
        if(s1[i] != s2[i]) {
            f = 1;
            break;
        }
        i++;
    }
    if(f == 0 && s1[i] == s2[i])
        printf("strings are same");
    else
        printf("strings are not same");
    return 0;
}

```

## OUTPUT

 ![Screenshot 2025-05-17 144538](https://github.com/user-attachments/assets/f695ad10-59c9-4dd0-be35-ec745d8a71ac)
 
![Screenshot 2025-05-17 144605](https://github.com/user-attachments/assets/d6295776-235d-4e6a-be89-bf0f3f2e89a1)




## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

