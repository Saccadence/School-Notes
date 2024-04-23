Austin Rolfe
4/21/2024
# Multiplication Table
## Requirements
Make a multiplication table using 2-dimensional arrays that's 11 x 11 and output each of the values you store in the array to make a multiplication table
## Code
```cpp
#include <iostream>
#include <iomanip>

using namespace std;


int main() {

    int multiTable[11][11] = {0};
    
    // Input
    int column = 0;
    int row = 0;
    for (;;) {
        if (row < 11) {
            column = 0;
            for (;;) {
                if (column < 11) {
                    multiTable[row][column] = ((row + 1) * (column + 1));
                    column ++;
                } else {break;}
            }
            row++;
        } else {break;}
    }

    // Output
    row = 0;
    for (;;) {
        if (row < 11) {
            column = 0;
            for (;;) {
                if (column < 11) {
                    cout << setw(4) << multiTable[row][column];
                    column ++;
                } else {break;}
            }
            cout << endl;
            row++;
        } else {break;}
    }

    system ("Pause");
    return 0;

}
```
## Run Screenshot
![[Screenshot_32.png]]
## Conclusion
It's the same thing as the previous multiplication table, minus a value, however I made the mistake of not checking for bounds originally and that served a learning moment of things to be more cautious of