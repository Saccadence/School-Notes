Austin Rolfe
03/17/2024
# Midterm - Code Fixing
## Requirements
Fix the code, create a flow chart, and attach working code screen shots
## Code
```cpp
#include <iostream>                         // "<oistream>>" to "<iostream>"
using namespace std;                            // removal of multiple unnecessary ";" after "std"
#include <string>
int main() {
   cout << "Name and Due date" << endl; //  On every program, the 1st line in the int main() function is your name and the due date..                   // fixed spelling of int main() and correction from random date to due date (both in comment)
   string favoriteFirstName = " ";    // Initialize with space
   int age = 0;
   char gender = 'x';
   cout << "Enter your favorite first name: ";  // cout allows you to write a message                       // type: namee to name     
   cin >> favoriteFirstName;                           // cin allows you to input a value                            // string variable typo (>>Favorite -> >> favorite) and comment not properly started (/ -> //)
   cout << endl;                                                                                            //  wrong syntax/typo: end1 to endl and >> to <<  
   cout << "Enter your age: ";                                                                                       // incorrect syntax and typo: "cout <> Enter youu" revised to  "cout << "Enter your"
   cin >> age;                                                                                              // Wrong variable name: "Age" to "age"
   cout << endl;
   cout << "Enter your Gender F/M: ";                                                                                // typo: "u" to "your"
   cin >> gender;                                                                                           // wrong variabe name: "Gender" to gender                                    
    // Logical AND table --  ((exp1) && (exp2) && (exp3) )...
   if ( ( age > 17 ) && ( gender == 'F') && ( favoriteFirstName == "YourFavoriteNameHere"  ) )                       // Incorrect syntax and variable name: "&" to "&&", "favoriteFirstNam" to "favoriteFirstName", and "=" to "=="
    {  // And coniditions: Takes ALL to be TRUE, so result is TRUE                                          // typo: "coniditions" to "conditions"
       cout << endl << " ALL conditions ARE TRUE " << endl;     }                                                   // wrong syntax: "<<<" to "<<" and "endll" to "endl" | technically wrong in some sense, but not in a code syntax way: the spaces at the start and end of the string in the CLI output (might be a copy/paste error)
    else     {        
       // And conditions: Only takes one FALSE condition, so result is FALSE                                // typo: "onditions" to "conditions"
       cout << " One or more conditions is FALSE " << endl;     }                                                   // syntax: "cout <>" to "<<"
    cout << "Programming is very fun" << endl;
    system("pause"); // pause statement Only for PC, not MAC  - Macs Comment // out this line   
return 0;                                   // formatting (potentially): return not in line with rest of code (again could be copy/paste but not touching it since it's usually personal preference anyways), formatting also applies to if...else... statement as it usually is indented also
}
```
## Run Screenshot
![[Screenshot_129.png]]
## Conclusion
Quite a bit of errors, but nothing to egregious in terms major code structure errors it seems (if you disregard formatting)
## Test Cases (If Any)

| Test Case(s) | Test 1                                                             | Test 2                                               |
| :----------- | ------------------------------------------------------------------ | ---------------------------------------------------- |
| Input        | favoriteFirstName = YourFavoriteNameHere<br>age = 21<br>gender = F | favoriteFirstName = Austin<br>age = 21<br>gender = F |
| Expected     | ALL conditions ARE TRUE                                            | One or more conditions is FALSE                      |
| Actual       | ALL conditions ARE TRUE                                            | One or more conditions is FALSE                      |
## Flow Chart
![[Pasted image 20240317211710.png]]