# c-reverse-a-string
#include <stdio.h>
#define MAX_SIZE 100
int main()
{
  char str[MAX_SIZE], reverse [MAX_SIZE];
  int i, strIndex, revIndex, len;
  printf("enter any string:");
  scanf("%s",str);
  i = 0;
  while(str[i]!='\0') i++;
  len = i;
  revIndex = 0;
  strIndex = len - 1;
  while(strIndex >= 0)
  {
    reverse[revIndex] = str[strIndex];
    strIndex--;
    revIndex++;
  }
  reverse[revIndex] = '\0';
  printf("\noriginal string = %s\n",str);
  printf("reverse string = %s",reverse);
  return 0;
}
