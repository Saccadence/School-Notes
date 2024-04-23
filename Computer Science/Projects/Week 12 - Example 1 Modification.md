Austin Rolfe
4/14/2024
# Example 1 Modification
## Requirements
Modify the conditional found  in example 1 and explain what each modification does and what it means.
## Code
```cpp
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
## Conclusions
- Empty
	- Compiler Error
		- The compiler is looking for some value to evaluate (proper syntax) and since there is nothing that would resemble true/false within the header, it breaks
- 0
	- Code doesn't run
		- 0 is the same as false and the code within the loop doesn't run
- 1
	- Infinite Loop
		- 1 is the same as true, and since this value is never modified, the code in the loop runs forever
- 42
	- Infinite Loop
		- Since 42 is a non-zero (true) value, it causes the loop to run forever
- true
	- Same as 1
		- Same as 1
- false
	- Same as 0
		- Same as 0
- (i x 3) < 10
	- Prints i = 0, 1, 2, 3
		- As long as 3i is less than 10, it will print the value of i. since 3x3 is 9 and 4x3 is 12, 3 is the highest value that i can be.
- i = 9
	- Infinite Loop
		- Same principle as 42 (and by proxy 1 and true), i is assigned the value 9, not compared to the value 9
- (i + 2) < 10
	- Prints i = 0, 1, 2, 3, 4, 5, 6, 7
		- Following the same idea as (i x 3) < 10 from before, 10 - 2 = 8 and since it won't print if i + 2 = 10, i will only print if it's 7 or lower.