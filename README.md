# PPSassignment

# (1) Write a program to add two numbers.

    #include<stdio.h>
    int main()
    {
        int a, b, sum;
        printf("Enter the first number: ");
        scanf("%d",&a);
        printf("Enter the second number: ");
        scanf("%d",&b);
        sum = a+b;
        printf("Sum of two numbers= %d",sum);    
        return 0;
    }
    
#### INPUT:
    Enter the first number: 2
    Enter the second number: 3
#### OUTPUT: 
    Sum of two numbers= 5


# (2) Write a program to find the average of'n' numbers.

    #include<stdio.h>
    int main()
    {
        int n, b, i;
        float sum=0, x, average;
        printf("Enter the number of digits whose average is to be calculated: ");
        scanf("%d",&n);
        printf("\nEnter %d digits: ",n);
        for(i=1; i<=n; i++)
         {
            scanf("%f",&x);
            sum=sum+x;
         }
        average=sum/n;
        printf("\nAverage of %d digits: %.2f\n",n, average);    
        return 0;
    } 

#### INPUT:
    Enter the number of digits whose average is to be calculated: 4
    
    Enter 4 digits: 1 2 3 4
#### OUTPUT:
    Average of 4 digits: 2.50
    
    
# (3) Write a program to print the weekdays using switch statement.

    #include<stdio.h>
    int main()
    {  
        int code;
        printf("Enter weekdays in number: ");
        scanf("%d",&code);
        if(code==1)
            printf("MONDAY");
        else if(code==2)
            printf("TUESDAY");
        else if(code==3)
            printf("WEDNESDAY");
        else if(code==4)
            printf("THURSDAY");
        else if(code==5)
            printf("FRIDAY");
        else if(code==6)
            printf("SATURDAY");
        else if(code==7)
            printf("SUNDAY");
        else
            printf("Invalid Output");        
        return 0;        
    } 

#### INPUT: 
    Case 1: Enter weekdays in number: 3
    Case 2: Enter weekdays in number: 10
#### OUTPUT:
    Case 1: WEDNESDAY
    Case 2: Invalid Output
    

# (4) Write a program to find whether the number is even or odd.

    #include<stdio.h>
    int main()
    {
        int a;
        printf("Enter a number: ");
        scanf("%d",&a);
        if(a%2==0)
          printf("%d is EVEN",a);
        else
          printf("%d is ODD",a);    
        return 0;        
    }

#### INPUT:
    Case 1: Enter a number: 2
    Case 2: Enter a number: 987
#### OUTPUT: 
    Case 1: 2 is EVEN
    Case 2: 987 is ODD   
    
# (5) Write a program to print a table using for loop.

    #include<stdio.h>
    int main()
    {       
        int i,n, mul;
        printf("Enter the number: ");
        scanf("%d",&n);
        for(i=0;i<=20;i++)
         {
            mul=n*i;
            printf("%d * %d = %d\n", n,i,mul);
         }     
        return 0;
    }

#### INPUT:
    Enter the number: 197
    
#### OUTPUT:
    197 * 0 = 0
    197 * 1 = 197
    197 * 2 = 394
    197 * 3 = 591
    197 * 4 = 788
    197 * 5 = 985
    197 * 6 = 1182
    197 * 7 = 1379
    197 * 8 = 1576
    197 * 9 = 1773
    197 * 10 = 1970
    197 * 11 = 2167
    197 * 12 = 2364
    197 * 13 = 2561
    197 * 14 = 2758
    197 * 15 = 2955
    197 * 16 = 3152
    197 * 17 = 3349
    197 * 18 = 3546
    197 * 19 = 3743
    197 * 20 = 3940


# (6) Write a program to check whether the number is an armstrong number or not.

    #include <stdio.h>    
    #include <math.h>
    int main()
    {      
        int num, sum=0, r, n;
        printf("\nEnter the number: ");
        scanf("%d",&num);
        n=num;
        while(n>0)
         {
            r=n%10;
            sum+=(r*r*r);
            n=n/10;
         }
        if(sum==num)
          printf("\n%d is an armstrong number\n",num);
        else
          printf("\n%d is not an armstrong number\n",num);    
        return 0;
    }

#### INPUT:
    Enter the number: 153

