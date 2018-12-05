#include <stdio.h>
main()
{
float student[10][2],totalgrad;
int i,j;
float avg;
    // Scan ID and Grad
     for (i=0;i<10;i++)
   {
   	  printf("\nStudent %d \n",i+1);
      for (j=0;j<2;j++) 
    {
      if(j == 0) printf("Enter your id :");
      else printf("Enter your grad :");
      scanf("%f",&student[i][j]);
    }
   }
    // PRINT ID and Grad
    for (i=0;i<10;i++)
   {
      for (j=0;j<2;j++) 
    {
      if(j == 0) printf("\nYour id :");
      else printf("\nYour grad :");
      printf("%f",student[i][j]);
    }
   } 
   // total grad
    for (i=0;i<10;i++)
   {
      for (j=1;j<2;j++) 
    {
        totalgrad = totalgrad+student[i][j];
        avg = totalgrad/10;
    }
   } 
   // Check Grad > 2.00
     for (i=0;i<10;i++)
   {
      for (j=0;j<2;j++) 
    {
       if(student[i][1] > 2) 
	   {
       	printf("\nStudent grad > 2.00");
	    printf("\n%f",student[i][0]);
	   }
    }
   } 
   // Show total grad,Avg grad
   printf("\nTotalgrad = %f",totalgrad);
   printf("\nAvg = %f",avg);
}
