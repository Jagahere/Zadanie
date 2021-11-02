# Zadanie
#include <stdio.h>

int main() {
	printf("Zadanie 1\n");

	int numerAlbumu = 123011;
	printf("Numer albumu: %d\n", numerAlbumu);

	printf("Zadanie 2\n");

	int liczba;
	printf("Podaj liczbe calkowita: ");
	scanf_s("%d", &liczba);
	int mod = liczba % 2;

	if (mod == 0) {
		printf("Liczba: %d jest parzysta\n", liczba);

	}
	else {
		printf("Liczba: %d nie jest parzysta\n", liczba);
	}

	printf("Zadanie 3\n");
	float a, b;
	printf("Podaj dwie liczby : ");
	scanf_s("%f %f", &a, &b);

	if (a > b) {
		printf("%f jest wieksza od %f\n", a, b);
	}
	else if (a == b) {
		printf("%f rowna sie %f\n", a, b);
	}
	else {
		printf("%f jest mniejsza od %f\n", a, b);
	}

	printf("Zadanie 4 \n");
	float c, d, e, f, srednia;
	printf("Wprowadz 4 liczby : ");
	scanf_s("%f %f %f %f", &c, &d, &e, &f);
	srednia = (c + d + e + f) / 4;
	printf("Srednia arytmetyczna liczb %f %f %f %f to %f\n", c, d, e, f, srednia);
  
  printf("Zadanie 5\n");
	int l1, l2;
	char kalkulator;
	printf("Wprowadz dwie liczby oraz symbol(+,-,*,/)\n");
	scanf_s("%d %d %c", &l1, &l2, &kalkulator);

	switch (kalkulator) {
	case '+':
		printf("%d\n", l1 + l2);
		break;
	case '-':
		printf("%d\n", l1 - l2);
		break;
	case '*':
		printf("%d\n", l1 * l2);
		break;
	case '/':
		printf("%d\n", l1 / l2);
		break;
	default:
		printf("Nie mozna uzyskac odpowiedzi");
		break;
	}
	return 0;
}
	
