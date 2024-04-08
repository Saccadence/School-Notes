Austin Rolfe
4/7/2024
# Walking Downstairs
## Requirements
Create a program that visually adjusts a person walking down a set of stairs in the console output (6 space width movement each time)
## Code
```cpp
#include <iostream>
#include <iomanip>

using namespace std;


int main() {

    int stairs;

    cout << "How many stairs should the man walk down? ";
    cin >> stairs;
    cout << endl << "Here he goes!" << endl << endl;

    for (int n = 0; n <= stairs; n++) {

        cout << setw((n*6)+5) <<"* o  " << endl;
        cout << setw((n*6)+5) <<"*/|\\ " << endl;
        cout << setw((n*6)+5) <<"*/ \\ " << endl;
        cout << setw((n*6)+5) <<"*****" << endl;

    }


    system("Pause");
    return 0;

}
```
## Run Screenshot
![[Screenshot_22.png]]
## Conclusion
setw() defines width, rather than padding, of a console output