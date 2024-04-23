# Overview
Similar to the FOR loops covered before, WHILE and DO WHILE (clarified later) similar things, but at different points in time than one another. All of these formats, in essence, work to execute a code block multiple times.
## Recap of Elements
**1)** Initialize variable(s) and assign a value - To be examined
**2)** Conditional attached to variable(s)
**3)** Modification of the variable(s) being evaluated
# WHILE Loop
This is a *pretest* loop so if the condition is FALSE from the start, the block of code is never run
- Advantage
	- Pretest (Doesn't have to run)
- Disadvantage
	- Elements can't be in header (disconnected from loop statement)
## Syntax
```cpp title:Syntax
declare variable = inital value

while (condition - check variable){
	
	//Code Block
	
	//Variable Modification
	
}
```
### Examples
```cpp title:"Loop Counter"
#include <iostream>

using namespace std;


int main(){
	
	int i = 0; // 1st element of loop
	
	while (i < 10){ // 2nd element of loop
		cout << "i = " << i << endl;
		i++; // 3rd element of loop
	}
	
	system ("Pause");
	return 0;
}
```
```cpp title:"Infinite Loop"
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
```cpp title:"Grade Average"
#include <iostream>

using namespace std;


int main() {
	
	int numberGrades = 0;
	int sumGrade = 0;
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
## Nesting Functionality
Does effectively the same thing as the FOR loop, but since the 3 elements **have** to be disconnected it can be harder to read the conditionals.
### Example
```cpp title:"Diamond Printer"
#include <iostream>

using namespace std;


int main() {
	// 10 by 10 square of diamonds
	
	// Declare loop variables
	int i = 0;
	int j = 0;
	
	while (i < 10){
	
		i++; // Outside index
		
		while (j < 10){
			j++; // Inside index
			cout << "*";
		}
		
		j = 0; // Reset inside index (run 10 times for every outside index)
		cout << endl;
		
	}
	
	
	system ("Pause");
	return 0;
}
```
# DO WHILE Loop
Unlike the WHILE loop, this is a *posttest* loop - It will always run the block of code at least once
- Advantage
	- The code runs at least once
- Disadvantage
	- Elements are still disconnected, and slightly more difficult to read, but not as confusing as parent WHILE loop
## Syntax
```cpp title:Syntax
declare variable = initial
value; do {
	// Code Block
	// Modify Value
} while (condition - check variable); // Note the ':' at the end of the statement
```
### Examples
```cpp title:"Single Loop "Counter""
#include <iostream>

using namespace std;


int main() {
	
	int i = 6;    // 1st element
	
	do {
		cout << "i = " << i << endl;
		i = 11;    // 2nd element
	} while (i < 10); // 3rd element
	
	
	system ("Pause");
	return 0;
}
```
```cpp title:Loop
#include <iostream>

using namespace std;


int main() {
	
	int i = 0; // 1st element
	
	do {
		cout << "i = " << i << endl;
		i++; // 2nd element
	} while (i <= 10); // 3rd element
	
	
	system ("Pause");
	return 0;
}
```
```cpp title:"Infinite Loop"
#include <iostream>

using namespace std;


int main() {
	
	int i = 0; // 1st element
	do {
		cout << "i = " << i << endl;
		i++; // 2nd element
	} while (i >= 0); // 3rd element
	
	system ("Pause");
	return 0;
}
```