Austin Rolfe
4/21/2024
# Explain
## Requirements
Comment what each line of this program with what it does
## Code
```cpp
// Programmer Explain the results  
#include <iostream>  
using namespace std;  
#include <cmath>  
#include <iomanip>

int main ()  
{  
	int arrayIntegers[50] = {0};    // Declare integer array with 50 values set to 0 
	int i = 0;                      // Declare i as integer set to 0
	  
	cout << fixed;                  // Force a consistent number of decimal places 
	cout << setprecision(0);        // How many decimal places for above 
	cout << setw(50);               // Set width of output (min/max)
	cout << right;                  // Set the code to output to the right side of the defined width above
	  
	for (i = 0 ; i < 50 ; i++ ) {   // Loop when i is < 50, start at 0 and add 1 each loop 
		cout << " ------------------------------------------- " << endl;   // Output a dividing line (clearer data ouput) 
		cout << " 2 ^ " << i << " = " << pow(2.0,i) << endl;;              // Output 2 ^ i = (2.0 ^ i) (where i is the loop number)
		arrayIntegers[i] = pow(2.0,i); // Set the array values (1-50 or index 0-49) to 2.0 ^ of the index value of the current # of loops 
		cout << " 2 ^ " << i << " = " << arrayIntegers[i] << endl;         // Output 2 ^ the value in the array at index i (where i is the loop number) 
	}
	  
	system ("pause");   // Pause the code before returning 0 and exiting 
 return 0;  
}
```
## Conclusion
The difference in the output of the array value and the integer value is the integer value is signed and the array values aren't making them overflow