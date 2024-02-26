# T-nh-s-n-m-c-n-g-i-ti-t-ki-m
Một người cần có một số tiền T, tích lũy bằng cách gửi tiết kiệm số tiền ban đầu là S với lãi suất có kỳ hạn theo năm là P% theo phương thức lũy tiến (lãi của mỗi năm được cộng vào với tiền gốc). Hãy nhập vào các số thực T, S, P và xác định số năm cần gửi tiết kiệm.
#include <stdio.h>
#include <conio.h>

void main()

{
	float s, t, p;
	int n;
	clrscr();

	printf("Nhap so tien ban dau : ");
	scanf("%f", &s);
	printf("Nhap so tien can co : ");
	scanf("%f", &t);
	printf("Nhap lai suat %% nam : ");
	scanf("%f", &p);

	for (p = 0.01 *p, n = 0; s < t; s += s *p, n++);
	printf("So nam can gui tiet kiem = %d\n", n);
	printf("Sau %d nam gui tiet kiem, so tien co la : %4.2f", n, s);

	getch();
}
