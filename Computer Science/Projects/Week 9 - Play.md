Austin Rolfe
03/17/2024
# Play
## Requirements
Create code that evaluates whether a child can go play, based on the chores/homework they've completed on a given day of the week.
## Code
```cpp
#include <iostream>


using namespace std;

int main () {

    // Declare variables
    int weekday;
    string weekdayName;
    bool cleanRoom;
    bool homeworkDone;

    // Intro and user prompts
    cout << "Are you able to play?" << endl << "Answer each prompt with a 1 or true (for yes), or 0 or false (for no), unless told otherwise."  << endl << endl;

    cout << "What day is it today? (Answer with the number that corresponds with the day)"
    << endl << "1) Monday"
    << endl << "2) Tuesday"
    << endl << "3) Wednesday"
    << endl << "4) Thursday"
    << endl << "5) Friday"
    << endl << "6) Saturday"
    << endl << "7) Sunday"
    << endl;
    cout << "Response: "; cin >> weekday;
    cout << endl << endl;

    // Define weekday int as string - allows it to be output later
    if (weekday == 1) {weekdayName = "Monday";}
    else if (weekday == 2) {weekdayName = "Tuesday";}
    else if (weekday == 3) {weekdayName = "Wednesday";}
    else if (weekday == 4) {weekdayName = "Thursday";}
    else if (weekday == 5) {weekdayName = "Friday";}
    else if (weekday == 6) {weekdayName = "Saturday";}
    else {weekdayName = "Sunday";}
    // Use switch to streamline this later

    // Define what work needs to be done before playing on each given day
    if (weekday == 1 || weekday == 2 || weekday == 3) {     // Another great place for switch with a function

        // Monday, Tuesday, or Wednesday
        cout << "Since today is " << weekdayName << ", you have to make sure your room is clean AND that your homework is done before you can go play!";
        cout << endl << "Have you cleaned your room today? "; cin >> cleanRoom;
        cout << "Have you completed your homework for today? "; cin >> homeworkDone;
        cout << endl;

        // Output of evaluation - with statements stating what still needs to be done
        if (cleanRoom == true && homeworkDone == true) {cout << "Great job! You can go play!";
        }
        else {        // Output for if ANY or ALL chores are forgotten

            if (cleanRoom == false) {
                cout << "You forgot to clean your room, do that and then you can go play!";
            } else if (homeworkDone == false) {    
                cout << "You forgot to finish your homework, do that and then you can go play!";
            } else {
                cout << "Make sure to do your chores before you try to go play!";
            }
        }
    } else {

        // Thursday, Friday, Saturday, or Sunday
        cout << "Since today is " << weekdayName << ", you have to make sure your room is clean OR that your homework is done before you can go play!";
        cout << endl << "Have you cleaned your room today? "; cin >> cleanRoom;
        cout << "Have you completed your homework for today? "; cin >> homeworkDone;
        cout << endl;

        // Output of evaluation - with statements stating what still needs to be done
        if (cleanRoom == false && homeworkDone == true) {cout << "Great job! You can go play!";
        }
        else {        // Output for if ANY chores are forgotten

            if (cleanRoom == false && homeworkDone == false) {cout << "Make sure you do your chores BEFORE you try and go play today!";
            } 
            else if (cleanRoom == false && homeworkDone == true) {cout << "Good job! You can go play!" << endl << "Don't forget to clean your room sometime today!";
            } 
            else {cout << "Good job! You can go play!" << endl << "Don't forget to finish your homework sometime today!";
            }
        }
    }

    cout << endl;


    // Terminate the program
    system("Pause");
    return 0;

}
```
## Run Screenshot
![[Pasted image 20240317202140.png]]
## Conclusion
I enjoyed this more and having the code output reminders for days where the chore completion could be either/or