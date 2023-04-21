# de-18
#include <stdio.h>

int main() {
    float arr[] = {-1.2, -2.5, -3.8, -4.7, -5.9};
    int n = sizeof(arr)/sizeof(arr[0]);
    int isNeg = 1;
    for (int i = 0; i < n; i++) {
        if (arr[i] >= 0) {
            isNeg = 0;
            break;
        }
    }
    if (isNeg) {
        printf("Mang toan gia tri am");
    } else {
        printf("Mang khong toan gia tri am");
    }
    return 0;
}

