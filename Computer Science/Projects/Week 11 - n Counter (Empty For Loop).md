Austin Rolfe
4/7/2024
# n Counter (Empty For Loop)
## Requirements
Output the loop count of n where the for statement must have an empty header (;;)
## Code
```cpp
#include <iostream>

using namespace std;


int main() {

    int n = 1;

    for ( ; ; ) {

        if (n < 11) {
            cout << n << endl;
            n++;
        } else {break;}
    }


    system("Pause");
    return 0;
}
```
## Run Screenshot
![[Screenshot_134.png]]
## Conclusion
Pretty interesting to find that this isn't a super uncommon thing in coding. Makes sense given the practical application of having an infinite loop running that doesn't necessitate evaluating an expression for the loop to start, rather you can just add code within it to break out of the loop.