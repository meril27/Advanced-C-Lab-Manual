## EXP NO:6 C PROGRAM PRINT THE LOWERCASE ENGLISH WORD CORRESPONDING TO THE NUMBER
## Aim:
To write a C program print the lowercase English word corresponding to the number
## Algorithm:
1.	Start
- Initialize an integer variable n.
2.	Input Validation
3.	Switch Statement cases.
-	Case 5: Print "seventy one"
-	Case 6: Print "seventy two"
-	Case 13: Print "seventy three"
-	...
-	Case 13: Print "seventy nine"
-	Default: Print "Greater than 13"
4.	Exit the program.
 
## Program:

```c
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    switch(n)
    {
        case 21:
        printf("twenty one");
        break;
        
        case 22:
        printf("twenty two");
        break;
        
        case 23:
        printf("twenty three");
        break;
        
        case 24:
        printf("twenty four");
        break;
        
        case 25:
        printf("twenty five");
        break;
        
        case 26:
        printf("twenty six");
        break;
        
        case 27:
        printf("twenty seven");
        break;
        
        case 28:
        printf("twenty eight");
        break;
        
        case 29:
        printf("twenty nine");
        break;
        
        default:
        printf("Greater than 29");
        break;
    }
}
```


## Output:

<img width="1181" height="347" alt="image" src="https://github.com/user-attachments/assets/7be28240-3b3a-4a83-85bf-0259bcab32bf" />



## Result:
Thus, the program is verified successfully
 
## EXP NO:7 C PROGRAM TO PRINT TEN SPACE-SEPARATED INTEGERS     IN A SINGLE  LINE DENOTING THE FREQUENCY OF EACH DIGIT FROM 0 TO 3 .
## Aim:
To write a C program to print ten space-separated integers in a single line denoting the frequency of each digit from 0 to 3.
## Algorithm:
1.	Start
2.	Declare char array a[50] outer loop for each digit from 0 to 3
3.	Initialize counter c to 0
4.	For each character in the string print count c for current digit, followed by a space
5.	Increment h to move to the next digit
6.	End
 
## Program:

```c
#include<stdio.h>
int main()
{
    char str[50];
    int array[20]={0};
    scanf("%s",str);
    for(int i=0; str[i]!='\0'; i++)
    {
        if(str[i]>='0' && str[i]<='3')
        {
            array[str[i]-'0']++;
        }
    }
    for(int i=0; i<4; i++)
    {
        printf("%d ",array[i]);
    }
    return 0;
}
```

## Output:

<img width="1182" height="307" alt="Screenshot 2026-09-17 105319" src="https://github.com/user-attachments/assets/fd5d4970-d9d1-4f98-a861-3e020c414b7a" />

## Result:
Thus, the program is verified successfully

## EXP NO:8 C PROGRAM TO PRINT ALL OF ITS PERMUTATIONS IN STRICT LEXICOGRAPHICAL ORDER.
## Aim:
To write a C program to print all of its permutations in strict lexicographical order.

## Algorithm:
1.	Start
2.	Declare variables s (pointer to an array of strings) and n (number of strings)
3.	Memory Allocation
Dynamically allocate memory for s to store an array of strings
4.	Input
Read the number of strings n from the user Dynamically allocate memory for each string in s
5.	Permutation Generation Loop
6.	Memory Deallocation
Free the memory allocated for each string in s Free the memory allocated for s
7.	End
 
## Program:

```c
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    char arr[50][50];
    for(int i=0;i<n;i++)
    {
        scanf("%s",arr[i]);
    }
    if(n==2)
    {
        printf("%s %s\n",arr[0],arr[1]);
        printf("%s %s",arr[1],arr[0]);
    }
    else
    {
        for(int i=0;i<n;i++)
        {
            for(int j=0;j<n;j++)
            {
                for(int k=0;k<n;k++)
                {
                    if(i!=j && j!=k && k!=i)
                    {
                        printf("%s %s %s\n",arr[i],arr[j],arr[k]);
                    }
                }
            }
        }
    }
}
```

## Output:

<img width="1185" height="471" alt="image" src="https://github.com/user-attachments/assets/3aaee18f-6e53-4c55-80d3-b7a1979801f8" />

## Result:
Thus, the program is verified successfully
 
## EXP NO:9 C PROGRAM PRINT A PATTERN OF NUMBERS FROM 1 TO N AS
SHOWN BELOW.
## Aim:
To write a C program to print a pattern of numbers from 1 to n as shown below.
Algorithm:
1.	Start
2.	Declare integer variables n, i, j, min
3.	Read the value of n from the user
4.	Calculate the length of the side of the square matrix: len = n * 2 - 1
5.	Matrix Generation Loop
6.	Calculate min as the minimum distance to the borders
7.	End
 
## Program:

```c
#include<stdio.h>
int main()
{
    int n,min1, min2, minf;
    scanf("%d",&n);
    int s=2*n-1;
    for(int i=0; i<s; i++)
    {
        for(int j=0; j<s; j++)
        {
            if(i<j)
            {
                min1=i;
            }
            else
            {
                min1=j;    
            }
            if((s-1-i)<(s-1-j))
            {
                min2=s-1-i;
            }
            else
            {
                min2=s-1-j;
            }
            if(min1<min2)
            {
                minf=min1;
            }
            else
            {
                minf=min2;
            }
            int num=n-minf;
            printf("%d ",num);
        }
        printf("\n");
    }   
}
```


## Output:

<img width="1252" height="960" alt="image" src="https://github.com/user-attachments/assets/cf463fae-770d-4e81-9571-0381df417628" />


## Result:
Thus, the program is verified successfully

## EXP NO:10 C PROGRAM TO FIND A SQUARE  OF NUMBER USING FUNCTION WITHOUT ARGUMENTS WITH RETURN TYPE

## Aim:

To write a C program that calculates the square of a number using a function that does not take any arguments, but returns the square of the number.

## Algorithm:

1.	Start.
2.	Define a function square() with no parameters. This function will return an integer value.
3.	Inside the function:
o	Declare an integer variable to store the number.
o	Ask the user to input a number.
o	Calculate the square of the number (multiply the number by itself).
o	Return the squared value.
4.	In the main function:
o	Call the square() function and display the result.
5.	End.

## Program:

```c
  #include <stdio.h>
  void square();
  int main()
{
      square();
      return 0;
  }
  void square(){
      int a;
      scanf("%d",&a);
      float ans = a*a;
      printf("The square of %d is : %.2f",a,ans);
  }

```

## Output:

<img width="938" height="301" alt="image" src="https://github.com/user-attachments/assets/735370f5-b9d3-46d1-84d8-cc7829b721dd" />




## Result:
Thus, the program is verified successfully

