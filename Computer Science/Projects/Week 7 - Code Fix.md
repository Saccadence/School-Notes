Austin Rolfe
3/3/2024
# Code Fix - Height (Feet to Inches)
## Requirements
Fix any errors in the code and document them through comments on each line fixed. Do not add or delete any lines in the source code.
## Code
```cpp
#include <iostream>                     // "include" after "#" and "<" before "iostream"; "using" moved to line 3

using namespace std;                            // Moved "using" from line 1 in front of "namespace std;"

int main ( ) { // start program         // "Int" to "int", removed space between slashes before comment "start program", and added open bracket "{"

// Declare and Initialize Variables int         // Added another slash to make this line an actual comment
    int height = 0;                     // Added "int" before height
    int feet = 0;                               // Added semicolon
    int inches = 0;                     // "Int" to "int"

    // Prompt for height cout >> “Enter your height in inches: ‘;
    cin >> height;                             // "><" to ">>" and "Height" to height

    // Calculate Height in feet and inches
    feet = height / 12;                 // Moved "= feet" to the left side ("feet =")
    inches = height % 12;

    //Print out height in feet and inches
    cout << "You are " << feet << " feet and " << inches << " inches." << endl; // removed second "t" in "coutt", resolved all copying errors from Word for " symbol, changed "< FEET" to "<< feet", "<>" to "<<", ">> "inches" ;" to "<< " inches."", and added "<< endl;"

    system("Pause"); // Mac user comment out this line by placing // in front of it.
    // PC users -Hint replace the “ with the ones on your computer–coping code cause error, so just type it.
    return 0;
} // end of program
```
## Run Screenshot
![[Pasted image 20240303010448.png]]
## Conclusion
I learned how to more rigorously check for errors and how to document those changes
## Test Cases (If Any)
Input Value: 8888" | 234" | 43"
Expected Output: 740' 8" | 19' 6" | 3' 7"
Actual Output: 740' 8" | 19' 6" | 3' 7"