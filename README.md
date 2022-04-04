# Codeforcescpp-143A
#include <bits/stdc++.h>
using namespace std;

int main() {
	int r1, r2, c1, c2, d1, d2;
	cin >> r1 >> r2 >> c1 >> c2 >> d1 >> d2;
	if (r1 + r2 == c1 + c2 && c1 + c2 == d1 + d2) {
		int b = (r1 + d2 - c1) / 2;
		int a = r1 - b;
		int c = d2 - b;
		int d = c2 - b;
		if (a != b && a != c && a != d && b != c && b != d && c != d &&
			a < 10 && b < 10 && c < 10 && d < 10 && a > 0 && b > 0 && c > 0 &&
			d > 0)
			cout << a << " " << b << endl << c << " " << d;
		else
			cout << -1;
	} else
		cout << -1;
	return 0;
}
