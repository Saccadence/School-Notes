Austin Rolfe
03/17/2024
# Assignment Title
## Requirements
Write code that allows for the input of a 0 or 1 and will output the result of conditional relationships in a truth table. Must run for all 8 rows and work.
## Code
```cpp
#include <iostream>


using namespace std;

// Declare variables and assign false as default value to be manipulated later - Assigned outside functions so they both can see these variables
bool a = false;
bool b = false;
bool c = false;
int row = 1;              // Used to output row #

void truth ();      // Declaring so main function can evaluate truth function

int main () {

    // Instruct user on first (and future) input
    cout << "Please enter 0 or false, and 1 or true for each variable" << endl << endl;

    // Evaluation and output through simplified function repeating
    truth();
    truth();
    truth();
    truth();
    truth();
    truth();
    truth();
    truth();


    // Terminate the program
    system("pause");
    return 0;

}

// Function to evaluate bools - below main so that manipulation of vairables transfers
void truth () {

    cout << "A = "; cin >> a;
    cout << "B = "; cin >> b;
    cout << "C = "; cin >> c;
    cout << endl << "----------------------------------" << endl;
    cout << "Row #" << row << ":";
    cout << endl << boolalpha << "A = " << a << " | B = " << b << " | C = " << c << endl << endl;

    if (a || b) {
        cout <<"A || B = TRUE";    
    } else {cout << "A || B = FALSE";}

    cout << endl;

    if ((a || b) && c) {
        cout <<"(A || B) && C = TRUE";
    }  else {cout << "(A || B) && C = FALSE";}
    cout << endl << "----------------------------------" << endl << endl;

    row ++;

}
```
## Run Screenshot
![[Pasted image 20240317193652.png]]
## Conclusion
I learned a lot about how to implement functions, mostly in avoidance of a for or while loop. Although not completely following the requirements, it does effectively the same things as running the program 8 times.
## Test Cases (If Any)
| Test Case(s) | Test 1                                     | Test 2                                    |
| :----------- | ------------------------------------------ | ----------------------------------------- |
| Input        | A = 0<br>B = 1<br>C = 0                    | A = 1<br>B = 0<br>C = 1                   |
| Expected     | A \|\| B = TRUE<br>(A \|\| B) && C = FALSE | A \|\| B = TRUE<br>(A \|\| B) && C = TRUE |
| Actual       | A \|\| B = TRUE<br>(A \|\| B) && C = FALSE | A \|\| B = TRUE<br>(A \|\| B) && C = TRUE |
