Austin Rolfe
4/14/2024
# Code Fix
## Requirements
Fix the program so that it is no longer an infinite loop
## Code
```cpp title:Original
#include <iostream>

using namespace std;


int main() {
	
	int i = 0; // 1st element of loop
	
	while (i >= 0){ // 2nd element
		cout << "i = " << i << endl;
		i++; // 3rd element
	}
	
	
	system ("Pause");
	return 0;
}
```
```cpp title:Fixed
#include <iostream>

using namespace std;


int main() {
	
	int i = 0; // 1st element of loop
	
	while (i <= 10){ // 2nd element         // "i >= 0" to "i <= 10"
		cout << "i = " << i << endl;
		i++; // 3rd element
	}
	
	
	system ("Pause");
	return 0;
}
```
## Run Screenshot
![[Screenshot_27.png]]
## Conclusion
Essentially, fixing an infinite loop is making sure the variable converges to the value it's evaluated with instead of diverging