Austin Rolfe
4/21/2024
# Reverse Names
## Requirements
With two arrays, have a set of names in order and another in reverse
## Code
```cpp
#include <iostream>
#include <string>

using namespace std;


int main() {

    string forwardNames[10] = {"Fred", "Tuyet", "Annie", "Moe", "Ria", "Luke", "Jim", "May", "Rex", "Omar"};
    string reverseNames[10] = {" "};

    // Input (Array Reversal)
    int j = 9;
    for (int i = 0; i < 10; i++) {
        reverseNames[i] = forwardNames[j];
        j--;
    }

    // Output
    cout << "Forward Order:" << endl;
    for (int i = 0; i < 10; i++) {

        cout << forwardNames[i];

        if ((i + 1) < 10) {
            cout << " - ";
        } else {cout << endl << endl;}

    }

    cout << "Reverse Order:" << endl;
    for (int i = 0; i < 10; i++) {
        
        cout << reverseNames[i];
        
        if ((i + 1) < 10) {
            cout << " - ";
        } else {cout << endl;}

    }


    system ("Pause");
    return 0;

}
```
## Run Screenshot
![[Screenshot_33 1.png]]
## Conclusion
Not sure how I was to use 2 arrays for the initial setup of the array (unless I just misunderstood the assignment), but I did use 3 total, 1 for setup and 2 for output