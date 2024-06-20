#include <stdio.h>
int isprime(int n)
{
  if(n==1)
  {
    return 0;
  }
  else if (n==2 || n== 3)
  {
    return 0;
  }
  else if(n%2==0 || n%3==0)
  {
    return 0;
  }
  for (int i =5 ;i*i<n;i=(i+6))
  {
    if( n% i==0 )
    {
      return 0;
    }
  }
  return 1;
}
int main()
{ 
  int n,a;
 printf("enter the n value\n" );
 scanf("%d",&n);
 a=isprime(n);
 if(a==1)
 {
   printf("number is prime");
 }
 else
 {
   printf("not prime");
 }
}
