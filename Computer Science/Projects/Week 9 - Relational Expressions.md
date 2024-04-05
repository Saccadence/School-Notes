Austin Rolfe
due/date/2024
# Assignment Title
## Requirements
Create code that evaluates relationships of a person's height and age.
## Code
```cpp
#include <iostream>


using namespace std;

int main () {

    int age = 21;
    double height = 5.75;

    cout << boolalpha << " 1. A person's age is greater then or equal to 18 and the person is taller than 5 feet = " << ((age >= 18) && (height > 5)) << endl;
    cout << boolalpha << " 2. A person is younger than 18 or the person is shorter than 6 feet = " << ((age < 18) || (height < 6)) << endl;
    cout << boolalpha << " 3. A person is between 6 and 7 feet, and between 18 and 65 years old = " << ((height > 6) && (height < 7) && (age > 18) && (age < 65)) << endl;
    cout << boolalpha << " 4. A person's age is not 0 = " << !(age == 0) << endl;
    cout << boolalpha << " 5. A person's age is 18 or 29 or 42 = " << ((age == 18) || (age == 29) || (age == 42)) << endl;


    // Terminate the program
    system("pause");
    return 0;

}
```
## Run Screenshot
![[Pasted image 20240317201331.png]]
## Conclusion
Same as previous program. Not stimulating enough