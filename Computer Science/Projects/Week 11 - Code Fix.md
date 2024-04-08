Austin Rolfe
4/7/2024
# j Counter - Code Fix
## Requirements
Fix the code so that it prints out the numbers 1 to 10
## Code
```cpp title:Original
#include <iostream>
using namespace std;

int main() {

    for( int j = 1; j > 0; j ++) {
        cout << "j = " << j << endl;
    }

    system("Pause");
    return 0;
}
```
```cpp title:Fixed
#include <iostream>
using namespace std;

int main() {

    for( int j = 1; j < 11; j ++) {     // j > 0 to j < 11
        cout << "j = " << j << endl;
    }

    system("Pause");
    return 0;
}
```
## Run Screenshot
Original - Infinite Loop
![[Screenshot_132.png]]
Fixed (Ignoring formatting preferences) - 1 to 10:
![[Screenshot_133.png]]
## Conclusion
There's a myriad of ways to accomplish this, but I decided to use < instead of <= as I feel it is cleaner and simpler to code it that way