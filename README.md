write a program to print the perfect subset from middle portion of the string example input missisipi out put middle value
#include <stdio.h>
#include<string.h>
int main()
{
   
   char str[100], sstr[100];
   
   int i=0,n,j=0,m;
   printf("\n enter the string");
   scanf("%s",str);
   printf("\n enter the starting index to copy");
   scanf("%d",&m);
   printf("\n enter the ending index to copy");
   scanf("%d",&n);
   i=m;
   while (str[i] !='\0' && n>0)
   {
       sstr[j] = str[i];
       i++;j++;n--;
   }
   sstr[i]='\0';
   printf("the substring is:");
   puts(sstr);
   return 0;
}
