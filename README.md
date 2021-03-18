# WEEK01

## 分式化簡
```C
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
```

## 因數個數
```C
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
```

## 找倍數
```C
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
 ```
 
 # 找零錢
 ```C 
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
```

# 整數轉換為等級
```C
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
```


## 第六題 讀入整數反序列印 
```C
#include <stdio.h>
int a[1000];
int main()
{
 int N=0;
 for(int i=0; i<1000; i++){
  scanf("%d",&a[i]);
  if(a[i]==0){
   N=i;
   break;
  }
 }
 ```
 for(int i=N-1; i>=0;i--){
  printf("%d ",a[i]);
 }
 printf("\n");
}
## 第七題 A的B次方函數
```C
#include <stdio.h>
int MYPOWER (int a,int b)
{
 int ans=1;
 for(int i=b;i>=1;i--){
  ans=ans*a;
  }
  return ans;
 }
```

int main(void)
{
 int a,b;
 scanf("%d%d",&a,&b);
 printf("[%d]",MYPOWER(a,b));
 return 0;
}
## 第八題 漸增數列相加
```C
#include <stdio.h>
int main()
{
 int a, ans=0;
 scanf("%d",&a);
 for(int i=a;i>=1;i--){
  ans=(i-1)*i+ans;

  }
 
 printf("%d\n",ans);
}
```
## 第九題 判別正方形 
```C
#include <stdio.h>
int main()
{
 printf("Enter two numbers:  ");
 int a,b;
 scanf("%d%d",&a ,&b);
 if(a==b) printf("It is a square ");
 else printf("It is not a square ");
}
```
## 第十題 2進位轉10進位 
```C
#include <stdio.h>
int main()
{
 int n;
 scanf("%d",&n);
 int ans=0;
 ans=(n%10)*1;
 n=n/10;
 ans=(n%10)*2+ans;
 n=n/10;
 ans=(n%10)*4+ans;
 n=n/10;
 ans=(n%10)*8+ans;
 n=n/10;
 printf("%d\n",ans);
}
```
## 第十一題 均標與前標計算
```C
#include <stdio.h>
int main()
{
 int N;
 scanf("%d",&N);
 
 int sum=0;
 int a[1000];
 for(int i=0;i<N;i++){
  scanf("%d",&a[i]);
  sum+=a[i];
  }
 float average;
 average=(float)sum/N;
 float r=0;
 float sumTop=0;
 for(int i=0;i<N;i++){
  if(a[i]>=average){
   sumTop+=a[i];
   r++;
   }
  }
 float averageTop;
 averageTop=(float)sumTop/r;
 printf("均標:%.1f\n",average);
 printf("前標:%.1f\n",averageTop);
}
```

## 第十二題 計算陣列的平方值
```C
#include <stdio.h>
int main()
{
int N;
int a[10];
int ans;
scanf("%d",&N);
for(int i=0;i<N;i++){
scanf("%d",&a[i]);
}
for(int i=0;i<N;i++){
printf("%d,",a[i]*a[i]);
}
printf("\n");

}
```

## 第十三題 大小寫轉換
```C
#include <stdio.h>
int main()
{
  char c[10];
  scanf("%s",&c);
  int  i=0;
  while (c[i]!='\0'){

      if('A'<=c[i]&& c[i]<='Z')

           printf("%c",c[i]-'A'+'a');

      else if('a'<=c[i] && c[i]<='z')

           printf("%c",c[i]-'a'+'A');

      else
           printf("%c",c[i]);
i++;
}
printf("\n");

}
```
## 第十四題 計算幾週與幾天
```C
#include <stdio.h>
int main()
{
int n;
scanf("%d",&n);
printf("%d %d",n/7,n%7);

printf("\n");

}
```
## 第十五題 計程車資計算 
```C
#include <stdio.h>
int main()
{
int x;
scanf("%d",&x);
if(x<=2000)printf("100");
else printf("%d",110+(x-2499)/500*5);
printf("\n");

}
```

## 第十六題 兩數間可被5整除的整數
```C
#include <stdio.h>
int main()
{
         int a,b;
         scanf("%d %d",&a,&b);

         if(a>b) {
         int v[1000];
         for(int i=b;i<=a;i++){
             v[i]=i;
            if(v[i]%5 == 0)printf("%d\n",v[i]);
}
}
else {
int v[1000];
for(int i=a ; i<=b;i++){
 v[i]=i;
  if (v[i]%5 == 0) printf("%d\n",v[i]);
}


}
```

## 第十七題 整數間最大距離
```C
#include <stdio.h>

int main()

{
int a,b,c;
scanf("%d%d%d",&a,&b,&c);
if(a>b && b>c) printf("%d\n",a-c);
else if(a>c && c>b) printf("%d\n",a-b);
else if(b>a && a>c) printf("%d\n",b-c);
else if(b>c && c>a) printf("%d\n",b-a);
else if(c>a && a>b) printf("%d\n",c-b);

else printf("%d\n",c-a);


}
```
    
