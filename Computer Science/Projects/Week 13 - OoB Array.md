Austin Rolfe
4/21/2024
# OoB Array
## Requirements
Explain what happens when code calls for a value OoB of an array set
## Code
```cpp
int ages[5] = {0}; // You use 0 to 10,  when you mean 0 to 3
for (int i =0; i <= 10; i++) {
	cout << "ages["  << i << "]: " << ages[i] << endl;
}
```
## Conclusion
Essential what happens is that the value being called for doesn't exist so it spits out data that is wrong and undefined. Problems mostly only happen in the form of code being unpredictable in output (i.e., sometimes it works, sometimes it doesn't, sometimes it demolishes itself). Using values from the OoB call will give you results that are wildly incorrect for the calculator use case.