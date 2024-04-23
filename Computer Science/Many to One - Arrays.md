# Overview
Grant the ability to have many declarative statements (that are iterations of a single naming scheme) to one, with accessibility to each declaration made relatively easily
## Use Case
The most notable usage of this revolves around the following issue:
```cpp title:Problem
int age1 = 0;
int age2 = 0;
int age3 = 0;
int age4 = 0;
int age5 = 0;
int age6 = 0;
int age7 = 0;
int age8 = 0;
int age9 = 0;
int age10 = 0;
```
This has 10 variables of 4 bytes each (40 bytes). each separated from the other in RAM.
- While doable, if you need a much larger number (i.e., 50,000), arrays can simplify both in terms of readability and optimization.
# Array
Turns a set of non-contiguous, contiguous bytes (separate variable declarations) into a contiguous set of contiguous bytes (one array statement with X amount of declarations in it).
## Syntax
```cpp title:Syntax
// Variable
	DataType VariableName = Value;

// Array
	DataType ArrayName[#] = {Value} or {Value, Value, Value...(for # defined)}
```
#### Definitions
Terms used in arrays
##### Array Size
Number of elements in an array
##### Index
Some value that accesses a value declared in an array
- First value in index is indexed as 0
	- To access the first value of `{cpp} cars[3] = {Honda, Toyota, Subaru}` you use `{cpp} cars[0] = Honda`
##### Offset
Distance from something
- Start = 0 | End = N-1
	- Where N is the number of entries defined in the array declaration
##### Element
Each declared entry in an array (size of each in ram determined by the data type declared in the array statement)
### Examples
```cpp title:"Make the Bucket"
// Example 1
	int ages[4];
	// Declare array of 4 integers
	
// Example 2
	double temps[1000];
	// Declare array of 1000 doubles
	
// Example 3
	char characters[40000];
	// Declare array 40,000 characters
```
```cpp title:"Access the Bucket"
// Example 1
	int x[10];
		for Size = 10
		do Index = 0 - 9

// Example 2
	char c[50];
		for Size = 50
		do Index = 0 to 49

// Example 3
	string s[1000];
		for Size = 1000
		do Index = 0 to 999

// Example 4
	double d[40000];
		for Size = 40000
		do Index = 0 to 39999
```
```cpp title:"Use the Bucket"
// Example 1
	ages[0] = 42;

// Example 2
	temps[10] = 72;

// Example 3
	characters[25001] = '$';
```
## Illustration of Arrays
![[Pasted image 20240418191214.png]]
## Initialization
Assigning an initial value allows for a consistent program output by always having the same value stored in RAM from computer to computer on first run.
### When You Declare It
Putting values in an array when declaring it
#### Short List Initialization
Best for large arrays where you can assign the same value to all values in the array (typically 0)
```cpp title:Examples
// Example 1
int ages[100] = {0};

// Example 2
double ages [1000] = {0.0};
```
#### Long List Initialization
Best for short arrays where you assign each variable in the array it's own individual value
```cpp title:Examples
// Example 1
int ages[4] = {42, 69, 104, 21};

// Example 2
string firstNames[4] = {"Tuyet", "Miguel", "Julie", "Amber"};

// Example 3
char letters[4] = {'a', '$', '8', 'P'};

// Example 4
double ages[4] = {42.1, 69.3, 104.98, 21.0};
```
### After You Declare It
Putting values in an array after you declare it
#### Individually
```cpp title:Example
int ages[4];
ages[0] = 42;
ages[1] = 69;
ages[2] = 104;
ages[3] = 21;
```
#### All With a Loop
```cpp title:Example
int ages[1000];
for (int i = 0; i < 1000; i++) {
	ages[i] = 0;
}
```
## Using Arrays
### Calculation
```cpp title:Example
int ages[4];
ages[0] = 42;
ages[1] = 69;
ages[2] = 104;
ages[3] = 21;

cout << ages[1] - ages[0]; // 69 - 42 = 27
ages[3] = ages[2] + 10;    // Adds 104 + 10 and Assign 114 to ages[3]
```
## Dimensionality
This is how many sets are attached to an array (simply put)
### One Dimensional
This is best described as a list as it's a single set of variables/values (on a graph: x)
- `{cpp}datatype myListArray[#]`
### Two Dimensional
This is best described as a table as it's two sets of variables/values intermingled (on a graph: x, y)
- `{cpp}datatype myTableArray[#][#}`
### Three Dimensional
This is best described as a cube as it's three sets of variables/values intermingled (on a graph: x, y, z)
- `{cpp}datatype myCubeArray[#][#][#]`
### Examples
```cpp title:"One Dimensional"
for (int i = 0; i < 10; i++) {
	myListArray[i] = 0;
}
```
```cpp title:"Two Dimensional"
for (int i = 0; i < 10; i++) {
	for (int j = 0; j < 10; j++) {
		myTableArray[i][j] = 0;
	}
}
```
```cpp title:"Three Dimensional"
for  (int i = 0; i < 10; i++) {
	for (int j = 0; j < 10; j++) {
		for (int k = 0; k < 10; k++) {
			myTableArray[#][#][#] = 0;
		}
	}
}
```
# Output Formatting
With more, and more complex, data being used and in more robust ways, one of the best things  to know are ways to format the output of our code on the command line.
## Usage
```cpp title:Formatting
#include <iomanip>

cout << fixed; // Do not show floating point numbers scientific notation
cout << setprecision(0); // Number of decimal places to show
cout << setw(50); // Width of space for each answer
```