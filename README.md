# -GRRRMONDAYS
#GRRRMONDAYS
/*************************
* Автор: Полудинцев Н.А. *
* Дата: 16.09.2026       *
* Название: Лаб №1       *
*************************/
// Example program
#include <iostream>
#include <cmath>

using namespace std;

int main() {
    const double pi = 3.14159265358979;
    double lya, firstRad, secondRad, firstTemp, secondTemp, F;
    lya = 59.034;
    firstRad = 25.2 / 100.0;
    secondRad = 29.3 / 100.0;
    firstTemp = 264.0;
    secondTemp = 43.0;
    F = 0.53;

    double Q = ((lya * F) / (secondRad - firstRad)) * (firstTemp - secondTemp);

    cout << "Q =" << Q;
}
