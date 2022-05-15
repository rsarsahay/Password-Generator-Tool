# Password-Generator-Tool
The Password Generator Tool Creates a Random and customized Password for users that helps them to create a strong Password which provides greater security.
In this project, the user has to select the password length and then click on the “Generate Password” button.
It will show the generated password below. If the user clicks on the “Copy To Clipboard” button, then it will copy the password automatically.
To build this project we will use the basic concept of python and libraries – Tkinter, pyperclip, random, string.
Tkinter is a standard GUI library and is one of the easiest ways to build a GUI application.
pyperclip module allows us to copy and paste text to and from the clipboard to your computer
The random module can generate random numbers
string module contains a number of functions to process the standard python string.

Project File Structure
Let’s check the step to build a Password Generator using Python

1.Import modules
2.Initialized Window
3.Select Password Length
4.Define Functions

Steps to create random password generator
1. Import Libraries
  ->The first step is to import libraries
  
2. Initialize Window
  ->Tk() initialized tkinter which means window created
 ->geometry() set the width and height of the window
 ->resizable(0,0) set the fixed size of the window
 ->title() set the title of the window
 
Label() widget use to display one or more than one line of text that users can’t able to modify.
 ->root is the name which we refer to our window
 ->text which we display on the label
 ->font in which the text is written
 ->pack organized widget in block
 
3. Select Password Length
 ->pass_len is an integer type variable that stores the length of a password.
 ->To select the password length we use Spinbox() widget.
 ->Spinbox() widget is used to select from a fixed number of values. Here the value from 8 to 32
 
4. Function to Generate Password
 ->pass_str is a string type variable that stores the generated password
 ->password = “” is the empty string
 ->First loop will generate a string of length 4 which is a combination of an uppercase letter, 
   a lowercase letter, digits, and a special symbol and that string will store in password variable.
 ->The second loop will generate a random string of length entered by the user – 4 and add to the password variable.
   Here we minus 4 to the length of the user because we already generate the string of length 4.
   
We have done this because we want a password which must contain an uppercase, a lowercase, a digit, and a special symbol.

Now the password is set to the pass_str() variable.
 ->Button() widget used to display button on our window
 ->command is called when the button is click
 ->Entry() widget used to create an input text field
 ->textvariable used to retrieve the current text to the entry widget
 
5. Function to Copy Password
 -> pyperclip.copy() used to copy the text to clipboard
 
Summary
 With these steps, we have successfully created a random password generator project using python.
 We used popular tkinter library to rendering graphics in our display window and we also learned about pyperclip and random library.

 We learned how to create buttons, input textfield, labels, and spinbox. In this way, we successfully created
 our password generator python project. Hope you enjoyed it.