#### OUTPUT:
    153 is an armstrong number

# (7) Write a program to print calculator using puts.

    #include <stdio.h>
    int main()
    {
        puts(" _______________");
        puts("|               | ");
        puts("|_______________| ");
        puts("| 1 | 2 | 3 |   | ");
        puts("|___|___|___|   | ");
        puts("| 4 | 5 | 6 | + | ");
        puts("|___|___|___|___| ");
        puts("| 7 | 8 | 9 | - | ");
        puts("|___|___|___|___| ");
        puts("|    0      | * | ");
        puts("|___________|___| ");    
        return 0;
    }

#### OUTPUT:
 _______________
|               | 
|_______________| 
| 1 | 2 | 3 |   | 
|___|___|___|   | 
| 4 | 5 | 6 | + | 
|___|___|___|___| 
| 7 | 8 | 9 | - | 
|___|___|___|___| 
|    0      | * | 
|___________|___| 


# (8) Write a program for bubble sort.

    #include<stdio.h>
    #include<math.h>
    int main()
    {
        int a[20], i, n, k, temp;
        printf("\nEnter the size of array: ");
        scanf("%d",&n);
        printf("\nEnter %d elements of array: ",n);
        for(i=0; i<n; i++)
         scanf("%d",&a[i]);
        for(k=0; k<n-1; k++)
         {
            for(i=0; i<n-k-1; i++)
             {
                if(a[i]>a[i+1])
                 {
                    temp = a[i];
                    a[i] = a[i+1];
                    a[i+1] = temp;
                 }
             }
         }
        printf("\nArray elements after sorting:\n ");
        for(i=0; i<n; i++)
         printf("%d\n",a[i]);    
        return 0;
    }

#### INPUT: 
    Enter the size of array: 6

    Enter 6 elements of array: 98 45 67 88 107 36 

#### OUTPUT:
    Array elements after sorting:
    36
    45
    67
    88
    98
    107


# (9) Write a program for binary search.

    #include <stdio.h>
    int main()
    {
        int c, first, last, middle, n, search, array[100];
        printf("Enter number of elements: ");
        scanf("%d",&n);
        printf("Enter %d integers: ", n);
        for (c = 0; c < n; c++)
        scanf("%d",&array[c]);
        printf("Enter value to find: ");
        scanf("%d", &search);
        first = 0;
        last = n - 1;
        middle = (first+last)/2;
        while (first <= last) 
         {
           if (array[middle] < search)
             first = middle + 1; 
           else if (array[middle] == search)
            {
              printf("\n%d found at location %d.", search, middle+1);
              break;
            }
        else
        last = middle - 1;
        middle = (first + last)/2;
        }
        if (first > last)
          printf("\nNot found! %d isn't present in the list.\n", search);
        return 0; 
    }

#### INPUT: 
    Enter number of elements: 5
    Enter 5 integers: 1 7 11 57 21
    Enter value to find: 7

#### OUTPUT:
    7 found at location 2.
    
    
# (10) Write a program to find factorial of a number.

    #include <stdio.h>
    int main()
    {
        int fct=1, num, i;
        printf("Enter any number: ");
        scanf("%d",&num);
        if(num==0)
          fct=1;
        else
          {
            for(i=1; i<=num; i++)
            fct=fct*i;
          }
        printf("The facorial of %d is: %d\n",num,fct);    
        return 0;
    }

#### INPUT:
    Enter any number: 5
    
#### OUTPUT:
    The facorial of 5 is: 120


# (11) Write a program for fizz buzz.

    #include<stdio.h>
    int main()
    {
        int i;
        for(i=1; i<=30; i++)
         if(i%15==0)
           printf("FIZZBUZZ\n");
         else if(i%5==0)
           printf("BUZZ\n");
         else if(i%3==0)
           printf("FIZZ\n");
         else
           printf("%d\n",i);
        return 0;
    }

#### OUTPUT:
    1
    2
    FIZZ
    4
    BUZZ
    FIZZ
    7
    8
    FIZZ
    BUZZ
    11
    FIZZ
    13
    14
    FIZZBUZZ
    16
    17
    FIZZ
    19
    BUZZ
    FIZZ
    22
    23
    FIZZ
    BUZZ
    26
    FIZZ
    28
    29
    FIZZBUZZ


