Austin Rolfe
03/10/2024
# Grade Conversion
## Requirements
Use nested "if else..." statements to assess numeric grades and output their corresponding letter grade
## Code
```cpp
#include <iostream>


using namespace std;

int main() {

    // Declare grade variable
    double grade;

    // Prompt user for numeric grade
    cout << "What is your grade? ";
    cin >> grade;

    // Nested else if - Evaluate numeric grade and output corresponding letter grade
    if (grade >100) {
        cout << endl << "Your letter grade is: A+" << endl << "You're an amazing student! (For better or for worse...)" << endl;
    } else if ((grade >= 90) && (grade <= 100)) {
        cout << endl << "Your letter grade is: A" << endl;
    } else if ((grade >= 80) && (grade < 90)) {
        cout << endl << "Your letter grade is: B" << endl;
    } else if ((grade >= 70) && (grade < 80)) {
        cout << endl << "Your letter grade is: C" << endl;
    } else if ((grade >= 60) && (grade < 70)) {
        cout << endl << "Your letter grade is: D" << endl;
    } else if ((grade > 0) && (grade < 60)) {
        cout << endl << "Your letter grade is: F" << endl;
    } else {cout << endl << "You don't deserve to be a student because you're clearly on another planet." << endl;}

    
    // Terminate program
    system ("pause");
    return 0;

}
```
## Run Screenshot
![[Screenshot_126.png]]
## Conclusion
I learned how to use nested "else if.." statements to evaluate a value to find an output that would best correspond with it
## Test Cases (If Any)
| Test Case(s) | Test 1 | Test 2 | Test 3 |
| :----------- | ------ | ------ | ------ |
| Input        | 100    | 87     | 101    |
| Expected     | A      | B      | A+     |
| Actual       | A      | B      | A+     |
## Classic
![[Pasted image 20240308012429.png]]
Thought I'd share my git commits cause just when I thought I had fixed the problem, I had made a small error somewhere else and then I missed something else.
- Point of Clarification: The git repo is private and inaccessible to anyone else. I use it solely for archiving changes, accessing my project elsewhere (mobile/laptop/desktop), and visually seeing my change log per line in Visual Studio Code