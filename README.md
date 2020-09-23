<div align="center">

## \_A Beginner's  STRCMP, STRCAT, and STRCPY tutorial \(VB\-LIKE String Manipulation\)


</div>

### Description

This tutorial is for mostly beginners that need to know how to manipulate char strings easily. I recently switched from vb, and it was very hard to get used to chars (from vb's String identifier). This will show you how copy, compare, and add strings together. This will help you have an almost "VB-Like" handle on strings. This is for all uses of strings (Win32 and Console). KEYWORDS: Compare COMPARE compare Add ADD add COPY copy Copy CHARS chars char CHAR Char VB vb STRINGS Strings strings STRING string String tutorial Tutorial TUTORIAL Combine Combining
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Jaime Muscatelli](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/jaime-muscatelli.md)
**Level**          |Beginner
**User Rating**    |4.4 (44 globes from 10 users)
**Compatibility**  |C\+\+ \(general\), Microsoft Visual C\+\+
**Category**       |[Strings](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/strings__3-26.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/jaime-muscatelli-a-beginner-s-strcmp-strcat-and-strcpy-tutorial-vb-like-string-manipulatio__3-5776/archive/master.zip)





### Source Code

// Jaime Muscatelli
<br>
// webmaster@jaimemuscatelli.zzn.com
<br>
// AOL SN: Jaime141974
<br>
<br>
Now, I have just switched from vb, and I know how stressful it is to get a grasp on strings using the char identifier. Even if you didn't, you still want to know how to manipulate strings easily right?
<br>
<br>
STRCMP // Used to compare strings
<br>
<br>
Lets say we made a simple password program, and we obviously needed to compare the real password against the password that the user entered. We would do this using an int variable, the strcmp method, and an if statement.
<br>
<br>
#define sRealPassword "JAIME" // The real password
<br>
#include <iostream.h>
<br>
<br>
int main()
<br>
{
<br>
int icompare; // The actual result
<br>
char sInput[50];
<br>
<br>
cout << "What is your name? : ";
<br>
cin >> sInput;
<br>
<br>
icompare = strcmp(sInput, sRealPassword);
<br>
if (icompare == 0) // if the strings match
<br>
{
<br>
cout << "Welcome\n";
<br>
}
<br>
<br>
That is it. All we did was compare the strings, and then took the result, and if it was equal, then do what we want.
<br>
<br>
<br>
STRCAT // To add strings together
<br>
<br>
This is what most of us want. This is how, in vb , you would say sString = "Jaime " + "Muscatelli".
<br>
<br>
I just used this today, after wanting to find how to do this for 2 months! I finally figured it out, and now I want to help others with the same dilemma. I used for my "Windows Enumeration" example here on PSC, where when a user double clicks on a list item, it will ask them "Do you wish to close 'Window name here'". 99% of programs use this string combination. For example, when you exit Microsoft Word, doesn't it ask you to save and then the file name.
<br>
<br>
This is just the usage, not a complete program...
<br>
<br>
char sMessage[256];
<br>
char sFileName[256];
<br>
<br>
strcpy(sMessage,"Are you sure you wish to close ");
<br>
strcat(sMessage,sFileName);
<br>
strcat(sMessage, "?");
<br>
MessageBox(NULL,sMessage,0,0,0); //
<br>
<br>
Now, what we did here was assign the "Are you sure..." text into the sMessage variable (used strcpy), and then used strcat to add the data from sFileName to the sMessage variable. In other words, in vb this would look like:
<br>
sMessage = sMessage + sFileName.
<br>
Very simple right? Ok, we learned how to compare strings, assign data to them, and also add data to an already exisiting string. That is it! That was pretty simple. I am sorry for any grammatical errors. I know this is a lot more complex, yet I wanted to simplify it. There are more functions, yet these are crucial to c/c++.
<br>
<br>
Email Me with questions or comments. ALso, don't forget to check out my other submissions, and please leave comments and VOTE!!!!!

