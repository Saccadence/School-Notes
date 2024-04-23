Austin Rolfe
4/14/2024
# Looped Temperature Conversion
## Requirements
Using previously used code, loop it and give the user the choice to maintain or break to loop (i.e. multiple conversions).
## Code
```cpp
#include <iostream>


using namespace std;

int main() {

    // Introduction
    cout << "Welcome to the Fahrenheit and Celsius Conversion Suite!" << endl << endl;

    int q = 1;

    while (q == 1) {

        // Declare variables
        int choice = 0;
        float tempIn = 0;
        float tempOut = 0;
        

        // Choose directionality of conversion
        cout << "To begin, please select the direction you wish to convert:" << endl;
        cout << "1) Fahreneheit - Celsius   2) Celsius - Farenheit    0) Exit" << endl;
        cout << "Input: ";
        cin >> choice;


        if (choice == 1) {                  // Fahrenheit to Celsius


            // Prompt user input
            cout << endl << "Please enter a temperature in Farenheit: ";
            cin >> tempIn;

            // Calculate and store tempOut
            tempOut = 5 * (tempIn - 32) / 9;
            
            // Output tempOut (Fahrenheit)
            cout << "Your value of " << tempIn << "° Fahrenheit is equivalent to " << tempOut << "° Celsius!" << endl << endl;

            // Ask to continue
            cout << "Would you like to do another conversion? (0 = No, 1 = Yes)" << endl;
            cout << "Input: ";
            cin >> q;


        } else if (choice == 2) {           // Celsius to Fahrenheit


            // Prompt user input
            cout << endl << "Please enter a temperature in Celsius: ";
            cin >> tempIn;

            // Calculate and store tempOut
            tempOut = tempIn * 9 / 5 + 32;

            // Output tempOut (Fahrenheit)
            cout << "Your value of " << tempIn << "° Celsius is equivalent to " << tempOut << "° Fahrenheit!" << endl << endl;

            // Ask to continue
            cout << "Would you like to do another conversion? (0 = No, 1 = Yes)" << endl;
            cout << "Input: ";
            cin >> q;

        
        } else if (choice == 0) {

            q = 0;
            break;

        } else {cout << "Invalid selection." << endl; q = 1;}  // Output for invalid choice in the beginning

        cout << endl;

    }


    // Terminate the program
    system ("pause");
    return 0;

}
```
## Run Screenshot
![[Screenshot_29.png]]
## Conclusion
I made the mistake of setting q = 1 and creating an infinite loop. Found it and added an exit option for when somebody accidentally says yes (so they don't have to through the whole process to exit). I thought about doing a cases structure, but this looks, and works, just as well. 