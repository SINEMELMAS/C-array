# C-array
ARRAYS
#include <stdio.h>
#define SIZE 10
int main(void) {
   float numbers[SIZE]={0.0,1.1,2.2,3.3,4.4,5.5,6.6,7.7,8.8,9.9}; 
   float *nPtr; 
   printf("Elements of the array\n");
   for (size_t x=0; x<SIZE; x++)
   {
       printf("%dth element is %.1f\n", x+1, numbers[x]);
   } 
  nPtr=numbers;
  nPtr=&numbers[0]; 
  printf("\nElements of the array\n");
  for (size_t x=0; x<SIZE; x++)
  {
      printf("%dth element is %.1f\n", x+1, *(nPtr+x));
  } 
  printf("\nElements of the array\n");
  for (size_t x=0; x<SIZE; x++)
  {
      printf("%dth element is %.1f\n", x+1, *(numbers+x));
  } 
  printf("\nElements of the array\n");
  for (size_t x=0; x<SIZE; x++)
  {
      printf("%dth element is %.1f\n", x+1, nPtr[x]);
  } 
  printf("\nThe address is %p\n", &numbers[8]);
  printf("The value of nPtr+8 is %f\n", *(nPtr+8)); 
  printf("\n4th element is %f\n", numbers[3]); 
  printf("4th element is %f\n", *(numbers+3)); 
  printf("4th element is %f\n", nPtr[3]); 
  printf("4th element is %f", *(nPtr+3)); 
}
