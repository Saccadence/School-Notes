Austin Rolfe
4/14/2024
# Prime Numbers
## Requirements
Have the premade code run as many times as you might one to evaluate multiple prime numbers.
## Code
```cpp title:Original
#include <stdio.h>
#include <iostream>

using namespace std;


int main() {

	int i = 0, j = 0, k = 0;
	double n = 0;
	
	cout << "Enter a number: ";
	cin >> n;
	
	for (i = 2; i <= n; i++){
		
		k = 0;
		
		for (j = 1; j <= i; j++){
			
			if (i % j == 0)
			k++;
			
		}
		
		if (k == 2){
			cout << ", " << i;
		}
		
	}
	
	
	system ("Pause");
	return 0;
}
```
```cpp title:Looped
#include <stdio.h>
#include <iostream>

using namespace std;


int main() {

    int
    numbers = 0,    // Total amount of numbers to be evaluated
    q = 0;          // Loop tracker

    cout << "How many numbers do you want to evaluate: ";
    cin >> numbers;
    cout << endl;

    while (q < numbers) {

        q++;

        int
        i = 0,      // Tracks working number
        j = 0,      // Divided into i
        k = 0;      // Every other evenly divisible value is a prime
        double n = 0;
        
        // Number to be evaluated
        cout << "Enter a number: ";
        cin >> n;

        // Output (evaluation) statement start
        cout << "The prime numbers before " << n << " are:" << endl << "1";
        
        // If i is less <= n (test every number before n)
        for (i = 2; i <= n; i++){
            
            // Reset evaluative variable
            k = 0;

            // If j is less than i, check if i is evenly divided by j
            for (j = 1; j <= i; j++){
                if (i % j == 0) {k++;}          // If it is, increment k
            }
            
            // If i is only divisible by 2 numbers (tracked by k)
            if (k == 2){                // If k is 2, there are only 2 numbers (1 and the value of i) that divide evenly into i
                cout << ", " << i;
            }
            
        }
        cout << endl << endl;
    }
	
	
	system ("Pause");
	return 0;
}
```
## Run Screenshot
![[Screenshot_28.png]]
## Conclusion
Going through and understanding what the code did was probably the most satisfying part of this. Having the code loop was easy and if I wanted to make it more interesting, I would  go through and replace the for loops.
## Test Cases (If Any)
| Test Case(s) | Test 1                      | Test 2                                                                         |
| :----------- | --------------------------- | ------------------------------------------------------------------------------ |
| Input        | 25                          | 99                                                                             |
| Expected     | 1 2 3 5 7 11 13<br>17 19 23 | 1 2 3 5 7 11 13 17<br>19 23 29 31 37 41<br>43 47 53 59 61 71<br>73 79 83 89 97 |
| Actual       | 1 2 3 5 7 11 13<br>17 19 23 | 1 2 3 5 7 11 13 17<br>19 23 29 31 37 41<br>43 47 53 59 61 71<br>73 79 83 89 97 |
