# Array Loop
#include <iostream>;
#include <string>
using namespace std;

int main() {
	const int MAX_NAMES = 100;
	string names[MAX_NAMES];

	int count;
	for (count = 0; count < MAX_NAMES; count++) {
		cout << "Please enter a name: ";
		cin >> names[count];
		if (names[count] == "stop") {
			break;
		}
	}

	cout << "The names you entered were: " << endl;
	for (int i = 0; i < count; i++) {
		cout << names[i] << endl;
	}

	return 0;
}
