#include <iostream>
#include <cmath>
using namespace std;
long long binhphuong(long long n)
{
	if (n < 1)
		return 0;
	return pow(n,3) + binhphuong(n - 1);
}
int main()
{
	long long a;
	cin >> a;
	cout << binhphuong(a) << endl;
	return 0;
}
