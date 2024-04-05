Austin Rolfe
3/3/2024
# Code Fix - Height (Feet to Inches)
## Requirements
Develop a program that calculates how tall someone is in inches from a user input of feet and inches.
## Code
```cpp
#include <iostream>


using namespace std;

int main () {

    // Initialization of variables
    int feet = 0;
    int inches = 0;

    // CLI I/O (Prompt/Input)
    cout << "How tall are you?" << endl << "Feet: ";
    cin >> feet;
    cout << "Inches: ";
    cin >> inches;

    // Conversion of Data
    inches = feet * 12 + inches;

    // CLI Output of Conversion (inches)
    cout << endl << "You are " << inches << " inches tall!" << endl;

    // Termination of Program
    system("Pause");
    return 0;

}
```
## Run Screenshot
![[Pasted image 20240303012612.png]]
## Conclusion
I learned how to more rigorously check for errors and how to document those changes
## Test Cases (If Any)
| Test Case(s) | Test 1 | Test 2 |
| :----------- | ------ | ------ |
| Input        | 5' 9"  | 10' 2" |
| Expected     | 69"    | 122"   |
| Actual       | 69"    | 122"   |
