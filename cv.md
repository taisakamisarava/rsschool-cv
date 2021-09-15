# Taisa Komissarova

## Contacts

- Location: Minsk, Belarus
- Phone: +375 33 602-90-77
- Email: komissarova.taisa@gmail.com
- GitHub: taisakamisarava

## About

I am studying for my Bachelor's degree in Business Informatics in BSU. I am keen on my field of studies and on everything connected with modern technologies.
My aim at the course is to get all required for _Junior Dev_ position!

## Code Examples

```
#include <iostream>
#include <clocale>
#include <stdio.h>
#include <conio.h>
#include <stdlib.h>
#include <ctime>

using namespace std;

int main()
{
   using std::setlocale;
   setlocale(LC_ALL,"");
   srand(time( 0));
   int a[15],n,i,k, r, z, kol=0;

   printf("Выберите тип ввода: 1-c клавиатуры, 2-с помощью rand() ");
   scanf("%d",&k);
   if ((k>0)&&(k<=2))
   {
     printf ("Введите размер массива не более 15 элементов, N = ");
     scanf("%d",&n);
     printf("Массив A \n");
     switch(k) {
       case 2: for (i=0; i<n; i++){
               a[i] = rand()%21-10;
               printf("%4d",a[i]);
               }
               break;
        case 1: for (i=0; i<n; i++) scanf("%d",&a[i]);
                break;
     }
   }
   else {puts("Не выбран тип ввода...");
         return 1;
         }
         int min = a[0];
         for (int i=1; i<n; i++){
           if (a[i]<min){
             min=a[i];
             z=i;
           }
         }
puts ("\n Минимальное число в масcиве");
printf("%d\n", min);
       r=0;
       for (int i=n-1; i>z; i--){    //алгоритм считает елементы с конца
           r=r+a[i];
           printf("%d\n",a[i]);
       }
       puts("\nРезультат");
       printf("%d\n",r );

   return 0;
}

```
