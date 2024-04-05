Austin Rolfe
03/10/2024
# Temperature Conversion (F <-> C)
## Requirements
Create a program that allows the user to select between F to C or C to F and output the correct conversion (with decimal places).
## Code
```cpp
#include <iostream>


using namespace std;

int main() {

    // Declare variables
    int choice;
    float tempIn;
    float tempOut;


    // Introduction
    cout << "Welcome to the Fahrenheit and Celsius Conversion Suite!" << endl << endl;

    // Choose directionality of conversion
    cout << "To begin, please select the direction you wish to convert:" << endl;
    cout << "1) Fahreneheit - Celsius   2) Celsius - Farenheit" << endl << "Input: ";
    cin >> choice;

    if (choice == 1) {                  // Fahrenheit to Celsius

        // Prompt user input
        cout << endl << "Please enter a temperature in Farenheit: ";
        cin >> tempIn;

        // Calculate and store tempOut
        tempOut = 5 * (tempIn - 32) / 9;
        
        // Output tempOut (Fahrenheit)
        cout << "Your value of " << tempIn << "° Fahrenheit is equivalent to " << tempOut << "° Celsius!" << endl;

    } else if (choice == 2) {           // Celsius to Fahrenheit

        // Prompt user input
        cout << endl << "Please enter a temperature in Celsius: ";
        cin >> tempIn;

        // Calculate and store tempOut
        tempOut = tempIn * 9 / 5 + 32;

        // Output tempOut (Fahrenheit)
        cout << "Your value of " << tempIn << "° Celsius is equivalent to " << tempOut << "° Fahrenheit!" << endl;

    } else {cout << "Invalid selection." << endl;}  // Output for invalid choice in the beginning


    // Terminate the program
    system ("pause");
    return 0;

}
```
## Run Screenshot
![[Pasted image 20240309114923.png]]
## Conclusion
I learned about how to setup a user selection system using if else. I also learned a bit about the difference in ASCII and Unicode and how they get interpreted/stored in RAM. Having done coding some before, I also explored some ideas of input format verification.
## Test Cases (If Any)
| Test Case(s) | Test 1    | Test 2    |
| :----------- | --------- | --------- |
| Input        | 67 F      | 19.4444 C |
| Expected     | 19.4444 C | 66.9999 F |
| Actual       | 19.4444 C | 66.9999 F |
