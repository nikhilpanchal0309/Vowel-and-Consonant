#include <iostream>
using namespace std;

int main() {
    char ch;

    cout << "Enter an alphabet: ";
    cin >> ch;

    if (ch >= 'A' && ch <= 'Z')
        ch = ch + 32;

    if (ch >= 'a' && ch <= 'z') {
        if (ch == 'a' || ch == 'e' || ch == 'i' ||
            ch == 'o' || ch == 'u') {
            cout << "Vowel";
        } else {
            cout << "Consonant";
        }
    } else {
        cout << "Invalid input";
    }

    return 0;
}