# (12) Write a program to find the sum of first 100 numbers.

    #include<stdio.h>
    int main()
    {
        int i,sum=0;
        for(i=1; i<=100; i++)
          sum=sum+i;
        printf("\nSum of first 100 numbers= %d\n", sum);    
        return 0;
    }

#### OUTPUT:
    Sum of first 100 numbers= 5050

# (13) Write a program to find the greater of 2 numbers.

    #include<stdio.h>
    int main()
    {
        int a,b;
        printf("Enter the first number: ");
        scanf("%d",&a);
        printf("Enter the second number: ");
        scanf("%d",&b);
        if(a>b)
          printf("%d is greater.",a);
        else
          printf("%d is greater.",b);    
        return 0;
    }

#### INPUT:
    Enter the first number: 97
    Enter the second number: 25

#### OUTPUT:
    97 is greater.
    
    
# (14) Write a program to find the greater of 3 numbers.

    #include <stdio.h>
    int main()
    {
        int a,b,c;
        printf("Enter the first number: ");
        scanf("%d",&a);
        printf("Enter the second number: ");
        scanf("%d",&b);
        printf("Enter the third number: ");
        scanf("%d",&c);
        if(a>b)
         {
            if(a>c)
            printf("The greater number is: %d\n",a);
            else
            printf("The greater number is: %d\n",c);
         }
        else if(b>c)
          printf("The greater number is: %d\n",b);
        else
          printf("The greater number is: %d\n",c);
        return 0;
    }

#### INPUT:
    Enter the first number: 34
    Enter the second number: 74
    Enter the third number: 2

#### OUTPUT:
    The greater number is: 74

# (15) Write a program to find gcd of two numbers.

    #include <stdio.h>
    int main()
    {
        int num1, num2, dividend, divisor, remainder, quotient;
        printf("Enter any number: ");
        scanf("%d",&num1);
        printf("Enter another number: ");
        scanf("%d",&num2);
        if(num1>num2)
         {
            dividend = num1;
            divisor =  num2;
         }
        else
         {
            dividend = num2;
            divisor = num1;
         }
        while(divisor)
         {
            remainder = dividend % divisor;
            dividend = divisor;
            divisor = remainder;
         }
        printf("\nGCD of %d and %d is= %d\n",num1, num2, dividend);
        return 0;
    }
    
#### OUTPUT:
    Enter any number: 24
    Enter another number: 18
    
#### INPUT:
    GCD of 24 and 18 is= 6
    
    
# (16) Write a program to check whether the year is a leap year or not.

    #include <stdio.h>
    int main()
    {
        int yr;
        printf("Enter any year:");
        scanf("%d",&yr);
        if((yr%4==0) &&((yr%100 !=0) || (yr%400==0)))
          printf("It is a leap year");
        else
          printf("It is not a leap year");    
        return 0;
    }

#### INPUT:
    Enter any year:2018

#### OUTPUT:
    It is not a leap year
    
    
# (17) Write a program for linear search.

    #include <stdio.h>
    int main()
    {
        int array[100], search, c, n;
        printf("Enter number of elements in array: ");
        scanf("%d", &n);
        printf("\nEnter %d integer(s): ", n); 
        for (c = 0; c < n; c++)
         scanf("%d", &array[c]);
        printf("\nEnter a number to search: ");
        scanf("%d", &search);
        for (c = 0; c < n; c++)
         {
            if (array[c] == search)    
             {
                printf("%d is present at location %d.\n", search, c+1);
                break;
             }
         }
        if (c == n)
        printf("%d is not present in the array.\n", search); 
        return 0;
    }

#### INPUT: 
    Enter number of elements in array: 5

    Enter 5 integer(s): 1 2 6 18 99

    Enter a number to search: 6

#### OUTPUT:
    6 is present at location 3.


