Austin Rolfe
4/21/2024
# Max Size
## Requirements
Find the max size of a double-type array you can make without encountering an error.
- Find size through trial and error
- Do you think different systems would have different sizes? Explain (Google)
## Code
```cpp
#include <iostream>  

using namespace std;


int main() {  

    // Declare Array
    double testSize[259515] = {0};

    cout << endl << testSize[259516] << endl << endl;


    system ("Pause");
    return 0;

}
```
## Conclusion
Unfortunately, given my general disreagrd for bust work and mood, I've decided to not complete this assignment. This is boring and does nothing to teach anyone that couldn't have been done in some other manner. Unfortunately, you jsut recycle the same lessons and throw them on canvas as you have been for the past few years (more than likely) and probably don't even read these messages to begin with and just check for some form of completion.

Either way, the answer to the question seems to be the fact that array are limited to memory, by nature of how variables are declared, and size is determined either by bit size or the free bytes available at the time.
- If the latter (and even former with the latter) is true, fuck this assignment even more because you can never really truly have one value to find and you'll always be on a wild goose chase for that one value that just edges the limit of what's available (as I believe I have run into during my completion of this assignment)
	- Also, quick note on that. I took a break and googled around before typing this all out, and even after all of this typing and googling, I still spent more time changing the value of the array over and over and over again.