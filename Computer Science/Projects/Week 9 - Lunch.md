Austin Rolfe
due/date/2024
# Assignment Title
## Requirements
Have a user input 6 condition responses and then evaluate if they can eat lunch at McDonalds based on the sum evaluation of those 6 conditions.
## Code
```cpp
#include <iostream>


using namespace std;

int main () {

    // Declare variables
    bool amHungry;
    bool haveMoney;
    bool haveTransportation;
    bool haveTime;
    bool keepDiet;
    bool openRestaurant;

    // Provide information
    cout << "Please answer each question with a 1 or true, or 0 or false for yes and no respectively.";
    cout << endl << "This will ensure that you get the most accurate result for whether you can eat at McDonalds or not :)";

    // Prompt user input
    cout << endl << endl << "Are you hungry?" << endl << "Response: ";
    cin >> amHungry;
    cout << endl << "Do you have money to spend at McDonalds?" << endl << "Response: ";
    cin >> haveMoney;
    cout << endl << "Do you have a functional form of transportation?" << endl << "Response: ";
    cin >> haveTransportation;
    cout << endl << "Do you have time to go and eat at McDonalds?" << endl << "Response: ";
    cin >> haveTime;
    cout << endl << "Is McDonalds apart of your diet? (If you don't have one, input 1 or true)" << endl << "Response: ";
    cin >> keepDiet;
    cout << endl << "Is McDonalds open right now?" << endl << "Response: ";
    cin >> openRestaurant;

    // Evaluate all the response together
    if ((amHungry && haveMoney && haveTransportation && haveTime && keepDiet && openRestaurant) == true) {
        cout << endl << "Congratulations! You're able to get lunch at McDonalds, have a great meal!";
    } else {cout << endl << "Unfortunately, you do not satisfy all the necessary criteria to get lunch at McDonalds right now.\nPlease reevaluate your responses marked 0 or false, thank you!";}
    cout << endl;

    // Terminate the program
    system("pause");
    return 0;

}
```
## Run Screenshot
![[Pasted image 20240317194449.png]]
## Conclusion
I didn't really feel I got much from this program. It was flat boring and didn't really provide anything unique or special (and I felt that it decreased the functionality/robustness of the code from the previous rendition of this assignment, which made it feel worse)
## Test Cases (If Any)
All test cases succeeded (i.e. any false value returned false for the whole expression)