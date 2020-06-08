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

To insert a variable’s value into a string, place the letter f immediately before the opening quotation mark. Put braces around the name or names of any variable you want to use inside the string. Python will replace each variable with its value when the string is displayed.

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


## Number


### Integers

You can add( + ),subtract( - ),multiply( * ), and divide(/) integers in Python. Moreover, Python uses two multiplication symbols to represent exponents. Python supports the order of operations too, so you can use multiple operations in one expression. You can also use parentheses to modify the order of operations so Python can evaluate your expression in the order you specify.

Here is the examples and results on terminal:

      >>> 2 + 3
      5
      >>> 3 - 2
      1
      >>> 2 * 3
      6
      >>> 3 / 2
      1.5
      
      >>> 3 ** 2
      9
      >>> 3 ** 3
      27
      >>> 10 ** 6
      1000000 
      
      >>> 2 + 3*4
      14
      >>> (2 + 3) * 4
      20


### Floats

Python calls any number with a decimal point a float. This term is used in most programming languages, and it refers to the fact that a decimal point can appear at any position in a number.

Mostly, you can simply use float as you will, but sometimes you can get an arbitrary number of decimal places in your answer:
 
      >>> 0.2 + 0.1
      0.30000000000000004
      >>> 3 * 0.1
      0.30000000000000004 
      
This happens in all languages and is of little concern. Python tries to find a way to represent the result as precisely as possible, which is sometimes difficult given how computers have to represent numbers internally.      


### Integers and Floats

Python defaults to a float in any operation that uses a float, even if the output is a whole number. For example:

      >>> 4/2
      2.0
      >>> 1 + 2.0
      3.0
      >>> 2 * 3.0
      6.0
      >>> 3.0 ** 2
      9.0


### Underscores in Numbers

When you’re writing long numbers, you can group digits using underscoresto make large numbers more readable:

      >>> universe_age = 14_000_000_000

When you print a number that was defined using underscores, Pythonprints only the digits:

      >>> print(universe_age)
      14000000000

Python ignores the underscores when storing these kinds of values. Even if you don’t group the digits in threes, the value will still be unaffected. To Python, 1000 is the same as 1_000, which is the same as 10_00. This feature works for integers and floats, but it’s only available in Python 3.6 and later.


### Multiple Assighment

You can assign values to more than one variable using just a single line. This can help shorten your programs and make them easier to read; you’ll use this technique most often when initializing a set of numbers.

      >>> x, y, z = 0, 0, 0   

You need to separate the variable names with commas, and do the same with the values, and Python will assign each value to its respectively positioned variable. As long as the number of values matches the number of variables, Python will match them up correctly.


### Constants

A constant is like a variable whose value stays the same throughout the life of a program. Python doesn’t have built-in constant types, but Python programmers use all capital letters to indicate a variable should be treated as a constant and never be changed:

MAX_CONNECTIONS = 5000


## Comments

In Python, the hash mark (#) indicates a comment. Anything following a hash mark in your code is ignored by the Python interpreter. 

When you’re determining whether to write a comment, ask yourself if you had to consider several approaches before coming up with a reasonable way to make something work; if so, write a comment about your solution. It’s much easier to delete extra comments later on than it is to go back and write comments for a sparsely commented program.


## The Zen of Python

You can access this brief set of principles for writing good Python code by entering **import this** into your interpreter.

      The Zen of Python, by Tim Peters
      
      Beautiful is better than ugly.
      Explicit is better than implicit.
      Simple is better than complex.
      Complex is better than complicated.
      Flat is better than nested.
      Sparse is better than dense.
      Readability counts.
      Special cases aren't special enough to break the rules.
      Although practicality beats purity.
      Errors should never pass silently.
      Unless explicitly silenced.
      In the face of ambiguity, refuse the temptation to guess.
      There should be one-- and preferably only one --obvious way to do it.
      Although that way may not be obvious at first unless you're Dutch.
      Now is better than never.
      Although never is often better than *right* now.
      If the implementation is hard to explain, it's a bad idea.
      If the implementation is easy to explain, it may be a good idea.
      Namespaces are one honking great idea -- let's do more of those!

------


## List

A list is a collection of items in a particular order. You can make a list that includes the letters of the alphabet, the digits from 0–9, or the names of all the people in your family. You can put anything you want into a list, it's a good idea to make the name of your list plural, such as **letters** , **digits**, or **names**. 

In Python, square brackets ([]) indicate a list, and individual elements in the list are separated by commas. Here is an example:

      riders = ['zio','decade','faiz','01']
      print(riders)

and Python returns its representation of the list as: ['zio','decade','faiz','01']  which is not the format you want your users to see
So this time try this:

      riders = ['zio','decade','faiz','01']
      print(riders[0].title())
      
you'll get **Zio** only! But why 0 instead of 1?

Python considers the first item in a list to be at position 0, not position 1. This is true of most programming languages, and the reason has to do with how the list operations are implemented at a lower level. Especially, by asking for the item at index -1, Python always returns the last item in the list:

      riders = ['zio','decade','faiz','01']
      print(riders[-1])

This convention extends to other negative index values as well. The index -2 returns the second item from the end of the list, the index -3 returns the third item from the end, and so forth.

You can also use individual values from a list just as you would any other variable. For example, you can use f-strings to create a message based on a value from a list.

      riders = ['zio','decade','faiz','01']
      message = f"My favorite kamen rider is {riders[-2].title()}!"
      print(message)
      
      
## Changing, Adding, and Removing Elements       

Most lists you create will be dynamic, meaning you’ll build a list and then add and remove elements from it as your program runs its course. 


### Modifying Elements in a List

The syntax for modifying an element is similar to the syntax for accessing an element in a list. To change an element, use the name of the list followed by the index of the element you want to change, and then provide the new value you want that item to have:

      riders = ['zio','faiz','01']
      riders[0] = 'decade'
      print(riders)

### Adding Elements to a List

 Python provides several ways to add new data to existing lists.


#### Appending Elements to the End of a List

The simplest way to add a new element to a list is to append the item to the list. When you append an item to a list, the new element is added to the end of the list:

     riders = ['zio','faiz','01']
     riders.append('decade')
     print(riders)

The append() method makes it easy to build lists dynamically. For example, you can start with an empty list and then add items to the list using a series of append() calls. 

      riders = []
      
      riders.append('zio')
      riders.append('decade')
      riders.append('faiz')
      print(riders)

Building lists this way is very common, because you often won’t know the data your users want to store in a program until after the program is running. To put your users in control, start by defining an empty list that will hold the users’ values. Then append each new value provided to the list you just created.


#### Inserting Elements into a List

You can add a new element at any position in your list by using the insert() method. You do this by specifying the index of the new element and the value of the new item.

      riders = ['zio','01','faiz']
      riders.insert(1,'decade')
      print(riders)

In this example, the code inserts the value 'decade' at the position 1 of the list. The **insert()** method opens a space at position 1 and stores the value 'decade' at that location.


### Removing Elements from a List

In Python, you can remove anitem according to its position in the list or according to its value.


#### Removing an Item Using the del Statement


































