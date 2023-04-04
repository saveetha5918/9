#include <stdio.h>

int main() {
    int num, reverse = 0, digit;

    printf("Enter a number: ");
    scanf("%d", &num);

    // Find reverse of number using for loop
    for(int temp = num; temp > 0; temp /= 10) {
        digit = temp % 10;
        reverse = reverse * 10 + digit;
    }

    printf("Reverse of %d = %d\n", num, reverse);

    return 0;
}
