##分式化簡
#include <stdio.h>
int main()
{
    int a,b,temp;
    scanf("%d%d",&a,&b);
    if(b>a)
    {
    for(int i=1;i<=b;i++)
    {
        if(a%i==0&&b%i==0)
        {
           temp=i;
        }
    }
}
if(a>b)
{
   for(int i=1;i<=a;i++)
   {
       if(a%i==0&&b%i==0)
       {
        temp=i;
       }
   }
}
a=a/temp;
b=b/temp;
printf("%d%d\n"a,b);
}
##因數個數
#include <stdio.h>
int main()
{
 int n;
 scanf("%d",&n);
 int a=0;
 for(int i=1;i<=n;i++){
    if(n%i==0){
    a++;
    }
}
printf("%d\n",a);
}
##找倍數
#include<stdio.h>
int main()
{
 int a[10],n=10;
 int ans=0;
 for(int i=1;i<=n;i++){
    scanf("%d",&a[10]);
    if(a[10]%3==0){
       ans++;
     }
 }
 printf("%d\n"ans);
 }
##找零錢
#include <stdio.h>
int main()
{
int n,a,b,c;
scanf("%d",&n);
a=n/50;
b=n%50/5;
c=n%50%5;
printf("%d=50*%d+5*%d+1*%d\n",n,a,b,c);
}
##整數轉換為等級
#include<stdio.h>
int main()
{
 int n;
 scanf("%d",&n);
 if(n>=90){
   printf("A\n");
 }
 else if(n<90&&n>=80){
      printf("B\n");
 }
 else if(n<80&&n>=60){
      printf("C\n");
 }
 else if(n<60)
 printf("F\n");
}
