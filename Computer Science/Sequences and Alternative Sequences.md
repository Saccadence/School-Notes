# Sequences
A set of instructions
## Sequence
A chain of commands that lead to an outcome with strict set of output(s)
## Alternative Sequence
A set of commands that lead to and outcome with a flexible (alternative) set of output(s)
### Choices
Decisions, Branching, Selection, Flow Control
- Made on the basis of a set of *criteria*
	- The tool we use to judge the best choice of which we will act on
##### Criteria
A rule, standard, test, measure, means to judge, or a touchstone
- Utilize comparisons (simple or complex) to make decisions in C++
	- Relational criteria
### Relational Criteria
| Symbol | Meaning                          | Example      | Comparison Result |
| :----- | -------------------------------- | ------------ | ----------------- |
| >      | Greater<br>than<br><br>          | var1 > var2  | True or False     |
| <      | Less<br>than                     | var1 < var2  | True or False     |
| >=     | Greater <br>than<br>or equal<br> | var1 >= var2 | True or False     |
| <=     | Less<br>than<br>or equal         | var1 <= var2 | True or False     |
| ==     | Equal                            | var1 == var2 | True or False     |
| !=     | Not<br>Equal                     | var1 != var2 | True or False     |
Can be used with the following data types:
- Numbers
	- integer, double, float
	- Compares numeric order
- Characters or Strings of Characters
	- Compares alphabetic order
### If Statement
Syntax: `{cpp icon} if (criteria) { Do this if TRUE }`
```cpp
int X = 3;

if ( X == 3 ){ cout << "True - X equals 3"; } // Prints if true
if ( X >= 3 ){ cout << "True - X greater than or equal to 3"; } // Prints if true and previous line(s) before aren't true
if ( X <= 3 ){ cout << "True - X less than or equal to 3"; } // Prints if true and previous line(s) before aren't true
```
#### Single Selection
Only the TRUE condition goes a different path
##### Example
```cpp
int num = 0; // declare variable and initialize to zero.  

cout << "Enter a number between 1 and 999: "; // Print Message  
cin >> num; // Wait for user input  

if ( num < 1 ) { cout << "Number to small, you entered a number less than 1" << endl; }  
if ( num < 100 ) { cout << "Number less than 100" << endl; }  
if ( num <= 500 ) { cout << "Number less than 500" << endl; }  
if ( num < 1000 ) { cout << "Number less than 1000" << endl; }  
if ( num > 999 ) { cout << "Number to large, you entered a number greater than 999" << endl; }  


system ("pause");  
return 0;  
```
### If Else
Syntax: 
`{cpp icon} if ( criteria ) { Do this if criteria result is TRUE }`
	`{cpp} else { Do this if criteria result is FALSE }`
#### Double Selection
Both the TRUE and the FALSE condition have different paths
- Both outcomes veer from main sequence
##### Examples:
```cpp title:>10
int x = 3; // Declare variable and assign initial value

if ( x > 10 )
	{ cout << "TRUE"; }
else
	{ cout << "FALSE"; }
cout << endl << endl;


system ("pause");
return 0;
```
```cpp title:>=10
int x = 0; // Make a variable to store an integer

cout << "Enter an Integer: "; // Allows you to write a message
cin >> x; // Allows the input to be placed into the variable x, by user entry

if ( x >= 10 ) {

	// Print message if condition is True - Greater than or Equal to 10
	cout << endl << "x (" << x << ") is greater than or equal to 10." << endl;

}
else {

	// Print message if condition is False - Less than 10
	cout << endl << "x (" << x << ") is less than 10." << endl;

}
cout << endl;


system ("pause");
return 0;
```
#### Cascades
Stacked "if else..." statements where the output only (exit) occurs if it reaches a condition that is fulfilled (true or false)
##### Example:
```cpp title:"Weather Warning"
int windSpeed = 0; // Declare variable and assing intial value

cout << "Enter Wind Speed: ";
cin >> windSpeed;

if ( windSpeed > 73 ) { cout << "Hurricane Warning"; } // If true, then ends here; if false, drop to next line
else if ( windSpeed > 54 ) { cout << "Storm Warning"; } // If true, then end here; if false, drop to next line
else if ( windSpeed > 38 ) { cout << "Gale Warning"; } // If true, then end here; if false, drop to next line
else if ( windSpeed > 24 ) { cout << "Small Craft Advisory"; } // If true, then end here; if false, drop to next line
else { cout << "Calm Seas"; } // Done
cout << endl;


system ("pause");
return 0;
```
```cpp title:"Grade Conversion (Points to Letter)"
int gradePoints = 0;

cout << "Enter Grade Points: "'
cin >> gradePoints;

if ( gradePoints >= 90 ) { cout << "Grade = A"; } // If true, then end here; if false, drop to next line
else if ( gradePoints >= 80 ) { cout << "Grade = B"; } // If true, then end here; if false, drop to next line
else if ( gradePoints >= 70 ) { cout << "Grade = C"; } // If true, then end here; if false, drop to next line
else if ( gradePoints >= 60 ) { cout << "Grade = D"; } // If true, then end here; if false, drop to next line
else { cout << "Grade = F"; } // Done
cout << endl;


system ("Pause");
return 0;
```
#### Nested
You can put if else statements inside one another
```cpp title:"If Else Diagram"
if (...) {
	if (...) {...;}
	else (...) {...;}
}
else (...) {
	if (...) {...;}
	else (...) {...;}
}
```