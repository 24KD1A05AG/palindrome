#include <stdio.h>

int main()
{
   int Number, Temp, Reminder, Rev = 0;
 
   printf("\nPlease Enter any value \n");
   scanf("%d", &Number);
  
   //Helps to prevent altering the original value
   Temp = Number;

   while ( Temp > 0)
   {
      Reminder = Temp %10;
      Rev = Rev *10+ Reminder;
       Temp = Temp /10;
   }
 
   printf("Rev of entered = %d\n", Rev);

   if ( Number == Rev )
      printf("\n%d is Palindrome.\n", Number);

   else
      printf("%d is not.\n", Number);
 
   return 0;
}
