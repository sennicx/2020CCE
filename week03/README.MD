##第十二題 計算陣列的平方值
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
##第十三題 大小寫轉換
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
##第十四題 計算幾週與幾天
#include <stdio.h>
int main()
{
int n;
scanf("%d",&n);
printf("%d %d",n/7,n%7);

printf("\n");

}
##第十五題 計程車資計算
#include <stdio.h>
int main()
{
int x;
scanf("%d",&x);
if(x<=2000)printf("100");
else printf("%d",110+(x-2499)/500*5);
printf("\n");

}
##第十六題 兩數間可被5整除的整數
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
##第十七題 整數間最大距離
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
