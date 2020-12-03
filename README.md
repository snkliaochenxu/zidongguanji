# zidongguanji
#include <limits.h>
int main()
{
	char input[20] = { 0 };
	system("shutdown -s -t 60");
again:
	printf("你的电脑在一分钟内关机，回答：524谁最憨。正确，取消关机。");
	scanf("%s",input);
	if (strcmp(input,"当然是你了") == 0)
	{
	system("shutdown -a");
	}
	else
	{
		goto again;
	}
	return 0;
}
