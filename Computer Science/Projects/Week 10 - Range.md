Austin Rolfe
3/24/2024
# Range
## Requirements
Create code that allows for the user input of a number and have it spit out the written format of that numerical value.
## Code
```cpp
#include <iostream>

using namespace std;


int main() {

    // Intialize variable
    int number;

    // Prompt user input for number
    cout << "Enter a number between 0 and 10: ";
    cin >> number;
    cout << endl;

    // If Statement
    cout << "If Statement:" << endl;
    if (number == 0) {
        cout << "You've entered the number zero.";
    } else if (number == 1) {
        cout << "You've entered the number one.";
    } else if (number == 2) {
        cout << "You've entered the number two.";
    } else if (number == 3) {
        cout << "You've entered the number three.";
    } else if (number == 4) {
        cout << "You've entered the number four.";
    } else if (number == 5) {
        cout << "You've entered the number five.";
    } else if (number == 6) {
        cout << "You've entered the number six";
    } else if (number == 7) {
        cout << "You've entered the number seven.";
    } else if (number == 8) {
        cout << "You've entered the number eight.";
    } else if (number == 9) {
        cout << "You've entered the number nine.";
    } else if (number == 10){
        cout << "You've entered the number ten.";
    } else {cout << "You've input an invalid number.";}
    cout << endl << endl;

    // Switch Statement
    cout << "Switch Statement:" << endl;
    switch (number) {

        case 0:
            cout << "You've entered the number zero."; break;
        case 1:
            cout << "You've entered the number one."; break;
        case 2:
            cout << "You've entered the number two."; break;
        case 3:
            cout << "You've entered the number three."; break;
        case 4:
            cout << "You've entered the number four."; break;
        case 5:
            cout << "You've entered the number five."; break;
        case 6:
            cout << "You've entered the number six."; break;
        case 7:
            cout << "You've entered the number seven."; break;
        case 8:
            cout << "You've entered the number eight."; break;
        case 9:
            cout << "You've entered the number nine."; break;
        case 10:
            cout << "You've entered the number ten."; break;
        default:
            cout << "You've input an invalid number."; break;

    }
    cout << endl;

    // Terminate the program
    system("Pause");
    return 0;

}
```
## Run Screenshot
![[Pasted image 20240324201406.png]]
## Conclusion
From visually inspecting the difference between if and switch, I can see the appeal of using switch more, although it does seem a bit more limited in it's functionality for expression evaluation, it does a great job of having a robust set of outputs for a set of calculations from a given expression.