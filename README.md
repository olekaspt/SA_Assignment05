# SA_Assignment05

## Localization

Clone the repo at https://github.com/olekaspt/TranslationWithBoost

Modify the code to pick up the local po file (see repo above for instructions to fix). And verify you can see the German text when running the Translation.exe

Perform the following:

1. Add in a new cpp and h file to have a new function.  And in this function make two calls to cout with two different strings.  These calls should use Localize with context function to localize the strings.  I don't care what the strings are as long as they are unique and different from the strings used translation.cpp.
1. Add in these two calls as well
```c++
std::cout << Localize("file", "open") << std::endl;
std::cout << Localize( "internet connection", "open") << std::endl;
```
1. Run the process to generate a po and mo file.  Make sure to use a different name than what is already used (by default it wants to output things as message.po).  HINT there is a -o outputfile option :)
1. Provide translation for the strings in the po file and fix up the header file (see repo mention above on what to do for header).  For the duplicates in the original message.po file, append an 2 to the string.   Generate mo file.  Place it in proper directory (see above repo instructions).   
1. Modify LocalizationUtils.cpp to pick up the new mo file (HINT genPtr->add_messages_domain("messages");)
1. Modify Translation.cpp to call you function 2 times.

As part of your submission you will package up your entire solution and upload it.


PDF
1. Povide screenshot of your program output.
1. Answer the following questions.
  1. The way the example was setup, each time we called the method to output the string we called Localize (and thus boost translate).  Is this an efficient methodology to retrieve the translated stirng.   HINT : Thing about the case when we called your function twice.  What is your suggestion as a best coding practice to resolve this.
  2. Imagine if forced you to have the new file you created put into a shared library.   And we wanted to reference the string for open file.  And if our DevOps processs runs the xgettext process on each file individually.   What issues do you foresee us having with this model?

## Signing

Using the process in the slide deck on self signing, sign the translation.exe with a self certificate.  

Provide as part of your upload this exe.

PDF
1. Show the steps you verifying the certificate of the exe.  Both using powershell commands and file explorer, RMB properties on the exe and looking at the digital cert.

## Journaling

Using Repo https://github.com/olekaspt/SoftwareArchitectureCLassApplication.git

