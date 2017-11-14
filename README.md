//Muneeb Siddiqui	
//msiddi07@uoguelph.ca
//0977722
//Star Pattern

#include <stdio.h>

int main(){

int i = 0;
int j = 0;
int numLine = 0;
int width = 0;
//int numStar = 0;

printf("Number of numLine?");
scanf("%d" , &numLine);
if (numLine % 2 > 0)  {
    printf ("Invalid input - number of numLine must be even");
}

printf("Width between left and right figure?");
scanf("%d" , &width);


for(i = 0; i < numLine; i++){
     if(i < (numLine/2) -1)  {

          for(j=0; j < ((numLine / 2) -1) -i ; j++){
          printf(" ");
          }

          for(j=0; j < 1 + i; j++){
          printf("*");
          }

          for(j=0; j < width; j++){
          printf(" ");
          }

          for(j=0; j < 1 + i; j++){
          printf("*");
          }
     printf("\n");
     }


     if (((i == (numLine / 2)- 1)) || (i == (numLine / 2))){ 

          for (j=0; j < numLine/ 2; j++){
          printf ("*");
          }


          for (j=0; j < width; j++){
          printf ("-");
          }

          for (j=0; j < numLine/ 2; j++)  {
          printf ("*");
          }
          printf ("\n");
          }
     if (i > numLine / 2)  {

          for (j=0; j < ( i -(numLine / 2)); j++ )  {
          printf (" ");
          }

          for (j=0; j < (numLine / 2) - (i - (numLine / 2)); j++ )  {
          printf ("*");
          }

          for (j=0; j < width; j++) {
          printf (" ");
          }

          for (j=0; j < (numLine / 2) - (i - (numLine / 2)); j++ )  {
          printf ("*");
          }
     printf ("\n");
     }
}

return 0;

}
