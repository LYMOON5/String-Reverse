#include<stdio.h>
#include<string.h>

//使输入的一个字符串按反序存放，在主函数中输入和输出字符串
void Reverse(char *arr)
{
	int i;
	int j;
	char tmp;
	j=strlen(arr);
	for(i=0;i<j/2;i++)
	{
		tmp=arr[i];
		arr[i]=arr[j-i-1];
		arr[j-i-1]=tmp;
	}
}

int main()
{
	char arr[100];         
	scanf("%s",arr);
	Reverse(arr);
	printf("%s",arr);
  
	return 0;
}
