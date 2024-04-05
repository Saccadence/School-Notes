Austin Rolfe
3/24/2024
# Main Menu
## Requirements
Create a program that prints out a "menu" for a user to select from and evaluate their choice using a switch statement
## Code
```cpp
#include <iostream>

using namespace std;


int main() {

    // Initialize the variable
    int menuChoice;

    // Output the menu choices and ask for user input
    cout << "Welcome to The Coding Game!" << endl << endl
    << "Please choose your method of play:" << endl;

    cout << "1) Singleplayer" << endl;
    cout << "2) Versus - CPU" << endl;
    cout << "3) Versus - Player" << endl;
    cout << "4) Multiplayer - Internet" << endl;
    cout << "5) Exit" << endl << endl;

    cout << "Selection (use the corresponding number): ";
    cin >> menuChoice;
    cout << endl;

    // Evaluate and output User's selection
    switch (menuChoice) {

        case 1:
            cout << "You've selected:" << endl << "Singleplayer"; break;
        case 2:
            cout << "You've selected:" << endl << "Versus - CPU"; break;
        case 3:
            cout << "You've selected:" << endl << "Versus - Player"; break;
        case 4:
            cout << "You've selected:" << endl << "Multiplayer - Internet"; break;
        case 5:
            cout << "You've selected:" << endl << "Exit"; break;
        default:
            cout << "Invalid Response."; break;
    }
    cout << endl;

    
    // Terminate the program
    system("Pause");
    return 0;

}
```
## Run Screenshot
![[Pasted image 20240324204344.png]]
## Conclusion
This was one of the most practical applications that I had wanted to use for a bit. Syntax is easy and even easier to follow