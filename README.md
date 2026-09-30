# -GRRRMONDAYS
/***************************
* Автор: Полудинцев Никита *
* Вариант: 8               *
* Название: Лаб №1         *
***************************/

#include <iostream>
#include <cmath>

using namespace std;

int main() {

    const double pi = 3.14159265358979;
    
    double lya, firstRad, secondRad, firstTemp, secondTemp, square, lenght, firstQ, secondQ, thirdQ;
    
    firstRad = 25.2 / 100.0;
    secondRad = 29.3 / 100.0;
    firstTemp = 264.0;
    secondTemp = 43.0;

    cout << "Lya:"; cin >> lya;
    
    cout << "Square:"; cin >> square;

    cout << "Lenght:"; cin >> lenght;

    firstQ = ((lya * square) / (secondRad - firstRad)) * (firstTemp - secondTemp);

    secondQ = ((2 * pi * lya * lenght) / log(secondRad / firstRad)) * (firstTemp - secondTemp);

    thirdQ = ((4 * pi * lya) / ((1.0 / firstRad) - (1.0 / secondRad))) * (firstTemp - secondTemp);

    cout << "Q1 = " << firstQ << ", Q2 = " << secondQ << ", Q3 = " << thirdQ << endl;
    
}
