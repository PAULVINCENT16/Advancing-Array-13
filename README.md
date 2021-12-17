# Advancing-Array-13
input/output array #include using namespace std; int main() { int i; int user[5]; cout << "Enter 5 numbers: "; for (i = 0; i < 5; i++) { cin >> user[i]; while (cin.fail()) { cin.clear(); cin.ignore(); cout << "Error try again" <<endl; cin >> user[i]; } } if (i == 5) { system("cls"); cout << "you entered number: " << endl; for (int j = 0; j < 5; j++) { cout << user[j] << endl; } } return 0; }

//Array Art #include using namespace std; int main() { int i, j; char patt[][5] = { { '-','-','-','-','-'}, { '-','0','-','0','-'}, {'-','@','@','@','-'}, {'-','^','^','^','-'}, {'-','v','v','v','-'} }; int sizearrRow; int sizearrCol;

sizearrRow = sizeof(patt) / sizeof(patt[0]);
sizearrCol = sizeof(patt[0]) / sizeof(char);

for (i = 0; i < sizearrRow; i++) {
	for (j = 0; j < sizearrCol; j++) {
		cout << patt[i][j] << " ";
	}
	cout << endl;
}


return 0;
}
