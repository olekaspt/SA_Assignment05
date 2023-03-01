# SA_Assignment05

Clone the repo at https://github.com/olekaspt/TranslationWithBoost

Modify the code to pick up the local po file (see repo above for instructions to fix). And verify you can see the German text when running the Translation.exe

Perform the following:

1. Add in a new cpp and h file to have a new function.  And in this function make two calls to cout with two different strings.  These calls should use Localize with context function to localize the strings.  I don't care what the strings are as long as they are unique and different from the strings used translation.cpp.
1. Add in these two calls as well
```c++
std::cout << Localize("file", "open") << std::endl;
std::cout << Localize( "internet connection", "open") << std::endl;
```
