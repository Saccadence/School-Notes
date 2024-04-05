Austin Rolfe
2/25/2024

# Higher Number
## Requirements
Use your VS or xCode IDE to create this third program
## Code
```cpp title: Higher Number
#include <iostream> //Name of prewritten code <file> you want to use
                    //Good programmers REUSE existing code
                    //#include names files/libraries of existing code you want to reuse
using namespace std; //Command to avoid typing std:: in front of cout and endl commands

int main() { //All programs start at 'main' -simple version of main, others possible

    cout << "Austin Rolfe - 2/22/2024" << endl;

    int firstNum = 0, secondNum = 0; //Declare and initialize variables

    cout << endl << "Enter the first number:" << endl;  //Print prompt for the first number
    cin >> firstNum;                        //Stop and wait for user to enter the first number
    cout << endl << "Enter the second number:" << endl; //Print prompt for the second number
    cin >> secondNum;                       //Stop and wait for user to enter the second number

    if (firstNum < secondNum) 
        {cout << endl << "The first number (" << firstNum << ") is less than the second number (" << secondNum << ")." << endl;}
        //Print to monitor message for when the first number is less than the second number
    else
        {cout << endl << "The first number (" << firstNum << ") is greater than, or equal to, the second number (" << secondNum << ")." << endl << endl;}
        //Print to monitor message for when the first number is greater than, or equal to, the second number
    
    system ("Pause");   //Command needed to see output on PC
    return 0;           //End program

}
```
## Conclusion
I learned how to manipulate the output more for formatting purposes and how operators work more
## Run Screenshot
![[Screenshot_12.png]]
## Test Cases
Input Values: 10, 5 | 5, 10
Expected Output: The first number is greater than, or equal to, the second number | The first number is less than the second number
Actual Output: The first number is greater than, or equal to, the second number | The first number is less than the second number