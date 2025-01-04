PRINTING PATTERN:
1

4*5*6

2*3

7*8*9*10

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM:
Take the number of rows as input from the user and store it in any variable.(‘l‘ in this case).
Run a loop ‘l’ number of times to iterate through each of the rows. From i=0 to i<l The loop should be structured as for( i=0 ; i<l: i++).
Run a nested loop to iterate through the columns. From j=0 to j<l. The loop should be structured as for(j=0 ; j<l; j++).
increment count and run an if condition if(j!=0).
if true then print star and count else print only count.
outside the nested loop print a newline
Run another nested loop under the main loop . From j=0 to j<=i+2. The loop should be structured as for(j=0 ; j<=i+2; j++).
increment count1 and run an if condition if(j!=0).
if true then print star and count1 else print only count1.
outside the nested loop print a newline
CODE IN C:
#include<stdio.h>
int main()
{
int i,j,l,count=0,count1=3; //declaring integers i,j for loops and l for number of rows
printf("Enter the number of rows\n"); //Asking user for input
scanf("%d",&l); //Taking the input for number of rows
for(int i=0;i<l/2;i++) //Outer loop for number of rows
  {
    for(j=0;j<=i;j++)
     {
      count++;
      if(j!=0)
        { 
          printf("*%d",count);
        }
      else
        {
          printf("%d",count);
        }
      }
    printf("\n");
    for(j=0;j<=i+2;j++)
      {
        count1++;
        if(j!=0)
          {
            printf("*%d",count1);
          }
        else
          {
            printf("%d",count1);
          }
      }
   printf("\n");
  }
}
TAKING INPUT:
DISPLAYING OUTPUT:
