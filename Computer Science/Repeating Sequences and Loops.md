# Overview
Loops enable the ability to repeat a set of instructions (code) without having to rewrite the code for every instance you want it to be done. The other benefit is that due to the nature of FOR and WHILE loops, the amount these can be repeated can be dynamic and without too much additional code (depending on application).
# Loops
The most common, and most practical, application is for the repetition of a block of code.
## Components
Loops run on 3 main things
#### Statement
This will be (more than likely) a FOR or a WHILE statement, of which will determine how the criteria is read and under what conditions a set/block of code is ran by
##### FOR (Pretest)
FOR loops identify and evaluate the criteria for a loop by examining it before executing a block of code one or more times
###### Syntax
```cpp title:Syntax
for (declare variable = initial value; criteria/condition checking value; change value) {
	// Block of code to be run
}
```
###### Examples
```cpp title:"Pre-Determined - Loop Counter"
#include <iostream>

using namespace std;


int main(){

	// Example - Print out value of counter during each loop
	// Declare and initialize loop counter
	int count = 20;

	// Declare i and initialize to 1, check if value of i <= 20, Add 1 to i
	for (int i = 1; i <= count; i++) {
		// Print out value of i each time loop is executed
		cout << i << endl;
	}


	system ("Pause");
	return 0;
}
```
```cpp title:"User Input - Loop Counter"
#include <iostream>

using namespace std;


int main(){

	// Example - Prompt user for loop count, and print out value at each loop
	int times = 0;
	cout << "Enter number of times to repeat (between 1 and 25): ";
	cin >> times;

	if ((times < 0) || (times > 25)) {
		//If times value is out of range
		cout << "Next time enter a number between 1 and 25" << endl;
	} else {
		// If times value is good, do a for loop
		// A simple for loop
		for (int i = 1; i <= times; i++) {
			// Print out value of i each time loop is executed
			cout << i << endl;
		}
	}


	system ("Pause");
	return 0;
}
```
```cpp title:"Largest Input"
#include <iostream>

using namespace std;


int main(){

	int count = 0;
	int maxNumber = 0;
	int enteredNumber = 0;

	cout << "This program determines which entered number is the largest" << endl;
	cout << "Enter the amount of numbers to check: ";
	cin >> count;

	// Print out message - Input number - Compare to see if new number is bigger - Repeat
	for  (int i = 0; i < count; i++) {
	
		cout << "Enter number " << i << ": ";
		cin >> enteredNumber;

		if (enteredNumber > maxNumber) {
			maxNumber = enteredNumber;
		}
	}

	// Output the largest number saved
	cout << endl << "The largest number is " << maxNumber << endl;


	system ("Pause");
	return 0;
}
```
```cpp title:"Diamond Printer"
#include <iostream>

using namespace std;


int main() {

	// Example - Fun printing diamonds
	int i = 0; int j = 0; int n = 1;
	int max = 0;
	int skip = 0;

	cout << endl << "Enter the max number of diamonds to print: ";
	cin >> max;
	cout << endl << "Enter the skip value: ";
	cin >> skip;

	// Example - For loop nested in a for loop
	for (i = 1; i <= max; ++i) {
		for (j = 1; j <= n; ++j) {
			cout << "*";
		}

		if (i <= max / skip) {
			n += skip;
		} else {n -= skip;}
		cout << endl;
	}


	system ("Pause");
	return 0;
}
```
##### WHILE (Posttest)
WHILE loops execute a block of code and then evaluate the criteria to determine whether or not to run the block of code again
#### Criteria
This involve some relation operator that compares some variable (usually one made specifically for loop) to some value (a termination point)