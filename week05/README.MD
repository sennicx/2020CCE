反序數字
```C
#include <stdio.h>
int f(int n)
{
 int p;
 int m=0;
 
 while(n>0)
 {
  p=n%10;
  n=n/10;
  m=p+m*10;
  }
  return m;
 
 
 
 
 }
int main()
{
int n,m;
scanf("%d",&n);
printf("%d+%d=%d\n",n,f(m), n+f(m));
}
```
絕對值函數 
```C
include <stdio.h>
int f(int n)
{
if(n<0){
return-n;
}
else return n;




}







int main(void)
{
	int n;
	scanf("%d",&n);
	printf("[%d]",f(n));
	return 0;
}
```
N數之和 
```C
#include <stdio.h>
int main()
{
int N;
scanf("%d",&N);
int a[10];
int ans;

for(int i=0;i<N;i++){
scanf("%d",&a[i]);
ans=ans+a[i];
}
printf("%d\n",ans-N);



}

```
三數極大 
```C
include <stdio.h>
int main()
{
int N;
scanf("%d",&N);
int a[10];
int ans;

for(int i=0;i<N;i++){
scanf("%d",&a[i]);
ans=ans+a[i];
}
printf("%d\n",ans-N);



}

```

計算商數 
```C
#include <stdio.h>
int main()
{
int a,b;
scanf("%d%d",&a,&b);
printf("%d",a/b);
printf("\n");





}
```
