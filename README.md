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
#include<stdio.h>
int main(){
    int a=44;
    a=a<<3;
    printf("After Left Shift Operation value of a is:%d",a);
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/2e66da95-c216-43c7-a1ec-51305deb588a)









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
#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    if(a==b)
    {
        printf("X is equal to Y");
    }
    else
    {
        printf("X is NOT equal to Y");
    }
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/f4d0708c-b6cd-4b2c-90e1-e10eaf63d062)

           
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
#include<stdio.h>
#include<ctype.h>
int main()
{
    char str[100];
    scanf("%s",str);
    for(int i=0;str[i] != '\0';i++)
    {
        str[i] = tolower(str[i]);
    }
    printf("Lower case String is:%s",str);
    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/e94a357e-474a-469a-88e5-681c96fdb66f)



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
    char str[100];
    int i = 0, count = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);  

    
    do {
        if (str[i] == ' ' || str[i] == '\t') {
            count++;
        }
        i++;
    } while (str[i] != '\0' && str[i] != '\n');  

    if (i == 1 && (str[0] == '\n' || str[0] == '\0')) {
        count = 0;
    } else {
        count++;  
    }

    printf("Total number of words: %d\n", count);

    return 0;
}

```
## OUTPUT

![Screenshot 2025-05-31 094157](https://github.com/user-attachments/assets/f5ce9998-f34a-4815-accf-d623146c4e32)





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
    char c1[100], c2[100];
    int i = 0, flag = 0;

    printf("Enter the first string: ");
    scanf("%[^\n]", c1); 

    getchar(); 

    printf("Enter the second string: ");
    scanf("%s", c2); 

    while (c1[i] != '\0' || c2[i] != '\0') {
        if (c1[i] != c2[i]) {
            flag = 1;
            break;
        }
        i++;
    }

    if (flag == 0)
        printf("Strings are same.\n");
    else
        printf("Strings are not same.\n");

    return 0;
}

```

## OUTPUT
 
![Screenshot 2025-05-31 094437](https://github.com/user-attachments/assets/190f036d-08ee-43a8-9dac-bb59eebc5b67)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

