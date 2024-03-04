#define _CRT_SECURE_NO_WARNINGS 1

#include<stdio.h>
//创建一个结构体
struct Book
{

	char name[30];
	short price;

};
int main()
{
	struct Book book1 = { "my life",20 };
	book1.name[30] = "my life";
	book1.price = 20;
	printf("书名：%s\n", book1.name);
	printf("价格：%d\n", book1.price);

	struct Book* pb = &book1;
	printf("书名：%s\n", pb->name);
	printf("价格：%d\n", pb->price);
	
	return 0;
}
