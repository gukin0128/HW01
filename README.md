#include <iostream>
using namespace std;

int Sum(int arr[], int size) {
    int sum = 0;
    for (int i = 0; i < size; ++i) {
        sum += arr[i];
    }
    return sum;
}

double Average(int arr[], int size) {
    int sum = Sum(arr, size);
    return (double)sum / size;
}

int main() {
    const int size = 5;
    int numbers[size];

    cout << "5개의 정수 입력 :  ";
    for (int i = 0; i < size; ++i) {
        cin >> numbers[i];
    }

    int sum = Sum(numbers, size);
    double average = Average(numbers, size);

    cout << "합계 : " << sum << endl;
    cout << "평균 : " << average << endl;

    return 0;
}
