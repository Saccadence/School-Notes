Austin Rolfe
03/10/2024
# Age Evaluation
## Requirements
Write and execute code that takes the user's name (string) and their age (int) and assess whether they are an adult or not (>= 18)
## Code
```cpp
#include <iostream>


using namespace std;

int main() {

    // Declaring variables
    string firstName;
    int age;

    // CLI prompt for name and age
    cout << "What is your first name? ";
    cin >> firstName;
    cout << "How many years old are you? ";
    cin >> age;

    // Evaluation and output of age determination (adult or not)
    if (age >= 18) {
        cout << endl << firstName << ", you are an adult!" << endl;
    } else {
        cout << endl << firstName << ", you not are an adult!" << endl;
    }


    // Terminate the program
    system ("pause");
    return 0;

}
```
## Run Screenshot
![[Screenshot_125.png]]
## Conclusion
I learned how to use a string declaration to utilize *strings* of characters, either via hardcoded input or user input
## Test Cases (If Any)
| Test Case(s) | Test 1  | Test 2  | Test 3  |
| :----------- | ------- | ------- | ------- |
| Input        | 21      | 17      | 67      |
| Expected     | ==Adult | !=Adult | ==Adult |
| Actual       | ==Adult | !=Adult | ==Adult |
