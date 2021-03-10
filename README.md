# 2020cce
## WEEK1
## 第一題
```c
#include <stdio.h>
int main()
{
	int a,b;
	scanf("%d%d",&a,&b);
	if(a>b)
	{
		int t=a;
		a=b;
		b=t;
	
	for(int i=2;i<=a;i++)
		{
			if(a%i==0&&b%i==0)
			{
				a=a/i;
				b=b/i;
			}
			
		}
		printf("%d %d\n",b,a);
	}else
	{
	for(int i=2;i<=a;i++)
	{
		if(a%i==0&&b%i==0)
		{
			a=a/i;
			b=b/i;
		}
		
	}
	printf("%d %d\n",a,b);
	}
}
```
## 第二題
```c
#include <stdio.h>
int main()
{
	int a[90],n=0;
	for(int i=1;i<=90;i++)
	{
		scanf("%d",&a[i]);
		n=n+1;
		if(a[i]==0) break ;
	}
	for(int k=n-1;k>0;k--)
	{
		printf("%d ",a[k]);
	}
	printf("\n");
	
}

```
## 第三題
```c
#include <stdio.h>
int MYPOWER(int a,int b,int c=1)
{
	for(int i=1;i<=b;i++)
	{
		c=c*a;
	}
	return c;
}
int main(void)
{
	int a,b;
	scanf("%d%d",&a,&b);
	printf("[%d]",MYPOWER(a,b));
	return 0;
}

```
## 第四題
```c
#include<stdio.h>
int main()
{
	int n,p=0;
	scanf("%d",&n);
	for(int i=1;i<n;i++)
	{
		p=p+i*(i+1);
	}
	printf("%d\n",p);
}

```
## 第五題
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	printf("%d=50*%d+5*%d+1*%d\n",n,n/50,n%50/5,n%50%5/1);
}
```
## 第六題
```c
#include <stdio.h>
int main()
{
	int n,a=0;
	scanf("%d",&n);
	for(int i=1;i<=n;i++)
	{
		if(n%i==0)  a=a+1;
		
	}
	printf("%d\n",a);
}
```
## 第七題
```c
#include <stdio.h>
int main()
{
	int a[10],n=0;
	for(int i=0;i<10;i++)
	{
		scanf("%d",&a[i]);
		if(a[i]%3==0)n=n+1;
	}
	printf("%d\n",n);
}
```
## 第八題
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	if(n>=90) printf("A\n");
	else if(n>=80) printf("B\n");
	else if(n>=60) printf("C\n");
	else printf("F\n");
}
```
## week 2
## 第一題
```c
#include <stdio.h>
int main()
{
	int n1=10,n2=20,n3=30;
	printf("n1:%d n2:%d n3:%d\n",n1,n2,n3);
	int *p=&n1;
	*p=200;
	printf("n1:%d n2:%d n3:%d\n",n1,n2,n3);
	return 0;
}
```
## 第二題
```c
#include <stdio.h>
int main()
{
	int n1=10,n2=20,n3=30;
	printf("n1:%d n2:%d n3:%d\n",n1,n2,n3);
	int *p=&n1;
	*p=200;
	printf("n1:%d n2:%d n3:%d\n",n1,n2,n3);
	int *p2=&n3;
	*p2=300;
	printf("n1:%d n2:%d n3:%d\n",n1,n2,n3);
	return 0;
}
```
## 第三題
```c
#include <stdio.h>
int main()
{
	int n1=10,n2=20,n3=30;
	printf("n1:%d n2:%d n3:%d\n",n1,n2,n3);
	int *p=&n1;
	*p=200;
	printf("n1:%d n2:%d n3:%d\n",n1,n2,n3);
	int *p2=&n3;
	*p2=300;
	printf("n1:%d n2:%d n3:%d\n",n1,n2,n3);
	p2=p;
	*p2=400;
	printf("n1:%d n2:%d n3:%d\n",n1,n2,n3);
	return 0;
}
```
## 第四題
```c
#include <stdio.h>
int main()
{
	int  n[3]={10,20,30};
	printf("n[0]:%d n[1]:%d n[2]:%d\n",n[0],n[1],n[2]);
	int *p=&n[0];
	*p=200;
	printf("n[0]:%d n[1]:%d n[2]:%d\n",n[0],n[1],n[2]);
	int *p2=&n[2];
	*p2=300;
	printf("n[0]:%d n[1]:%d n[2]:%d\n",n[0],n[1],n[2]);
	p2=p;
	*p2=400;
	printf("n[0]:%d n[1]:%d n[2]:%d\n",n[0],n[1],n[2]);
	return 0;
}
```
