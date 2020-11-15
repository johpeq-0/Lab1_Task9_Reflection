# Lab1_Task9_Reflection

Before I started with this lab I didn't know much about C or C++, nor anything about GitHub. I had some previous experience with C# from high school and some experience with Python from the last programming course. I now have som basic understanding of how cin and cout works as well as some understanding of printf and scanf. Just getting scanf to work in VisualStudio2019 was a bit of work as it is deemed unsafe by Visual Studio. As more or less always, googling the problem and watching YouTube videos is a good way to find a solution to this. I found out that one could either go into Project/Properties/Configuration Properties/C C++/Preprocessor Definitions and write _CRT_SECURE_NO_WARNINGS or just write #define _CRT_SECURE_NO_WARNINGS in the beginning of the program.

Another thing that I found a bit tricky is the user input with cin and scanf. The problem as I see it is that they only take one argument as input and when a whitespace occurs the information behind it is instead sent to the next cin or scanf, and so on and so on. In regards of cin I found a solution by using #include <iomanip> and in the cin input using setw() to limit the max number of letters or arguments and then using cin.clear() and cin.ignore() to ignore everything behind the whitespace and to clear the stream. For scanf I found out that you could use %n to limit the input to n number of characters and then using [^n] to change the behaviour of scanf to take all arguments until a newline characters. 
So far I have only gotten that to work on char arrays.
  
In general I feel that making stable code in C++ or C seems a lot harder for a beginner than doing the same in Python or C# but at the same time it's exiting to work with such a powerful programming language as C++. 

I think that the lab was good, but an improvement to the lab could be a some more information what is expected of our program. How stable should it be? (User input handling etcetera.)

I probably worked around 35 hours on this lab.
