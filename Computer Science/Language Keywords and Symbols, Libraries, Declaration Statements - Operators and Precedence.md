# Programming Language
Derives from some of the same foundational ideas of normal/spoken language (for higher level programming languages that is)
- Words and Grammar most notably
## Words
Predefined Words
- Also called Commands or Key Words
- Each have a specific meaning
	- They get translated to Machine Code
## Grammar
Syntax
- The structure of the key words that causes the intended output
	- Incorrect syntax can lead to unintended outputs
## Libraries
Save time by defining prewritten code to be used more easily and accessibly instructions that are commonly needed
- include them into source code with`{cpp icon} #include <iostream>`
### Typical Libraries included in C++ IDEs
**cctype** - Character Handling
**cmath** - Math Functions Library
**iostream** - Keyboard Input/Monitor Output Library
**fstream** - Read and Write a File
**string** - Strings of Characters
## Symbols
Each represents some instruction
![[Pasted image 20240226144308.png]]
# Ram/Memory
Declaring a Variable sets aside a set of bytes for that variable to be manipulated and not overwritten
- Information Programmer
	- Provides number of bytes, type of data, and a unique name/identifier for the allocated bytes
- OS Memory Manager
	- Automatically assigns/allocates a certain address in RAM to use for the variable
## Declaration Statement
### Syntax
DataType VariableName
- DataType determines number of bytes to set aside
- VariableName is the identifier for those bytes
#### Left Side
Tells the computer the number of bytes and the type of data
#### Right Side
The Alias for the address of the stored byte(s)
- Not important to know the address the Alias is assigned to, OS Memory Manager handles that
### Data
| Data Type   | Description                                        | Size            | Min-Max Value Range                                                         |
| ----------- | -------------------------------------------------- | --------------- | --------------------------------------------------------------------------- |
| **char**    | Character or <br>Small Integer                     | **1** byte      | signed: -128 to 127 <br>unsigned: 0 to 255                                  |
| short int   | Short Integer                                      | 2 bytes         | signed: -32,768 to 32,767<br>unsigned: 0 to 65,535<br>                      |
| **int**     | Integer                                            | **4** bytes     | signed: -2,147,483,648 to 2,147,483,647<br>unsigned: 0 to 4,294,967,295<br> |
| long int    | Long Integer                                       | 8 bytes         | signed: -2,147,483,648 to 2,147,483,647<br>unsigned: 0 to 4,294,967,295     |
| bool        | Boolean Value<br>                                  | 1 byte          | True or False                                                               |
| float       | Floating Point <br>Number                          | 4 bytes         | +/- 3.4e +/- 38 (~7 digits)                                                 |
| **double**  | Double Precision<br>Floating Point Number<br><br>  | **8** bytes     | +/- 1.7e +/- 308 (~15 digits)                                               |
| long double | Long Double Precision<br>Floating Point Number<br> | 16 bytes        | +/- 1.7e +/- 308 (~15 digits)                                               |
| wchar_t     | Wide Character                                     | 2 or<br>4 bytes | 1 wide character                                                            |
### Variable Naming
C++ is case sensitive
- Result of different ASCII code for 'a' and 'A'
- Can only use certain symbols
	- a to z, A to Z, 0 to 9, and underscore
#### Camel Case Naming Convention
First or Only word is lower case, second and higher are capitalized on the first letter
- int age
- int ageGrowth
- int ageYoungPerson
- int ageOldPerson
## Assignment Statement
The Container and the Contents of the Container (analogy)
### Syntax
Variable Name = Expression
- Move value from the right to the left identifier (overwrite bytes on the left with the value on the right)
- Equals (=) in programming is the move/copy/assign operator
You can declare and modify on separate lines, or on the same line
```cpp
int price;
price = 3;

int discount;
discount = price - 1;
```
is the same as
```cpp
int price = 3;
int discount = price - 1;
```
#### User Input
```run-cpp
	int age = 0; // Input - message and capture value
	cout << "Input your age: "; // Print out message to monitor - let the user know what to do
	cin >> age; // Pause and wait for user to enter integer - places typed-in value into age variable
	cout << endl << endl << "Your age is: " << age << endl; // Print out message and variable value to monitor
```