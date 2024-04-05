Austin Rolfe
3/24/2024
# Ticket Price
## Requirements
Create a switch statement version of the if else code provided in the lecture.
## Code
```cpp
#include <iostream>

using namespace std;


int main() {

    // Initialize the variable
    int age;

    // Prompt and store UserInput of age
    cout << "Enter age to see ticket price: ";
    cin >> age;
    cout << endl;

    // Evaluate age and output it's corrsponding ticket price
    if (age >= 0) {

        cout << "The ticket price is: ";

        switch (age) {

            case 0: cout << "$0.00"; break;
            case 1: cout << "$0.00"; break;
            case 2: cout << "$0.00"; break;
            case 4: cout << "$0.00"; break;
            case 5: cout << "$0.00"; break;

            case 6: cout << "$10.00"; break;
            case 7: cout << "$10.00"; break;
            case 8: cout << "$10.00"; break;
            case 9: cout << "$10.00"; break;
            case 10: cout << "$10.00"; break;
            case 11: cout << "$10.00"; break;
            case 12: cout << "$10.00"; break;

            case 13: cout << "$18.00"; break;
            case 14: cout << "$18.00"; break;
            case 15: cout << "$18.00"; break;
            case 16: cout << "$18.00"; break;
            case 17: cout << "$18.00"; break;
            case 18: cout << "$18.00"; break;
            case 19: cout << "$18.00"; break;
            case 20: cout << "$18.00"; break;
            case 21: cout << "$18.00"; break;
            case 22: cout << "$18.00"; break;
            case 23: cout << "$18.00"; break;
            case 24: cout << "$18.00"; break;
            case 25: cout << "$18.00"; break;
            case 26: cout << "$18.00"; break;

            default: cout << "$15.00"; break;

        }
    } else {cout << "Invalid Input!";}
    cout << endl;


    //  Terminate the program
    system("Pause");
    return 0;

}
```
## Run Screenshot
![[Pasted image 20240324210627.png]]
## Conclusion
I think it's obvious that the better solution is to use if else for a situation that evaluates range, there are some extensions that allow for the compiler to read a form of switch statements as "0 ... 5" for values within [0, 5]. It's also not entirely unreadable as it can display range as a visual rather than a numerical one, but it is highly impractical to make and even more impractical in larger ranges.