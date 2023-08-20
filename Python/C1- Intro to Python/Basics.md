# Chapter 1: Python Basics
- Guido Van Russo
- General purpose: build anything
- Open source! Free!
- Python packages, for Data Science
#### ipython shell
- runs commands interactively
### Python scripts
- Text files with the extension .py
- List of Python commands that are executed
- To add comments to the Python script, use the # tag
- Use print() to generate output from the script
### Operations
- Addition, subtraction: +, -
- Multiplication, division: *,/
- modulo: returns remainder: %
- Exponentiation: **. This operator raises the number to its left to the power of the number to its right.
### Variables
- variable: a specific, case-sensitive name.
- a variable allows you to refer to a value with a name.
- After declaring a variable, you can later call up its value by typing the variable name.
- Variables help to make your code reproducible.
### Python data types
- Check out the type of a value with the type function.
- float type: Real number, can have both an integer part and a fraction part
- int type: Integer number
- String: String is Python's way of representing text.
- bool: True or False, logical value. (The capitalization is important!).
- For different data types, operators behave differently.
### Variable Assignment
- x = 5
- = in Python means assignment, it doesn't test equality!
###Type conversion
- Using the + operator to paste together two strings can be very useful in building custom messages. This is called the concatenation of string.
- can only concatenate str with string, not "int" to str. So to concatenate an int to string, first you have to do type conversion of int to str.
- functions such as int(), float(), str() and bool() will help you convert Python values into any type.

# Chapter 2: Python Lists
- int, float, str data type variables store a single value
- In data science, we may need to work with many data points
### List
- A list is a compound data type; you can group values together.
- A list is a way to give a single name to a collection of values.
- can contain any data type value.
- list = []
- my_list = [el1, el2, el3]
- A list can also contain a mix of Python types including strings, floats, booleans, etc.
- A list can also contain lists inside it, a list of lists.
### Subsetting Lists
- to access items in list index is used
- zero indexing: index starts at 0
- To count backward, negative indexing is used. So the last element is list[-1]
### List slicing
- Allows you to select multiple elements from the list
- slicing syntax: my_list[start:end] [inclusive : exclusive]
- The start index will be included, while the end index is not.
- [:4] means start slice from index 0
- [4:] means include all elements up to and including the last element in the list
### Manipulating Lists
- ways to change elements in your list, or to add elements to and remove elements from your list.
- Replacing list elements is pretty easy. Simply subset the list and assign new values to the subset. You can select single elements or you can change entire list slices at once.
- changing list item: list[index] = new_value or list[idx1 : idx2] = [new_value1, new_value2]
- adding new items to a list: list_updated = list + [value 1, value 2]
- deleting items from list: del(list[index])
- Pay attention here: as soon as you remove an element from a list, the indexes of the elements that come after the deleted element all change!

### Copying Lists
- - What actually happens when you create a new list, x, you're storing a list in your computer memory, and storing the 'address' of that list in x.
- This means that x does not actually contain all the list elements, it rather contains a reference to the list.
- list1 = list2 means copying the reference to the list. It means any change or update in one list will also change or update both lists.
- If you want to create a list y that points to a new list in the memory with the same values as list x, you'll need to use something else than the equals sign. You can use the list function of use slicing to select all list elements explicitly.
- new_list = list(old_list) or new_list = old_list[:]



- The ; sign is used to place commands on the same line. The following two code chunks are equivalent:
-  Same line: command1; command2
- Separate lines:
- command1
- command2


