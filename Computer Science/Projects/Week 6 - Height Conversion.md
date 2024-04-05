Austin Rolfe
2/25/2024

# Height Conversion
## Requirements
Use your VS or xCode IDE to create this second program
## Code
```cpp title: Height Conversion
#include <iostream> //Name of prewritten code <file> you want to use
                    //Good programmers REUSE existing code
                    //#include names files/libraries of existing code you want to reuse
using namespace std; //Command to avoid typing std:: in front of cout and endl commands

int main() { //All programs start at 'main' -simple version of main, others possible

    cout << "Austin Rolfe - 2/22/2024" << endl << endl;

    int height = 0, feet = 0, inches = 0;   //Declare and initalize variables
    cout << "What is your height in inches? " << endl; //Print prompt for height
    cin >> height;                          //Stop and wait for user to enter height
    feet = height / 12;                     //Calculate feet from whole number of division output
    inches = height % 12;                   //Calculate inches from remainder of division output
    cout << endl << "My height is " << feet << " feet and " << inches << " inches." << endl << endl;
                                            //Print to monitor message and results of calculations
    system ("Pause");                       //Command needed to see output on PC
    return 0;                               //End program

}
```
## Conclusion
I learned how to setup and use my IDE for formatting neatly
## Run Screenshot
![[Screenshot_13.png]]
## Test Cases
Input Value: 60 | 69
Expected Output: 5 feet | 5 feet and 9 inches
Actual Output: 5 feet | 5 feet and 9 inches