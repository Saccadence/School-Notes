Austin Rolfe
due/date/2024
# Assignment Title
## Requirements
Evaluate expressions by putting them in C++ and running the code
## Code
```cpp
#include <iostream>


using namespace std;

int main () {

    bool a = 2;
    bool b = 0;

    cout << boolalpha << " 1. (13 > 42) || (4 < 9) = " << ((13 > 42) || (4 < 9)) << endl;
    cout << boolalpha << " 2. (11 > 3) && (7 <= 7) = " << ((11 > 3) && (7 <= 7)) << endl;
    cout << boolalpha << " 3. !false = " << !false << endl;
    cout << boolalpha << " 4. !(31 != 4) = " << !(31 != 4) << endl;
    cout << boolalpha << " 5. (9 != 7) && !0 = " << ((9 != 7) && !0) << endl;
    cout << boolalpha << " 6. 2 = " << a << endl;
    cout << boolalpha << " 7. 0 = " << b << endl;
    cout << boolalpha << " 8. 0 || 1 || 42 = " << (0 || 1 || 42) << endl;
    cout << boolalpha << " 9. !!0 = " << !!0 << endl;
    cout << boolalpha << "10. 1 && 1 && 1 && 1 && 1 && 0 = " << (1 && 1 && 1 && 1 && 1 && 0) << endl;


    // Terminate the program
    system("pause");
    return 0;

}
```
## Run Screenshot
![[Pasted image 20240317195322.png]]
## Conclusion
Didn't really learn much about this except for how to properly evaluate numbers by themselves by assigning them to a bool variable (otherwise it just spits out the number). Took a logic class so most of this just rehashing things I did for 4 months straight last semester. 