# (18) Write a program for matrix addition.

    #include <stdio.h>
    int main()
    {
        int m, n, c, d, first[10][10], second[10][10], sum[10][10];
        printf("Enter the number of rows and columns of matrix:\n");
        scanf("%d%d", &m, &n);
        printf("Enter the elements of first matrix:\n");
        for (c = 0; c < m; c++)
        for (d = 0; d < n; d++)
        scanf("%d", &first[c][d]);
        printf("Enter the elements of second matrix:\n");
        for (c = 0; c < m; c++)
        for (d = 0 ; d < n; d++)
        scanf("%d", &second[c][d]);
        printf("Sum of entered matrices:-\n");
        for (c = 0; c < m; c++) 
         {
            for (d = 0 ; d < n; d++) 
             {
                sum[c][d] = first[c][d] + second[c][d];
                printf("%d\t", sum[c][d]);
             }
            printf("\n");
         }
        return 0;
    }

#### INPUT: 
    Enter the number of rows and columns of matrix:
    2 3
    Enter the elements of first matrix:
    1 2 3 4 5 6 
    Enter the elements of second matrix:
    1 2 3 4 5 6

#### OUTPUT:
    Sum of entered matrices:-
    2       4       6
    8       10      12

             
# (19) Write a program to find the transpose of a matrix.

    #include<stdio.h>
    int main()
    {
        int a[10][10], transpose[10][10], n, m, i, j;
        printf("Enter rows and columns of matrix: ");
        scanf("%d %d", &n, &m);
        printf("\nEnter elements of matrix:\n");
        for(i=0; i<n; ++i)
         {
            for(j=0; j<m; ++j)
             {
                printf("Enter element a%d%d: ",i+1, j+1);
                scanf("%d", &a[i][j]);
             }  
         }   
        printf("\nEntered Matrix: \n");
        for(i=0; i<n; ++i)
         {
            for(j=0; j<m; ++j)
             {
                printf("%d  ", a[i][j]);
                if (j == m-1)
                  printf("\n\n");
             }    
         }   
        for(i=0; i<n; ++i)
        for(j=0; j<m; ++j)
         {
            transpose[j][i] = a[i][j];
         } 
        printf("\nTranspose of Matrix:\n");
        for(i=0; i<m; ++i)
         {
            for(j=0; j<n; ++j)
             {
                printf("%d  ",transpose[i][j]);
                if (j == n-1)
                  printf("\n\n");
             }
         }      
        return 0;          
    }

#### INPUT:
    Enter rows and columns of matrix: 2 3

    Enter elements of matrix:
    Enter element a11: 1
    Enter element a12: 2
    Enter element a13: 3
    Enter element a21: 4
    Enter element a22: 5
    Enter element a23: 6

    Entered Matrix: 
    1  2  3 

    4  5  6 

#### OUTPUT:
    Transpose of Matrix:
    1  4 

    2  5 

    3  6
    
    
# (20) Write a program to find the sum of digits of a number.

    #include<stdio.h>
    int main()
    {
        int digit, temp,  num,sum=0;
        printf("Enter any number: ");
        scanf("%d",&num);
        temp=num;
        while(temp>0)
         {
            digit=temp%10;
            sum= sum+digit;
            temp=temp/10;
         }
        printf("\nSum of digits of %d= %d\n",num,sum);
        return 0;
    }

#### INPUT:
    Enter any number: 179

#### OUTPUT:
    Sum of digits of 179= 17
    
    
# (21) Write a program to check whether the number is a palindrome number or not.

    #include<stdio.h>
    int main()
    {
        int sum=0, digit, num, temp;
        printf("\nEnter any positive number: ");
        scanf("%d",&num);
        temp = num;
        while(temp>0)
         {
            digit = temp%10;
            temp = temp/10;
            sum = sum*10 + digit;
         }
        if(num==sum)
         {
            printf("\n%d is a PALINDROME NUMBER",num);
         }
        else
         {
            printf("\n%d is not a PALINDROME NUMBER",num);
         }
        return 0;
    }

#### INPUT:
    Enter any positive number: 121

#### OUTPUT: 
    121 is a PALINDROME NUMBER


# (22) Write a program to swap two numbers using call by value method.

    #include<stdio.h>
    void swap( int a, int b );
    void main()
    {
        int x,y;
        printf("Enter the value for x: ");
        scanf("%d",&x);
        printf("Enter the value for y: ");
        scanf("%d",&y);
        printf("\nBefore calling SWAP FUNCTION\n");
        printf("\nValue of x=%d, Value of y=%d\n",x,y);
        swap(x,y);
        printf("\nAfter returning from SWAP FUNCTION");
        printf("\nValue of x=%d, Value of y=%d\n",x,y);
    }
    void swap( int a, int b)
    {
        int temp;
        printf("\nInside the function\n");
        printf("\nValue of a=%d, Value of b=%d before swap\n",a,b);
        temp=a;
        a=b;
        b=temp;
        printf("\nValue of a=%d, Value of b=%d after swap\n",a,b);
    } 

