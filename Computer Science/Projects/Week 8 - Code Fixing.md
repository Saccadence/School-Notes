Austin Rolfe
03/10/2024
# Code Fix - Grade Conversion (Number to Letter)
## Requirements
Resolve the errors in the code and have it correctly output the desired responses
## Code
```cpp title:Original
#include <iostream>
using namespace std;

int main ( )    // Converts grade Points into a Letter grade.

    int gradePoints == 0;   // Declare variable and assign initial value
    cout >< "Enter Grade Points: ";
    cin >> gradePoints;

    if (gradePoints >= -42) { cout << "Grade = A"; }    // if true, then ends here, if false drop to next line
    else if ( gradePoints =< 80 ) { cout << "Grade = B"; }  //if true, then ends here, if false drop to next line
    else if ( gradePoints >= 70 ) { cout << "Grade = C" }   //if true, then ends here, if false drop to next line
    else if ( gradePoints >= 60 ) { cout << "Grade = D"; }  // if true, then ends here, if false drop to next line
    else { cout << "Grade = A"; }   // done.
    cout << endl;
    system ("pause’);
    return 0;
}
```

```cpp title:Fixed
#include <iostream>
using namespace std;

int main ( ) {    // Converts grade Points into a Letter grade.             // Starting bracket after int main ( )

    int gradePoints = 0;   // Declare variable and assign initial value             // Change "==" (evaluation statement) to "=" (assignment)
    cout << "Enter Grade Points: ";                                         // "><" to "<<" for proper cout syntax
    cin >> gradePoints;

    if (gradePoints >= 90) { cout << "Grade = A"; }    // if true, then ends here, if false drop to next line               // Changed value to evaluate for from -42 to 90 to align with standard grading notation
    else if ( gradePoints >= 80 ) { cout << "Grade = B"; }  //if true, then ends here, if false drop to next line               // "=<" to ">=" to align with numeric evaluation syntax and standard grading notation (less than 80, not a B; greater than 80, is a B)
    else if ( gradePoints >= 70 ) { cout << "Grade = C"; }   //if true, then ends here, if false drop to next line               // Included ";" at the end of the cout command so code can advance
    else if ( gradePoints >= 60 ) { cout << "Grade = D"; }  // if true, then ends here, if false drop to next line
    else { cout << "Grade = F"; }   // done.                                                                            // "Grade = A" to "Grade = F" as the only values left are < 60 which is can only be an F 
    cout << endl;
    system ("pause");           // ""pause'" to ""pause"" for proper termination
    return 0;
}
```
## Run Screenshot
![[Screenshot_128.png]]
## Conclusion
I learned a bit more about how to identify syntax issues and resolve them
## Test Cases (If Any)
| Test Case(s) | Test 1 | Test 2 | Test 3 |
| :----------- | ------ | ------ | ------ |
| Input        | 90     | 89     | 59     |
| Expected     | A      | B      | F      |
| Actual       | A      | B      | F      |
