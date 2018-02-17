# mario_cs50
week1
// Подключаем библиотеки, без которых функции не будут работать
#include <cs50.h>
#include <stdio.h>

int main(void)
{
    int a;
    // делаем запрос на ввод числа, символа и строки, просто чтобы вывести их и проверить что все работает
    do {
    a = get_int("get height of piramid: \n");
    } while (a < 0 || a > 23);
    for (int i = a; i > 0; i--) {
        //printf("new line %i:", i);
        for (int space = i-1; space >0; space--){
        printf(" ");
        }
        for (int symbol = i; symbol <= a+1; symbol++){
            printf("#");
        }
        printf("\n");
    }


}
