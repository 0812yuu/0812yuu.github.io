# 0812yuu.github.io
hello 
# long long int 可以裝比較長的整數
```cpp
#include<stdio.h>
int main()
{
    int n=9876543210;
    printf("int 印出來%d\n",n);

    long long int a=9876543210;
    printf("long long int 印出來%lld\n",a);
}
```
# 最大公因數 改用long long int
```cpp
#include<stdio.h>
int main()
{
    long long int a,b;
    scanf("%lld %lld",&a,&b);

    long long int ans;
    for(long long int i=1; i<=a; i++){
        if(a%i==0 && b%i==0) ans=i;
    }
    printf("最大公因數是:%lld\n",ans);
}
```

# 輾轉相除法改用long long int
```cpp
#include<stdio.h>
int main()
{
    long long int a,b,c;
    scanf("%lld %lld",&a,&b);
    while(1){
        c = a % b ;
        printf ("a:%lld b:%lld c:%lld\n",a,b,c);
        if(c==0) break;
        a = b;
        b = c;
    }
    printf ("答案是:%lld\n",b);


}
```

#  剝皮
```cpp
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);

    printf("現在的個位數:%d\n",n%10);
    n = n / 10;

    printf("現在的個位數:%d\n",n%10);
    n = n / 10;

    printf("現在的個位數:%d\n",n%10);
    n = n / 10;

    printf("現在的個位數:%d\n",n%10);
    n = n / 10;

    printf("現在的個位數:%d\n",n%10);
    n = n / 10;

    printf("現在的個位數:%d\n",n%10);
    n = n / 10;

    printf("現在的個位數:%d\n",n%10);
    n = n / 10;

    printf("現在的個位數:%d\n",n%10);
    n = n / 10;

    printf("現在的個位數:%d\n",n%10);
    n = n / 10;

    printf("現在的個位數:%d\n",n%10);
    n = n / 10;


}
