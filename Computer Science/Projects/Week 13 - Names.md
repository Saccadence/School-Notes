Austin Rolfe
4/21/2024
# Names
## Requirements
Write code that prompts a user to input 6 names and store them in an array to be accessed later
## Code
```cpp
#include <iostream>
#include <string>

using namespace std;


int main() {

    string names[6];

    // Input
    for (int n = 0; n < 6; n++) {
        cout << "Enter Name #" << (n + 1) << ": ";
        cin >> names[n];
    }
    cout << endl;

    // Output
    for (int i = 0; i < 6; i++){
        cout << "Name #" << (i + 1) << " is " << names[i] << ".";
        cout << endl;
    }
    cout << endl;


    system ("Pause");
    return 0;

}
```
## Run Screenshot
![[Screenshot_31.png]]
## Conclusion
Arrays are cool and you definitely should make this the second assignment and ditch the previous one since this actually does more for students