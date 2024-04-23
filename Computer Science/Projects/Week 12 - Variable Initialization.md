Austin Rolfe
4/14/2024
# Variable Initialization
## Requirements
Explain what happens when a variable is not initialized
## Code
```cpp
#include <iostream>

using namespace std;


int main() {
	
	int numberGrades = 0;
	int sumGrades;
	int aGrade = 0;
	
	cout << "How many grades to enter: ";
	cin >> numberGrades;
	
	int i = 1;    // 1st element
	while (i <= numberGrades){    // 2nd element
		cout << "Enter Grade: ";
		cin >> aGrade;
		sumGrades = sumGrades + aGrade;
		i++;    // 3rd element	
	}
	
	cout << "Grade Average = " << sumGrades/numberGrades << endl;
	
	
	system ("Pause");
	return 0;
}
```
## Conclusion
On my end, I don't notice anything odd as it seems to work as intended. This may be due to the way that I run code, or me previously having run it without removing the 0 first. That being said, the fundamental issue is the fact that not assigning a value will pull the last used value stored, if any, in that location. If there is none stored, this will behave unpredictably as, understandably, there is no (known) value to pull when requested.