#include <iostream>
#include <bitset>
#include <vector>
#include <string>
#include <cmath>
#include <algorithm>
#include <set>
#include <map>
#include <cmath>
#include <iomanip>


using namespace std;

bool pal(string);

int main() {
	string s;
	while (cin >> s) {
		set<string>palin;
		for (int i = 0; i < s.size(); ++i) {
			for (int j = 1; j <= s.size() - i; ++j) {
				string str = s.substr(i, j);
				if (pal(str)) palin.insert(str);
			}
		}
		cout << "The string '" << s << "' contains " << palin.size() << " palindromes.\n";
	}
	return 0;
}

bool pal(string s) {
	for (int i = 0; i < s.size()/2; ++i)
		if (s[i] != s[s.size() - 1 - i])
			return false;
	return true;
}
