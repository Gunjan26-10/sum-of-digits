# sum-of-digits
Developed by Gunjan Narkhede
#include<stdio.h>
int s(int n)
{
	int j,sum=0;
	while(n>0)	
		{
		   for(j=1;j<10;j++)
		   {
			  if(j==n%10)
			  {
				  n=n/10;
				  sum+=j;
				  break;
			  }
		   }
	  }   
      return sum;
}
int main()
{
	int n,sum=0;
	printf("enter the number");
	scanf("%d",&n);
	sum=s(n);
	printf("sum of digits of %d is %d",n,sum);
    return 0;
}