#### INPUT:
    Enter the value for x: 4
    Enter the value for y: 7

#### OUTPUT:
    Before calling SWAP FUNCTION

    Value of x=4, Value of y=7

    Inside the function

    Value of a=4, Value of b=7 before swap

    Value of a=7, Value of b=4 after swap

    After returning from SWAP FUNCTION
    Value of x=4, Value of y=7


# (23) Write a program to swap two numbers using call by refrence method.

    #include <stdio.h>
    void swap(int * num1, int * num2);
    int main()
    {
        int num1, num2;
        printf("Enter two numbers: ");
        scanf("%d%d", &num1, &num2);
        printf("Before swapping in main: \n");
        printf("Value of num1 = %d \n", num1);
        printf("Value of num2 = %d \n\n", num2);
        swap(&num1, &num2);
        printf("After swapping in main: \n");
        printf("Value of num1 = %d \n", num1);
        printf("Value of num2 = %d \n\n", num2);
        return 0;
    }
    void swap(int * num1, int * num2)
    {
        int temp;
        temp = *num1;
        *num1 = *num2;
        *num2 = temp;
        printf("After swapping in swap function: \n");
        printf("Value of num1 = %d \n", *num1);
        printf("Value of num2 = %d \n\n", *num2);
    }
    
#### INPUT:
    Enter two numbers: 4 7

#### OUTPUT:
    Before swapping in main 
    Value of num1 = 4 
    Value of num2 = 7 

    After swapping in swap function nValue of num1 = 7 
    Value of num2 = 4 

    After swapping in main 
    Value of num1 = 7 
    Value of num2 = 4


# (24) Write a program to enter the details of an employee using structures.

    #include<stdio.h>
    #include<string.h>
    struct Employee
    {
        int code;
        char name[25];
        char department[15];
        float salary;
    };
    void main()
    {
        struct Employee aEmployee;
        printf("Enter employee's code: ");
        scanf("%d",&aEmployee.code);
        printf("Enter employee's name: ");
        scanf("%s",&aEmployee.name);
        printf("Enter employee's department: ");
        scanf("%s",&aEmployee.department);
        printf("Enter employee's salary: ");
        scanf("%f",&aEmployee.salary);
        printf("\n\nParticulars of employees are: ");
        printf("\nEmployee's code: %d",aEmployee.code);
        printf("\nEmployee's name: %s",aEmployee.name);
        printf("\nEmployee's department: %s",aEmployee.department);
        printf("\nEmployee's salary: Rs.%.2f\n",aEmployee.salary);
    }

#### INPUT:
    Enter employee's code: 12
    Enter employee's name: Ram
    Enter employee's department: IT
    Enter employee's salary: 20000

#### OUTPUT:
    Particulars of employees are: 
    Employee's code: 12
    Employee's name: Ram
    Employee's department: IT
    Employee's salary: Rs.20000.00


# (25) Write a program to find the product of fractions using structures.

    #include <stdio.h>
    struct product
    {
        int numerator, denominator;
    };
    void main()
    {
        struct product V1,V2,V3;
        printf("Enter the numerator of first fraction: ");
        scanf("%d",&V1.numerator);
        printf("Enter the denominator of first fraction: ");
        scanf("%d",&V1.denominator);
        printf("Enter the numerator of second fraction: ");
        scanf("%d",&V2.numerator);
        printf("Enter the denominator of second fraction: ");
        scanf("%d",&V2.denominator);
        V3.numerator = V1.numerator * V2.numerator;
        V3.denominator = V1.denominator * V2.denominator;
        printf("Product= %d/%d",V3.numerator, V3.denominator);
    }

#### INPUT:
    Enter the numerator of first fraction: 2
    Enter the denominator of first fraction: 3
    Enter the numerator of second fraction: 4
    Enter the denominator of second fraction: 5
    
#### OUTPUT:
    Product= 8/15
