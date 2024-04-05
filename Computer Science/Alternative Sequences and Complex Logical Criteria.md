# Complex Criteria
A set of comparisons that, together, lead to a decision/output
- Recall PHIL 100 (Logic)
## Simple
A singular condition that leads to an outcome
- x > 4 ---> True/False
## Complex
Two or more conditions that lead to an outcome
- Hungry, Spending money, Transport, etc. ----> Eating lunch at McDonalds
- Requires all conditions to be true in order to have the outcome occur
	- This is evaluated and expressed with logical operators
# Logical Operators
The symbols, or sets of symbols, that allow for the evaluation of a set of criteria to determine the outcome/output of the input data
## Table of Expressions
|                                                                                                     Symbol                                                                                                     |               English Meaning               | Definition through a Truth Table |     <     |     <      |                                                                 Key Concept                                                                  |
|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------:|:--------------------------------:|:---------:|:----------:|:--------------------------------------------------------------------------------------------------------------------------------------------:|
|                                                                                     <br><br><br><br><br><br><br><br><br>&&                                                                                     | <br><br><br><br><br><br><br><br><br>**AND** |    **AND (&&) - TRUTH TABLE**    |     <     |     <      |     <br><br><br><br><br><br><br>**All** conditions must be true to result in TRUE<br><br>If one or more conditions is false, then FALSE      |
|                                                                                                       ^                                                                                                        |                      ^                      |            Condition             | Condition | **Output** |                                                                      ^                                                                       |
|                                                                                                       ^                                                                                                        |                      ^                      |             **TRUE**             | **TRUE**  |  **TRUE**  |                                                                      ^                                                                       |
|                                                                                                       ^                                                                                                        |                      ^                      |               TRUE               |   FALSE   |   FALSE    |                                                                      ^                                                                       |
|                                                                                                       ^                                                                                                        |                      ^                      |              FALSE               |   TRUE    |   FALSE    |                                                                      ^                                                                       |
|                                                                                                       ^                                                                                                        |                      ^                      |              FALSE               |   FALSE   |   FALSE    |                                                                      ^                                                                       |
| <br><br><br><br><br><br><br><br>II<br>(Stand-in for standard notation as it breaks my table in Markdown syntax and using escape characters aren't working without some other formatting syntax surrounding it) | <br><br><br><br><br><br><br><br><br>**OR**  |   **OR (\|\|) - TRUTH TABLE**    |     <     |     <      | <br><br><br><br><br><br><br>Only **one** condition must be true to result in **TRUE**<br><br>All conditions must be FALSE to result in FALSE |
|                                                                                                       ^                                                                                                        |                      ^                      |            Condition             | Condition |  *Output*  |                                                                      ^                                                                       |
|                                                                                                       ^                                                                                                        |                      ^                      |               TRUE               |   TRUE    |    TRUE    |                                                                      ^                                                                       |
|                                                                                                       ^                                                                                                        |                      ^                      |               TRUE               |   FALSE   |    TRUE    |                                                                      ^                                                                       |
|                                                                                                       ^                                                                                                        |                      ^                      |              FALSE               |   TRUE    |    TRUE    |                                                                      ^                                                                       |
|                                                                                                       ^                                                                                                        |                      ^                      |             *FALSE*              |  *FALSE*  |  *FALSE*   |                                                                      ^                                                                       |
|                                                                                             <br><br><br><br><br>!                                                                                              |         <br><br><br><br><br>**NOT**         |    **NOT (!) - TRUTH TABLE**     |     <     |     <      |               <br><br><br>All conditions must be true to result in TRUE<br><br>If one or more conditions is false, then FALSE                |
|                                                                                                       ^                                                                                                        |                      ^                      |            Condition             |     <     |   Output   |                                                                      ^                                                                       |
|                                                                                                       ^                                                                                                        |                      ^                      |               TRUE               |     <     |   FALSE    |                                                                      ^                                                                       |
|                                                                                                       ^                                                                                                        |                      ^                      |              FALSE               |     <     |    TRUE    |                                                                      ^                                                                       |
## Definitions/Concepts
### Expression
A condition, value, or math formula resulting in an answer
#### Syntax
```cpp
if ((expression1) && (expression2))...
if ((expression1) || (expression2))...
if ((expression1) && (expression2) && (expression3))...
if ((expression1) || (expression2) || (expression3))...
if ((expression1) && (expression2) || (expression3))...
```
### Truth Table
The official definition of AND, OR, and NOT logical relationships
### Logical Operator
The AND, OR, and NOT symbols whose relationship results are defined in a truth table.
## Example
```cpp title:"AND/&&"
string favoriteFirstName;
int age = 0;
char gender = 'x';

cout << "Enter your favorite first name: ";
cin >> favoriteFirstName;

cout << endl;
cout << "Enter your age: ";
cin >> age;

cout << endl;
cout << "Enter your Gender F/M: ";
cin >> gender;

//Logical AND Table
if ((age < 20) && (gender == 'F') && (favoriteFirstName == "Ann")) {
	cout << endl << " ALL ARE TRUE " << endl;
} else {cout << " One or more conditions is FALSE " << endl;}
```
# Short-Circuit Evaluation
All conditional evaluations are read left to right
## AND
One FALSE statement on either side of an AND condition makes the whole evaluation FALSE
## OR
One TRUE statement on either side of an OR condition makes the whole evaluation TRUE