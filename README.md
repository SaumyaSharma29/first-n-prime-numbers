# first-n-prime-numbers

#include<stdio.h>

void main()
{
	int i, n, m=0;
	
	printf("Enter the range:\t");
	scanf("%d", &n);
	
	while(m <= n)
	{
		for(i = 2; i <= m; i++)
		{
			if(m % i == 0)
				break;
		}
		
		if(i == m)
			printf("%d\t", m);
		m++;
	}
	printf("\n");
}
