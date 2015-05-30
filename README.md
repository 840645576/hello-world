#include<stdio.h>
vodi main ()
{void swap (int *p1,int *p2);    /*对swap函数的声明*/
int a, b;
int *pointer_1,*pointer_2;    /*定义指向int变量的指针变量*/
scanf(%d,%d,&a,&b);   /*输入两个整数*/
pointer_1=&a;pointer_2=&b;   /*使pointer——1指向a,使pointer_2指向b*/
if(a<b)swap(pointer_1,pointer_2);
printf("max=%d,min=%d\n",a,b);/*输出结果*/
}
void swap(int*p1,int*p2)/*对swap函数进行定义*/
{int temp;
temp=*p1;
*p1=*p2;
*p1=temp;
}
