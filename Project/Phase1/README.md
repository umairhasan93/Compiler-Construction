The language specifications for Mini C can be found here:  
1- http://compilersatkiet.22web.org/lang(2).pdf?i=1  
2- http://www2.cs.arizona.edu/~debray/Teaching/CSc453/DOCS/cminusminusspec.html  
3- https://www.ibm.com/docs/en/xl-c-and-cpp-aix/13.1.0?topic=statements-statement
# Example Code For our Project  
## Simple if (nesting not allowed)  
if (number >= 0)
   printf("Number is positive\n");
else
   printf("Number is negative\n");


## Switch Statement (nesting not allowed)  
char key;

printf("Enter an arithmetic operator\n");
scanf("%c",&key);

switch (key)
{
   case '+':
      add();
      break;

   case '-':
      subtract();
      break;

   case '*':
      multiply();
      break;

   case '/':
      divide();
      break;

   default:
      printf("invalid key\n");
      break;
}

## Repetition Statement (nesting not allowed)  
A. Repeat  
        Until ()  
B. int count = 1;
   while (count <= 20)
  {
     printf("count = %d\n", count);
     count++;
  }  
C. int count;
   for (count = 1; count <= 20; count++)
   printf("count = %d\n", count);

## I/O Statement  
#include <stdio.h>
  
int main()
{

    char str[50];


    printf("Enter the Word: ");
    scanf("%s\n", str);
  
    printf("\nEntered Word is: %s", str);
  

    printf("\n\nEnter the Sentence: ");
    scanf("%[^\n]\ns", str);
  
    printf("\nEntered Sentence is: %s", str);
  
    return 0;
}

## Program Structure  
Decleration:  
Start  
End


