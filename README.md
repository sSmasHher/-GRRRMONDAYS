# -GRRRMONDAYS
#GRRRMONDAYS
/*************************
* Автор: Полудинцев Н.А. *
* Дата: 16.09.2026       *
* Название: Лаб №1       *
*************************/
#include <iostream>
#include <cmath>

using namespace std;

int main() {
    const double pi = 3.14159265358979;
    double lya, firstRad, secondRad, firstTemp, secondTemp, F, L;
    lya = 59.034;
    firstRad = 25.2 / 100.0;
    secondRad = 29.3 / 100.0;
    firstTemp = 264.0;
    secondTemp = 43.0;
    F = 0.53;
    L = 1;
    double firstQ = ((lya * F) / (secondRad - firstRad)) * (firstTemp - secondTemp);
    double secondQ = ((2 * pi * lya * L) / log(secondRad / firstRad)) * (firstTemp - secondTemp);
    double thirdQ = ((4 * pi * lya) / ((1.0 / firstRad) - (1.0 / secondRad))) * (firstTemp - secondTemp);
    cout << "Q1 = " << firstQ << endl;
    cout << "Q2 = " << secondQ << endl;
    cout << "Q3 = " << thirdQ << endl;
}
