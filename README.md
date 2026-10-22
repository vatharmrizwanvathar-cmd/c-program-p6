# c-program-p6
/* WACP to read a number,find the sum of digits, reverse the number and check if for palindrome */
#include<stdio.h>
int main()
{
    int num,sum=0,rev=0,d,n;
    printf(" enter the number");
    scanf("%d",&num);
    n=num;
    while(num)
        {
            d=num%10;
            num=num/10;
            sum=sum+d;
            rev=rev*10+d;
        }
    printf("sum of digits=%d",sum);
    printf("\n reverse of the number=%d",rev);
    if(n==rev)
        printf("\n%d number is palindrome",rev);
    else
        printf("\n number is no palindrome",rev);
}
output:
enter the number565
sum of digits=16
 reverse of the number=565
565 number is palindrome
