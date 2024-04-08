Austin Rolfe
4/7/2024
# Multiplication Table
## Requirements
Create a multiplication table using two nested for loops
## Code
```cpp
#include <iostream>
#include <iomanip>

using namespace std;


int main() {

    int row = 1;

    for (;;) {
        if (row < 13) {
            int column = 1;
            for (;;) {
                if (column < 13) {
                    cout << setw(4) << row * column;
                    column ++;
                } else {break;}
            }
            cout << endl;

            row++;
        } else {break;}
    }


    system("Pause");
    return 0;
}
```
## Run Screenshot
![[Screenshot_135.png]]
## Conclusion
Fairly simple, but neat, code and output. The logic behind creating this was at least a bit more interesting than previous assignments