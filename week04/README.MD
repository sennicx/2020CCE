除惡務盡
#include <stdio.h>
```c
int main()
{
char a[100];
scanf("%s",&a);//將字串讀入依序放入陣列,最後加'\0'
int i=0;
while(a[i]!='\0')
{
if(a[i]!='2')
printf("%c",a[i]);

i++;

}
printf("\n");



}
 ```
 
 擲骰統計
 ```c
 #include <stdio.h>
int main()
{
char n[100];
scanf("%s",&n);

int i=0;

int a=0,b=0,c=0,d=0,e=0,f=0;
while(n[i]!='\0')
{
 if(n[i]=='1')a++;
 else if(n[i]=='2')b++;
 else if(n[i]=='3')c++;
 else if(n[i]=='4')d++;
 else if(n[i]=='5')e++;
 else if(n[i]=='6')f++;
i++;
}
printf("1:%d\n2:%d\n3:%d\n4:%d\n5:%d\n6:%d\n",a,b,c,d,e,f);





}
```

函數找整數的最大數字
```c
#include<stdio.h>
int main()
{
  char a[100];
  scanf("%s",&a);
  
  char ans=a[0];
  int i=0;
  while(a[i]!='\0')
  {
     if(a[i]>ans)ans=a[i];
     i++;
  
  
  
  
  
  }
  printf("[%c]",ans);
}
/* 上方C++ 的 main 函數 等價於 下方 C 的 main 函數
int main(void){
  int n;
  scanf("%d", &n);
  printf("[%d]", max_digit(n));
  return 0;
}
*/
```
星星等腰三角 
```c
#include <stdio.h>
int main()
{
int n;
scanf("%d",&n);
for(int i=1;i<=n;i++)
{
for(int j=0;j<(n-i);j++)
printf(" ");
for(int j=0;j<(i*2-1);j++)
printf("*");
printf("\n");
}

}
```
分開整數的每個數字
```c
#include <stdio.h>
#include <string.h>
int main()
{
char a[100];
scanf("%s",&a);
int i=0;
while(i<(strlen(a)-1))
{
printf("%c   ",a[i]);
i++;
}
printf("%c",a[i]);



}

```
字元判別 
```c
#include <stdio.h>
int main()
{
char a;
scanf("%c", &a);
if('A'<=a && a<='Z')
     printf("U");
else if('a'<=a && a<='z')
     printf("L");
else if('0'<=a && a<='9')
     printf("D");
else 
     printf("O");


}

```
數字之首 
```C
#include <stdio.h>
int main()
{
char a[100];
scanf("%s",&a);
int i=0;
printf("%c",a[0]);





}
```
輸出從0到N的偶數 
```C
#include <stdio.h>
int main()
{
int N;
scanf("%d",&N);
for(int i=1;i<=N/2;i++){
printf("%d ",2*i);

}



}
```
