# Switch Statement
## Function
An expression that sets the statement to be TRUE upon the first TRUE case
- Will then ignore all other case outcomes (Fall Through)
- Simpler to read than traditional "if else" statements
- Has some functional applications that are easier to make than "if else"
## Syntax
```cpp
Switch (expression) {// The expression must be of an integer type (int or char).

	case constant-Expression:
		//Statements

	case constant-Expression:
		// Statements

	Default: // Optional
		// Statements

}
```
If break statement is used in a case, then the switch statement ends and moves to what comes after.
## Fall Through
Switch is off by default but then changes to on upon the first true expression. It will then run all statements under each case (regardless if they're true/false) after the first true expression is found.