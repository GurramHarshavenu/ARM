#include<LPC21XX.H>

#define LED1      1<<2
#define LED2      1<<8
#define LED3      1<<16
#define LED4      1<<20
#define join(a,b)    a##b
void delay(int i)
{
	int j;
	for(;i>0;i--)
	for(j=12000;j>0;j--);
}
int main()
{
  int count=20,j;
	int i[4]={LED1,LED2,LED3,LED4};

	IODIR0=LED1|LED2|LED3|LED4;

	while(count--)
	{ for(j=0;j<4;j++)
		IOCLR0=i[j];
		delay(500);
		for(j=0;j<4;j++)
		IOSET0=i[j];
		delay(500);
  }
}
