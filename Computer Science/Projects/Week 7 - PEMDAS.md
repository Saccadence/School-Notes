Austin Rolfe
3/3/2024
# Assignment Title
## Requirements
Write a program with the declarations:
- double a = 18, b = 6, c = 3
Then, calculate:
- a + b / c
- (a + b) / c
- a + (b / c)
Finally, explain the difference, or lack thereof, in the output(s).
## Code
```cpp
#include <iostream>

using namespace std;

int main() {
	
    // Declaration of Variables
    double a = 18;
    double b = 6;
    double c = 3;

    // Computation and CLI Output of Variables
    cout << a + b / c << endl;
    cout << (a + b) / c << endl;
    cout << a + (b / c) << endl;

    // Termination of the Program
    system ("Pause");
    return 0;

}
```
## Run Screenshot
![[Pasted image 20240303014307.png]]
## Conclusion
The difference in output 1 and 3 from out 2 comes down to the fact that, in order of operations, output 2 is the only manipulation of the variables in the expression that meaningfully modified how the code interacted calculated them together.
## Test Cases (If Any)
N/A