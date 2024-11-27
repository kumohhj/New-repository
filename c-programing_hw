#include <stdio.h>
#include <stdlib.h>

void inputLength(int*);
void sbinary();

void main()
{
	int binaryLength = 0;
	int res = 0;
	int m = 1;
	char* binary;
	int* multi;
	int* decimal;

	printf("길이 입력 :");
	scanf_s("%d", &binaryLength);

	binary = (char*)malloc(binaryLength * sizeof(char));
	multi = (int*)malloc(binaryLength * sizeof(int));
	decimal = (int*)malloc(binaryLength * sizeof(int));

	printf("이진수 입력 :");
	scanf_s("%s", binary, sizeof(binary));

	for (int i = 0; i < binaryLength - 1; i++)
	{
		m *= 2;

	}

	for (int j = 0; j < binaryLength; j++) {
		multi[j] = m;
		m = m / 2;
	}

	for (int k = 0; k < binaryLength; k++)
	{
		if (binary[k] == '1') {
			decimal[k] = multi[k];
		}
		else if (binary[k] == '0') {
			decimal[k] = 0;
		}
	}

	for (int k = 0; k < binaryLength; k++)
	{
		res = res + decimal[k];
	}
	printf("10진수로 변환 : %d \n", res);
}

void inputLength(int* length)
{
	printf("길이 입력 :");
	scanf_s("%d", &length);
}
