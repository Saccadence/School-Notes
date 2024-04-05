Austin Rolfe
03/10/2024
# Lunch at McDonalds
## Requirements
Create a program that gives the user a checklist to complete on whether or not they can get McDonalds for lunch.
## Code
```cpp
#include <iostream>


using namespace std;

int main () {

    // Declare variables
    bool amHungry;
    bool haveMoney;
    bool haveTime;
    bool haveTransportation;
    bool restaurantOpen;

    // Introduction and user prompt/input
    cout << "So you want to go eat at McDonalds? Take this survey to find out if you're able to do so!";
    cout << endl << endl <<"(All answer should be recorded as 1 or true, and 0 or false, for yes and no respectively - any responses that don't follow this format be marked as TRUE by default)";

    cout << endl << endl << "Are you hungry?";
    cout << endl << "Response: ";
    cin >> amHungry;                                                                                              // Hungry

    // Begin nested if else for evaluation of criteria to go to a restaurant
    if (amHungry == true) {                                                                                         // Money

        cout << endl << "That's a great place to begin!";

        // Prompt for input on financial capability
        cout << endl << endl << "Do you have the spending money available to go out to eat?";
        cout << endl << "Response: ";
        cin >> haveMoney;

        if (haveMoney == true) {                                                                                        // Time
        
            // Prompt for input on time availability
            cout << endl << endl << "Do you have time to spare to go out to eat?";
            cout << endl << "Response: ";
            cin >> haveTime;

            if (haveTime == true) {                                                                                         // Transportation

                cout << endl << "Almost there!";

                // Prompt for input on available transportation
                cout << endl << endl << "Do you have a mode of transportation readily available and usable to be able to go out to eat?";
                cout << endl << "Response: ";
                cin >> haveTransportation;

                if (haveTransportation == true) {                                                                                   // Restaurant Open

                    cout << endl << "It seems you have everything you need! Just one last - and very important - question left.";
        
                    // Prompt for input on whether the restaurant is open or not
                    cout << endl << endl << "Is McDonalds open right now?";
                    cout << endl << "Response: ";
                    cin >> restaurantOpen;

                    if (restaurantOpen == true) {                                                                                           // Conclusion - "Approved"

                        cout << endl << "Congratulations! You're able to go and eat at McDonalds! I hope you get something good and enjoy your meal! :)" << endl;

                    } else {cout << endl << "It's recommended that McDonalds is open before you go and try to eat there. Please go through the checklist at a later time or date! :)" << endl;}

                } else {cout << endl << "It's recommended that you try to have a mode of transportation before you plan to go eat out at McDonalds. Please go through the checklist at a later time or date! :)" << endl;}

            } else {cout << endl << "It's recommended that you have time to spare before you consider going to purchase and eat McDonalds. Please go through the checklist at a later time or date! :)" << endl;}

        } else {cout << endl << "It's recommended that you at least have spending money available before you consider going to purchase McDonalds. Please go through the checklist at a later time or date! :)" << endl;}

    } else {cout << endl << "It's recommended that you at least be hungry before you consider going to purchase McDonalds. Please go through the checklist at a later time or date! :)" << endl;}


    // Terminate the program
    system ("pause");
    return 0;

}
```
## Run Screenshot
![[Screenshot_127.png]]
## Conclusion
I learned about how to conduct a checklist using nested "if else..." statements and apply them in a manner that is practical for anyone looking to get McDonalds. Following the previous assignments, I would like to find a way to verify response inputs which seems to be a tall order within the parameters of the applied knowledge we're using right now.
## Test Cases (If Any)
All true (**if**) statements output the proper strings and all potential false (**else**) strings when prompted.
# Alternate Idea for Formatting
Prompt for all responses and give a unique output for each set of responses given
- e.x. (in order of responses as a bool) 0, 1, 1, 0, 1 == "unfortunately, you can't go because of \[response #1, #2], please resolve these issues and check later"
- more detailed and inclusive of all data points, but is longer to code and requires (probably) more planning to get right