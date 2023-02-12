# zadanie10

/*
Лабораторная 3 задание 3
Найти наибольшую степень двойки, на которую делится заданное число.
*/

#include <bits/stdc++.h>
using namespace std;

int stdel2(int n)
{
	setlocale(LC_ALL, "Russian");
	int res = 0;
	for (int i = n; i >= 1; i--) 
    {
	
		if ((i & (i - 1)) == 0) {
			res = i;
			break;
		}
	}
	return res;
}

// ****************************//
int main()
{
    int n;
    cout<<"значние n"<<endl;
	cin>> n;
	cout << stdel2(n);
    system("pause");
	return 0;
}
