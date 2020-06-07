# zzr2311559_python
record on my python learning process based on PYTHON CRASH COURSE written by Eric Matthes

![GitHub pull requests](https://img.shields.io/github/issues-pr/zzr2311559/zzr2311559_python)
![GitHub issues](https://img.shields.io/github/issues/zzr2311559/zzr2311559_python)


## Changing Case in a String with Methods
Here is the code:

      name = "ada zzr2311559"
      print(name.title())

**name** &emsp; &ensp; is the variable refers to the lowercase string "ada zzr2311559"

**title()** &ensp;&nbsp; is a method 

**.** &emsp;&emsp;&nbsp; is a sign to tell python to make the **title()** method act on the variable **name**



method: A method is an action that Python can preform on a piece of data. Every method is followed by a set of parentheses, because
methods often need additional information to do their work. That information is provided inside the parentheses.  The title() function doesn’t need any additional information, so its parentheses are empty. 

*Tips* ：you can change a string to all uppercase or all lowercase letters like this:

      name = 'Ada zzr2311559'
      print(name.upper())
      print(name.lower())


## Using Variables in Strings
How to use a variable’s value inside a string?
Here is the code:
      
      first_name = "ada"
      last_name = "zzr2311559"
      full_name = f"{first_name} {last_name}"
      print(full_name)

To insert a variable’s value into a string, place the letter f immediately before the opening quotation mark . Put braces around the name or names of any variable you want to use inside the string. Python will replace each variable with its value when the string is displayed.

These strings are called **f-strings**. The f is for format, because Python formats the string by replacing the name of any variable in braces with its value.

*Tips*:F-strings were first introduced in Python 3.6. If you’re using Python 3.5 or earlier, you’ll need to use the format() method rather than this f syntax. To use format(), list the variables you want to use in the string inside the parentheses following format. Each variable is referred to by a set of braces; the braces will be filled by the values listed in parentheses in the order provided:

      full_name = "{} {}".format(first_name, last_name)   
      

## Adding Whitespace to Strings with Tabs or Newlines

To add a *tab* to your text, use the character combination  **\t**  

      print("\tZzr2311559")

To add a *newline* in a string, use the character combination  **\n**

      print("\nZzr2311559")

You can also combine *tabs* and *newlines* in a single string. The string **\n\t"** tells Python to move to a new line, and start the next line with a tab. 
      
      print("User:\n\tZzr2311559\nGender:\n\tMale")


## Stripping Whitespace

Python can look for extra whitespace on the right and left sides of a string. To ensure that no whitespace exists at the right or left end of a string, use the rstrip() or lstirp() method.If you want to strip both of them, use strip() method.

Here is the code and its result on terminal

      >>> favorite_language = ' python '
      >>> favorite_language
      ' python '
      >>> favorite_language.rstrip()
      ' python'
      >>> favorite_language
      'python '#......................................as you can see, you actually only execute this command instead of changing the variable  **favorite_language** itself 
      >>> favorite_language.lstrip()
      'python '
      >>> favorite_language.strip()
      'python'












