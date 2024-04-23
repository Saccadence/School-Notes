Austin Rolfe
4/21/2024
# Variables vs. Arrays
## Requirements
Write a program first using variables and then arrays (within the same program):
- 17 variables/values initialized to 0
	- User input of value then output value (basically a confirmation of functionality)
- Use loop for array IO
## Code
```cpp
#include <iostream>

using namespace std;


int main() {

// Part 1

    cout << "Variable Functionaility" << endl << endl;

    // Variable Declarations
    int number1 = 0;
    int number2 = 0;
    int number3 = 0;
    int number4 = 0;
    int number5 = 0;
    int number6 = 0;
    int number7 = 0;
    int number8 = 0;
    int number9 = 0;
    int number10 = 0;
    int number11 = 0;
    int number12 = 0;
    int number13 = 0;
    int number14 = 0;
    int number15 = 0;
    int number16 = 0;
    int number17 = 0;

    // I/O Requests
    cout << "Input a value for number 1: ";
        cin >> number1;
        cout << number1;
        cout << endl << endl;

    cout << "Input a value for number 2: ";
        cin >> number2;
        cout << number2;
        cout << endl << endl;

    cout << "Input a value for number 3: ";
        cin >> number3;
        cout << number3;
        cout << endl << endl;

    cout << "Input a value for number 4: ";
        cin >> number4;
        cout << number4;
        cout << endl << endl;

    cout << "Input a value for number 5: ";
        cin >> number5;
        cout << number5;
        cout << endl << endl;

    cout << "Input a value for number 6: ";
        cin >> number6;
        cout << number6;
        cout << endl << endl;

    cout << "Input a value for number 7: ";
        cin >> number7;
        cout << number7;
        cout << endl << endl;

    cout << "Input a value for number 8: ";
        cin >> number8;
        cout << number8;
        cout << endl << endl;

    cout << "Input a value for number 9: ";
        cin >> number9;
        cout << number9;
        cout << endl << endl;

    cout << "Input a value for number 10: ";
        cin >> number10;
        cout << number10;
        cout << endl << endl;

    cout << "Input a value for number 11: ";
        cin >> number11;
        cout << number11;
        cout << endl << endl;

    cout << "Input a value for number 12: ";
        cin >> number12;
        cout << number12;
        cout << endl << endl;

    cout << "Input a value for number 13: ";
        cin >> number13;
        cout << endl << number13;
        cout << endl << endl;

    cout << "Input a value for number 14: ";
        cin >> number14;
        cout << number14;
        cout << endl << endl;

    cout << "Input a value for number 15: ";
        cin >> number15;
        cout << number15;
        cout << endl << endl;

    cout << "Input a value for number 16: ";
        cin >> number16;
        cout << number16;
        cout << endl << endl;

    cout << "Input a value for number 17: ";
        cin >> number17;
        cout << number17;
        cout << endl << endl;

    cout << endl;


// Part 2

    cout << "----------------------------------" << endl << endl;
    cout << "Array Functionality" << endl << endl;

    // Array Declaration
    int number[17] = {0};

    // I/O Requests
    for (int i = 0; i < 17; i++) {
        cout << "Input a value for number " << i + 1 << ": ";
        cin >> number[i];
        cout << number[i];
        cout << endl << endl;
    }


    system ("Pause");
    return 0;

}
```
## Run Screenshot
![[Screenshot_30.png]]
## Conclusion
As anyone might have expected, when iterating with any given value, it's better to automate the creation of those iterations when possible. This is especially the case because any edit made to the iteration(s) needs to be reflected amongst them all and this is best/easiest to do when in a loop.