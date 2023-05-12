# https://www.interviewbit.com/python-interview-questions/

**What is Python? What are the benefits of using Python?**

Python is a high-level, interpreted, general-purpose programming language. Being a general-purpose language,
it can be used to build almost any type of application with the right tools/libraries. Additionally, python
supports objects, modules, threads, exception-handling, and automatic memory management which help in
modelling real-world problems and building applications to solve these problems.

Benefits of using Python:
Python is a general-purpose programming language that has a simple, easy-to-learn syntax that emphasizes
readability and therefore reduces the cost of program maintenance. Moreover, the language is capable of
scripting, is completely open-source, and supports third-party packages encouraging modularity and code reuse.
Its high-level data structures, combined with dynamic typing and dynamic binding, attract a huge community
of developers for Rapid Application Development and deployment.

----

**What is a dynamically typed language?**

Before we understand a dynamically typed language, we should learn about what typing is. Typing refers to
type-checking in programming languages. In a strongly-typed language, such as Python, "1" + 2 will result
in a type error since these languages don't allow for "type-coercion" (implicit conversion of data types).
On the other hand, a weakly-typed language, such as Javascript, will simply output "12" as result.
Type-checking can be done at two stages -
Static - Data Types are checked before execution.
Dynamic - Data Types are checked during execution.
Python is an interpreted language, executes each statement line by line and thus type-checking is
done on the fly, during execution. Hence, Python is a Dynamically Typed Language.

----

**What is an Interpreted language?**

An Interpreted language executes its statements line by line. Languages such as Python, Javascript, R, PHP, and
Ruby are prime examples of Interpreted languages. Programs written in an interpreted language runs directly from
the source code, with no intermediary compilation step.

----

**What is PEP 8 and why is it important?**

PEP stands for Python Enhancement Proposal. A PEP is an official design document providing information to the
Python community, or describing a new feature for Python or its processes. PEP 8 is especially important since
it documents the style guidelines for Python Code. Apparently contributing to the Python open-source community
requires you to follow these style guidelines sincerely and strictly.

----

**What is Scope in Python?**

Every object in Python functions within a scope. A scope is a block of code where an object in Python remains
relevant. Namespaces uniquely identify all the objects inside a program. However, these namespaces also have
a scope defined for them where you could use their objects without any prefix. A few examples of scope created
during code execution in Python are as follows:
- A local scope refers to the local objects available in the current function.
- A global scope refers to the objects available throughout the code execution since their inception.
- A module-level scope refers to the global objects of the current module accessible in the program.
- An outermost scope refers to all the built-in names callable in the program. The objects in this scope are searched last to find the name referenced.

Note: Local scope objects can be synced with global scope objects using keywords such as global.

----

**What are lists and tuples? What is the key difference between the two?**

Lists and Tuples are both sequence data types that can store a collection of objects in Python. The objects
stored in both sequences can have different data types.

Lists are represented with square brackets:

```python
['sara', 6, 0.19]
```

while tuples are represented with parantheses:

```python
('ansh', 5, 0.97).
```

But what is the real difference between the two?
The key difference between the two is that while lists are mutable, tuples on the other hand are immutable
objects. This means that lists can be modified, appended or sliced on the go but tuples remain constant and
cannot be modified in any manner. You can run the following example on Python IDLE to confirm the difference:

```python
example_tuple = ('sara', 6, 5, 0.97)
example_list = ['sara', 6, 5, 0.97]

print(example_tuple[0]) # output => 'sara'
print(example_list[0]) # output => 'sara'

# my_tuple[0] = 'ansh' # modifying tuple => throws an error
# Exception has occurred: TypeError
# 'tuple' object does not support item assignment

example_list[0] = 'ansh' # modifying list => list modified
print(example_tuple[0]) # output => 'sara'
print(example_list[0]) # output => 'ansh'
```

----

**What are the common built-in data types in Python?**

There are several built-in data types in Python. Although, Python doesn't require data types to be defined
explicitly during variable declarations type errors are likely to occur if the knowledge of data types
and their compatibility with each other are neglected. Python provides type() and isinstance() functions
to check the type of these variables. These data types can be grouped into the following categories-

__None Type__

None keyword represents the null values in Python. Boolean equality operation can be performed using these NoneType objects.

| Class Name | Description | Example |
| --------- | ------------- | ------- |
| NoneType | Represents the NULL values in Python. | ```python print(type(None)) ``` |

__Numeric Types__

There are three distinct numeric types:
- integers
- floating-point numbers
- complex numbers.
- Additionally, booleans are a sub-type of integers.

| Class Name | Description | Example |
| ---------- | ----------- | ------- |
| int | Stores integer literals including hex, octal and binary numbers as integers. | ```python print(443) ``` |
| float | Stores literals containing decimal values and/or exponent signs as floating-point numbers. | ```python print(34.89) ``` |
| complex | Stores complex numbers in the form (A + Bj) and has attributes: real and image. | ```python print(complex(3)), Output: (3+0j) ``` |
| bool | Stores boolean value (True or False). | ```python print(1 == 1), Output: True ``` |

Note: The standard library also includes [fractions](https://docs.python.org/3/library/fractions.html) to store rational numbers and decimal
to store floating-point numbers with user-defined precision.

__Sequence Types:__

According to Python Docs, there are three basic Sequence Types:
- lists
- tuples
- range objects.

Sequence types have the in and not in operators defined for their traversing their elements. These operators share the same priority as
the comparison operations.

| Class Name | Description | Example |
| ---------- | ----------- | ------- |
| list | Mutable sequence used to store collection of items. | ```python print([1,2,3,4]) ``` |
| tuple | Immutable sequence used to store collection of items. | ```python print(("mouse", [8, 4, 6], (1, 2, 3))) ``` |
| range | Represents an immutable sequence of numbers generated during execution. | ```python range(3, 6) ``` |
| str | Immutable sequence of Unicode code points to store textual data. | ```python print("This is an example string") ``` |

Note: The standard library also includes additional types for processing:
1. Binary data such as
   * bytearray - ```python array1 = bytearray(str, 'utf-8') # encoding the string with utf-8.```
   * bytes - ```python b'\xf0\xf1\xf2'.hex() # Return a string object containing two hexadecimal digits for each byte in the instance.```
   * [memoryview](https://www.geeksforgeeks.org/memoryview-in-python/) - ```python memoryview(b'abcefg')```
 , and ...
3. Text strings such as str.

__Mapping Types:__

A mapping object can map hashable values to random objects in Python. Mappings objects are mutable and there is currently only one standard mapping type, the dictionary.

| Class Name | Description | Description |
| ---------- | ----------- | ------------ |
| dict | Stores comma-separated list of key: value pairs | ```python { "name": "thisIsAFirstName", "age": 25 }``` |

__Set Types:__

Currently, Python has two built-in set types - set and frozenset. set type is mutable and supports methods like add() and remove().
frozenset type is immutable and can't be modified after creation.

| Class Name | Description | Examples |
| ---------- | ----------- | -------- |
| set | Mutable unordered collection of distinct hashable objects. | ```python  myset = {"apple", "banana", "cherry"}``` |
| frozenset | Immutable collection of distinct hashable objects. | ```python  frozenset(["apple", "banana", "cherry"])``` |

Note: set is mutable and thus cannot be used as key for a dictionary.
On the other hand, frozenset is immutable and thus, hashable, and can be used as a dictionary key or as an element of another set.

__Modules:__

Module is an additional built-in type supported by the Python Interpreter. It supports one special operation, i.e., attribute access:

```python
mymod.myobj
```

where mymod is a module and myobj references a name defined in m's symbol table. The module's symbol table resides in a
very special attribute of the module __dict__, but direct assignment to this module is neither possible nor recommended.

__Callable Types:__

Callable types are the types to which function call can be applied. They can be user-defined functions, instance methods, generator
functions, and some other built-in functions, methods and classes.
Refer to the documentation at docs.python.org for a detailed view of the callable types.

----

**What is 'pass' in Python?**

The pass keyword represents a null operation in Python. It is generally used for the purpose of filling up empty blocks of code which may
execute during runtime but has yet to be written. Without the pass statement in the following code, we may run into some errors during code execution.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def empty_func_with_pass():
    """Do nothing here."""
    pass

def empty_func_without_pass():
    """Do othing here without using
    pass statement.
    """

def main():
    """Running code."""
    # nothing happens
    empty_func_with_pass()
    # no pass statement in python 3 needed
    empty_func_without_pass()

if __name__ == '__main__':
    main()
```

----

**What are modules and packages in Python?**

Python packages and Python modules are two mechanisms that allow for modular programming in Python.

Modularizing has several advantages:

__Simplicity:__

Working on a single module helps you focus on a relatively small portion of the problem at hand. This makes development easier and less error-prone.

__Maintainability:__

Modules are designed to enforce logical boundaries between different problem domains. If they are written in a manner that reduces interdependency,
it is less likely that modifications in a module might impact other parts of the program.

__Reusability:__

Functions defined in a module can be easily reused by other parts of the application.

__Scoping:__

Modules typically define a separate namespace, which helps avoid confusion between identifiers from other
parts of the program.

Modules, in general, are simply Python files with a .py extension and can have a set of functions, classes,
or variables defined and implemented. They can be imported and initialized once using the import statement.
If partial functionality is needed, import the requisite classes or functions using from foo import bar.

Packages allow for hierarchial structuring of the module namespace using dot notation. As, modules help
avoid clashes between global variable names, in a similar manner, packages help avoid clashes between
module names. Creating a package is easy since it makes use of the system's inherent file structure.
So just stuff the modules into a folder and there you have it, the folder name as the package name.
Importing a module or its contents from this package requires the package name as prefix to the module
name joined by a dot.

NOTE: You can technically import the package as well, but alas, it doesn't import the modules within the
package to the local namespace, thus, it is practically useless.

----

**What are global, protected and private attributes in Python?**

**Global variables** are public variables that are defined in the global scope. To use the variable in the global scope inside a function, we
use the global keyword.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def my_func():
  x = "fantastic"
  print("Python is " + x)

def main():
    x = "awesome"
    print(my_func("Python is " + x))
    print("Python is " + x)

if __name__ == '__main__':
    main()
```

**Protected attributes** are attributes defined with an underscore prefixed to their identifier eg. _sara. They can still be accessed and
modified from outside the class they are defined in but a responsible developer should refrain from doing so.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

class Student:

    _schoolName = 'XYZ School' # protected class attribute

    def __init__(self, name, age):
        self._name = name # protected instance attribute
        self._age = age # protected instance attribute

def main():
    student_1 = Student("Jack", 25)
    print(student_1._name)
    student_1._name = "John"
    print(student_1._name)

if __name__ == '__main__':
    main()
```

**Private attributes** are attributes with double underscore prefixed to their identifier eg. __ansh. They cannot be accessed or modified
from the outside directly and will result in an AttributeError if such an attempt is made.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

class Geek:
    def _single_method(self):
        pass
    def __double_method(self): # for mangling
        pass
class Pyth(Geek):
    def __double_method(self): # for mangling
        pass

def main():
    pass

if __name__ == '__main__':
    main()
```

----

**What is the use of 'self' in Python?**

Used to represent the instance of the class. With this keyword, you can access the attributes and methods of
the class in python. It binds the attributes with the given arguments. self is used in different places and
often thought to be a keyword. But unlike in C++, self is not a keyword in Python.

----

**What is '__init__'?**

```python __init__ ``` is a constructor method in Python and is automatically called to allocate memory when a new object/instance is created. All classes
have such a __method associated with them__. It helps in distinguishing methods and attributes of a class from local variables.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

class Student:

    def __init__(self, fname, lname, age, section):
        self.firstname = fname
        self.lastname = lname
        self.age = age
        self.section = section

def main():
    stu_1 = Student("Sara", "Ansh", 22, "A2")
    print(stu_1)

if __name__ == '__main__':
    main()
```

----

**What is 'break', 'continue' and 'pass' in Python?**

__break__

The break statement terminates the loop immediately and the control flows to the statement after
the body of the loop.

__continue__

The continue statement terminates the current iteration of the statement, skips the rest of
the code in the current iteration and the control flows to the next iteration of the loop.

__pass__

As explained above, the pass keyword in Python is generally used to fill up empty blocks and
is similar to an empty statement represented by a semi-colon in languages such as
Java, C++, Javascript, etc.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def main():
    pat = [1, 3, 2, 1, 2, 3, 1, 0, 1, 3]
    for p in pat:
        if (p == 0):
            current = p
            break
        elif (p % 2 == 0):
            continue
        print(p) # output => 1 3 1 3 1
    print(current) # output => 0

if __name__ == '__main__':
    main()
```

----

**What are unit tests in Python?**

Unit test is a unit testing framework of Python.

Unit testing means testing different components of software separately.

__Can you think about why unit testing is important?__

Imagine a scenario, you are building software that uses three components namely A, B, and C.
Now, suppose your software breaks at a point time. How will you find which component was
responsible for breaking the software? Maybe it was component A that failed, which in turn
failed component B, and this actually failed the software. There can be many such combinations.

This is why it is necessary to test each and every component properly so that we know which component might be highly responsible for the failure of the software.

Example can be viewed here:

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

import random
import unittest

class TestDemo:

    def __init__(self, s: str):
        self.obj_counter: int = 0
        self.id: int = self.obj_counter+1
        print (s + ": count = " + id)

    def close(self):
        print ("Cleaning up: " + id)

    def some_condition(self):
        return 0
    
    def objCounter(self):
        for i in range(random.randint(0,10)):
            print(i)

class Test(unittest.Testcase):

    def __init__(self):
        self.test_1 = TestDemo("test1")
        self.test_2 = TestDemo("test2")

    def cleanup(self):
        self.test_2.close()
        self.test_1.close()

    def test_a(self):
        print("TestDemo.testA")
        self.assertIsNotNone(self.test_1.some_condition())

    def test_b(self):
        print("TestDemo.testB")
        self.assertIsNotNone(self.test_2.some_condition())
        self.assertIsNotNone(TestDemo.objCounter != 0)
        # Causes the build to halt:
        def test_3(self):
            self.assertTrue(0) 
```

----

**What are 'docstrings' in Python?**

Documentation string or docstring is a multiline string used to document a specific code segment.
The docstring should describe what the function or method does. The ensemble of docstrings should
be read like a history in the program.

----

**What is slicing in Python?**

As the name suggests, slicing is taking parts of.

Syntax for slicing is:

```python
[start : stop : step]
```

- start is the starting index from where to slice a list or tuple. Default value: 0
- stop is the ending index or where to sop.
- step is the number of steps to jump.

Default value for start is 0, stop is number of items, step is 1.

Slicing can be done on strings, arrays, lists, and tuples.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def main():
    numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    print(numbers[1::2]) # output : [2, 4, 6, 8, 10]
    print(numbers[:1]) # output : [1]
    print(numbers[0]) # output : 1 (get value of index 0)
    print(numbers[:2]) # output : [1, 2]
    print(numbers[2:]) # output : [3, 4, 5, 6, 7, 8, 9, 10]
    print(numbers[:3]) # output : [1, 2, 3]
    print(numbers[4:]) # output : [5, 6, 7, 8, 9, 10]
    print(numbers[:-3]) # output : [1, 2, 3, 4, 5, 6, 7]
    print(numbers[-4:]) # output : [7, 8, 9, 10]

if __name__ == '__main__':
    main()
```

----

**Explain how can you make a Python Script executable on Unix?**

Script file must begin with:

```python
#!/usr/bin/env python3
```

```python
#!/usr/bin/python3 // run with system Python
#!/usr/bin/env python3 // run with dev version

def main():
    ...

if __name__ == '__main__':
    main()    
```

----

**What is the difference between python arrays and lists?**

*Arrays* in python can only contain __elements of same data types__ i.e., data type of array should be homogeneous.
It is a thin wrapper around C language arrays and consumes far less memory than lists.

```python
# Example
int_array = array.array('i', [-1, 0, 1, 2])
```

*Lists* in python can contain elements of different data types i.e., data
type of lists can be heterogeneous.
It has the disadvantage of consuming large memory.

```python
int_list = [1,3,"firstName","secondName"]
```

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

import array

def main():
    a = array.array('i', [1, 2, 3])
    for i in a:
        print(i, end=' ') # OUTPUT: 1 2 3
    # a = array.array('i', [1, 2, 'string']) #OUTPUT: TypeError: an integer is required (got type str)
    a = [1, 2, 'string']
    for i in a:
        print(i, end=' ') # OUTPUT: 1 2 string

if __name__ == '__main__':
    main()
```

----

**How is memory managed in Python?**

Memory management in Python is handled by the *Python Memory Manager*. The memory allocated by the manager is
in form of a *private heap space dedicated to Python*. All Python objects are stored in this heap and being
private, it is *inaccessible to the programmer*. Though, python does provide some core API functions to work
upon the private heap space.

Additionally, Python has an *in-built garbage collection* to recycle the unused memory for the private heap space.

----

**What are Python namespaces? Why are they used?**

A namespace in Python ensures that object names in a program are unique and can be used without any conflict.

Python implements these namespaces as dictionaries with 'name as key' mapped to a corresponding *object as value*.
This allows for multiple namespaces to use the same name and map it to a separate object.

A few examples of namespaces are as follows:

*Local Namespace* includes local names inside a function. the namespace is temporarily created for
a function call and gets cleared when the function returns.

*Global Namespace* includes names from various imported packages/ modules that are being used in the
current project. This namespace is created when the package is imported in the script and lasts
until the execution of the script.

*Built-in Namespace* includes built-in functions of core Python and built-in names for various types of exceptions.
The lifecycle of a namespace depends upon the scope of objects they are mapped to. If the scope of an object ends, the lifecycle of
that namespace comes to an end. Hence, it isn't possible to access inner namespace objects from an outer namespace.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def some_func():
    print("Inside some_func")
    def some_inner_func():
        var = 10
        print("Inside inner function, value of var:",var)
    some_inner_func()
    print("Try printing var from outer function: ",var)

def main():
    # var1 is in the global namespace
    var1 = 5
    
    def some_func():
        # var2 is in the local namespace
        var2 = 6

        def some_inner_func():
            # var3 is in the nested local
            # namespace
            var3 = 7

    # Python program processing
    # global variable
    count = 5
    def some_method():
        global count
        count = count + 1
        print(count)
    some_method()

    # Python program showing
    # a scope of object
    some_func()        

if __name__ == '__main__':
    main()
```

**What is Scope Resolution in Python?**

Sometimes objects within the same scope have the same name but function differently. In such cases,
__scope resolution__ comes into play in Python automatically.

An example of such behavior are:

Python modules namely 'math' and 'cmath' have a lot of functions that are common to both of them - log10(), acos(), exp() etc.
To resolve this ambiguity, it is necessary to prefix them with their respective module, like math.exp() and cmath.exp().

```python
# Consider the code below, an object temp has been initialized to 10 globally and
# then to 20 on function call. 
# However, the function call didn't change the value of the temp globally. Here, we
# can observe that Python draws a clear line between global and local variables,
# treating their namespaces as separate identities.
temp = 10 # global-scope variable
def func():
     temp = 20 # local-scope variable
     print(temp)
print(temp) # output: 10
func() # output: 20
print(temp) # output: 10
```

```python
# This behavior above can be overridden using the global keyword inside
# the function, as shown in the following example:
temp = 10   # global-scope variable
def func():
     global temp
     temp = 20   # local-scope variable
     print(temp)
print(temp) # output; 10
func() # output; 20
print(temp)# output; 20
```

----

**What are decorators in Python?**

Decorators in Python are essentially functions that add functionality to an existing function in Python without changing the structure
of the function itself. They are represented the @decorator_name in Python and are called in a bottom-up fashion.

For example:

```python
# decorator function to convert to lowercase
def lowercase_decorator(function):
   def wrapper():
       func = function()
       string_lowercase = func.lower()
       return string_lowercase
   return wrapper
   
# decorator function to split words
def splitter_decorator(function):
   def wrapper():
       func = function()
       string_split = func.split()
       return string_split
   return wrapper
   
def main():
    @splitter_decorator # this is executed next
    @lowercase_decorator # this is executed first
    def hello():
        return 'Hello World'
    hello() # output: [ 'hello' , 'world' ]
    
if __name__ == '__main__':
    main()    
```

The beauty of the decorators lies in the fact that besides adding functionality to the output of the method, they can even
accept arguments for functions and can further modify those arguments before passing it to the function itself. The inner
nested function, i.e. 'wrapper' function, plays a significant role here. It is implemented to enforce encapsulation and thus,
keep itself hidden from the global scope.

```python
# decorator function to capitalize names
def names_decorator(function):
    def wrapper(arg1, arg2):
        arg1 = arg1.capitalize()
        arg2 = arg2.capitalize()
        string_hello = function(arg1, arg2)
        return string_hello
    return wrapper
   
def main():
    @names_decorator
    def say_hello(name1, name2):
        return 'Hello ' + name1 + '! Hello ' + name2 + '!'
    say_hello('sara', 'ansh')   # output => 'Hello Sara! Hello Ansh!'

if __name__ == '__main__':
    main()  
```

----

**What are Dict and List comprehensions?**

Python comprehensions, like decorators, are syntactic sugar constructs that help build altered and filtered lists, dictionaries, or sets
from a given list, dictionary, or set. Using comprehensions saves a lot of time and code that might be considerably more verbose
(containing more lines of code). Let's check out some examples, where comprehensions can be truly beneficial:

```python
# Performing mathematical operations on the entire list
my_list = [2, 3, 5, 7, 11]
squared_list = [x**2 for x in my_list]    # list comprehension
# output: [4 , 9 , 25 , 49 , 121]

squared_dict = {x:x**2 for x in my_list}    # dict comprehension
# output: {11: 121, 2: 4 , 3: 9 , 5: 25 , 7: 49}

# Performing conditional filtering operations on the entire list
my_list = [2, 3, 5, 7, 11]
squared_list = [x**2 for x in my_list if x%2 != 0]    # list comprehension
# output: [9 , 25 , 49 , 121]

squared_dict = {x:x**2 for x in my_list if x%2 != 0}    # dict comprehension
# output: {11: 121, 3: 9 , 5: 25 , 7: 49}

# Combining multiple lists into one

# Comprehensions allow for multiple iterators and hence, can be used to combine multiple lists into one. 
a = [1, 2, 3]
b = [7, 8, 9]
[(x + y) for (x,y) in zip(a,b)] # parallel iterators
# output: [8, 10, 12]

[(x,y) for x in a for y in b] # nested iterators
# output: [(1, 7), (1, 8), (1, 9), (2, 7), (2, 8), (2, 9), (3, 7), (3, 8), (3, 9)] 

# Flattening a multi-dimensional list

# A similar approach of nested iterators (as above) can be applied to flatten a multi-dimensional list
# or work upon its inner elements. 
my_list = [[10,20,30],[40,50,60],[70,80,90]]
flattened = [x for temp in my_list for x in temp]
# output: [10, 20, 30, 40, 50, 60, 70, 80, 90]
```

Note: List comprehensions have the same effect as the map method in other languages.
They follow the mathematical set builder notation rather than map and filter functions in Python.

----

**What is lambda in Python? Why is it used?**

Lambda is an anonymous function in Python, that can accept any number of arguments, but can only have a single expression.
It is generally used in situations requiring an anonymous function for a short time period. Lambda functions can be used
in either of the two ways:

```python
# assigning lambda functions to a variable:
mul = lambda a, b : a * b
print(mul(2, 5)) # output: 10
Wrapping lambda functions inside another function:
def myWrapper(n):
 return lambda a : a * n
mulFive = myWrapper(5)
print(mulFive(2)) # output: 10
```

----

**How do you copy an object in Python?**

In Python, the assignment statement ('='-operator) does not copy objects. Instead, it creates a binding between
the existing object and the target variable name. To create copies of an object in Python, we need to use the
copy module. Moreover, there are two ways of creating copies for the given object using the copy module:

*Shallow Copy* is a bit-wise copy of an object. The copied object created has an exact copy of the values in the original object. If either of the values
is a reference to other objects, just the reference addresses for the same are copied.

*Deep Copy* copies all values recursively from source to target object, i.e. it even duplicates the objects referenced by the source object.

```python
from copy import copy, deepcopy
list_1 = [1, 2, [3, 5], 4]

# shallow copy
list_2 = copy(list_1) 
list_2[3] = 7
list_2[2].append(6)
list_2 # output: [1, 2, [3, 5, 6], 7]
list_1 # output: [1, 2, [3, 5, 6], 4]

# deep copy
list_3 = deepcopy(list_1)
list_3[3] = 8
list_3[2].append(7)
list_3 # output: [1, 2, [3, 5, 6, 7], 8]
list_1 # output: [1, 2, [3, 5, 6], 4]
```

----

**What is the difference between xrange and range in Python?**

*xrange() and range()* are quite similar in terms of functionality. They both generate a sequence of integers,
with the only difference that range() returns a Python list, whereas, xrange() returns an xrange object.

*So how does that make a difference?*

It sure does, because unlike range(), xrange() doesn't generate a static list, it creates the value on the go. This technique is
commonly used with an object-type generator and has been termed as "yielding".

Yielding is crucial in applications where memory is a constraint. Creating a static list as in range() can lead to a Memory Error in such
conditions, while, xrange() can handle it optimally by using just enough memory for the generator (significantly less in comparison).

```python
for i in xrange(10): # numbers from 0 to 9
   print i # output => 0 1 2 3 4 5 6 7 8 9
for i in xrange(1,10): # numbers from 1 to 9
   print i # output => 1 2 3 4 5 6 7 8 9
for i in xrange(1, 10, 2): # skip by two for next
   print i # output => 1 3 5 7 9
```

Note: xrange has been deprecated as of Python 3.x. Now range does exactly the same as what xrange used to
do in Python 2.x, since it was way better to use xrange() than the original range() function in Python 2.x.

----

**What is pickling and unpickling?**

Python library offers a feature - *serialization out of the box*.

Serializing an object refers to transforming it into a format that can be stored, so as to be able to
deserialize it, later on, to obtain the original object. Here, the pickle module comes into play.

*Pickling:*

Pickling is the name of the serialization process in Python. Any object in Python can be serialized into a byte stream and dumped as a file in the memory.
The process of pickling is compact but pickle objects can be compressed further. Moreover, pickle keeps track of the objects it has serialized and the
serialization is portable across versions. The function used for the above process is:

```python
pickle.dump()
```

*Unpickling:*

Unpickling is the complete inverse of pickling. It deserializes the byte stream to recreate the objects stored in the file and loads the object to memory.
The function used for the above process is:

```python
pickle.load().
```

Note: Python has another, more primitive, serialization module called marshall, which exists primarily to support .pyc files in Python and differs significantly from the pickle.

----

*What are generators in Python?*

Generators are functions that return an iterable collection of items, one at a time, in a set manner. Generators, in general, are used to create iterators with a different approach. They employ the use of
yield keyword rather than return to return a generator object.
Let's try and build a generator for fibonacci numbers -

```python
## generate fibonacci numbers upto n
def fib(n):
   p, q = 0, 1
   while(p < n):
       yield p
       p, q = q, p + q
x = fib(10)    # create generator object 
 
## iterating using __next__(), for Python2, use next()
x.__next__()    # output => 0
x.__next__()    # output => 1
x.__next__()    # output => 1
x.__next__()    # output => 2
x.__next__()    # output => 3
x.__next__()    # output => 5
x.__next__()    # output => 8
x.__next__()    # error
 
## iterating using loop
for i in fib(10):
   print(i)    # output => 0 1 1 2 3 5 8
```

----

**What is PYTHONPATH in Python?**

PYTHONPATH is an environment variable which you can set to add additional directories where Python will
look for modules and packages.

This is especially useful in maintaining Python libraries that you do not wish to install in the global default location.

----

**What is the use of help() and dir() functions?**

__help()__

help() function in Python is used to display the documentation of modules, classes, functions, keywords,
etc.

```python
help('print')
help('math')
help('')
```

If no parameter is passed to the help() function, then an interactive help utility is launched on the console.

__dir()__

dir() function tries to return a valid list of attributes and methods of the object it is called upon. It behaves differently with different objects, as it aims to produce the most relevant data, rather than the complete information.

```python
class Person:
    
    def __init__(self, name, age, country):
      ...
      self.name = name
      self.age = age
      self.country = country
     
     def get_name(self):
        return self.name
     
     def get_coutry(self):
        ...

print(dir(Person))
```

For Modules/Library objects, it returns a list of all attributes, contained in that module.
For Class Objects, it returns a list of all valid attributes and base attributes.
With no arguments passed, it returns a list of attributes in the current scope.

----

**What is the difference between .py and .pyc files?**

.py files contain the source code of a program. Whereas, .pyc file contains the bytecode of your program.
We get bytecode after compilation of .py file (source code).

.pyc files are not created for all the files that you run. It is only created for the files that you import.

Before executing a python program python interpreter checks for the compiled files. If the file is
present, the virtual machine executes it. If not found, it checks for .py file. If found, compiles
it to .pyc file and then python virtual machine executes it.
Having .pyc file saves you the compilation time.

----

**How Python is interpreted?**

Python as a language is not interpreted or compiled. Interpreted or compiled is the property of the implementation.

Python is a bytecode(set of interpreter readable instructions) interpreted generally.

Source code is a file with .py extension.

Python compiles the source code to a set of instructions for a virtual machine. The Python interpreter
is an implementation of that virtual machine. This intermediate format is called __bytecode__.

.py source code is first compiled to give .pyc which is bytecode. This bytecode can be then interpreted
by the official CPython or JIT(Just in Time compiler) compiled by PyPy.

----

**How are arguments passed by value or by reference in python?**

*Pass by value:* Copy of the actual object is passed. Changing the value of the copy of the object
will not change the value of the original object.

*Pass by reference:* Reference to the actual object is passed. Changing the value of the new object
will change the value of the original object.

In Python, arguments are passed by reference, i.e., reference to the actual object is passed.

```python
def appendNumber(arr):
  arr.append(4)

arr = [1, 2, 3]
print(arr)  # output: [1, 2, 3]
appendNumber(arr)
print(arr)  # output: [1, 2, 3, 4]
```

----

**What are iterators in Python?**

An iterator is an object.

It remembers its state i.e., where it is during iteration (see code below to see how)
__iter__() method initializes an iterator.

It has a __next__() method which returns the next item in iteration and points to the next element.
Upon reaching the end of iterable object __next__() must return StopIteration exception.
It is also self-iterable.

Iterators are objects with which we can iterate over iterable objects like lists, strings, etc.

```python
class ArrayList:

   def __init__(self, number_list):
       self.numbers = number_list
       
   def __iter__(self):
       self.pos = 0
       return self
       
   def __next__(self):
       if(self.pos < len(self.numbers)):
           self.pos += 1
           return self.numbers[self.pos - 1]
       else:
           raise StopIteration
           
array_obj = ArrayList([1, 2, 3])
it = iter(array_obj)
print(next(it)) #output: 2
print(next(it)) #output: 3
print(next(it))
# Throws Exception
# Traceback (most recent call last):
# ...
# StopIteration
```

----

**Explain how to delete a file in Python?**

Use command:

```python
os.remove(file_name)
```

```python
import os
os.remove("ChangedFile.csv")
print("File Removed!")
```

**Explain split() and join() functions in Python?**

You can use split() function to split a string based on a delimiter to a list of strings.
You can use join() function to join a list of strings based on a delimiter to give a single string.
string = "This is a string."
string_list = string.split(' ') # delimiter is ‘space’ character or ‘ ‘
print(string_list) #output: ['This', 'is', 'a', 'string.']
print(' '.join(string_list)) # output: This is a string.

----

**What does *args and **kwargs mean?**

__*args__

is a special syntax used in the function definition to pass variable-length arguments.

'*' means variable length and 'args' is the name used by convention. You can use any other.

```python
def multiply(a, b, *argv):
   mul = a * b
   for num in argv:
       mul *= num
   return mul
print(multiply(1, 2, 3, 4, 5)) #output: 120
```

__**kwargs__

is a special syntax used in the function definition to pass variable-length keyworded arguments.
Here, also, “kwargs” is used just by convention. You can use any other name.
Keyworded argument means a variable that has a name when passed to a function.
It is actually a dictionary of the variable names and its value.

```python
def tellArguments(**kwargs):
   for key, value in kwargs.items():
       print(key + ": " + value)
tellArguments(arg1 = "argument 1", arg2 = "argument 2", arg3 = "argument 3")
# output:
# arg1: argument 1
# arg2: argument 2
# arg3: argument 3
```

----

**What are negative indexes and why are they used?**

Negative indexes are the indexes from the end of the list or tuple or string.

arr[-1] means the last element of array arr[]

```python
arr = [1, 2, 3, 4, 5, 6]
# get the last element
print(arr[-1]) # output 6
#get the second last element
print(arr[-2]) # output 5
```

----

**How do you create a class in Python?**

To create a class in python, we use the keyword 'class' as shown in the example below:

```python
class InterviewbitEmployee:

   def __init__(self, emp_name):
       self.emp_name = emp_name

# To instantiate or create an object from the class created above, we do the following:
emp_1=InterviewbitEmployee("Mr. Employee")

# To access the name attribute, we just call the attribute using the dot operator as shown below:
print(emp_1.emp_name) # output: Mr. Employee
```

To create methods inside the class, we include the methods under the scope of the class as shown below:

```python
class InterviewbitEmployee:
   def __init__(self, emp_name):
       self.emp_name = emp_name
       
   def introduce(self): # method under the scope of the class: self is needed
       print(f"Hello I am {self.emp_name}")
```

The self parameter in the init and introduce functions represent the reference to the current class
instance which is used for accessing attributes and methods of that class. The self parameter has to
be the first parameter of any method defined inside the class. The method of the class
InterviewbitEmployee can be accessed as shown below:

```python
emp_1.introduce()
```

The overall program would look like this:

```python
class InterviewbitEmployee:

   def __init__(self, emp_name):
       self.emp_name = emp_name
       
   def introduce(self):
       print("Hello I am " + self.emp_name)

# create an object of InterviewbitEmployee class
# <!-- emp_1 = InterviewbitEmployee("Mr Employee")
print(emp_1.emp_name) # print employee name
# emp_1.introduce() # introduce the employee
```

----

**How does inheritance work in python? Explain it with an example?**

Inheritance gives the power to a class to access all attributes and methods of another class. It aids in code
reusability and helps the developer to maintain applications without redundant code. The class inheriting from
another class is a child class or also called a derived class. The class from which a child class derives the
members are called parent class or superclass.

Python supports different kinds of inheritance, they are:

__Single Inheritance:__

Child class derives members of one parent class.

```python
# Parent class
class ParentClass:
    
    def par_func(self):
         print("I am parent class function")

# Child class
class ChildClass(ParentClass):
    
    def child_func(self):
         print("I am child class function")

# Driver code
obj1 = ChildClass()
print(obj1.par_func())
print(obj1.child_func())
```

__Multi-level Inheritance:__

The members of the parent class, A, are inherited by child class which is then inherited by another child class, B. The features
of the base class and the derived class are further inherited into the new derived class, C. Here, A is the grandfather class of class C.

```python
# Parent class
class A:
   def __init__(self, a_name):
       self.a_name = a_name
   
# Intermediate class
class B(A):
   def __init__(self, b_name, a_name):
       self.b_name = b_name
       # invoke constructor of class A
       A.__init__(self, a_name)

# Child class
class C(B):
   def __init__(self,c_name, b_name, a_name):
       self.c_name = c_name
       # invoke constructor of class B
       B.__init__(self, b_name, a_name)
       
   def display_names(self):
       print("A name : ", self.a_name)
       print("B name : ", self.b_name)
       print("C name : ", self.c_name)

#  Driver code
obj1 = C('child', 'intermediate', 'parent')
print(obj1.a_name)
obj1.display_names()
```

__Multiple Inheritance:__

This is achieved when one child class derives members from more than one parent class. All features of parent classes are inherited in the child class.

```python
# Parent class1
class Parent1:
   def parent1_func(self):
       print("Hi I am first Parent")

# Parent class2
class Parent2:
   def parent2_func(self):
       print("Hi I am second Parent")

# Child class
class Child(Parent1, Parent2):
   def child_func(self):
       self.parent1_func()
       self.parent2_func()

# Driver's code
obj1 = Child()
obj1.child_func()
```

__Hierarchical Inheritance:__

When a parent class is derived by more than one child class, it is called hierarchical inheritance.

```python
# Base class
class A:
     def a_func(self):
         print("I am from the parent class.")

# 1st Derived class
class B(A):
     def b_func(self):
         print("I am from the first child.")

# 2nd Derived class
class C(A):
     def c_func(self):
         print("I am from the second child.")
 
# Driver's code
obj1 = B()
obj2 = C()
obj1.a_func()
obj1.b_func()    #child 1 method
obj2.a_func()
obj2.c_func()    #child 2 method
```

----

**How do you access parent members in the child class?**

Following are the ways using which you can access parent class members within a child class:



```python
# ----
# By using Parent class name: You can use the name of the parent class to access the attributes as shown in the example below:
class Parent(object):  
   # Constructor
   def __init__(self, name):
       self.name = name    
 
class Child(Parent): 
   # Constructor
   def __init__(self, name, age):
       Parent.name = name
       self.age = age
 
   def display(self):
       print(Parent.name, self.age)
 
# Driver Code
obj = Child("Interviewbit", 6)
obj.display()
# ----

# ----
# By using super(): The parent class members can be accessed in child class using the super keyword.
class Parent(object):
   # Constructor
   def __init__(self, name):
       self.name = name    
 
class Child(Parent):
   # Constructor
   def __init__(self, name, age):         
       ''' 
       In Python 3.x, we can also use super().__init__(name)
       ''' 
       super(Child, self).__init__(name)
       self.age = age
 
   def display(self):
      # Note that Parent.name cant be used 
      # here since super() is used in the constructor
      print(self.name, self.age)
  
# Driver Code
obj = Child("Interviewbit", 6)
obj.display()
# ----
```

----

**Are access specifiers used in python?**

Python does not make use of access specifiers specifically like private, public, protected, etc. However,
it does not derive this from any variables. It has the concept of imitating the behaviour of variables by
making use of a single (protected = attr./method can only be used in class where it si defined) or
double underscore (private = can be viewed an accessed within the class) as prefixed to the variable names. By default, the variables without prefixed
underscores are public.

```python
# Example:
# to demonstrate access specifiers
class InterviewbitEmployee:
   
    # protected members
    _emp_name = None
    _age = None
    
    # private members
    __branch = None
    
    # constructor
    def __init__(self, emp_name, age, branch): 
        self._emp_name = emp_name
        self._age = age
        self.__branch = branch
    
    # public member
    def display():
        print(self._emp_name +" "+self._age+" "+self.__branch)
```

----

**Is it possible to call parent class without its instance creation?**

Yes, it is possible if the base class is instantiated by other child classes or if the base class is a
static method.

----

**How is an empty class created in python?**

An empty class does not have any members defined in it. It is created by using the pass keyword (the
pass command does nothing in python). We can create objects for this class outside the class.
For example:

```python
class EmptyClassDemo:
  pass
  
obj=EmptyClassDemo()
print(obj.name="Interviewbit")
print("Name created = ",obj.name)
# Output: Name created = Interviewbit
```

----

**Differentiate between new and override modifiers?**

The new modifier is used to instruct the compiler to use the new implementation and not the base
class function. The Override modifier is useful for overriding a base class function inside the
child class.

----

**Why is finalize used?**

Finalize method is used for freeing up the unmanaged resources and clean up before the garbage collection method is invoked.
This helps in performing memory management tasks.

----

**What is init method in python?**

The init method works similarly to the constructors in Java.

The method is run as soon as an object is instantiated. It is useful for initializing any attributes
or default behaviour of the object at the time of instantiation.

For example:

```python
class InterviewbitEmployee:

   # init method / constructor
   def __init__(self, emp_name):
       self.emp_name = emp_name

   # introduce method
   def introduce(self):
       print('Hello, I am ', self.emp_name)

emp = InterviewbitEmployee('Mr Employee') # __init__ method is called here and initializes the object name with "Mr Employee"
emp.introduce()
```

----

**How will you check if a class is a child of another class?**

This is done by using a method called issubclass() provided by python. The method tells us if any
class is a child of another class by returning true or false accordingly.

```python
# For example:
class Parent(object):
   pass   
 
class Child(Parent):
   pass   
 
# Driver Code
print(issubclass(Child, Parent))    #True
print(issubclass(Parent, Child))    #False
We can check if an object is an instance of a class by making use of isinstance() method:
obj1 = Child()
obj2 = Parent()
print(isinstance(obj2, Child))    #False 
print(isinstance(obj2, Parent))   #True 
Python Pandas Interview Questions
```

----

**What do you know about pandas?**

Pandas is an open-source, python-based library used in data manipulation applications requiring high performance.

The name is derived from *Panel Data* having multidimensional data.

This was developed in 2008 by Wes McKinney and was developed for data analysis.

Pandas are useful in performing 5 major steps of data analysis:
- Load the data
- Clean/manipulate it
- Prepare it
- Model it
- Analyze it

----

**Define pandas dataframe?**

A dataframe is a 2D mutable and tabular structure for representing data labelled with axes - rows
and columns.

The syntax for creating dataframe:

```python
import pandas as pd
dataframe = pd.DataFrame( data, index, columns, dtype)
# data - Represents various forms like series, map, ndarray, lists, dict etc.
# index - Optional argument that represents an index to row labels.
# columns - Optional argument for column labels.
# Dtype - the data type of each column. Again optional.
```

----

**How will you combine different pandas dataframes?**

The dataframes can be combines using the below approaches:

*append() method:*

This is used to stack the dataframes horizontally. Syntax:

```python
df1.append(df2)
```

*concat() method:*

This is used to stack dataframes vertically. This is best used when the dataframes have the same columns and similar fields. Syntax:

```python
pd.concat([df1, df2])
```

*join() method:*

This is used for extracting data from various dataframes having one or more common columns.

```python
f1c.join(df2)
```

----

**Can you create a series from the dictionary object in pandas?**

One dimensional array capable of storing different data types is called a series.
We can create pandas series from a dictionary object as shown below:

```python
import pandas as pd    
dict_info = {'key1' : 2.0, 'key2' : 3.1, 'key3' : 2.2}  
series_obj = pd.Series(dict_info)    
print(series_obj)    
# Output:
# x     2.0
# y     3.1
# z     2.2
# dtype: float64
```

If an index is not specified in the input method, then the keys of the dictionaries are sorted in ascending
order for constructing the index. In case the index is passed, then values of the index label will be
extracted from the dictionary.

----

**How will you identify and deal with missing values in a dataframe?**

We can identify if a dataframe has missing values by using the isnull() and isna() methods.

```python
missing_data_count=df.isnull().sum()
```

We can handle missing values by either replacing the values in the column with 0 as follows ...

```python
df['column_name'].fillna(0)
```
... or by replacing it with the mean value of the column

```python
df['column_name'] = df['column_name'].fillna((df['column_name'].mean()))
```

----

**What do you understand by reindexing in pandas?**

Reindexing is the process of conforming a dataframe to a new index with optional filling logic. If the values
are missing in the previous index, then NaN/NA is placed in the location.

A new object is returned unless a new index is produced that is equivalent to the current one. The copy value
is set to False. This is also used for changing the index of rows and columns in the dataframe.

----

**How to add new column to pandas dataframe?**

A new column can be added to a pandas dataframe as follows:

```python
import pandas as pd

data_info = {'first' : pd.Series([1, 2, 3], index=['a', 'b', 'c']),    
       'second' : pd.Series([1, 2, 3, 4], index=['a', 'b', 'c', 'd'])}    
  
df = pd.DataFrame(data_info) 

# to add new column third
df['third']=pd.Series([10,20,30],index=['a','b','c'])    
print(df)

# to add new column fourth
df['fourth']=df['first']+info['third']    
print(df)
```

----

**How will you delete indices, rows and columns from a dataframe?**

To delete an Index:

```python
del df.index.name
```

... for removing the index by name.

Alternatively, the

```python
df.index.name
```

can be assigned to None.

For example, if you have the below dataframe:

   Names            Column 1             
   John               1
   Jack               2
   Judy               3
   Jim                4

To drop the index name "Names":

```python
df.index.name = None
# or run the below:
del df.index.name
print(df)
```

Names        Column 1
John          1
Jack          2
Judy          3
Jim           4

To delete row/column from dataframe:

*drop() method* is used to delete row/column from dataframe.
The axis argument is passed to the drop method where if the value is 0, it indicates to drop/delete a
row and if 1 it has to drop the column.

Additionally, we can try to delete the rows/columns in place by setting the value of inplace to True. This makes
sure that the job is done without the need for reassignment.

The duplicate values from the row/column can be deleted by using the drop_duplicates() method.

----

**Can you get items of series A that are not available in another series B?**

This can be achieved by using the *~ (not/negation symbol)* and *isin()* method as shown below.

```python
import pandas as pd
df1 = pd.Series([2, 4, 8, 10, 12])
df2 = pd.Series([8, 12, 10, 15, 16])
df1=df1[~df1.isin(df2)]
print(df1)
"""
Output:
0    2
1    4
dtype: int64
"""
```

**How will you get the items that are not common to both the given series A and B?**

We can achieve this by first performing the union of both series, then taking the intersection of both series.
Then we follow the approach of getting items of union that are not there in the list of the intersection.

The following code demonstrates this:

```python
import pandas as pd
import numpy as np
df1 = pd.Series([2, 4, 5, 8, 10])
df2 = pd.Series([8, 10, 13, 15, 17])
p_union = pd.Series(np.union1d(df1, df2))  # union of series
p_intersect = pd.Series(np.intersect1d(df1, df2))  # intersection of series
unique_elements = p_union[~p_union.isin(p_intersect)]
print(unique_elements)
"""
Output:
0     2
1     4
2     5
5    13
6    15
7    17
dtype: int64
"""
```

**While importing data from different sources, can the pandas library recognize dates?**

Yes, they can, but with some bit of help. We need to add the parse_dates argument while we are reading data
from the sources. Consider an example where we read data from a CSV file, we may encounter different date-time
formats that are not readable by the pandas library. In this case, pandas provide flexibility to build our
custom date parser with the help of lambda functions as shown below:

```python
import pandas as pd
from datetime import datetime
dateparser = lambda date_val: datetime.strptime(date_val, '%Y-%m-%d %H:%M:%S')
df = pd.read_csv("some_file.csv", parse_dates=['datetime_column'], date_parser=dateparser)
```

----

**What do you understand by NumPy?**

NumPy is one of the most popular, easy-to-use, versatile, open-source, python-based, general-purpose package
that is used for processing arrays.

NumPy is short for NUMerical PYthon.

This is very famous for its highly optimized tools that result in high performance and powerful N-Dimensional array processing feature that is
designed explicitly to work on complex arrays.

Due to its popularity and powerful performance and its flexibility to perform various operations like trigonometric operations,
algebraic and statistical computations, it is most commonly used in performing scientific computations and various broadcasting functions.

The NumPy API is used extensively in Pandas, SciPy, Matplotlib, scikit-learn, scikit-image and most other data science and scientific Python packages.

----

**How are NumPy arrays advantageous over python lists?**

The list data structure of python is very highly efficient and is capable of performing various functions.
But, they have severe limitations when it comes to the computation of vectorized operations which deals
with element-wise multiplication and addition.

The python lists also require the information regarding the type of every element which results in overhead as
type dispatching code gets executes every time any operation is performed on any element. This is where the
NumPy arrays come into the picture as all the limitations of python lists are handled in NumPy arrays.

Additionally, as the size of the NumPy arrays increases, NumPy becomes around 30x times faster than the Python List. This is
because the Numpy arrays are densely packed in the memory due to their homogenous nature. This ensures the memory free up is also faster.

**What are the steps to create 1D, 2D and 3D arrays?**

```python
# 1D array creation:
import numpy as np
one_dimensional_list = [1,2,4]
one_dimensional_arr = np.array(one_dimensional_list)
print("1D array is : ",one_dimensional_arr) 
# 2D array creation:
two_dimensional_list=[[1,2,3],[4,5,6]]
two_dimensional_arr = np.array(two_dimensional_list)
print("2D array is : ",two_dimensional_arr)
# 3D array creation:
three_dimensional_list=[[[1,2,3],[4,5,6],[7,8,9]]]
three_dimensional_arr = np.array(three_dimensional_list)
print("3D array is : ",three_dimensional_arr) 
# ND array creation: This can be achieved by giving the ndmin attribute. The below example
# demonstrates the creation of a 6D array:
ndArray = np.array([1, 2, 3, 4], ndmin=6)
print(ndArray)
print('Dimensions of array:', ndArray.ndim)
```

----

**You are given a numpy array and a new column as inputs. How will you delete the second column and replace the column with a new column value?**

```python
# Example:

# Given array:
example_array = [[35 53 63]
                [72 12 22]
                [43 84 56]]
New Column values:
[  
   20,
   30,
   40
]

# Solution:
import numpy as np
#inputs
inputArray = np.array([[35,53,63],[72,12,22],[43,84,56]])
new_col = np.array([[20,30,40]])
# delete 2nd column
arr = np.delete(inputArray , 1, axis = 1)
#insert new_col to array
arr = np.insert(arr , 1, new_col, axis = 1)
print(arr)
```

----

**How will you efficiently load data from a text file?**

We can use the method numpy.loadtxt() which can automatically read the file’s header and footer lines and
the comments if any.

This method is highly efficient and even if this method feels less efficient, then the data should be
represented in a more efficient format such as CSV etc. Various alternatives can be considered depending
on the version of NumPy used.

Following are the file formats that are supported:

*Text files:* These files are generally very slow, huge but portable and are human-readable.

*Raw binary*: This file does not have any metadata and is not portable. But they are fast.

*Pickle:* These are borderline slow and portable but depends on the NumPy versions.

*HDF5:* This is known as the High-Powered Kitchen Sink format which supports both PyTables and h5py format.

*.npy:* This is NumPy's native binary data format which is extremely simple, efficient and portable.

**How will you read CSV data into an array in NumPy?**

This can be achieved by using the genfromtxt() method by setting the delimiter as a comma.

```python
from numpy import genfromtxt
csv_data = genfromtxt('sample_file.csv', delimiter=',')
```

----

**How will you sort the array based on the Nth column?**

For example, consider an array arr.

```python
arr = np.array([[8, 3, 2],
                [3, 6, 5],
                [6, 1, 4]])

# Let us try to sort the rows by the 2nd column so that we get:
# [[6, 1, 4],
# [8, 3, 2],
# [3, 6, 5]]

# 1. We can do this by using the sort() method in numpy as:
import numpy as np
arr = np.array([[8, 3, 2],
          [3, 6, 5],
          [6, 1, 4]])

#sort the array using np.sort
arr = np.sort(arr.view('i8,i8,i8'),
       order=['f1'],
       axis=0).view(np.int)

# 2. We can also perform sorting and that too inplace sorting by doing:
arr.view('i8,i8,i8').sort(order=['f1'], axis=0)
```

----

**How will you find the nearest value in a given numpy array?**

We can use the argmin() method of numpy as shown below:

```python
import numpy as np
def find_nearest_value(arr, value):
   arr = np.asarray(arr)
   idx = (np.abs(arr - value)).argmin()
   return arr[idx]
# driver code
arr = np.array([ 0.21169,  0.61391, 0.6341, 0.0131, 0.16541,  0.5645,  0.5742])
value = 0.52
print(find_nearest_value(arr, value)) # Prints 0.5645
```

----

**How will you reverse the numpy array using one line of code?**

This can be done as shown in the following:

```python
reversed_array = arr[::-1]
```

where arr = original given array, reverse_array is the resultant after reversing all elements in the input.

----

**How will you find the shape of any given NumPy array?**

We can use the shape attribute of the numpy array to find the shape. It returns the shape of the array in
terms of row count and column count of the array.

```python
import numpy as np
arr_two_dim = np.array([("x1","x2", "x3","x4"),
             ("x5","x6", "x7","x8" )])
arr_one_dim = np.array([3,2,4,5,6])
# find and print shape
print("2-D Array Shape: ", arr_two_dim.shape)
print("1-D Array Shape: ", arr_one_dim.shape)
"""
Output:
2-D Array Shape:  (2, 4)
1-D Array Shape:  (5,)
"""
```

----

**Differentiate between a package and a module in python?**

The module is a single python file. A module can import other modules (other python files) as objects.
Whereas, a package is the folder/directory where different sub-packages and the modules reside.

A python module is created by saving a file with the extension of .py. This file will have classes and functions that are reusable in the code as well as across modules.

A python package is created by following the below steps:

1. Create a directory and give a valid name that represents its operation.
1. Place modules of one kind in this directory.
1. Create __init__.py file in this directory. This lets python know the directory we created is a package. The contents of this package can be imported across different modules in other packages to reuse the functionality.

----

**What are some of the most commonly used built-in modules in Python?**

Python modules are the files having python code which can be functions, variables or classes.
These go by *.py* extension. The most commonly available built-in modules are:

```python
import os
import math
import sys
import random
import re
import datetime
import JSON
```

**What are lambda functions?**

Lambda functions are generally inline, anonymous functions represented by a single expression. They are used
for creating function objects during runtime. They can accept any number of parameters. They are usually used
where functions are required only for a short period. They can be used as:

```python
mul_func = lambda x,y : x*y
print(mul_func(6, 4))
# Output: 24
```

----

**How can you generate random numbers?**

Python provides a module called random using which we can generate random numbers.

We have to import a random module and call the random() method as shown below:
The random() method generates float values lying between 0 and 1 randomly.

```python
import random
print(random.random())
```

To generate customised random numbers between specified ranges, we can use the randrange() method
Syntax:

```python
import random
# randrange(beginning, end, step)
print(random.randrange(5,100,2))
```

----

**Can you easily check if all characters in the given string is alphanumeric?**

This can be easily done by making use of the isalnum() method that returns true in case the string has only alphanumeric characters.

```python
xample_1: str = "abdc1321"
xample_2: str = "xyz@123$"
print(xample_1.isalnum()) # Output: True
print(xample_2.isalnum()) # Output: False
```

Another way is to use match() method from the re (regex) module as shown:

```python
import re
print(bool(re.match('[A-Za-z0-9]+$','abdc1321'))) # Output: True
print(bool(re.match('[A-Za-z0-9]+$','xyz@123$'))) # Output: False
```

----

**What are the differences between pickling and unpickling?**

*Pickling* is the conversion of python objects to binary form. Whereas, *unpickling* is the conversion of binary
form data to python objects.

*The pickled objects* are used for storing in disks or external memory locations. 

*Unpickled objects* are used for getting the data back as python objects upon which processing can be done in python.

Python provides a pickle module for achieving this. Pickling uses the pickle.dump() method to dump python objects into disks. Unpickling uses the pickle.load() method to get back the data as python objects.

----

**Define GIL?**

GIL stands for *Global Interpreter Lock*. This is a mutex used for limiting access to python objects and aids
in effective thread synchronization by avoiding deadlocks. GIL helps in achieving multitasking (and not
parallel computing).

There are three threads:
- First Thread acquires the GIL first and starts the I/O execution.
- When the I/O operations are done, thread 1 releases the acquired GIL which is then taken up by the second thread.
- The process repeats and the GIL are used by different threads alternatively until the threads have completed
their execution. The threads not having the GIL lock goes into the waiting state and resumes execution only when it
acquires the lock.

----

**Define PYTHONPATH?**

It is an environment variable used for incorporating additional directories during the import of a module or a
package. PYTHONPATH is used for checking if the imported packages or modules are available in the existing
directories. Not just that, the interpreter uses this environment variable to identify which module needs to be
loaded.

----

**Define PIP?**

PIP stands for Python Installer Package. As the name indicates, it is used for installing different python modules.
It is a command-line tool providing a seamless interface for installing different python modules. It searches over
the internet for the package and installs them into the working directory without the need for any interaction with
the user. The syntax for this is:

```python
pip install <package_name>
```

----

**Are there any tools for identifying bugs and performing static analysis in python?**

Yes, there are tools like PyChecker and Pylint which are used as static analysis and linting tools respectively.
PyChecker helps find bugs in python source code files and raises alerts for code issues and their complexity.
Pylint checks for the module's coding standards and supports different plugins to enable custom features to meet
this requirement.

----

**Differentiate between deep and shallow copies?**

Shallow copy does the task of creating new objects storing references of original elements. This does not undergo recursion
to create copies of nested objects. It just copies the reference details of nested objects.

Deep copy creates an independent and new copy of an object and even copies all the nested objects of the original element recursively.

----

**What is a main function in python? How do you invoke it?**

In the world of programming languages, the main is considered as an entry point of execution for a program.
But in python, it is known that the interpreter serially interprets the file line-by-line. This means that
python does not provide main() function explicitly. But this doesn't mean that we cannot simulate the execution
of main. This can be done by defining user-defined main() function and by using the __name__ property of
python file. This __name__ variable is a special built-in variable that points to the name of the current
module. This can be done as shown below:

```python
def main():
   print("Hello world!")

if __name__=="__main__": # oints to the name of the current module
   main()
```

----

**Write python function which takes a variable number of arguments?**

A function that takes variable arguments is called a function prototype. Syntax:

```python
def function_name(*arg_list)
    # For example:
    def func(*var):
        for i in var:
            print(i)
func(1)
func(20,1,6)
# The * in the function argument represents variable arguments in the function.
```

----

**WAP (Write a program) which takes a sequence of numbers and check if all numbers are unique?**

You can do this by converting the list to set by using set() method and comparing the length of this set with
the length of the original list. If found equal, return True.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def check_distinct(data_list):
    if len(data_list) == len(set(data_list)):
        return True
    else:
        return False

def main():
    print(check_distinct([1,6,5,8])) # Prints True
    print(check_distinct([2,2,5,5,7,8])) # Prints False

if __name__ == '__main__':
    main()
```

----

**Write a program for counting the number of every character of a given text file?**

The idea is to use collections and pprint module as shown below:

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

import collections
import pprint

def manipulate_data(data_list):
    """Manipulate data in Text.
    """
    with open(data_list, 'r', encoding='utf-8') as data:
        count_data = collections.Counter(data.read().upper())
        count_value = pprint.pformat(count_data)
        print(count_value)

def main():
    """Driver code."""
    manipulate_data("sample_file.txt")

if __name__ == '__main__':
    main()
```

----

**Write a program to check and return the pairs of a given array A whose sum value is equal to a target value N?**

This can be done easily by using the phenomenon of hashing. We can use a hash map to check for the current value of the array, x. If the map has the value of (N-x), then there is our pair.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def print_pairs(arr, N):
    # hash set
    hash_set = set()

    for i in range(0, len(arr)):
        val = N-arr[i]
        if (val in hash_set): # check if N-x is there in set, print the pair
            print(f"Pairs {str(arr[i])}, {str(val)}")
        hash_set.add(arr[i])

def main():
    arr = [1, 2, 40, 3, 9, 4]
    N = 3
    print_pairs(arr, N)

if __name__ == '__main__':
    main()
```

----

**Write a Program to add two integers > 0 without using the plus operator?**

We can use bitwise operators to achieve this.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def add_nums(num1, num2):
    """Add two integers > 0 without plus operator
    """
    while num2 != 0:
        data = num1 & num2
        print(f"data: {data}")
        num1 = num1 ^ num2
        print(f"num1: {num1}")
        num2 = data << 1
    return num1

def main():
    print(add_nums(2, 10))

if __name__ == '__main__':
    main()
```

----

**Write a Program to solve the given equation assuming that a,b,c,m,n,o are constants:**

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def main():
    """
    # ax + by = c
    # mx + ny = o
    # By solving the equation, we get:
    """
    a, b, c, m, n, o = 5, 9, 4, 7, 9, 4
    temp = a*n - b*m
    if n != 0:
        x = (c*n - b*o) / temp
        y = (a*o - m*c) / temp
        print(str(x), str(y))

if __name__ == '__main__':
    main()
```

----

**Write a Program to match a string that has the letter 'a' followed by 4 to 8 'b’s?**

We can use the re module of python to perform regex pattern comparison here.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

import re

def match_text(txt_data):
    pattern = 'ab{4,8}'
    if re.search(pattern,  txt_data): # search for pattern in txt_data
        return 'Match found :-)'
    else:
        return 'Match not found :-('

def main():
    print(match_text("abc")) # prints Match not found
    print(match_text("aabbbbbc"))  # prints Match found

if __name__ == '__main__':
    main()
```

----

**Write a Program to convert date from yyyy-mm-dd format to dd-mm-yyyy format?**

We can again use the re module to convert the date string as shown below:

```python

import re
from datetime import datetime

def transform_date_format(date):
    return re.sub(r'(\d{4})-(\d{1,2})-(\d{1,2})', '\\3-\\2-\\1', date)
date_input = "2021-08-01"
print(transform_date_format(date_input))

# You can also use the datetime module as shown below:
new_date = datetime.strptime("2021-08-01", "%Y-%m-%d").strftime("%d:%m:%Y")
# new_date = datetime.strptime("2021-08-01", "%Y-%m-%d %d:%m:%Y")
print(new_data)
```

----

**Write a Program to combine two different dictionaries. While combining, if you find the same keys, you can add the values of these same keys. Output the new dictionary**

We can use the Counter method from the collections module

```python
from collections import Counter

d1 = {'key1': 50, 'key2': 100, 'key3':200}
d2 = {'key1': 200, 'key2': 100, 'key4':300}

new_dict = Counter(d1) + Counter(d2)
print(new_dict)
```

----

**How will you access the dataset of a publicly shared spreadsheet in CSV format stored in Google Drive?**

We can use the StringIO module from the io module to read from the Google Drive link and then we can use the
pandas library using the obtained data source.

```python
from io import StringIO
import pandas
csv_link = "https://docs.google.com/spreadsheets/d/..."
data_source = StringIO.StringIO(requests.get(csv_link).content))
dataframe = pd.read_csv(data_source)
print(dataframe.head())
```

----

**Suppose list1 = [3,4,5,2,1,0], what is list1 after list1.pop(1)?**

```python
list_1 = [3,4,5,2,1]
list_2 = [3,4,5,2,0]
list_3 = [3,5,2,1,0] (true, second element was taken out of the list)
list_4 = [3,4,5,2]
```

----

**What is the output of the following statement "Hello World"[::-1]?**

- "Hello World"
- "World Hello"
- "dlroW olleH" (correct)
- "olleH dlroW"

----

**What is the difference between lists and tuples?**

- List is a sequence data type, while tuple is not. (false)
- Tuples are mutable but lists are immutable. (false)
- Tuple is a sequence data type, while lists is not. (false)
- Lists are mutable but tuples are immutable. (true)

----

**Let func = lambda a, b : (a ** b), what is the output of func(float(10),20)?**

- 100000000000000000000
- 1e+20 (true)
- 100000000000000000000.0
- 1.0e+20

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def main():
    func_1 = lambda a, b : (a ** b)
    print(func_1(float(10),20))

if __name__ == '__main__':
    main()
```
----

**Which statement is false for __init__?**

- __init__ is called manually on object creation. (false)
- __init__ is a constructor method in Python. (true)
- All classes have a __init__ method associated with them. (true, it is built-in)
- __init__ allocates memory for objects. (false)

----

**Which of the following is the function responsible for pickling?**

- pickle.save() (false)
- pickle.store() (false)
- pickle.pickle() (false)
- pickle.dump() (true)

----

**Which of the following is a protected attribute?**

- __sara__ (false, built-in function)
- _ansh (true, protected)
- __sara (false, private)
- ansh__ (false, means nothing)

----

**Which of the following is untrue for Python namespaces?**

- Python namespaces are implemented as a dictionary in Python.
- Python namespaces have keys as addresses of the objects.
- Lifecycle of a namespace depends upon the scope of the objects they are mapped to.
- Namespaces ensure that object names in a program are unique.

----

**Let list1 = ['s','r','a','s'] and list2 = ['a','a','n','h'], what is the output of ["".join([i, j]) for i, j in zip(list1, list2)]?**

- ['s', 'a', 'r', 'a', 'a', 'n', 's', 'h']
- ['s', 'r', 'a', 's', 'a', 'a', 'n', 'h']
- ['sa', 'ra', 'an', 'sh'] (true)
- ['sa', 'sa', 'sn', 'sh', 'ra', 'ra', 'rn', 'rh', 'aa', 'aa', 'an', 'ah', 'sa', 'sa', 'sn', 'sh']

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def main():
    list1 = ['s','r','a','s']
    list2 = ['a','a','n','h']
    print(["".join([i, j]) for i, j in zip(list1, list2)])

if __name__ == '__main__':
    main()
```

----

**time.time() in Python returns?**

- Current time.
- Current time in milliseconds.
- Current time in milliseconds since midnight, January 1, 1970.
- Current time in milliseconds since midnight, January 1, 1970 GMT (the Unix time).

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

import time

def main():
    print(time.time())

if __name__ == '__main__':
    main()
```

----

**What is the output of the following program?**

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

class A(object):

   def __init__(self, a):
       self.num = a
       
   def mul_two(self):
       self.num *= 2
 
class B(A):

   def __init__(self, a):
       A.__init__(self, a)
       
   def mul_three(self):
       self.num *= 3

def main():
    obj = B(4)
    print(obj.num)
    
    obj.mul_two()
    print(obj.num)
    
    obj.mul_three()
    print(obj.num)

if __name__ == '__main__':
    main()
```

- 4 8 24 (true)
- 4 4 64
- 4 8 64
- None of the above

----

**What is the output of the below program?**

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

class Human(object):

   def __init__(self, name):
       self.human_name = name
         
   def get_human_name(self):
       return self.human_name
     
   def is_employee(self):
       return False
 
class IBEmployee(Human):

   def __init__(self, name, emp_id): 
       super(IBEmployee, self).__init__(name)
       self.emp_id = emp_id
         
   def is_employee(self):
       return True
         
   def get_emp_id(self):
       return self.emp_id

def main():
    employee = IBEmployee("Mr Employee", "IB007") 
    print(employee.get_human_name(), employee.is_employee(), employee.get_emp_id())

if __name__ == '__main__':
    main()
```

- (None, True, ‘IB007’) (true)
- (‘Mr Employee’, True, ‘IB007’)
- (“”, False, ‘IB007’)
- Runtime error

----

**Which among the below options will correct the below error obtained while reading “sample_file.csv” in pandas?**

__Traceback (most recent call last): File "input", line 10, in module UnicodeEncodeError: 'ascii' codec can't encode character.__
  
- pd.read_csv("sample_file.csv", encoding='utf-8')
- pd.read_csv("sample_file.csv", compression='gzip')
- pd.read_csv("sample_file.csv", dialect='comma')

----

**Which among the following options helps us to check whether a pandas dataframe is empty?**

- df.emptyframe
- df.blank
- df.isempty
- df.empty (true)

**How will you find the location of numbers which are multiples of 5 in a series?**

- import pandas as pd
- import numpy as np
- series_data = pd.Series(np.random.randint(1, 20, 7))

```python
# insert code here
np.search(series_data % 5)
np.find(series_data % 5 ==0)
np.argwhere(series_data % 5==0)
np.locate(series_data % 5)
```

----

**What is the output of the below code?**

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

class Person:

   def __init__(self, first_name, last_name):
       self.first_name = first_name
       self.last_name = last_name

def main():
    first_name = "XYZ"
    person = Person(first_name, "ABC")
    first_name = "LMN"
    person.last_name = "PQR"
    print(person.first_name, person.last_name)

if __name__ == '__main__':
    main()
```

- XYZ ABC
- XYZ PQR (true)
- LMN ABC
- LMN PQR

----

**Which among the below options picks out negative numbers from the given list?**

- [num for num < 0 in list]
- [num<0 in list]
- [num for num in list if num < 0] (true)
- [num in list for num<0]

----

**What is the output of the below code?**

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def main():
    
    main_dict={}

    def insert_item(item):
        if item in main_dict:
            main_dict[item] += 1
        else:
            main_dict[item] = 1

    insert_item('Key1')
    insert_item('Key2')
    insert_item('Key2')
    insert_item('Key3')
    insert_item('Key1')
    print(len(main_dict))

if __name__ == '__main__':
    main()
```

- 5
- Runtime error
- Duplicate Key Exception
- 3 (true)

----

**What is the output of the below code?**

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

class X:

    def __init__(self):
        self.__num1 = 5
        self.num2 = 2

    def display_values(self):
        print(self.__num1, self.num2)

class Y(X):

    def __init__(self):
        super().__init__()
        self.__num1 = 1
        self.num2 = 6 

def main():
    obj = Y()
    print(obj.display_values())


if __name__ == '__main__':
    main()
```

- 5 6 (true)
- 1 2
- 5 2
- 1 6

# https://www.interviewbit.com/python-interview-questions/

# https://www.edureka.co/blog/interview-questions/python-interview-questions/

**What is the difference between list and tuples in Python?**

LIST vs TUPLES

Lists are mutable i.e. they can be edited.

Tuples are immutable (tuples are lists which can’t be edited).

Lists are slower than tuples.

Tuples are faster than list.

```python
# Syntax:
list_1 = [10, ‘Chelsea’, 20]

# Syntax:
tup_1 = (10, ‘Chelsea’ , 20)
```

----

**What are the key features of Python?**

Python is an *interpreted language*. That means that, unlike languages like C and its variants, Python does
not need to be compiled before it is run. Other interpreted languages include PHP and Ruby.

Python is *dynamically typed*, this means that you don’t need to state the types of variables when you declare them or anything like that. You can do things like x=111 and then x="I'm a string" without error

Python is well suited to *object orientated programming* in that it allows the definition of classes along
with composition and inheritance. Python does not have access specifiers (like C++’s public, private).

In Python, *functions* are *first-class objects*. This means that they can be assigned to variables, returned from other functions and passed into functions.

*Classes* are also *first class objects*.

Writing Python code is quick but running it is often slower than compiled languages. Fortunately，Python allows the inclusion of C-based extensions so bottlenecks can be optimized away and often are. The numpy package is a good example of this, it’s really quite quick because a lot of the number-crunching it does isn’t actually done by Python
Python finds use in many spheres – web applications, automation, scientific modeling, big data applications and many more. It’s also often used as “glue” code to get other languages and components to play nice. Learn more about Big Data and its applications from the Azure Data Engineering Training Course.

----

**What type of language is python? Programming or scripting?**

Python is capable of scripting, but in general sense, it is considered as a general-purpose programming language.

----

**Python an interpreted language? Explain?**

An interpreted language is any programming language which is not in machine-level code before runtime.
Therefore, Python is an interpreted language.

----

**What is PEP 8?**

PEP stands for __Python Enhancement Proposal__. It is a set of rules that specify how to format Python code
for maximum readability.

----

**What are the benefits of using Python?**

The benefits of using python are:

_Easy to use_ – Python is a high-level programming language that is easy to use, read, write and learn.

_Interpreted language_ – Since python is interpreted language, it executes the code line by line and stops
if an error occurs in any line.

_Dynamically typed_ – the developer does not assign data types to variables at the time of coding. It automatically gets assigned during execution.

_Free and open-source_ – Python is free to use and distribute. It is open source.

_Extensive support for libraries_ – Python has vast libraries that contain almost any function needed.
It also further provides the facility to import other packages using Python Package Manager(pip).

_Portable_ – Python programs can run on any platform without requiring any change. The data structures used in
python are user friendly. It provides more functionality with less coding. Find out our Python Training in Top Cities/Countries

----

**What are Python namespaces?**

A _namespace_ in python refers to the name which is assigned to each object in python. The objects are variables
and functions. As each object is created, its name along with space(the address of the outer function in which the
object is), gets created. The namespaces are maintained in python like a dictionary where the key is the namespace
and value is the address of the object.

_There 4 types of namespace:_

- Built-in namespace : These namespaces contain all the built-in objects in python and are available whenever python is running.
- Global namespace : These are namespaces for all the objects created at the level of the main program.
- Enclosing namespaces : These namespaces are at the higher level or outer function.
- Local namespaces : These namespaces are at the local or inner function.

----

**What are Dict and List comprehensions?**

Dictionary and list comprehensions are just another concise way to define dictionaries and lists.

```python
# Example of list comprehension is : 
x = [i for i in range(5)]
# The above code creates a list as below:
# 1
# 2
# 4
# [0,1,2,3,4]
```

```python
# Example of dictionary comprehension is-
x=[i : i+2 for i in range(5)]
# The above code creates a list as below-
[0: 2, 1: 3, 2: 4, 3: 5, 4: 6]
```

----

**What are the common built-in data types in Python?**

_The common built-in data types in python are:_

*Numbers :* They include integers, floating-point numbers, and complex numbers. eg. 1, 7.9,3+4i

*List :* An ordered sequence of items is called a list. The elements of a list may belong to different data types. Eg. [5,'market',2.4]

*Tuple :* It is also an ordered sequence of elements. Unlike lists , tuples are immutable, which means they can’t be changed. Eg. (3,’tool’,1)

*String :* A sequence of characters is called a string. They are declared within single or double-quotes. Eg. “Sana”, ‘She is going to the market’, etc.

*Set :* Sets are a collection of unique items that are not in order. Eg. {7,6,8}

*Dictionary :* A dictionary stores values in key and value pairs where each value can be accessed through its key. The order of items is not important. Eg. {1:’apple’,2:’mango}

*Boolean :* There are 2 boolean values- True and False.

----

**What is the difference between .py and .pyc files?**

The .py files are the python source code files. While the .pyc files contain the bytecode of the python files. .pyc files are created when
the code is imported from some other source. The interpreter converts the source .py files to .pyc files which helps by saving time. You
can get a better understanding with the Data Engineering Course in Washington.

----

**What is slicing in python?**

Slicing is used to access parts of sequences like lists, tuples, and strings. The syntax of slicing is-[start:end:step]. The step can be omitted
as well. When we write [start:end] this returns all the elements of the sequence from the start (inclusive) till the end-1 element. If the start
or end element is negative i, it means the ith element from the end. The step indicates the jump or how many elements have to be skipped. Eg.
if there is a list- [1,2,3,4,5,6,7,8]. Then [-1:2:2] will return elements starting from the last element till the third element by printing
every second element.i.e. [8,6,4].

----

**What are Keywords in python?**

Keywords in python are reserved words that have special meaning.They are generally used to define type of variables. Keywords cannot be used
for variable or function names. There are following 33 keywords in python:

And
Or
Not
If
Elif
Else
For
While
Break
As
Def
Lambda
Pass
Return
True
False
Try
With
Assert
Class
Continue
Del
Except
Finally
From
Global
Import
In
Is
None
Nonlocal
Raise
Yield

----

**What are Literals in Python and explain about different Literals?**

A literal in python source code represents a fixed value for primitive data types.

There are 5 types of literals in python:

1. String literals : A string literal is created by assigning some text enclosed in single or double quotes to a variable. To create multiline literals, assign the multiline text enclosed in triple quotes. Eg.name=”Tanya”

2. A character literal : It is created by assigning a single character enclosed in double quotes. Eg. a=’t’

3. Numeric literals :  Include numeric values that can be either integer, floating point value, or a complex number. Eg. a=50

4. Boolean literals : These can be 2 values- either True or False.

5. Literal Collections : These are of 4 types ...
  - a. List collections-Eg. a = [1,2,3,’Amit’]
  - b. Tuple literals- Eg. a = (5,6,7,8)
  - c. Dictionary literals- Eg. dict = {1: ’apple’, 2: ’mango, 3: ’banana`’}
  - d. Set literals- Eg. {"Tanya", "Rohit", "Mohan"}

Special literal:  Python has 1 special literal None which is used to return a null variable.

----

**How to combine dataframes in pandas?**

The dataframes in python can be combined in the following ways:

- Concatenating them by stacking the 2 dataframes vertically.
- Concatenating them by stacking the 2 dataframes horizontally.
- Combining them on a common column. This is referred to as joining.

The concat() function is used to concatenate two dataframes. Its syntax is- pd.concat([dataframe1, dataframe2]).

Dataframes are joined together on a common column called a key. When we combine all the rows in dataframe it is union
and the join used is outer join. While, when we combine the common rows or intersection, the join used is the inner join.
Its syntax is:

```python
pd.concat([dataframe1, dataframe2], axis='axis', join=’type_of_join)
```

----

**Is python case sensitive?**

Yes. Python is a case sensitive language.

----

**What is type conversion in Python?**

Type conversion refers to the conversion of one data type into another.

- int() – converts any data type into integer type
- float() – converts any data type into float type
- ord() – converts characters into integer
- hex() – converts integers to hexadecimal
- oct() – converts integer to octal
- tuple() – This function is used to convert to a tuple.
- set() – This function returns the type after converting to set.
- list() – This function is used to convert any data type to a list type.
- dict() – This function is used to convert a tuple of order (key, value) into a dictionary.
- str() – Used to convert integer into a string.
- complex(real,imag) – This function converts real numbers to complex(real,imag) number.

----

**How to install Python on Windows and set path variable?**

To install Python on Windows, follow the below steps:

1. Install python from this link: [https://www.python.org/downloads/](https://www.python.org/downloads/)
1. After this, install it on your PC. Look for the location where PYTHON has been installed on your PC using the following command on your command
1. prompt: cmd python. 
1. Then go to advanced system settings and add a new variable and name it as PYTHON_NAME and paste the copied path.
1. Look for the path variable, select its value and select ‘edit’.
1. Add a semicolon towards the end of the value if it’s not present and then type %PYTHON_HOME% 

----

**Is indentation required in python?**

Indentation is necessary for Python. It specifies a block of code. All code within loops, classes, functions, etc is specified within an
indented block. It is usually done using four space characters. If your code is not indented necessarily, it will not execute accurately
and will throw errors as well.

----

**What is the difference between Python Arrays and lists?**

Arrays and lists, in Python, have the same way of storing data. But, arrays can hold only a single data type elements whereas lists can hold any data type elements.

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

import array as arr

def main():
    My_Array=arr.array('i',[1,2,3,4])
    My_list=[1,'abc',1.20]
    print(My_Array)
    print(My_list)

if __name__ == '__main__':
    main()
# Output:
# array(‘i’, [1, 2, 3, 4]) [1, ‘abc’, 1.2]
```

----

**What are functions in Python?**

A function is a block of code which is executed only when it is called. To define a Python function, the 'def' keyword is used.

----

**What is self in Python?**

Self is an instance or an object of a class. In Python, this is explicitly included as the first parameter. However, this is not the
case in Java where it’s optional.  It helps to differentiate between the methods and attributes of a class with local variables.

The self variable in the init method refers to the newly created object while in other methods, it refers to the object whose method
was called.

----

**How can you randomize the items of a list in place in Python?**

Consider the example shown below:

```
#!/usr/bin/python3
# -*- coding: utf-8 -*-

from random import shuffle

def main():
    x = ['Keep', 'The', 'Blue', 'Flag', 'Flying', 'High']
    shuffle(x)
    print(x)

if __name__ == '__main__':
    main()
# Output:
# ['Flying', 'Keep', 'Blue', 'High', 'The', 'Flag']
```

----

**What are python iterators?**

Iterators are objects which can be traversed though or iterated upon.

----

**How can you generate random numbers in Python?**

Random module is the standard module that is used to generate a random number. The method is defined as:

```python
import random
import random.random
```

The statement random.random() method return the floating-point number that is in the range of [0, 1]. The function generates random float numbers.
The methods that are used with the random class are the bound methods of the hidden instances. The instances of the Random can be done to show
the multi-threading programs that creates a different instance of individual threads. The other random generators that are used in this are:

```python
randrange(a, b)
# It chooses an integer and define the range in-between [a, b). It returns the elements by selecting it randomly
# from the range that is specified. It doesn’t build a range object.
```

```python
uniform(a, b)
# It chooses a floating point number that is defined in the range of [a,b).
# Iyt returns the floating point number
```

```python
normalvariate(mean, sdev)
# It is used for the normal distribution where the mu is a mean and the sdev is a sigma
# that is used for standard deviation. The Random class that is used and instantiated
# creates independent multiple random number generators.
```

----

**How do you write comments in python?**

Comments in Python start with a # character. However, alternatively at times, commenting is done using docstrings(strings enclosed within
triple quotes).

```python
# Example:
# 1
# 2
# 3
# <span data-mce-type="bookmark" style="display: inline-block; width: 0px; overflow: hidden; line-height: 0;" class="mce_SELRES_end"></span>
# <pre><span>#Comments in Python start like this
# print("Comments in Python start with a #")
# Output: Comments in Python start with a #
```

----

**What are the generators in python?**

Introduced with PEP 255, generator functions are a special kind of function that return a lazy iterator.
These are objects that you can loop over like a list. However, unlike lists, lazy iterators do not store
their contents in memory. For an overview of iterators in Python, take a look at Python “for” Loops (Definite Iteration).

```python
# Reading Large Files
# A common use case of generators is to work with data streams or large files, like CSV files. These text files separate
# data into columns by using commas. This format is a common way to share data. Now, what if you want to count the number
# of rows in a CSV file? The code block below shows one way of counting those rows:
csv_gen = csv_reader("some_csv.txt")
row_count = 0

for row in csv_gen:
    row_count += 1

print(f"Row count is {row_count}")
```

```python
# Generating an Infinite Sequence
# Let’s switch gears and look at infinite sequence generation. In Python, to get a finite sequence,
# you call range() and evaluate it in a list context:

def infinite_sequence():
    num = 0
    while True:
        yield num
        num += 1
```

----

**How will you capitalize the first letter of string?**

In Python, the capitalize() method capitalizes the first letter of a string. If the string already consists of a capital letter
at the beginning, then, it returns the original string.

```python
str = "capitalize this string here!"
output=str.capitalize()
print("The resultant string is:", output)
```

----

**How will you convert a string to all lowercase?**

To convert a string to lowercase, lower() function can be used.

```python
# Example:
# 1
# 2
stg='ABCD'
print(stg.lower())
# Output: abcd
```

----

**How to comment multiple lines in python?**

Multi-line comments appear in more than one line. All the lines to be commented are to be prefixed by a #. You can
also a very good shortcut method to comment multiple lines. All you need to do is hold the ctrl key and left click
in every place wherever you want to include a # character and type a # just once. This will comment all the lines
where you introduced your cursor.

----

**What are docstrings in Python?**

Docstrings are not actually comments, but, they are documentation strings. These docstrings are within triple
quotes. They are not assigned to any variable and therefore, at times, serve the purpose of comments as well.

```python
"""
Using docstring as a comment.
This code divides 2 numbers
"""
x=8
y=4
z=x/y
print(z)
# Output: 2.0
```

----

**What is the purpose of 'is', 'not' and 'in' operators?**

Operators are special functions. They take one or more values and produce a corresponding result.

_is_ : returns true when 2 operands are true  (Example: "a" is 'a')

_not_ : returns the inverse of the boolean value

_in_ : checks if some element is present in some sequence

----

**What is the usage of help() and dir() function in Python?**

Help() and dir() both functions are accessible from the Python interpreter and used for viewing a consolidated dump of built-in functions. 

_Help() function:_ The help() function is used to display the documentation string and also facilitates you to see the help related to modules, keywords, attributes, etc.

_Dir() function:_ The dir() function is used to display the defined symbols.

----

**Whenever Python exits, why isn’t all the memory de-allocated?**

Whenever Python exits, especially those Python modules which are having circular references to other objects or the objects that are referenced from
the global namespaces are not always de-allocated or freed. It is impossible to de-allocate those portions of memory that are reserved by the C library.
On exit, because of having its own efficient clean up mechanism, Python would try to de-allocate/destroy every other object.

----

**What is a dictionary in Python?**

The built-in datatypes in Python is called dictionary. It defines one-to-one relationship between keys and values. Dictionaries
contain pair of keys and their corresponding values. Dictionaries are indexed by keys.

Let’s take an example:

The following example contains some keys. Country, Capital & PM. Their corresponding values
are India, Delhi and Modi respectively.

```python
dict={'Country':'India','Capital':'Delhi','PM':'Modi'}
print dict[Country]
# Output : India
print dict[Capital]
# Output : Delhi
print dict[PM]
# Output : Modi
```

----

**How can the ternary operators be used in python?**

The Ternary operator is the operator that is used to show the conditional statements. This consists of the true
or false values with a statement that has to be evaluated for it.

```python
# The Ternary operator will be given as:
[on_true] if [expression] else [on_false]x, y = 25, 50big = x if x < y else y

# Example:
# Program to demonstrate conditional operator
a, b = 10, 20
# Copy value of a in min if a < b else copy b
min = a if a < b else b
print(min)
# The expression gets evaluated like if x < y else y, in this case if x < y is true then the value is returned as big=x and
# if it is incorrect then big=y will be sent as a result.
```

----

**What does this mean: *args, **kwargs? And why would we use it?**

We use *args when we aren’t sure how many arguments are going to be passed to a function, or if we want to pass a
stored list or tuple of arguments to a function. __**kwargs__ is used when we don’t know how many keyword arguments will
be passed to a function, or it can be used to pass the values of a dictionary as keyword arguments. The identifiers
args and kwargs are a convention, you could also use *bob and __**billy__ but that would not be wise.

----

**What does len() do?**

It is used to determine the length of a string, a list, an array, etc.

```python
stg='ABCD'
len(stg)
# Output:4
```

----

**Explain split(), sub(), subn() methods of “re” module in Python?**

To modify the strings, Python’s “re” module is providing 3 methods:

_split()_ : Uses a regex pattern to "split" a given string into a list.

_sub()_ : Finds all substrings where the regex pattern matches and then replace them with a different string.

_subn()_ : It is similar to sub() and also returns the new string along with the no. of replacements.

----

**What are negative indexes and why are they used?**

The sequences in Python are indexed and it consists of the positive as well as negative numbers. The numbers that
are positive uses ‘0’ that is uses as first index and ‘1’ as the second index and the process goes on like that.

The index for the negative number starts from ‘-1’ that represents the last index in the sequence and '-2' as the
penultimate index and the sequence carries forward like the positive number.

The negative index is used to remove any new-line spaces from the string and allow the string to except the last
character that is given as S[:-1]. The negative index is also used to show the index to represent the string in
correct order.

----

**What are Python packages?**

Python packages are namespaces containing multiple modules.

----

**How can files be deleted in Python?**

To delete a file in Python, you need to import the OS Module. After that, you need to use the os.remove() function.

```python
import os
os.remove("xyz.txt")
```

----

**What are the built-in types of python?**

Built-in types in Python are as follows:

- Integers
- Floating-point
- Complex numbers
- Strings
- Boolean
- Built-in functions

----

**What advantages do NumPy arrays offer over (nested) Python lists?**

Python's lists are efficient general-purpose containers. They support (fairly) efficient insertion, deletion, appending, and concatenation, and Python's list
comprehensions make them easy to construct and manipulate.

They have certain limitations: they don’t support “vectorized” operations like elementwise addition and multiplication, and the fact that they can contain
objects of differing types mean that Python must store type information for every element, and must execute type dispatching code when operating on each element.

NumPy is not just more efficient; it is also more convenient. You get a lot of vector and matrix operations for free, which sometimes allow one to avoid unnecessary work.
And they are also efficiently implemented. NumPy array is faster and You get a lot built in with NumPy, FFTs, convolutions, fast searching, basic statistics, linear algebra,
histograms, etc. 

---

**How to add values to a python array?**

Elements can be added to an array using the append(), extend() and the insert (i,x) functions.

```python
a=arr.array('d', [1.1 , 2.1 ,3.1] )
a.append(3.4)
print(a)
a.extend([4.5,6.3,6.8])
print(a)
a.insert(2,3.8)
print(a)
Output:
array('d', [1.1, 2.1, 3.1, 3.4])
array('d', [1.1, 2.1, 3.1, 3.4, 4.5, 6.3, 6.8])
array('d', [1.1, 2.1, 3.8, 3.1, 3.4, 4.5, 6.3, 6.8])
```

----

**How to remove values to a python array?**

Array elements can be removed using pop() or remove() method. The difference between these two functions is that the former
returns the deleted value whereas the latter does not.

```python
a=arr.array('d', [1.1, 2.2, 3.8, 3.1, 3.7, 1.2, 4.6])
print(a.pop())
print(a.pop(3))
a.remove(1.1)
print(a)
# Output:
# 4.6
array('d', [2.2, 3.8, 3.7, 1.2])
```

----

**Does Python have OOps concepts?**

Python is an object-oriented programming language. This means that any program can be solved in python by creating an object model.
However, Python can be treated as a procedural as well as structural language.

----

**What is the difference between deep and shallow copy?**

_Shallow copy_ is used when a new instance type gets created and it keeps the values that are copied in the new instance. Shallow copy
is used to copy the reference pointers just like it copies the values. These references point to the original objects and the changes
made in any member of the class will also affect the original copy of it. Shallow copy allows faster execution of the program and it
depends on the size of the data that is used.

```python
# Example:
# importing copy module
import copy
# initializing list 1
li1 = [1, 2, [3, 5], 4]
li2 = copy.copy(li1)
print("li2 ID: ", id(li2), "Value: ", li2)
```

_Deep copy_ is used to store the values that are already copied. Deep copy doesn’t copy the reference pointers to the objects. It
makes the reference to an object and the new object that is pointed by some other object gets stored. The changes made in the
original copy won’t affect any other copy that uses the object. Deep copy makes execution of the program slower due to making
certain copies for each object that is been called.

```python
# Example:
# importing copy module
import copy
# initializing list 1
li1 = [1, 2, [3, 5], 4]
# using deepcopy for deepcopy
li3 = copy.deepcopy(li1)
print("li3 ID: ", id(li3), "Value: ", li3)
```

----

**How is Multithreading achieved in Python?**

Python has a multi-threading package but if you want to multi-thread to speed your code up, then it’s usually not a good idea to use it.
Python has a construct called the Global Interpreter Lock (GIL).

The GIL makes sure that only one of your ‘threads’ can execute at any one time. A thread acquires the GIL, does a little work, then passes the GIL onto the next thread.

This happens very quickly so to the human eye it may seem like your threads are executing in parallel, but they are really just taking turns using the same CPU core.

All this GIL passing adds overhead to execution. This means that if you want to make your code run faster then using the threading package often isn’t a good idea.

----

**What is the process of compilation and linking in python?**

The compiling and linking allow the new extensions to be compiled properly without any error and the linking can be done only when
it passes the compiled procedure. If the dynamic loading is used then it depends on the style that is being provided with the system.
The python interpreter can be used to provide the dynamic loading of the configuration setup files and will rebuild the interpreter.

The steps that are required in this as:

- Create a file with any name and in any language that is supported by the compiler of your system. For example file.c or file.cpp
- Place this file in the Modules/ directory of the distribution which is getting used.
- Add a line in the file Setup.local that is present in the Modules/ directory.
- Run the file using spam file.o
- After a successful run of this rebuild the interpreter by using the make command on the top-level directory.
- If the file is changed then run rebuildMakefile by using the command as ‘make Makefile’.

----

**What are Python libraries? Name a few of them?**

Python libraries are a collection of Python packages. Some of the majorly used python libraries are – Numpy, Pandas, Matplotlib,
Scikit-learn and many more.

----

**What is split used for?**

The split() method is used to separate a given String in Python.

```python
a="example string to split"
print(a.split())
# Output: [‘edureka’, ‘python’]
```

----

**How to import modules in python?**

Modules can be imported using the import keyword.  You can import modules in three ways-

```python
import array # importing using the original module name
import array as arr # importing using an alias name
from array import * # imports everything present in the array module
```

----

**Explain Inheritance in Python with an example?**

Inheritance allows One class to gain all the members(say attributes and methods) of another class. Inheritance provides code
reusability, makes it easier to create and maintain an application. The class from which we are inheriting is called super-class
and the class that is inherited is called a derived / child class.

They are different types of inheritance supported by Python:

_Single Inheritance_ – where a derived class acquires the members of a single super class:

```python
# Python program to demonstrate
# single inheritance
 
# Base class
class Parent:
    def func1(self):
        print("This function is in parent class.")
 
# Derived class
class Child(Parent):
    def func2(self):
        print("This function is in child class.")
 
# Driver's code
object = Child()
object.func1()
object.func2()
```

_Multi-level inheritance_ – a derived class d1 in inherited from base class base1, and d2 are inherited from base2:

```python
# Python program to demonstrate
# multilevel inheritance

# Base class
class Grandfather:
	def __init__(self, grandfathername):
		self.grandfathername = grandfathername

# Intermediate class
class Father(Grandfather):
	def __init__(self, fathername, grandfathername):
		self.fathername = fathername

		# invoking constructor of Grandfather class
		Grandfather.__init__(self, grandfathername)

# Derived class
class Son(Father):
	def __init__(self, sonname, fathername, grandfathername):
		self.sonname = sonname

		# invoking constructor of Father class
		Father.__init__(self, fathername, grandfathername)

	def print_name(self):
		print('Grandfather name :', self.grandfathername)
		print("Father name :", self.fathername)
		print("Son name :", self.sonname)


# Driver code
s1 = Son('Prince', 'Rampal', 'Lal mani')
print(s1.grandfathername)
s1.print_name()
```

_Hierarchical inheritance_ – from one base class you can inherit any number of child classes:

```python
# Python program to demonstrate
# Hierarchical inheritance

# Base class
class Parent:
	def func1(self):
		print("This function is in parent class.")

# Derived class1
class Child1(Parent):
	def func2(self):
		print("This function is in child 1.")

# Derivied class2
class Child2(Parent):
	def func3(self):
		print("This function is in child 2.")


# Driver's code
object1 = Child1()
object2 = Child2()
object1.func1()
object1.func2()
object2.func1()
object2.func3()

```

_Hybrid inheritance_ – a derived class is inherited from more than one base class:

```python
# Python program to demonstrate
# hybrid inheritance


class School:
	def func1(self):
		print("This function is in school.")


class Student1(School):
	def func2(self):
		print("This function is in student 1. ")


class Student2(School):
	def func3(self):
		print("This function is in student 2.")


class Student3(Student1, School):
	def func4(self):
		print("This function is in student 3.")


# Driver's code
object = Student3()
object.func1()
object.func2()

```


----

**How are classes created in Python?**

Class in Python is created using the class keyword.

```python
class Employee:
    def __init__(self, name):
        self.name = name

E1=Employee("abc")
print(E1.name)
# Output: abc
```

----

**What is monkey patching in Python?**

In Python, the term monkey patch only refers to dynamic modifications of a class or module at run-time.

```python
# m.py
class MyClass:
def f(self):
print("f()")
```

```python
import m
def monkey_f(self):
print("monkey_f()")
 
m.MyClass.f = monkey_f
obj = m.MyClass()
obj.f()
# The output will be as below:
# monkey_f()
# As we can see, we did make some changes in the behavior of f() in MyClass using the function we defined, monkey_f(), outside of the module m.
```

----

**Does python support multiple inheritance?**

Multiple inheritance means that a class can be derived from more than one parent classes. Python does support multiple inheritance, unlike Java.

----

**What is Polymorphism in Python?**

Polymorphism means the ability to take multiple forms. So, for instance, if the parent class has a method named
ABC then the child class also can have a method with the same name ABC having its own parameters and variables.
Python allows polymorphism.

```python
# Polymorphism with class methods:
# The below code shows how Python can use two different class types, in the same way. We create a for loop that iterates
# through a tuple of objects. Then call the methods without being concerned about which class type each object is. We
# assume that these methods actually exist in each class. 
class India():
	def capital(self):
		print("New Delhi is the capital of India.")

	def language(self):
		print("Hindi is the most widely spoken language of India.")

	def type(self):
		print("India is a developing country.")

class USA():
	def capital(self):
		print("Washington, D.C. is the capital of USA.")

	def language(self):
		print("English is the primary language of USA.")

	def type(self):
		print("USA is a developed country.")

obj_ind = India()
obj_usa = USA()
for country in (obj_ind, obj_usa):
	country.capital()
	country.language()
	country.type()
```

----

**Define encapsulation in Python?**

Encapsulation means binding the code and the data together. A Python class in an example of encapsulation.

----

**How do you do data abstraction in Python?**

Data Abstraction is providing only the required details and hiding the implementation from the world.
It can be achieved in Python by using interfaces and abstract classes.

```python
# Consider a real-life example of encapsulation, in a company, there are different sections like the accounts section, finance section,
# sales section etc. The finance section handles all the financial transactions and keeps records of all the data related to finance.
# Similarly, the sales section handles all the sales-related activities and keeps records of all the sales. Now there may arise a
# situation when due to some reason an official from the finance section needs all the data about sales in a particular month. In
# this case, he is not allowed to directly access the data of the sales section. He will first have to contact some other officer
# in the sales section and then request him to give the particular data. This is what encapsulation is. Here the data of the sales
# section and the employees that can manipulate them are wrapped under a single name “sales section”. Using encapsulation also hides
# the data. In this example, the data of the sections like sales, finance, or accounts are hidden from any other section.

# Python program to
# demonstrate protected members

# Creating a base class
class Base:
	def __init__(self):

		# Protected member
		self._a = 2

# Creating a derived class
class Derived(Base):
	def __init__(self):

		# Calling constructor of
		# Base class
		Base.__init__(self)
		print("Calling protected member of base class: ",
			self._a)

		# Modify the protected variable:
		self._a = 3
		print("Calling modified protected member outside class: ",
			self._a)

obj1 = Derived()
obj2 = Base()
# Calling protected member
# Can be accessed but should not be done due to convention
print("Accessing protected member of obj1: ", obj1._a)
# Accessing the protected variable outside
print("Accessing protected member of obj2: ", obj2._a)
```

----

**Does python make use of access specifiers?**

Python does not deprive access to an instance variable or function. Python lays down the concept of prefixing
the name of the variable, function or method with a single or double underscore to imitate the behavior of
protected and private access specifiers.  

----

**How to create an empty class in Python?**

An empty class is a class that does not have any code defined within its block. It can be created using the
pass keyword. However, you can create objects of this class outside the class itself. IN PYTHON THE
PASS command does nothing when its executed. it’s a null statement. 

```python
class a:
    pass
obj=a()
obj.name="xyz"
print("Name = ",obj.name)
# Output: 
# Name = xyz
```

----

**What does an object() do?**

It returns a featureless object that is a base for all classes. Also, it does not take any parameters.
Next, let us have a look at some Basic Python Programs in these Python Interview Questions.
Basic Python Programs – Python Interview Questions

----

**Write a program in Python to execute the Bubble sort algorithm?**

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def bubble_sort(arr):
	n = len(arr)
	# optimize code, so if the array is already sorted, it doesn't need
	# to go through the entire process
	swapped = False
	# Traverse through all array elements
	for i in range(n-1):
		# range(n) also work but outer loop will
		# repeat one time more than needed.
		# Last i elements are already in place
		for j in range(0, n-i-1):
			# traverse the array from 0 to n-i-1
			# Swap if the element found is greater
			# than the next element
			if arr[j] > arr[j + 1]:
				swapped = True
				arr[j], arr[j + 1] = arr[j + 1], arr[j]
		if not swapped:
			# if we haven't needed to make a single swap, we
			# can just exit the main loop.
			return

def main():
    arr = [32,5,3,6,7,54,87]
    print(bubble_sort(arr))

if __name__ == '__main__':
    main()
```

----

**Write a program in Python to produce Star triangle?**

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def gen_star_triangle(r):
    for x in range(r):
        print(' '*(r-x-1)+'*'*(2*x+1))

def main():
    print(gen_star_triangle(9))

if __name__ == '__main__':
    main()
```

----

**Write a program to produce Fibonacci series in Python?**

```python
# Enter number of terms needednbsp;#0,1,1,2,3,5....
a = int(input("Enter the terms"))
f = 0;#first element of series
s = 1 # second element of series
if a = 0:
   print("The requested series is",f)
else:
  print(f,s,end=" ")
   for x in range(2,a): 
         print(next,end=" ")
         f=s
         s=next
# Output: Enter the terms 5 0 1 1 2 3
```

----

**Write a program in Python to check if a number is prime?**

```python
a=int(input("enter number"))
if a=1:
   for x in range(2,a):
         if(a%x)==0:
          print("not prime")
   break
   else:
      print("Prime")
else:
   print("not prime")
# Output:
# enter number 3
# Prime
```

----

**Write a program in Python to check if a sequence is a Palindrome?**

```python
a=input("enter sequence")
b=a[::-1]
if a==b:
  print("palindrome")
else:
  print("Not a Palindrome")
# Output:
# enter sequence 323 palindrome
```

----

**Write a one-liner that will count the number of capital letters in a file. Your code should work even if the file is too big to fit in memory?**

Let us first write a multiple line solution and then convert it to one-liner code.

```python
with open(SOME_LARGE_FILE) as fh:
count = 0
text = fh.read()
for character in text:
    if character.isupper():
count += 1

# We will now try to transform this into a single line.
count sum(1 for line in fh for character in line if character.isupper())
```

# https://www.edureka.co/blog/interview-questions/python-interview-questions/

# https://intellipaat.com/blog/interview-question/python-interview-questions/

**What is Python?**

Python is a high-level, interpreted, interactive, and object-oriented scripting language. It uses English keywords frequently. Whereas, other languages use punctuation, Python has fewer syntactic constructions.
Python is designed to be highly readable and compatible with different platforms such as Mac, Windows, Linux, Raspberry Pi, etc.
Python is one of the most demanding skills right now in the market. Enroll in our Python Certification Course and become a Python Expert.

----

**Python is an interpreted language. Explain?**

An interpreted language is any programming language that executes its statements line by line. Programs written in Python run directly from the source code, with no intermediary compilation step.

----

**What is the difference between lists and tuples?**

Lists	Tuples
Lists are mutable, i.e., they can be edited	Tuples are immutable (they are lists that cannot be edited)
Lists are usually slower than tuples	Tuples are faster than lists
Lists consume a lot of memory	Tuples consume less memory when compared to lists
Lists are less reliable in terms of errors as unexpected changes are more likely to occur	Tuples are more reliable as it is hard for any unexpected change to occur
Lists consist of many built-in functions.	Tuples do not consist of any built-in functions.
Syntax:
list_1 = [10, ‘Intellipaat’, 20]

Syntax:
tup_1 = (10, ‘Intellipaat’ , 20)

----

**What is PEP 8?**

PEP in Python stands for Python Enhancement Proposal. It is a set of rules that specify how to write and design Python code for maximum readability.

----

**What are the common built-in data types in Python?**

Python supports the below-mentioned built-in data types:

Immutable data types:

Number
String
Tuple
Mutable data types:

List
Dictionary
set
Watch this Video on Python for Data Science Tutorial

----

**What are local variables and global variables in Python?**

Local variable: Any variable declared inside a function is known as Local variable and it’s accessibility remains inside that function only.

Global Variable: Any variable declared outside the function is known as Global variable and it can be easily accessible by any function present throughout the program.

```python
g=4 #global variable
def func_multiply():
l=5 #local variable
m=g*l
return m
func_multiply()
Output: 20
# If you try to access the  local variable outside the multiply function
# then you will end up with getting an error.
```

----

**What is type conversion in Python?**

Python provides you with a much-needed functionality of converting one form of data type into the needed one and this is known as type conversion.

Type Conversion is classified into types:

----

**Implicit Type Conversion: In this form of type conversion python interpreter helps in automatically converting the data type?**

Into another data type without any user involvement.

----

**Explicit Type Conversion: In this form of Type conversion the data type inn changed into a required type by the user?**

Various Functions of explicit conversion are shown below:

int() – function converts any data type into integer.
float() – function converts any data type into float.
ord() – function returns an integer representing the Unicode character

hex() – function converts integers to hexadecimal strings.

oct() – function converts integer to octal strings.

tuple() – function convert to a tuple.

set() – function returns the type after converting to set.

list() – function converts any data type to a list type.

dict() – function is used to convert a tuple of order (key,value) into a dictionary.

str() –  function used to convert integer into a string.

complex(real,imag) – function used to convert real numbers to complex(real,imag) numbers.

----

**What does [::-1] do?**

[::-1] ,this is an example of slice notation and helps to reverse the sequence with the help of indexing.

[Start,stop,step count]

Let’s understand with an example of an array:

import array as arr
Array_d=arr.array('i',[1,2,3,4,5])
Array_d[::-1] # reverse the array or sequence
# Output: 5,4,3,2,1

----

**What are Python packages?**

A Python package refers to the collection of different sub-packages and modules based on the similarities of the function.

----

**What are decorators?**

In Python, decorators are necessary functions that help add functionality to an existing function without changing the structure of
the function at all. These are represented by @decorator_name in Python and are called in a bottom-up format.

Let’s have a look how it works:

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def decorator_lowercase(function): # defining python decorator
    def wrapper():
        func = function()
        input_lowercase = func.lower()
        return input_lowercase
    return wrapper

@decorator_lowercase # calling decoractor
def intro(): # normal function
    return 'Hello,I AM SAM'

def main():
    print(intro())

if __name__ == '__main__':
    main()
    
# Output:
# "hello,i am sam"    
```

----

**Is indentation required in Python?**

Indentation in Python is compulsory and is part of its syntax.

All programming languages have some way of defining the scope and extent of the block of codes. In Python, it is indentation.
Indentation provides better readability to the code, which is probably why Python has made it compulsory.

Learn the Pros and Cons of Python in our comprehensive blog on the Advantages and Disadvantages of Python.

----

**How does break, continue, and pass work?**

These statements help to change the phase of execution from the normal flow that is why they are termed loop control statements.

__Python break:__

This statement helps terminate the loop or the statement and pass the control to the next statement.

```python
for i in range(10):
    print(i)
    if i == 2:
        break
```

__Python continue:__

This statement helps force the execution of the next iteration when a specific condition meets, instead of terminating it.

```python
for var in "Geeksforgeeks":
	if var == "e":
		continue
	print(var)
```

__Python pass:__

This statement helps write the code syntactically and wants to skip the execution. It is also considered a null operation as nothing happens when you execute the pass statement.

```python
n = 26

if n > 26:
	# write code your here

print('Geeks')
```

----

**How can you randomize the items of a list in place in Python?**

This can be easily achieved by using the Shuffle() function from the random library as shown below:

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

from random import shuffle

def main():
    List = ['He', 'Loves', 'To', 'Code', 'In', 'Python']
    shuffle(List)
    print(List)
    # Output: [‘Loves’,’He’ ,’To ,’In’, ‘Python’,’Code’]

if __name__ == '__main__':
    main()
```

----

**How to comment with multiple lines in Python?**

To add a multiple lines comment in python, all the line should be prefixed by #.

```python
#This is a comment
#written in
#more than just one line
print("Hello, World!") 

"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")
```

----

**What type of language is python? Programming or scripting?**

Generally, Python is an all purpose Programming Language ,in addition to that Python is also Capable to perform scripting.

----

**What are negative indexes and why are they used?**

To access an element from ordered sequences, we simply use the index of the element, which is the position number of that particular element.
The index usually starts from 0, i.e., the first element has index 0, the second has 1, and so on.

Python Indexing
When we use the index to access elements from the end of a list, it’s called reverse indexing. In reverse indexing, the indexing of elements starts
from the last element with the index number ‘−1’. The second last element has index ‘−2’, and so on. These indexes used in reverse indexing are
called negative indexes.

----

**Explain split(), sub(), subn() methods of re module in Python?**

These methods belong to the Python RegEx or ‘re’ module and are used to modify strings.

__split():__

This method is used to split a given string into a list.

```python
txt = "welcome to the jungle"
x = txt.split()
print(x)
```

__sub():__

This method is used to find a substring where a regex pattern matches, and then it replaces the matched substring with a different string.

```python
# Importing re module
import re
# Given String
s = "I am a human being."
# Performing Sub() operation
res_1 = re.sub('a', 'x', s)
res_2 = re.sub('[a,I]','x',s)
# Print Results
print(res_1)
print(res_2)
# The original string remains unchanged
print(s)
```

__subn():__

This method is similar to the sub() method, but it returns the new string, along with the number of replacements.

```python
import re
print(re.subn('ov', '~*' , 'movie tickets booking in online'))
t = re.subn('ov', '~*' , 'movie tickets booking in online', flags = re.IGNORECASE)
print(t)
print(len(t))
print(t[0])
```

----

**What is a map function in Python?**

The map() function in Python has two parameters, function and iterable. The map() function takes a function as an argument and then
applies that function to all the elements of an iterable, passed to it as another argument. It returns an object list of results.

For example:

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def calc_sequence(n):
    return n*n

def main():
    numbers = (2, 3, 4, 5)
    result = map(calc_sequence, numbers)
    print(result)

if __name__ == '__main__':
    main()
```

----

**What are the generators in python?**

Generator refers to the function that returns an iterable set of items.

----

**What are python iterators?**

These are the certain objects that are easily traversed and iterated when needed.

----

**Do we need to declare variables with data types in Python?**

No. Python is a dynamically typed language, I.E., Python Interpreter automatically identifies the data type of a variable based on the type of value assigned to the variable.

Certification in Full Stack Web Development

----

**What are Dict and List comprehensions?**

Python comprehensions are like decorators, that help to build altered and filtered lists, dictionaries, or sets from a given list, dictionary, or set.
Comprehension saves a lot of time and code that might be considerably more complex and time-consuming.

Comprehensions are beneficial in the following scenarios:

- Performing mathematical operations on the entire list
- Performing conditional filtering operations on the entire list
- Combining multiple lists into one
- Flattening a multi-dimensional list

For example:

```python
my_list = [2, 3, 5, 7, 11]
squared_list = [x**2 for x in my_list]    # list comprehension
# output => [4 , 9 , 25 , 49 , 121]
squared_dict = {x:x**2 for x in my_list}    # dict comprehension
# output => {11: 121, 2: 4 , 3: 9 , 5: 25 , 7: 49}
```

----

**Is multiple inheritance supported in Python?**

Yes, unlike Java, Python provides users with a wide range of support in terms of inheritance and its usage. Multiple
inheritance refers to a scenario where a class is instantiated from more than one individual parent class. This provides
a lot of functionality and advantages to users.

----

**What do you understand by Tkinter?**

Tkinter is a built-in Python module that is used to create GUI applications. It is Python’s standard toolkit for GUI development.
Tkinter comes with Python, so there is no separate installation needed. You can start using it by importing it in your script.

----

**Is Python fully object oriented?**

Python does follow an object-oriented programming paradigm and has all the basic OOPs concepts such as inheritance, polymorphism, and more,
with the exception of access specifiers. Python doesn’t support strong encapsulation (adding a private keyword before data members). Although,
it has a convention that can be used for data hiding, i.e., prefixing a data member with two underscores.

----

**Differentiate between NumPy and SciPy?**

__NumPy !=SciPy__

NumPy stands for Numerical Python	SciPy stands for Scientific Python.

It is used for efficient and general numeric computations on numerical data saved in arrays. E.g., sorting, indexing, reshaping, and more.

This module is a collection of tools in Python used to perform operations such as integration, differentiation, and more.

There are some linear algebraic functions available in this module, but they are not full-fledged	Full-fledged algebraic functions are available in SciPy for algebraic computations

----

**Explain all file processing modes supported in Python?**

Python has various file processing modes.

__For opening files, there are three modes:__

read-only mode (r)
write-only mode (w)
read–write mode (rw)

__For opening a text file using the above modes, we will have to append ‘t’ with them as follows:__

read-only mode (rt)
write-only mode (wt)
read–write mode (rwt)

__Similarly, a binary file can be opened by appending ‘b’ with them as follows:__

read-only mode (rb)
write-only mode (wb)
read–write mode (rwb)

__To append the content in the files, we can use the append mode (a):__

For text files, the mode would be ‘at’
For binary files, it would be ‘ab’

----

**What do file-related modules in Python do? Can you name some file-related modules in Python?**

Python comes with some file-related modules that have functions to manipulate text files and binary files in a file system. These modules
can be used to create text or binary files, update their content, copy, delete, and more.

Some file-related modules are os, os.path, and shutil.os. The os.path module has functions to access the file system, while the shutil.os
module can be used to copy or delete files.

----

**Explain the use of the 'with' statement and its syntax?**

In Python, using the `with` statement, we can open a file and close it as soon as the block of code, where with is used, exits.
In this way, we can opt for not using the close() method.

```python
with open("filename", "mode") as file_var:
```

----

**Write a code to display the contents of a file in reverse?**

To display the contents of a file in reverse, the following code can be used:

```python
for line in reversed(list(open(filename.txt))):
print(line.rstrip())
```

----

**Which of the following is an invalid statement?**

xyz = 1,000,000
x y z = 1000 2000 3000 (invalid)
x,y,z = 1000, 2000, 3000
x_y_z = 1,000,000

----

**Write a command to open the file c:\hello.txt for writing?**

Command:

```python
f = open(“hello.txt”, “wt”)
```

----

**What does len() do?**

len() is an inbuilt function used to calculate the length of sequences like list, python string, and array.

```python
my _list=[1,2,3,4,5]
print(len(my_list))
```

----

**What does *args and **kwargs mean?**

__*args:__ It is used to pass multiple arguments in a function.

__**kwargs:__ It is used to pass multiple keyworded arguments in a function in python.

----

**How will you remove duplicate elements from a list?**

To remove duplicate elements from the list we use the set() function.

Consider the below example:

```python
demo_list=[5,4,4,6,8,12,12,1,5]
unique_list = list(set(demo_list))
output:[1,5,6,8,12]
```

----

**How can files be deleted in Python?**

You need to import the OS Module and use os.remove() function for deleting a file in python.
consider the code below:

```python
import os
os.remove("file_name.txt")
```

----

**How will you read a random line in a file?**

We can read a random line in a file using the random module.

For example:

```python
import random
def read_random(fname):
lines = open(fname).read().splitlines()
return random.choice(lines)
print(read_random (‘hello.txt’))
```

----

**Write a Python program to count the total number of lines in a text file?**

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-

def file_count(fname):
    with open(fname) as f:
        for i in enumerate(f):
            pass
    return i+1
  
def main():
    print(f"Total number of lines in the text file: {file_count('file.txt')}")

if __name__ == '__main__':
    main()
```

----

**What would be the output if I run the following code block?**

```python
list1 = [2, 33, 222, 14, 25]
print(list1[-2])
# Output: 14
```

----

**What is the purpose of is, not and in operators?**

Operators are referred to as special functions that take one or more values(operands) and produce a corresponding result.

is: returns the true value when both the operands are true  (Example: “x” is ‘x’)
not: returns the inverse of the boolean value based upon the operands (example:”1” returns “0” and vice-versa.
In: helps to check if the element is present in a given Sequence or not.

----

**Whenever Python exits, why isn’t all the memory de-allocated?**

Whenever Python exits, especially those Python modules which are having circular references to other objects or the objects that are referenced from the global namespaces are not always de-allocated or freed.
It is not possible to de-allocate those portions of memory that are reserved by the C library.
On exit, because of having its own efficient clean up mechanism, Python would try to de-allocate every object.

----

**How to add values to a python array?**

In python, adding elements in an array can be easily done with the help of extend(),append() and insert() functions.
Consider the following example:

```python
x = arr.array('d', [11.1 , 2.1 ,3.1] )
x.append(10.1)
print(x) # [11.1,2.1,3.1,10.1]
x.extend([8.3,1.3,5.3])
print(x) # [11.1,2.1,3.1,10.1,8.3,1.3,5.3]
x.insert(2,6.2)
print(x) # [11.1,2.1,6.2,3.1,10.1,8.3,1.3,5.3]
```

----

**How to remove values to a python array?**

Elements can be removed from the python array using pop() or remove() methods.

__pop():__ This function will return the removed element .

__remove():__ It will not return the removed element.

Consider the below example :

```python
x=arr.array('d', [8.1, 2.4, 6.8, 1.1, 7.7, 1.2, 3.6])
print(x.pop())
print(x.pop(3))
x.remove(8.1)
print(x)
# Output:
# 3.6
# 1.1  # element popped at 3 rd  index
array('d', [ 2.4, 6.8, 7.7, 1.2])
```

----

**Write a code to sort a numerical list in Python?**

The following code can be used to sort a numerical list in Python:

```python
list = ["2", "5", "7", "8", "1"]
list = [int(i) for i in list]
list.sort()
print(list)
```

----


**Can you write an efficient code to count the number of capital letters in a file?**

The normal solution for this problem statement would be as follows:

with open(SOME_LARGE_FILE) as countletter:

```python
count = 0
text = countletter.read()
for character in text:
if character.isupper():
count += 1
# To make this code more efficient, the whole code block can be converted into a one-liner code using the
# feature called generator expression. With this, the equivalent code line of the above code block would be as follows:
count sum(1 for line in countletter for character in line if character.isupper())
```

----

**How will you reverse a list in Python?**

The function list.reverse() reverses the objects of a list.

----

**How will you remove the last object from a list in Python?**

```
list.pop(obj=list[-1]):
# Here, −1 represents the last element of the list. Hence, the pop() function removes the last object (obj) from the list.
```

Get certified in Python from the top Python Course in Singapore now!

----

**How can you generate random numbers in Python?**

This achieved with importing the random module,it is the module that is used to generate random numbers.

Syntax:

import random
random.random # returns the  floating point random number between the range of [0,1].

----

**How will you convert a string to all lowercase?**

lower() function is  used to convert a string to lowercase.

For Example:

```python
demo_string='ROSES'
print(demo_string.lower())
Learn the complete Python Training in Hyderabad in 24 hours!
```

----

**Why would you use NumPy arrays instead of lists in Python?**

NumPy arrays provide users with three main advantages as shown below:
- NumPy arrays consume a lot less memory, thereby making the code more efficient.
- NumPy arrays execute faster and do not add heavy processing to the runtime.
- NumPy has a highly readable syntax, making it easy and convenient for programmers.

----

**What is Polymorphism in Python?**

Polymorphism is the ability of the code to take multiple forms. Let’s say, if the parent class has a method named XYZ then the child class can
also have a method with the same name XYZ having its own variables and parameters.

----

**Define encapsulation in Python?**

encapsulation in Python refers to the process of wrapping up the variables and different functions into a single entity or capsule.
Python class is the best example of encapsulation in python.

----

**What advantages do NumPy arrays offer over (nested) Python lists?**

__Nested Lists:__

Python lists are efficient general-purpose containers that support efficient operations like insertion,appending,deletion and concatenation.
The limitations of lists are that they don’t support “vectorized” operations like element wise addition and multiplication, and the fact that they can contain objects of differing types mean that Python must store type information for every element, and must execute type dispatching code when operating on each element.

__Numpy:__

NumPy is more efficient and more convenient as you get a lot of vector and matrix operations for free, which helps to avoid unnecessary work and complexity of the code.Numpy is also efficiently implemented when compared to nested
NumPy array is faster and contains a lot of built-in functions which will help in FFTs, convolutions, fast searching, linear algebra,basic statistics, histograms,etc.
Advanced Python Interview Questions for Experienced Professionals

----

**What is the lambda function in Python?**

A lambda function is an anonymous function (a function that does not have a name) in Python. To define anonymous functions, we use the ‘lambda’ keyword instead of the ‘def’ keyword, hence the name ‘lambda function’. Lambda functions can have any number of arguments but only one statement.

For example:

```
l = lambda x,y : x*y
print(a(5, 6))
# Output:30
```

----

**What is self in Python?**

Self is an object or an instance of a class. This is explicitly included as the first parameter in Python. On the other hand, in Java it is optional.
It helps differentiate between the methods and attributes of a class with local variables.

The self variable in the init method refers to the newly created object, while in other methods, it refers to the object whose method was called.

Syntax:

```
Class A:
    def __init__(self):
        ...
    
    def func(self):
        print(“Hi”)
```

----

**What is the difference between append() and extend() methods?**

Both append() and extend() methods are methods used to add elements at the end of a list.

__append(element):__ Adds the given element at the end of the list that called this append() method

__extend(another-list):__ Adds the elements of another list at the end of the list that called this extend() method

----

**How does Python Flask handle database requests?**

Flask supports a database-powered application (RDBS). Such a system requires creating a schema, which needs piping the schema.sql file
into the sqlite3 command. Python developers need to install the sqlite3 command to create or initiate the database in Flask.

Flask allows to request for a database in three ways:

__before_request():__ They are called before a request and pass no arguments.
__after_request():__ They are called after a request and pass the response that will be sent to the client.
__teardown_request():__ They are called in a situation when an exception is raised and responses are not guaranteed. They are called
after the response has been constructed. They are not allowed to modify the request, and their values areignored.

Sign up for the Full Stack Developer Course to begin your career journey today.

----

**How is Multithreading achieved in Python?**

Python has a multi-threading package, but commonly not considered as good practice to use it as it will result in increased code
execution time.

Python has a constructor called the [Global Interpreter Lock (GIL)](https://realpython.com/python-gil/). The GIL ensures that only one of your ‘threads’ can execute at
one time. The process makes sure that a thread acquires the GIL, does a little work, then passes the GIL onto the next thread.

This happens at a very Quick instance of time and that’s why to the human eye it seems like your threads are executing parallely, but
in reality they are executing one by one by just taking turns using the same CPU core.

----

**What is slicing in Python?**

Slicing is a process used to select a range of elements from sequence data type like list, string and tuple. Slicing is beneficial
and easy to extract out the elements. It requires a : (colon) which separates the start index and end index of the field.

All the data sequence types List or tuple allows us to use slicing to get the needed elements. Although we can get elements by
specifying an index, we get only a single element whereas using slicing we can get a group or appropriate range of needed elements.

Example:

```python
print(list_name[start:stop])
```

----

**What is functional programming? Does Python follow a functional programming style? If yes, list a few methods to implement functionally oriented programming in Python?**

Functional programming is a coding style where the main source of logic in a program comes from functions.

Incorporating functional programming in our codes means writing pure functions.

Pure functions are functions that cause little or no changes outside the scope of the function. These changes are referred to as
side effects. To reduce side effects, pure functions are used, which makes the code easy-to-follow, test, or debug.

Python does follow a functional programming style. Following are some examples of functional programming in Python.

_filter():_ Filter lets us filter some values based on a conditional logic.

```python
list(filter(lambda x:x>6,range(9))) [7, 8]
```

_map():_ Map applies a function to every element in an iterable.

```python
list(map(lambda x:x**2,range(5))) [0, 1, 4, 9, 16, 25]
```

_reduce():_ Reduce repeatedly reduces a sequence pair-wise until it reaches a single value.

```python
from functools import reduce >>> reduce(lambda x,y:x-y,[1,2,3,4,5]) -13
```

----

**Which one of the following is not the correct syntax for creating a set in Python?**

```python
set([[1,2],[3,4],[4,5]])
set([1,2,2,3,4,5])
{1,2,3,4}
set((1,2,3,4))
set([[1,2],[3,4],[4,5]])
```

Explanation: The argument given for the set must be iterable.

----

**What is _monkey patching_ in Python?**

Monkey patching is the term used to denote the modifications that are done to a class or a module during the runtime.
This can only be done as Python supports changes in the behavior of the program while being executed.

The following is an example, denoting monkey patching in Python:

```python
class X:
    def __init__(self):
        pass
    
    def func(self):
        print "func() is being called"
        
# The above module (monkeyy) is used to change the behavior of a
# function at the runtime as shown below:
import monkeyy
def monkey_f(self):
    print "monkey_f() is being called"

# replacing address of “func” with “monkey_f”
monkeyy.X.func = monkey_f
obj = monk.X()
# calling function “func” whose address got replaced
# with function “monkey_f()”
obj.func()
```

----

**What is the difference between / and // operator in Python?**

/: is a division operator and returns the Quotient value.

```python
x = 10/3
print(x)
# Output: 3.33
```

// : is known as floor division operator and used to return only the value of quotient before decimal

```python
y = 10//3
print(y)
# Output: 3
```

----

**What is pandas?**

Pandas is an open source python library which supports data structures for data based operations associated with data analyzing and data Manipulation.
Pandas with its rich sets of features fits in every role of data operation,whether it be related to implementing different algorithms or for solving
complex business problems. Pandas helps to deal with a number of files in performing certain operations on the data stored by files.

----

**What are dataframes?**

A dataframe refers to a two dimensional mutable data structure or data aligned in the tabular form with labeled axes(rows and column).

```python
pandas.DataFrame( data, index, columns, dtype)
# data:It refers to various forms like ndarray, series, map, lists, dict, constants and can take other DataFrame as Input.
# index:This argument is optional as the index for row labels will be automatically taken care of by pandas library.
# columns:This argument is optional as the index for column labels will be automatically taken care of by pandas library.
# Dtype: refers to the data type of each column.
```

----

**How to combine dataframes in pandas?**

The different dataframes can be easily combined with the help of functions listed below:

```python
# <li>Append():</li>
```

This function is used for horizontal stacking of dataframes.
data_frame1.append(data_frame2)
concat(): This function is used for vertical stacking and best suites when the dataframes to be combined possess the same column and similar fields.
pd.concat([data_frame1, data_frame2])
join(): This function is used to extract data from different dataframes which have one or more columns common.
data_frame1.join(data_frame2)

----

**How do you identify missing values and deal with missing values in Dataframe?**

Identification:

isnull() and isna() functions are used to identify the missing values in your data loaded into dataframe.

```python
missing_count=data_frame1.isnull().sum()
```

There are two ways of handling the missing values :

1. Replace the  missing values with 0

```python
df['col_name'].fillna(0)
```

2. Replace the missing values with the mean value of that column

```python
df['col_name'] = df['col_name'].fillna((df['col_name'].mean()))
```

----

**What is regression?**

Regression is termed as supervised machine learning algorithm technique which is used to find the correlation between variables and
help to predict the dependent variable(y) based upon the independent variable(x). It is mainly used for prediction, time series
modeling, forecasting, and determining the causal-effect relationship between variables.

Scikit library is used in python to implement the regression and all machine learning algorithms.

There are two different types of regression algorithms in machine learning :

Linear Regression: Used when the variables are continuous and numeric in nature.

Logistic Regression: Used when the variables are continuous and categorical in nature.

----

**What is classification?**

[Classification](https://www.geeksforgeeks.org/getting-started-with-classification/) refers to a predictive modeling process where a class label is predicted for a given example of input data. It
helps categorize the provided input into a label that other observations with similar features have. For example, it can be
used for classifying a mail whether it is spam or not, or for checking whether users will churn or not based on their behavior.

These are some of the classification algorithms used in Machine Learning:
- Decision Trees
- Bayesian Classifiers
- Neural Networks
- K-Nearest Neighbour
- Support Vector Machines
- Linear Regression
- Logistic Regression

----

**How do you split the data in train and test dataset in python?**

This can be achieved by using the scikit machine learning library and importing train_test_split function in python as shown below:

```python
Import sklearn.model_selection.train_test_split
# test size = 30% and train = 70 %
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33, random_state=0).
```

----

**What is SVM?**

_Support Vector Machine (SVM)_ is a supervised machine learning model that considers the classification algorithms for two-group classification problems. Support vector machine is a representation of the training data as points in space are separated into categories with the help of a clear gap that should be as wide as possible.

----

**Write a code to get the indices of N maximum values from a NumPy array?**

We can get the indices of N maximum values from a NumPy array using the below code:

```python
import numpy as np
ar = np.array([1, 3, 2, 4, 5, 6])
print(ar.argsort()[-3:][::-1])
```

----

**What is the easiest way to calculate percentiles when using Python?**

The easiest and the most efficient way you can calculate percentiles in Python is to make use of NumPy arrays and its functions.

Consider the following example:

```python
import numpy as np
a = np.array([1,2,3,4,5,6,7])
p = np.percentile(a, 50)  #Returns the 50th percentile which is also the median
print(p)
```

----

**Write a Python program to check whether a given string is a palindrome or not, without using an iterative method?**

A palindrome is a word, phrase, or sequence that reads the same backward as forward, e.g., madam, nurses run, etc.

```python
#!/usr/bin/python3 // run with system Python
#!/usr/bin/env python3 // run with dev version
# -*- coding: utf-8 -*-

def fun(string):
    s1 = string
    s = string[::-1]
    if(s1 == s):
        return true
    else:
        return false
    
def main():
    print(fun("madam"))

if __name__ == '__main__':
    main()
```

----

**Write a Python program to calculate the sum of a list of numbers?**

```python
#!/usr/bin/python3 // run with system Python
#!/usr/bin/env python3 // run with dev version
# -*- coding: utf-8 -*-

def sum_it_up(num):
    if len(num) == 1:
        # with only one element in the list, the
        # sum result will be equal to the element.
        return num[0]
    else:
        return num[0] + sum(num[1:])
    
def main():
    print(sum_it_up([2, 4, 5, 6, 7]))

if __name__ == '__main__':
    main()
```

----

**Write a program in Python to produce Star triangle?**

```python
#!/usr/bin/python3 // run with system Python
#!/usr/bin/env python3 // run with dev version
# -*- coding: utf-8 -*-

def star_triangle(n):
    for x in range(n):
        print(' '*(n-x-1)+'*'*(2*x+1))
    
def main():
    star_triangle(6)

if __name__ == '__main__':
    main()
```

----

**Write a program to produce Fibonacci series in Python?**

Fibonacci series refers to the series where the element is the sum of two elements prior to it.

```python
n = int(input("number of terms? "))
n1, n2 = 0, 1
count = 0
 
if n <= 0:
print("Please enter a positive integer")
elif n == 1:
print("Fibonacci sequence upto",nterms,":")
print(n1)
else:
print("Fibonacci sequence:")
while count < n:
print(n1)
nth = n1 + n2
n1 = n2
n2 = nth
count += 1
```

----

**Write a program in Python to check if a number is prime?**

```python

# Output: 13 is a prime number
```

----

**Write a sorting algorithm for a numerical dataset in Python?**

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-
  
def main(num):
    if num > 1:
        for i in range(2, int(num/2)+1):
            if (num % i) == 0:
                print(num, "is not a prime number")
                break
            else:
                print(num, "is a prime number")
                break
    else:
        print(num, "is not a prime number")

if __name__ == '__main__':
    main(14)
```

----

**Write a Program to print ASCII Value of a character in python?**

```python
x = 'a'
# print the ASCII value of assigned character stored in x
```

```python
print(" ASCII value of '" + x + "' is", ord(x))
```

# https://intellipaat.com/blog/interview-question/python-interview-questions/

# https://www.fullstack.cafe/blog/advanced-python-interview-questions

**What are virtualenvs?**

A virtualenv is what Python developers call an isolated environment for development, running, debugging Python code.
It is used to isolate a Python interpreter together with a set of libraries and settings.

Together with pip, it allows develop, deploy and run multiple applications on a single host, each with its own version of
the Python interpreter, and a separate set of libraries.

----

**What are the Wheels and Eggs? What is the difference?**

Wheel and Egg are both packaging formats that aim to support the use case of needing an install artifact that doesn’t
require building or compilation, which can be costly in testing and production workflows.

The Egg format was introduced by setuptools in 2004, whereas the Wheel format was introduced by PEP 427 in 2012.

Wheel is currently considered the standard for built and binary packaging for Python.

Here’s a breakdown of the important differences between Wheel and Egg.

Wheel has an official PEP. Egg did not.

Wheel is a distribution format, i.e a packaging format.

1 Egg was both a distribution format and a runtime installation format (if left zipped), and was designed to be importable.

Wheel archives do not include .pyc files. Therefore, when the distribution only contains Python files (i.e. no compiled extensions), and is compatible with Python 2 and 3, it’s possible for a wheel to be “universal”, similar to an sdist.

Wheel uses PEP376-compliant .dist-info directories. Egg used .egg-info.

Wheel has a richer file naming convention. A single wheel archive can indicate its compatibility with a number of Python language versions and 
implementations, ABIs, and system architectures.

Wheel is versioned. Every wheel file contains the version of the wheel specification and the implementation that packaged it.

Wheel is internally organized by sysconfig path type, therefore making it easier to convert to other formats.

----

**What does an x = a or b assignment do in Python?**

```python
x = a or b
# If bool(a) returns False, then x is assigned the value of b.
```

----

**What does the Python nonlocal statement do (in Python 3.0 and later)?**

In short, it lets you assign values to a variable in an outer (but non-global) scope.
The nonlocal statement causes the listed identifiers to refer to previously bound variables in the nearest enclosing scope
excluding globals.

For example, the counter generator can be rewritten to use this so that it looks more like the idioms of languages with closures.

```python
def make_counter():
    count = 0
    def counter():
        nonlocal count
        count += 1
        return count
    return counter
```

----

**What is the function of self?**

Self is a variable that represents the instance of the object to itself. In most object-oriented programming languages, this is
passed to the methods as a hidden parameter that is defined by an object. But, in python, it is declared and passed explicitly.
It is the first argument that gets created in the instance of the class A and the parameters to the methods are passed
automatically. It refers to a separate instance of the variable for individual objects.

Let's say you have a class ClassA which contains a method methodA defined as:

```python
def methodA(self, arg1, arg2): # do something
# and ObjectA is an instance of this class.
```

Now when ObjectA.methodA(arg1, arg2) is called, python internally converts it for you as:

```python
ClassA.methodA(ObjectA, arg1, arg2)
The self variable refers to the object itself.
```

----

**What is the python with statement designed for?**

The with statement simplifies exception handling by encapsulating common preparation and cleanup tasks in so-called context managers.

For instance, the open statement is a context manager in itself, which lets you open a file, keep it open as long as the execution
is in the context of the with statement where you used it, and close it as soon as you leave the context, no matter whether you
have left it because of an exception or during regular control flow.

As a result you could do something like:

```python
with open("foo.txt") as foo_file:
    data = foo_file.read()
```

OR

```python
from contextlib import nested
with nested(A(), B(), C()) as(X, Y, Z):
    do_something()
```

OR (Python 3.1)

```python
with open('data') as input_file, open('result', 'w') as output_file:
    for line in input_file:
        output_file.write(parse(line))
```

OR

```python
lock = threading.Lock()
with lock: # critical section of code
```

----

**Can you explain Closures (as they relate to Python)?**

In Python, a closure is a function object that remembers values in the enclosing lexical scope even if they are not present in
memory. It is a record that stores a function together with an environment: a mapping associating each free variable of the
function (variables that are used locally, but defined in an enclosing scope) with the value or reference to which the name
was bound when the closure was created. 

Closures are created when a function is defined inside another function and it uses variables from the outer function's
scope. The inner function, which is the closure, remembers those variables even if the outer function has finished
executing. 

Here's an example of a closure in Python:

```python
def outer_func(x):
    def inner_func(y):
        return x + y
    return inner_func

closure = outer_func(10)
result = closure(5)
print(result) # Output: 15
```

In this example, `outer_func` is a function that takes an argument `x` and returns another function `inner_func`.
`inner_func` takes an argument `y` and returns the sum of `x` and `y`. 

When `outer_func(10)` is called, it returns a closure `inner_func` that remembers the value of `x` as `10`. We
assign this closure to the variable `closure`. Then, we call `closure(5)` which returns the sum of `10` and `5`
which is `15`.

Closures are useful in many situations, such as when you want to create a function factory that generates functions
with pre-defined behavior. They are also used extensively in functional programming paradigms.

# https://www.fullstack.cafe/blog/advanced-python-interview-questions

# https://medium.com/@saint_sdmn/10-hardest-python-questions-98986c8cd309

----

**type == object?**

What is the result of the execution of the following code:

```python
isinstance(type, object)
isinstance(object, type)
isinstance(object, object)
isinstance(type, type)
# Correct answer: True, True, True, True
```

Everything is an object in Python, thus any instance check for an object will return True: isinstance(Anything, object) #=> True.

Python type represents a metaclass for constructing all Python types. Therefore all types: int, str, object are instances of a type class, which is, as everything in python, an object.

type is the only object in Python, that is an instance of itself.

```python
# >>> type(5)
# <class 'int'>
# >>> type(int)
# <class 'type'>
# >>> type(type)
# <class 'type'>
```

----

**Empty booleans?**

What is the result of the execution of the following code:

```python
# >>> any([])
# >>> all([])
# Answer: False, True
```

From the definition of any built-in functions we know, that it will:

Return True if any element of the iterable is true.

Logical operators in Python are lazy, the algorithm is to look for a first occurrence of a true element and, if none were
found, return False, Since the sequence is empty, there are no elements that can be true, therefore any([])returns False.

All example is a little bit more complicated, since it represents the concept of vacuous truth. Like with chained lazy logical
operators, the algorithm is to look for the first false element, and if none were found, return True. Since there are no false
elements in an empty sequence, all([]) returns True.

----

**Roundabout?**

What is the result of the execution of the following code:

```python
round(7 / 2)
round(3 / 2)
round(5 / 2)
# Answer: 4, 2, 2
```

Why does round(5 / 2) return 2 instead of 3? The issue here is that Python’s round method implements
__banker’s rounding__, where all half values will be rounded to the closest even number.

----

**Instance first!?**

What this code will print into console?

class A:
    answer = 42
    def __init__(self):
        self.answer = 21
        self.__add__ = lambda x, y: x.answer + y
    def __add__(self, y):
        return self.answer - y
print(A() + 5)
Answer: 16 (21 - 5)

In order to resolve an attribute name, Python will firstly search for it on an instance level, then on class level, then in parent classes.
This hold true for everything but __dunder__ methodd. While searching for them, Python will skip an instance check and search directly in
a class instead.

----

**Add it all together?**

What is the result of the execution of the following code:

```python
sum("")
sum("", [])
sum("", {})
# Answer: 0, [], {}
```

In order to understand what is happening here we need to inspect the signature of the sum function:

```python
sum(iterable, /, start=0)
```

Sums start and the items of an iterable from left to right and returns the total. The iterable’s items are normally numbers, and the start value is not allowed to be a string.

In all the cases above “” (empty string) is treated as an empty sequence, therefore sum will simply return the start argument as a total result.
In the first case it defaults to zero, for the second and the third case it implies that empty list and dictionary are passed in as a start argument.

----

**Unexpected attribute?**

What is the result of the execution of the following code:

```python
sum([el.imag for el in [0, 5, 10e9, float('inf'), float('nan')]])
# Answer: 0.0
```

This snippet won’t cause AttributeError. All numerical types in Python (int, real, float) are inherited from a base object class. Despite this,
all of them support real and imag attributes, returning real and imaginary parts respectively. That includes Infinity and NaN as well.

----

**Lazy Python?**

What is the result of the execution of the following code:

```python
class A:
    def function(self):
        return A()
a = A()
A = int
print(a.function())
# Answer: 0
```

Code inside python functions will be executed only upon invocation, meaning that all NameErrors will be raised and variables will be bonded only
when you actually call the method. In the example above, during method definition Python allows to reference the class that is not defined yet.

However, during the execution Python will bind the name A from the outer scope, which means that function method will return a newly created int instance.

----

**I want -1 times more?**

What is the result of the execution of the following code:

```python
"this is a very long string" * (-1)
# Answer: ‘’ (empty string)
```

From the python docs:
__"Values of n less than 0 are treated as 0 (which yields an empty sequence of the same type as s)"__

This holds true for any sequence types.

----

**Breaking the rules of math?**

What is the result of the execution of the following code:

```python
max(-0.0, 0.0)
Answer: -0.0
```

Why is that happens? This occurs because of the two reasons.

Negative zero and zero are treated as equal in Python.
Max function description from python docs states:
__"If multiple items are maximal, the function returns the first one encountered."__

Therefore max function returns the first occurrence of zero, which just happens to be the negative one.

----

**Breaking the rules of math (again)?**

What is the result of the execution of the following code:

```python
x = (1 << 53) + 1
x + 1.0 > x
# Answer: False
```

There are three things to blame for that counter-intuitive behavior: long arithmetic, float precision limits and numeric comparisons.
Python can support very large integers, switching a computation mode if the limit was exceeded implicitly (Or explicitly with a long
type in Python 2.*), but the float precision in Python is limited. The number is question:

```python
2**5**3 + 1 = 9007199254740993
```

Is the smallest integer that cannot be fully represented as a Python float. Therefore, in order to perform x + 1.0 Python casts xto float,
rounding it to 9007199254740992.0 which Python can represent, then adds 1.0 to it, but because of the same representation limits it sets it
back to 9007199254740992.0.

Another issue here is the comparison rules. Unlike other languages, Python and Ruby do not throw an error for float vs int comparison and neither
they try to cast both operands to the same type. Instead they compare actual numerical values. And because 9007199254740992.0 is lover than
9007199254740993 Python returns False.

# https://medium.com/@saint_sdmn/10-hardest-python-questions-98986c8cd309

# https://www.stratascratch.com/blog/advanced-python-interview-questions/

**Exploring the dataset?**

According to the question, we are required to calculate the sales growth per territory for Q3 and Q4 of 2021. In order to calculate the same, we need two parameters:
- Territories and their Q3 2021 sales total
- Territories and their Q4 2021 sales total

Firstly, locate the information in the tables provided. The first table provided is fct_customer_sales which has the following schema:

Table: fct_customer_sales
cust_id	prod_sku_id	order_date	order_value	order_id
C274	P474	2021-06-28	1500	O110
C285	P472	2021-06-28	899	O118
C282	P487	2021-06-30	500	O125
C282	P476	2021-07-02	999	O146
C284	P487	2021-07-07	500	O149
Show all
Toggle dTypes
From the preview of the table, we can observe that this is a list of Amazon orders, and the columns we need from this table are the order_value as well as the order_date.

Going back to the parameters we require, the second information we need is the territory of the sale. Let’s take a look at the second table provided,
which is the map_customer_territory table. Following are the schema and a preview of the table:

Table: map_customer_territory
cust_id	territory_id
C273	T3
C274	T3
C275	T1
C276	T1
C277	T1
Show all
Toggle dTypes
If we hadn’t been provided this schema, we would be confused about whether the location of the sale refers to the customer-related location or the seller’s
location. With this insight, we can assume that this analysis will reveal which areas have the strongest customer sales and is indicative of successful
marketing efforts or strong consumer demand.

An edge case to anticipate in this advanced python interview question is that some locations may not have had a sale at all for either of the quarters (Q3, Q4) of 2021.

There are a couple of reasons for this, new store openings or temporary closures. You could also consider a case where there may be missing locations.
Handling such edge cases in the database can be a little tricky. It can either be entered in the database as zero, blank, or no entry for the territory.
Given how the fct_customer_sales table is structured, it will most likely be the latter option.

----

**Writing out the approach?**

It’s time to lay out the approach you will be using to solve the problem.

Firstly, when it comes to Python, we always start with importing the necessary libraries. This is crucial because it gives you access to the various
packages and functions that are needed to manipulate the data. After we’re done importing the libraries, we can begin preparing our data for analysis.

Secondly, keeping in mind the required information for the solution, we need the territories and their sales value for Q3 and Q4 of 2021.
We will achieve this in two steps which can be performed interchangeably.

Filter for rows showing Q3 and Q4 sales of 2021; and
Identify the territory of sale by merging the two tables.
Thirdly, we need to analyze the sales quarterly, as opposed to at a transactional level. So, we will aggregate the sales by
summing this for each territory-quarter pair, viz., T1-Q3, T1-Q4, T2-Q3, and so on.

The expected table after these steps are performed will contain the territory ID, quarter, and their respective sum of sales.

It is good practice to think ahead about the format that you need your data to be in to make your operations easier. It is best to
have the table in the form of Territory ID | Q3 Sales | Q4 Sales. This step is to allow us to quickly calculate the ratio
using the Q3 and Q4 sales columns.

Let’s merge Q3 sales with Q4 sales in an inner join, relating them using the territory_id. This step is necessary to transform our data
into the structure we mentioned above. An inner join is what we’re going for here as we only want the territories with both Q3 and Q4
sales. This way, we exclude the territories which have a sale only in Q3 or Q4, which includes newly opened stores and stores with
temporary closures.

Now, we can calculate the sales growth ratio using the formula provided in the question.

Finally, select only the territory_id and sales_growth columns from the table. So, to summarize, the approach to solving the question can be seen written as:

Step 1: Import libraries
Step 2: Filter for rows showing Q3 and Q4 sales
Step 3: Identify the territory of sales by merging the two tables
Step 4: Output table: Territory ID | Quarter | Sum of sales
Step 5: Territory ID | Q3 Sales | Q4 Sales
Step 6: Merge Q3 sales with Q4 sales in an inner join, relating them by territory_id
Step 7: Calculate the Sales Growth Ratio using the following formula: (Q4 Sales - Q3 Sales) / Q3 Sales * 100
Step 8: Show the territory and the sales growth ratio

----

**Coding the solution?**

Now, let’s begin coding the solution. Let’s follow our written approach.

1. Import pandas and datetime libraries first

import pandas as pd
import datetime as dt

2. Filter for rows showing Q3 and Q4 sales

Prepare the data by selecting only the sales for Q3 and Q4 across all the territories in 2021. For this, we will use the datetime package, which allows us to identify the year and quarter information from the order_date column.

fct_customer_sales_21 = fct_customer_sales[
    (fct_customer_sales.order_date.dt.quarter.isin([3,4])) & 
    (fct_customer_sales.order_date.dt.year==2021)

Output for advanced python interview question

3. Identify the territory of sales by merging the two tables

The table above does not include the territory information that we require, so we will need to merge it with the map_customer_territory table using the common column cust_id.

sales = fct_customer_sales_21.merge(map_customer_territory, on='cust_id', how='inner')

Output 2 for advanced python interview question

From this table, let us filter only the territories of the customer, order_date, and order_value.

sales = fct_customer_sales_21.merge(map_customer_territory, on='cust_id', how='inner')[['territory_id', 'order_date', 'order_value']]

Output 3 for advanced python interview question

4. Output Table: Territory ID | Q3 Sales | Q4 Sales

Next, let us summarize the sales information by territory and by quarter. The first step to achieve that is to create groups based on unique territory_id and quarter combinations using the groupby() function and then aggregate this by summing up the fields.

sales = sales.groupby([sales.territory_id, sales.order_date.dt.quarter]).sum()

Output 4 for advanced python interview question


Now, this snippet only returns the field you are aggregating, i.e., order_value as the columns sales.territory_id and sales.order_date.dt.quarter specified in the groupby() function are used as an index.

We want the territory and quarter columns as well, so we will reset the index.

sales = sales.groupby([sales.territory_id, sales.order_date.dt.quarter]).sum().reset_index()

Output 5 for advanced python interview question

5. Territory ID | Q3 Sales | Q4 Sales

The next step is to transform this table into a table with the columns territory, Q3 sales, and Q4 sales. Let’s take a subset from the sales table, containing the Q3 sales.

sales = sales[sales.order_date==3]

Output 6 for advanced python interview question

6. Merge Q3 sales with Q4 sales in an inner join, relating them by territory_id

Now, let us merge it with another subset containing the Q4 sales.

sales = sales[sales.order_date==3].merge(sales[sales.order_date==4], how='inner', on='territory_id', suffixes=['_q3', '_q4'])
An important thing to note here is that when merging datasets, using suffixes can be very handy. It helps identify which table the columns are derived from. The default suffixes are ‘_x’ and ‘_y’ but for the sake of transparency, we will customize these to display ‘_q3’ and ‘_q4’.

Output 7 for advanced python interview question

7. Calculate the Sales Growth Ratio using the following formula:

(Q4 Sales - Q3 Sales) / Q3 Sales * 100

We have all the required data to calculate the sales growth ratio. Hence, with the formula provided, let's create a new column names ‘sales_growth’ and calculate it.

sales['sales_growth'] = (sales['order_value_q4'] - sales['order_value_q3'])/sales['order_value_q3']*100

Output 8 for advanced python interview question

8
9. . Show the territory and the sales growth ratio

Finally, let us select only the columns that we require, viz., territory_id and sales_growth.

sales[['territory_id', 'sales_growth']]

Our final solution looks like this:

import pandas as pd
import datetime as dt
fct_customer_sales_21 = \
    fct_customer_sales[fct_customer_sales.order_date.dt.quarter.isin([3,
                       4]) & (fct_customer_sales.order_date.dt.year
                       == 2021)]
sales = fct_customer_sales_21.merge(map_customer_territory, on='cust_id'
                                    , how='inner')[['territory_id'
                                    , 'order_date', 'order_value']]
sales = sales.groupby([sales.territory_id,
                      sales.order_date.dt.quarter]).sum().reset_index()
sales = sales[sales.order_date == 3].merge(sales[sales.order_date == 4]
                                    , how='inner', on='territory_id'
                                    , suffixes=['_q3', '_q4'])
sales['sales_growth'] = (sales['order_value_q4']
                         - sales['order_value_q3']) \
                         / sales['order_value_q3'] * 100
sales[['territory_id', 'sales_growth']]
Go to the question on the platform
Python
Tables: fct_customer_sales, map_customer_territory
 
The dataset has already been loaded as a pandas.DataFrame. print() functions and the last line of code will be displayed in the output.

In order for your solution to be accepted, your solution should be located on the last line of the editor and match the expected output data type listed in the question.

Reset
Run Code
Check Solution
Use Alt + Enter to run query

Our desired table looks like this:

Solution output for advanced python interview question

Considering Edge Cases
Always go beyond solving the problems in your interviews and discuss edge cases that could impact the scenario. There are certain benefits to discussing edge cases in interviews.

Ensures the robustness of your solution
Demonstrates strong attention to detail
Establishes your understanding of the business and the data capture process
For example, in this advanced python interview question, you can talk about missing values that could potentially occur due to new store openings and closures that we have identified already. Another scenario to discuss, especially in the case of eCommerce businesses like Amazon, is ‘refunds’.

To account for the scenario of refunds, it is important to recognize that refunds may take place anywhere between a few weeks to months after the sale. In such an edge case, it is acceptable to make reasonable assumptions.

For instance, are refunds logged separately as a different dataset or the in the same table as sales but recognized as a negative number? After considering this scenario, use the 3-step framework we laid out in the article to solve the problem.

You could analyze the net sales instead of gross sales. Here, net sales will be the sales amount after the refunds. For that as well, you will have to consider how the data is being logged.

Let us assume that the refunds are logged in another table along with the corresponding order_id. With this information, you can merge the refunds dataset with that of sales through the common order_id column. You can use a left join from the sales table for refunds, as not all sales will have a refund processed for it. Also, in order to avoid errors while subtracting refunds from sales, it is best to impute the missing refund values with a zero. This difference will result in ‘net sales’ and, thereafter, can be proceeded with the other steps as discussed in the solution.

# https://www.stratascratch.com/blog/advanced-python-interview-questions/

# https://www.simplilearn.com/django-interview-questions-article

**So what is Django?**

Django is an open-source web application framework written in Python. Developed in a fast-paced newsroom, Django enables the
rapid development of easily maintainable and secure websites. It’s a favorite of newbies and advanced programmers alike.

----

**Is Django named after that Quentin Tarantino movie?**

No, Django is named after [Django Reinhardt](https://de.wikipedia.org/wiki/Django_Reinhardt), a jazz guitarist from the 1930s to the early 1950s who is considered one of the
best guitarists of all time.

----

**What are Django's most prominent features?**

Programmers like Django mostly for its convenient features like:
- Excellent documentation
- python- Web-framework
- SEO Optimised
- High Scalability
- Versatile in Nature
- Offers High Security
- Thoroughly tested
- Provides rapid development
- Source: [https://data-flair.training/blogs/django-features/](https://data-flair.training/blogs/django-features/)
----

**Can you name some companies that use Django?**

Some of the more well-known companies that use Django include:

1. Instagram - A social media platform for sharing photos and videos.
2. Disqus - A commenting system used by many websites.
3. Mozilla - A non-profit organization that develops open-source software.
4. Pinterest - A visual discovery and bookmarking platform.
5. Dropbox - A cloud-based file hosting service.
6. The Washington Post - A major American newspaper.
7. Spotify - A popular music streaming service.
8. Eventbrite - A ticketing and event technology platform.
9. Bitbucket - A web-based hosting service for Git repositories.
10. YouTube - A video sharing platform.

There are many more companies that use Django, but these are just a few examples of the wide range
of industries and applications that use the framework.

----

**Why do web developers prefer Django?**

Web developers use Django because it:

Allows code modules to be divided into logical groups, making them flexible to change.
Provides an auto-generated web admin module to ease website administration.
Provides a pre-packaged API for common user tasks.
Enables developers to define a given function’s URL.
Allows users to separate business logic from the HTML.
Is written in Python, one of the most popular programming languages available today.
Gives you a system to define the HTML template for your web page, avoiding code duplication.

----

**What is CRUD?**

It has nothing to do with dirt or grime. It’s a handy acronym for Create, Read, Update, and Delete. It’s a mnemonic framework used to remind developers
on how to construct usable models when building application programming interfaces (APIs).

----

**Does Django have any drawbacks?**

Django’s disadvantages include:
- Its monolithic size makes it unsuitable for smaller projects.
- Everything hinges on Django’s ORM (Object-Relational Mapping).
- Everything must be explicitly defined due to a lack of convention.

----

**What does Django architecture look like?**

Django architecture consists of:

__Models:__ Describes the database schema and data structure.
__Views:__ Controls what a user sees. The view retrieves data from appropriate models, executes any calculations made, and passes it on to the template.
__Templates:__ Controls how the user sees the pages. It describes how the data received from the views need to be altered or formatted to display on the page.
__Controller:__ Made up of the Django framework and URL parsing.

----

**Explain the Django project directory structure?**

Django organizes the various sections of the web application using a directory structure by generating a project and an app
folder. Creating and arranging a proper project aids in keeping the project DRY (Don't Repeat Yourself) and clean. When you
create a Django project, Django creates a root directory for the project using the project name you provide. It contains
the files required to provide basic functionality to your web applications.

----

**What are models in Django?**

A Django model is a built-in feature of Django that allows you to construct tables, fields, and constraints. SQL (Structured Query Language) is 
complicated language that includes many different queries for generating, removing, updating, and other database-related tasks. 

----

**What are the views in Django?**

Django views are Python functions similar to HTML documents and accept HTTP requests and return HTTP responses.

----

**What is Django ORM?**

Django ORM is a database abstraction API using which we can interact with its database models i.e., perform actions
like add, delete, modify and query objects.

----

**Define static files and explain their uses?**

The word "static files" refers to files in a web app that do not change, such as CSS, JavaScript, or pictures.
They remain still. Static files are served up by the local Django web server for local development, and minimal
configuration is required.

----

**What are Django-admin and manage.py and explain their commands?**

“Django-admin” is the command line utility of Django to perform administrative tasks. And manage.py is created automatically in every
Django project. It performs the same functions as Django-admin, but it also modifies the DJANGO SETTINGS MODULE environment variable
to point to your project's settings.py file.

----

**What is Jinja templating?**

Jinja is a modern, designer-friendly Python templating language that was inspired by Django
templates and is frequently used for execution.

----

**What are Django URLs?**

In Django, URLs serve as the front door to your online application. In urls.py, you can configure how
Django routing works.

----

**What are the different model inheritance styles in Django?**

In Django, there are three types of inheritance. 

_Abstract base classes_ - When the parent class contains common fields and the parent class table is undesirable, use this.

_Multi-table inheritance_ - When the parent class has common fields, but the parent class table already exists in the database on its own, use this.

_Proxy models_ - Use this when you want to change the parent class's behavior, for as by modifying the order or adding a new model manager.

----

**In Django' context, what’s the difference between a project and an app?**

The project covers the entire application, while an app is a module or application within the project that deals with one dedicated requirement. So, a project consists of several apps, while an app features in multiple projects.

----

**What' a model in Django?**

A model consists of all the necessary fields and attributes of your stored data. They are a single, definitive source of information regarding your data.

----

**What are Django' templates?**

Django templates render information in a designer-friendly format to present to the user. Using the Django Template Language
(DTL), a user can generate HTML dynamically. Django templates consist of simple text files that can create any text-based
format such as XML, CSV, and HTML.

----

**Discuss Django' Request/Response Cycle?**

Starting the process off, the Django server receives a request. The server then looks for a matching URL in the URL patterns
defined for the project. If the server can’t find a matching URL, it produces a 404-status code. If the URL matches, it
executes the corresponding code in the view file associated with the URL and sends a response.

----

**What is the Django Admin interface?**

Django comes equipped with a fully customizable, built-in admin interface. This portal lets developers see and make changes to
all the data residing in the database that contains registered apps and models. The model must be registered in the admin.py
file to use a database table with the admin interface.

----

**How do you install Django?**

Users download and install Python per the operating system used by the host machine.
Then run the command:

```cmd
pip install django=2.2/"
```

on the terminal and wait for the installation to finish.

----

**How do you check which version of Django that you have installed on your system?**

You can check the version by opening the command prompt and entering the command:

```cmd
Python-m Django–version
```

You can also visit the Django homepage https://www.djangoproject.com/ and look at the “Download latest release” button located on the right of the page.

----

**What are signals in Django?**

Signals are pieces of code containing information about what is currently going on. A dispatcher is used to both send and listen for signals.

----

**Explain user authentication in Django?**

Django includes a user authentication system that handles objects such as users, groups, user permissions, and some cookie-based user sessions.

----

**What databases are supported by Django?**

The following databases are that Django formally supports:
- PostgreSQL
- MariaDB
- MySQL
- Oracle
- SQLite

----

**What's the use of a session framework?**

The session structure enables per-site-visitor storage and retrieval of any type of data. It abstracts the sending
and receiving of cookies and keeps data on the server side.

----

**What is the context in Django?**

In Django, a context is a dictionary where the keys are the names of the variables and the values are the values of those
variables. The template receives this dictionary (context), which it uses along with the variables to output the dynamic
content.

----

**What are Django.shortcuts.render functions?**

The render function is a shortcut function that allows the developer to quickly pass the data dictionary together with the template. The template is then combined with the data dictionary using the templating engine in this function. Finally, the render() function provides a HttpResponse containing the rendered text, which is the data returned by the models. As a result, Django render() saves the developer time and allows him to utilize multiple template engines. 

----

**What's the significance of the settings.py file?**

This file, as the name implies, stores our Django project's configurations or settings, such as database configuration, backend engines, middlewares, installed applications, main URL configurations, static file addresses, templating engines, security keys, allowed hosts etc.

----

**How to view all items in the Model?**

The 'all()' function in your interactive shell can be used as follows to display every item in your database:

* Where XYZ is a class you've generated in your models, XYZ.objects.all()

You can either use the get() function or the filter method to remove a specific element from your database, as seen below:

* pk=1 XYZ.objects.filter

* XYZ.objects(id=1)

Unleash a High-paying Automation Testing Job!
Automation Testing Masters ProgramEXPLORE PROGRAMUnleash a High-paying Automation Testing Job!

----

**How to filter items in the Model?**

Depending on the user's interests, it is a very normal need for the web application to display data on the web page. The application is made more user-friendly by its search feature. The filter() method of the Django framework can be used to filter data from database tables. A table may have numerous records, and depending on the specific criteria, it may be necessary to determine some specific data. By utilizing the filter() technique in numerous ways, this process gets simpler.  There are four types of filtering: Simple filtering, filter data with multiple fields, filter data with Q objects, and Filter data using filter chaining. 

We have covered the easy and intermediate Django interview questions, now let's look into the advanced level of Django interview questions and answers.

Advanced Django Interview Questions
We conclude with eight considerably tougher Django interview questions, designed for the expert-level Django users.

----

**What is the Django Rest Framework?**

The Django Rest Framework (DRF) is a framework that helps you quickly create RESTful APIs. They are ideal for web applications due to low bandwidth utilization.

----

**What do you use middleware for in Django?**

You use middleware for four different functions:

Content Gzipping
Cross-site request forgery protection
Session management
Use authentication

----

**What does a URLs-config file contain?**

The URLs-config file in Django contains a list of URLs and mappings created to view those URLs' functions. The URLs can map to view functions, class-based views, and the URLs-config of other applications.

----

**Does Django support multiple-column primary keys?**

No, Django supports only single-column primary keys.

----

**How can you see raw SQL queries running in Django?**

To begin, make sure that the DEBUG setting is set to True. If the setting is squared away, then type the following commands:

1) from Django.db import connection

2) connection.queries

----

**List several caching strategies supported by Django?**

Django supports these caching strategies:

Database caching
In-memory caching
File System Caching
Memcached 

----

**What is a QuerySet in the context of Django?**

QuerySet is a collection of SQL queries. The command print(b.query) shows you the SQL query created from the Django filter call.

----

**What do you use django.test.Client class for?**

The Client class acts like a dummy web browser, enabling users to test views and interact with Django-powered applications programmatically. This is especially useful when performing integration testing.

----

**How to use file-based sessions?**

To use a file-based session, you must set the SESSION_ENGINE settings to "Djangoo.contrib.sessions.backends.file".

----

**What is mixin?**

In Django, a mixin is a Python class that is inherited by another class to carry out extra functions. Classes that can be reused and scaled are mixins.
A unique form of multiple inheritances is a mixin. Mixins are typically employed in two contexts:

You wish to give a class several optional features.
You wish to apply a specific feature to numerous classes.

----

**What is Django Field Class?**

In general, "Field" is an abstract class that represents a database table column. In turn, RegisterLookupMixin is a subclass of the Field class.
These fields are utilized by Django's get prep value() and from db value() methods to construct database tables (db type()), which are then used
to transfer Python types to the database. As a result, fields are essential components of other Django APIs like models and querysets.

----

**Why is permanent redirection not a good option?**

Permanent redirection is only employed if it does not require visitors to be directed to the old URLs. The browser caches the response of
permanent redirections, thus attempting to redirect to somewhere different will cause problems. Because this is a browser-side process, if
your user navigates to a different page, it will load the same page.

----

**Difference between Django OneToOneField and ForeignKey Field?**

Both are among the most frequent sorts of fields in Django. The sole difference between these two is that the ForeignKey field includes an on_delete
option in addition to a model's class because it is used for many-to-one relationships, whilst the OneToOneField only handles one-to-one relationships
and requires only the model's class.

----

**How to combine multiple QuerySets in a View?**

QuerySets can be combined into another QuerySet, and they do not have to be from the same model.

To merge QuerySets from the same model, use the Python union operator.

The union operator can be used to combine two or more QuerySets with the following syntax: 

model_combination = model_set1 | model_set2 | model_set3 

Additionally, you can concatenate two or more QuerySets from other models by using the chain() method from the Itertools package. 

from itertools import chain

model_combination = list(chain(model_set1, model_set2)) 

As an alternative, you can merge two or more QuerySets from other models using union(), passing all=TRUE to allow for duplication.

model_combination = model_set1.union(model_set2, all=TRUE)  

----

**Mention the ways used for the customization of the functionality of the Django admin interface?**

Numerous customization options are available in the Django admin interface, and additional admin interfaces can even be created to enable user
separation through permissions. The ModelAdmin class, which serves as a representation of a model in the administration interface, can be used
to perform the majority of adjustments.

----

**Difference between select_related and prefetch_related?**

Django's select-related and prefetch-related functions are intended to reduce the number of database queries that are generated when related objects are accessed. 

When a query is executed, select related() "follows" foreign-key relationships and choose extra related-object data.

Prefetch related() performs the "joining" in Python by performing a separate lookup for each relationship.

When picking a single object, such as an OneToOneField or a ForeignKey, users utilize the select-related function. When retrieving a "set" of items, such as ManyToManyFields or reverse ForeignKeys, users utilize prefetch related. 

----

**Explain Q objects in Django ORM?**

When writing complex queries, Q objects are employed because filter() functions only allow you to 'AND' the conditions; whereas, Q objects allow you to 'OR' the conditions. 

----

**What are Django exceptions?**

An exception is an unusual event that causes a programme to fail. Django has its exception classes to cope with this circumstance, and it also supports all fundamental Python exceptions. The Django. core. exceptions module defines the Django core exceptions classes.

# https://www.simplilearn.com/django-interview-questions-article

# https://mindmajix.com/django-interview-questions

**What is Django? And why is it used?**

Django is a high-level Python web framework that enables the rapid development of secure and maintainable websites. It's free and open source. It takes care of much of the hassle of web development and allows you to focus on writing apps without any need to reinvent the wheel. 

The purpose behind developing this framework is to make developers spend time on new application components instead of already developed components.

The reasons why Django is most preferred are:
The Django framework is fast and flexible.
Suits for any web app development 
It's secure and Scalable.
Portable

----

**2. Is Django backend or front end?**

Django is suitable for both the backend and frontend. It's a collection of Python libraries that allow you to develop useful web apps ideal for backend and frontend purposes.

----

**3. What is the latest version of Django? And explain its features?**

The latest version of Django is Django 3.1. The new features of it are:

Supports asynchronous views and middleware
Provides JSON field support for all database backends
Admin layout
Path lib
Code Reusability
CDN Integration

SECURE_REFERRER_POLICY
If you want to enrich your career and become a professional in Python Django, then enroll in "Python Django Training". This course will help you to achieve excellence in this domain.

----

**4. What is the difference between Python and Django?**

Both Python and Django are intertwined but not the same. Python is a programming language used for
various application developments:machine learning, artificial intelligence, desktop apps, etc.

Django is a Python web framework used for full-stack app development and server development.

Using core Python, you can build an app from scratch or craft the app with Django using prewritten bits of code

----

**What architecture does Django use?**

Django follows a Model-View-Template (MVT) architecture. It contains three different parts:

Model: Logical data structure behind the entire app and signified by a database.
View: It's a user interface. What you see when you visit a website is called a user interface. Represented by HTML/CSS/Javascript files.
Template: Deals with the presentation of data.
Model template view

----

**Explain Django Architecture?**

As discussed in the previous question, Django follows MVT architecture - Model, Template, View.

The below diagram depicts the working cycle of Django MVT architecture: 

Django Architecture

From the diagram, you'll notice Template is on the Client side, and both the Model and View are on the Server side. Django uses request and response objects to communicate between the client and server.

If the website receives the request, it is transmitted from browser to server to manage the view file using a template.

After sending the correct URL request, the app logic and Model initiate the right response to the presented request. After that, a detailed response is sent back to View to check the response and transmit it as an HTTP response or desired user format. Then it again passes to the browser via Templates.

For your clear understanding, let's take a real-life example:

While logging into Django based website, you open the login page. It happens because View will process the request and send it to the login page URL. Then the response is sent from a server to the browser.

After then, you'll enter the credentials in Template, and the data sent back to the View to rectify the request, and then data is presented in the Model. Then the Model verifies the data provided by the user in the connected database.

If the user's data matches, it sends the related data (profile name, image, etc.) to the Views. 

Otherwise, the model passes the negative result to the Views. 

That's how the Django MVT architecture is working.

----

**Explain Django's code reusability?**

Compared to other frameworks, Django offers more code reusability. As Django is a combination of apps, copying those apps from one directory to another with some tweaks to the settings.py file won't need much time to write new applications from scratch.

That is why Django is the rapid development framework, and this kind of code reusability is not allowed in any other framework.

----

**Is Django easy to learn?**

Yes, Django is an easy-to-learn framework compared to others. Having some knowledge of Python and web-working helps you to start developing with Django.

----

**What are the unique features of Django that make it a better framework?**

The best features of Django that make it better compared to others are:

Compared to other open-source technologies, Django offers excellent documentation in the market.
It's aweb framework and one of the main reasons that people started using it. It's the only one that can solve any kind of operation out there.
Django is SEO optimized.
Django is scalable and can flexibly switch from small to large-scale projects.
Versatile in nature. Django allows you to build applications for various types of domains.
It has a vast community to connect with and share.
Provides rapid development

----

**What are the advantages of Django?**

Django has many advantages, but we'll look at major ones that differentiate it from other frameworks.

Better CDN connectivity and content management
Designed as batteries included framework
Supports MVC programming paradigm
Provides robust security features
Accelerated custom web app development       
Compatible with major operating systems and databases

----

**Describe the inheritance styles in Django?**

Django offers three inheritance styles:

__Abstract base classes:__

You use this style when you want the parent class to retain the data you don't want to type out for every child model.

__Multi-table inheritance:__

You use this style when you want to use a subclass on an existing model and want each model to have its database table.

__Proxy models:__

You use this style to modify Python-level behaviour with the models without changing the Model's field. 

----

**What are Django Models?**

A model is a definitive source of information about data, defined in the “app/models.py”. 

Models work as an abstraction layer that structures and manipulates data. Django models are a subclass of the "django.db.models". Model class and the attributes in the models represent database fields.

----

**13. Give a brief about the settings.py file?**

As the name implies, it's the main settings file of the Django file. Everything inside the Django project, like databases, middlewares, backend engines, templating engines, installed applications, static file addresses, main URL configurations, allowed hosts and servers, and security key stores in this file as a dictionary or list.

So when Django files start, it first executes the settings.py file and then loads the respective databases and engines to quickly serve the request.

----

**14. Is Django a CMS?**

No, Django is not CMS (Content Management System). It's just a web framework and programming tool that allows you to build websites.

----

**15. What are static files in Django? And how can you set them?**

In Django, static files are the files that serve the purpose of additional purposes such as images, CSS, or JavaScript files. Static files managed by “django.contrib.staticfiles”. There are three main things to do to set up static files in Django:

1) Set STATIC_ROOT in settings.py

2) Run manage.py collect static

3) Set up a Static Files entry on the PythonAnywhere web tab

----

**16. What is the use of Middlewares in Django?**

Middlewares in Django is a lightweight plugin that processes during request and response execution. It performs functions like security, CSRF protection, session, authentication, etc. Django supports various built-in middlewares.

----

**17. What is the difference between CharField and TextField in Django?**

TextField is a large text field for large-sized text. In Django, TextField is used to store paragraphs and all other text data. The default form widget for this field is TextArea.
CharField is a string field used for small- to large-sized strings. It is like a string field in C/C++. In Django, CharField is used to store small strings like first name, last name, etc.

----

**18. Describe Django Field Class types?**

Every field in a model is an instance of the appropriate field class. In Django, field class types determine:

- The column type describes the database about what kind of data to store. E.g., INTEGER, VARCHAR, TEXT
- The default HTML widget, while rendering a form field.
- The minimal validation requirements used in automatically generated forms and Django admin.

----

**19. What is the usage of "Django-admin.py" and "manage.py"?**

Django-admin.py - It is a command-line utility for administrative tasks. 
manage.py - It is automatically created in each Django project and controls the Django project on the server or even to begin one. It has the following usage:

Manages the project's package on the sys. path.
Sets the DJANGO_SETTINGS_MODULE environment variable

----

**20. What are signals in Django?**

Django includes a "signal dispatcher" to notify decoupled applications when some action takes place in the framework. In a nutshell, signals allow specific senders to inform a suite of receivers that some action has occurred. They are instrumental when we use more pieces of code in the same events.

Django provides a set of built-in signals that enable users to get notified of specific actions.

Signal	Description
Django.db.models.signals.pre_save(or)django.db.models.signals.post_save	Sent before or after a model’s save() method calls.
django.db.models.signals.pre_delete  (or)django.db.models.signals.post_delete	Sent before or after a model’s delete() method or query set’s delete() method calls.
django.db.models.signals.m2m_changed	We use this signal when ManyToManyField on a model changes.
Django.core.signals.request_started(or)django.core.signals.request_finished	We use this signal when Django starts or finishes an HTTP request.
Django Interview Questions for Experienced 

----

**21. What’s the difference between a project and an app in Django?**

The app is a module that deals with the dedicated requirements in a project. On the other hand, the project covers an entire app. In Django terms, a project can contain different apps, while an app features in various projects.

----

**22. Explain Django URL in brief?**

Django allows you to design URL functions however you want. For this, you need to create a Python module informally called URLconf (URL configuration).

This module is purely a Python code and acts as a mapping between URL path expressions and Python functions. Also, this mapping can be as long or short as needed and can also reference other mappings.

The length of this mapping can be as long or short as required and can also reference other mappings. Django also provides a way to translate URLs according to the active language.

----

**23. What are Django Exceptions?**

An exception is an abnormal event that leads to program failure. Django uses its exception classes and python exceptions as well to deal with such situations.

We define Django core exceptions in "Django.core.exceptions". The following classes are present in this module:

Exception 	Description
AppRegistryNotReady	This class raises for using models before loading the app process.
ObjectDoesNotExist	It’s a base class for DoesNotExist exceptions.
EmptyResultSet	This exception arises when the query fails to return results.
FieldDoesNotExist	When the requested file does not exist, this exception arises.
MultipleObjectsReturned	It raises by the query multiple objects returned when we expect only one object. 
SuspiciousOperation	It raises when the user has performed some operation, which is considered suspicious from a security perspective.
PermissionDenied	It arises when a user does not have permission to execute a specific action requested. 
ViewDoesNotExist	When the requested view does not exist, this exception raises.
MiddlewareNotUsed	When there is no middleware in server configuration, this exception arises.
ImproperlyConfigured	When Django configuration is improper, this exception arises.
FieldError	When there is a problem with the model field, this exception arises.
ValidationError	It raises when data validation fails.

----

**24. Explain Django session**

Django uses the session to keep track of the state between the site and a particular browser. Django supports anonymous sessions. The session framework stores and retrieves data on a per-site-visitor basis. It stores the information on the server side and supports sending and receiving cookies. Cookies store the data of session ID but not the actual data itself.

----

**25. What are Django cookies?**

A cookie is a piece of information stored in the client's browser. To set and fetch cookies, Django provides built-in methods. We use the set_cookie() method for setting a cookie and the get() method for getting the cookie.

You can also use the request.COOKIES['key'] array to get cookie values.

----

**26. Flask vs. Django: What's the difference between Flask & Django?**

Flask and Django are the two most popular Python web frameworks. The following table lists some significant differences between Django and Flask

Comparison Factor	Django	Flask
created	Django is a web development framework for Python. Its created in 2005	Flask is a web microframework offering basic features of web apps. Its created in 2010
Project Type	High-level Python web framework for easy and simple projects.	Low-level Python web framework. 
Features	The best features of Django are open-source, rapid development, robust documentation, great community, and easy to learn.	The best features of Flask are open source, lightweight, and require less code to develop an app.
Type of Framework	Full-stack web framework	WSGI (Web Server Gateway Interface ) framework
Templates, Admin, and ORM	Built-in	Requires installation
Flexibility 	Django Web Framework supports a large number of third-party applications.	Flask Web Framework doesn't offer support for third-party applications.
Companies using	Instagram, Coursera, Udemy.	Netflix, Reddit, Lyft, MIT
Visual Debugging	Django does not support visual debugging.	Flask supports visual debugging.
Bootstrapping tool	Builtin	Not available
Working style	Offers monolithic working style	Offers diversified working style
Project layout	The structure of the project layout is conventional.	The structure of the project layout for the flask is random.

----

**27. How to check the version of Django installed on your system?**

To check the version of Django installed on your system, open the command prompt and enter the following command:

py -m django --version
You can also try to import Django and use the get_version() method as follows:

import django
print(django.get_version())

----

**28. Give a brief about Django Admin?**

Django Admin is the command-line utility for administrative tasks. It's a preloaded interface to fulfill all web developer's needs and is imported from the "django.contrib packages". 

Django Admin interface has its user authentication and offers advanced features like authorizing the access, CMS (Content Management System), managing various models, etc.

You can even perform the following tasks using Django admin as listed out in the table:

Command	Task
django-admin help	Displays the usage of the information and commands list provided by each application.
django-admin help –command	Displays available commands
django-admin help <command>	Displays the command description and its available options
django-admin version	Determines Django’s version
django-admin make migrations	Depending on the changes done in the model creates new migrations
django-admin migrate	Synchronizes the database state with the present set of models and migrations
django-admin runserver	Starts the development server
django-admin sendtestemail	A test mail sent to confirm Django email working status
django-admin shell	Starts the Python interactive interpreter
django-admin showmigrations	Displays all the project’s migrations

----

**29. How do you create a Django project?**

To create a Django project, navigate to the directory where you want to do a project and type the following command:

```cmd
$ django-admin startproject ABC
```

That will create an "ABC" folder with the following structure −
ABC/
  manage.py
  myproject/
      __init__.py
      settings.py
      urls.py
      wsgi.py

Note: Here, "ABC" is the name of the project. You can mention any name you want.

----

**30. Name some companies using Django?**

Various companies out there are using Django. Of them, major are Instagram, Pinterest, Udemy, Mozilla Firefox, Reddit, etc.

----

**31. How do Django views work?**

Django views are the critical component of the framework They serve the purpose of encapsulation. They encapsulate the logic
liable to process a user's request and return a response to the user.

Either they return HTTP responses or raise an exception such as 404 in Django. Besides, Views also perform tasks like reading
records from a database, generating PDF files, etc.

Every app in Django comes with a views.py file, and this contains the views functions. Views function can be imported
directly in the URLs file in Django.

To achieve that, you have to import the view function in the urls.py file first and add the path/URL that the browser should
request to call that View function.

Explore Python Interview Questions that help you grab high-paying jobs.

----

**32. Give a brief about Django Template?**

Django Templates generate dynamic web pages. Using templates, you can show the static data and the data from various databases
connected to the app through a context dictionary. You can create any number of templates based on project requirements. Even
it's OK to have none of them.

Django template engine handles the templating in the Django web framework. Some template syntaxes declare variables, filters,
control logic, and comments.

Django ships built-in backends for its template system called the Django template language (DTL).

----

**33. Describe Django ORM?**

In Django, the most notable feature is Object-Relational Mapper (ORM), which allows you to interact with app data
from various relational databases such as SQLite, MySQL, and PostgreSQL. 

Django ORM is the abstraction between web application data structure (models) and the database where the data is stored.
Without writing any code, you can retrieve, delete, save, and perform other operations over the database.

The main advantage of ORMs is rapid development. ORMs make projects more portable. It's easier to change the database with Django ORM.

----

**34. When to use iterators in Django ORM?**
Iterators are containers in Python containing several elements. Every object in the iterator implements two methods
that are __init__() and the __next__() methods.

In Django, the fair use of an iterator is when you process results that take up a large amount of memory space. For this, you can use the iterator() method, which evaluates the QuerySet and returns the corresponding iterator over the results.

----

**35. What is Django caching? And explain the strategies used to implement it?**

Caching is the process of saving expensive calculation output to avoid performing the same calculation again.

Django supports a robust cache system to save web pages such that they don't have to be evaluated repeatedly for each request.

They are few strategies to implement caching in Django, and the following table lists them:

Strategy	Description 
Memcached	The most efficient and faster memory-based cache server
Filesystem caching	Cache files store in serial order in separate files.
Local-memory caching	If you have not specified any other, this is the default cache. It’s per-process and threads safe as well.
Database caching	Cache data will be stored in the database and works OK if you have a well-indexed database server.

----

**36. How does Django process a request?**

Whenever the Django Server receives a request, the system follows an algorithm to determine which Python code needs execution. Here are the steps that sum up the algorithm:

Django checks the root URL configuration.
Next, Django looks at all the variable URL patterns in the URLconf for the match of the requested URL
If the URL matches, it returns the associated view function.
It will then request the data from the Model of that app for any data requirement and pass it to the corresponding Template rendered by the browser. 
Django sends an error-handling view if none of the URLs match the requested URL.

----

**37. Which Python version should be used with Django?**

Python 3 is the most recommended version for Django. Because it's faster, has more features, and is better supported. 

----

**38. Explain the file structure of a typical Django project?**

A typical Django project consists of these four files:

manage.py
settings.py
__init__.py
urls.py
wsgi.py
The final four files are inside a directory, which is at the same level as manage.py.

manage.py is the command-line utility of your Django project and controls the Django project on the server.
settings.py file includes information on all the apps installed in the project.
The urls.py file acts as a map for the whole web project. 
The __init__.py file is an empty file that makes the python interpreter understand that the directory consisting of settings.py is a module/ package.
The wsgi.py file is for the server format WSGI

----

**Why is Django called a loosely coupled framework?**

Django is known as a loosely coupled framework beca+use of its MVT architecture.

Django's architecture is a variant of MVC architecture, and MVT is beneficial because it completely discards server code from the client's machine. Models and Views are present on the client machine, and templates only return to the client.

All the architecture components are different from each other. Both frontend and backend developers can work simultaneously on the projects as they won't affect each other when changed.

----

**What is the Django REST framework (DRF)?**

Django REST framework is a flexible and powerful toolkit for building Web APIs rapidly.

The following are the significant reasons that are making REST framework perfect choice:

Web browsable API 
Authentication policies 
Serialization
Extensive documentation and excellent community support.
Perfect for web apps since they have low bandwidth.
Global companies like Red Hat, Mozilla, Heroku, Eventbrite, etc., trust this framework.
Advanced Django Interview Questions

----

**Is Django too monolithic? Explain this statement?**

The Django framework is monolithic, which is valid to some extent. As Django's architecture is MVT-based, it requires some rules that developers need to follow to execute the appropriate files at the right time.

With Django, you get significant customizations with implementations. Through this, you cannot change file names, variable names, and predefined lists.

Django's file structure is a logical workflow. Thus the monolithic behavior of Django helps developers to understand the project efficiently.

----

**42. Explain user authentication in Django?**

Django comes with a built-in user authentication system to handle objects such as users, groups, permissions, etc. It not only performs authentication but authorization as well. 

Following are the system objects:

users
Groups
Password Hashing System
Permissions
A pluggable backend system
Forms Validation
Apart from this, there are various third-party web apps that we can use instead of the default system to provide more user authentication with more features.

----

**What is the "django.shortcuts.render" function?**

When a View function returns a web page as HttpResponse instead of a simple string, we use the render function.

Render is a shortcut for passing a data dictionary with a template. This function uses a templating engine to combine templates with a data dictionary.

Finally, the render() returns the HttpResponse with the rendered text, the models' data.

Syntax:

render(request, template_name, context=None, content_type=None, status=None, using=None)
The request generates a response.

The template name and other parameters pass the dictionary.

For more control, specify the content type, the data status you passed, and the render you are returning. 

----

**What is the use of forms in Django?**

Forms serve the purpose of receiving user inputs and using that data for logical operations on databases. Django supports form class to create HTML forms. It defines a form and how it works and appears.

Django's forms handle the following parts:

Prepares and restructures data to make it ready for rendering
Creates HTML forms for the data
Processes submitted forms and data from the client.

----

**Can you explain how to add View functions to the urls.py file?**

There are two ways to add the view function to the main URLs config:

1. Adding a function View

In this method, import the particular View's function and add the specific URL to the URL patterns list.

2. Adding a Class-based view 

This one is a more class-based approach. For this, import the class from the views.py and then add the URL to the URL patterns. An inbuilt method is needed to call the class as a view.

Write the name of the function on the previous method as shown below:

class_name.as_view()
This will pass your view class as a view function.

Both function-based and class-based have their advantages and disadvantages. Depending on the situation, you can use them to get the right results.

----

**Explain Django Security?**

Protecting user's data is an essential part of any website design. Django implements various sufficient protections against several common threats. The following are Django's security features:

Cross-site scripting (XSS) protection
SQL injection protection
Cross-site request forgery (CSRF) protection
Enforcing SSL/HTTPS
Session security
Clickjacking protection
Host header validation

----

**What is Ajax in Django?**

AJAX (Asynchronous JavaScript And XML) allows web pages to update asynchronously to and from the server by exchanging data in Django. That means without reloading a complete webpage you can update parts of the web page.

It involves a combination of a browser built-in XMLHttpRequest object, HTML DOM, and JavaScript.

----

**How to handle Ajax requests in Django?**

To handle Ajax requests in the Django web framework, perform the following:

Initialize Project 
Create models
Create views
Write URLs
Carry out requests with Jquery Ajax.
Register models to admin 

----

**What are Django generic views?**

Writing views is a heavy task. Django offers an easy way to set Views called Generic Views. They are classes but not functions and stored in "django.views.generic". 

Generic views act as a shortcut for common usage patterns. They take some common idioms and patterns in view development and abstract them to write common views of data without repeating yourself quickly.

----

**What is the correct way to make a variable available to all your templates?**

In case all your templates need the same objects, use "RequestContext." This method takes HttpRequest as the first parameter and populates the context with a few variables simultaneously as per the engine's context_processors configuration option.

Django FAQs

----

**Tell me how to use a file-based session?**

For this, we have to set the SESSION_ENGINE settings to “Django.contrib.sessions.backends.file.”

----

**What command-line loads data in Django?**

“Django-admin.py load data” loads data in Django. This command line performs data searching and loads the contents of the named fixtures into the database.

----

**What is CRUD?**

CRUS is an acronym for Create, Read, Update, and Delete. It’s a mnemonic framework used for constructing models when building application programming interfaces (APIs).

----

**Explain Django’s Request/Response Cycle?**

When a process starts, the Django server receives a request and checks for a matching URL in the project-defined URL patterns. If the URL matches, it executes the associated code in the view file with the URL and sends a response. If the server can’t find a matching URL, it invokes a 404-status code.

----

**What do you use middleware for in Django?**

For the following functions, you can use Middleware in Django:

Cross-site request forgery protection
Content Gzipping
User authentication
Session management

----

**Does Django support multiple-column primary keys?**

Django does not support multiple-column primary keys. It only supports single-column primary keys.

----

**What is a QuerySet?**

In the context of Django, QuerySet is a set of SQL queries. To see the SQL query from the Django filter call, type the command print(b.query).

----

**How to check the raw SQL queries running in Django?**

Make sure that the DEBUG setting is set to True, and type the following commands:

from Django.db import connection
connection.queries

----

**Are Django signals asynchronous?**

No, Django signals are synchronous. There is no background thread or asynchronous jobs to execute them. When we use signals in applications, they allow you to maintain the code to understand application behavior and solve issues faster and better.

----

**What are the Django disadvantages?**

Not suitable for small projects due to its monolithic size

Everything connects on Django’s ORM.
Everything must be defined explicitly due to a lack of convention.
Django web framework has a steep learning curve.

# https://mindmajix.com/django-interview-questions

# https://www.interviewbit.com/django-interview-questions/

**Explain Django Architecture?**

Django follows the MVT (Model View Template) pattern which is based on the Model View Controller architecture. It’s slightly different from the MVC pattern as it maintains its own conventions, so, the controller is handled by the framework itself. The template is a presentation layer. It is an HTML file mixed with Django Template Language (DTL). The developer provides the model, the view, and the template then maps it to a URL, and finally, Django serves it to the user.

----

**Explain the django project directory structure?**

manage.py - A command-line utility that allows you to interact with your Django project
__init__.py - An empty file that tells Python that the current directory should be considered as a Python package
settings.py - Comprises the configurations of the current project like DB connections.
urls.py - All the URLs of the project are present here
wsgi.py - This is an entry point for your application which is used by the web servers to serve the project you have created.

----

**What are models in Django?**
A model in Django refers to a class that maps to a database table or database collection. Each attribute of the Django model class represents a database field. They are defined in app/models.py

Example: 

from django.db import models
class SampleModel(models.Model):
field1 = models.CharField(max_length = 50)
field2 = models.IntegerField()
class Meta:
db_table = “sample_model”
Every model inherits from django.db.models.Model

Our example has 2 attributes (1 char and 1 integer field), those will be in the table fields.

The metaclass helps you set things like available permissions, singular and plural versions of the name, associated database table name, whether the model is abstract or not, etc.

To get more information about models you can refer here: https://docs.djangoproject.com/en/3.1/topics/db/models/.

You can download a PDF version of Django Interview Questions.

Download PDF

----

**What are templates in Django or Django template language?**

Templates are an integral part of the Django MVT architecture. They generally comprise HTML, CSS, and js in which dynamic variables and information are embedded with the help of views. Some constructs are recognized and interpreted by the template engine. The main ones are variables and tags.

A template is rendered with a context. Rendering just replaces variables with their values, present in the context, and processes tags. Everything else remains as it is.

The syntax of the Django template language includes the following four constructs :

Variables
Tags
Filters
Comments
To read more about templates you can refer to this: https://docs.djangoproject.com/en/3.1/topics/templates/

**What are views in Django?**

A view function, or “view” for short, is simply a Python function that takes a web request and returns a web response. This response can be HTML contents of a web page, or a redirect, or a 404 error, or an XML document, or an image, etc. 

Example:

from django.http import HttpResponse
def sample_function(request):
 return HttpResponse(“Welcome to Django”)
There are two types of views:

Function-Based Views: In this, we import our view as a function.
Class-based Views: It’s an object-oriented approach.

----

**What is Django ORM?**

This ORM (an acronym for Object Relational Mapper) enables us to interact with databases in a more pythonic way like we can avoid writing raw queries, it is possible to retrieve, save, delete and perform other operations over the database without ever writing any SQL query. It works as an abstraction layer between the models and the database.

----

**Define static files and explain their uses?**

Websites generally need to serve additional files such as images. Javascript or CSS. In Django, these files are referred to as “static files”, Apart from that Django provides django.contrib.staticfiles to manage these static files.

----

**What is Django Rest Framework(DRF)?**

Django Rest Framework is an open-source framework based upon Django which lets you create RESTful APIs rapidly.

----

**What is django-admin and manage.py and explain its commands?**

django-admin is Django’s command-line utility for administrative tasks. In addition to this, a manage.py file is also automatically created in each Django project. Not only does it perform the same purpose as the django-admin but it also sets the DJANGO_SETTINGS_MODULE environment variable to point to the project's settings.py file.

django-admin help - used to display usage information and a list of the commands provided by each application.
django-admin version - used to check your Django version.
django-admin check - used to inspect the entire Django project for common problems.
django-admin compilemessages - Compiles .po files created by makemessages to .mo files for use with the help of built-in gettext support.
django-admin createcachetable - Creates the cache tables for use in the database cache backend.
django-admin dbshell - Runs the command-line client for the database engine specified in your ENGINE setting(s), with the connection parameters (USER, PASSWORD, DB_NAME, USER etc.) specified settings file.
django-admin diffsettings - Shows the difference between the existing settings file and Django’s default settings.
django-admin dumpdata - Used to the dumpdata from the database.
django-admin flush - Flush all values from the database and also re-executes any post-synchronization handlers specified in the code.
django-admin inspectdb - It generates django models from the existing database tables.
django-admin loaddata - loads the data into the database from the fixture file.
django-admin makemessages - Used for translation purpose and it generates a message file too.
django-admin makemigrations - Generates new migrations as per the changes detected to your models.
django-admin migrate - Executes SQL commands after which the database state with the current set of models and migrations are synchronized.
django-admin runserver - Starts a light-weight Web server on the local machine for development. The default server runs on port 8000 on the IP address 127.0.0.1. You can pass a custom IP address and port number explicitly if you want.
django-admin sendtestemail - This is used to confirm email sending through Django is working by sending a test email to the recipient(s) specified.
django-admin shell - Starts the Python interactive interpreter.
django-admin showmigrations - Shows all migrations present in the project.
django-admin sqlflush - Prints the SQL statements that would be executed for the flush command mentioned above.
django-admin sqlmigrate - Prints the SQL statement for the named migration.
django-admin sqlsequencereset - output the SQL queries for resetting sequences for the given app name(s).
django-admin squashmigrations - Squashes a range of migrations for a particular app_label.
django-admin startapp - Creates a new Django app for the given app name within the current directory or at the given destination.
django-admin startproject - Creates a new Django project directory structure for the given project name within the current directory or at the given destination.
django-admin test - Runs tests for all installed apps.
django-admin testserver - Runs a Django development server (which is also executed via the runserver command) using data from the given fixture(s).
django-admin changepassword - offers a method to change the user's password.
django-admin createsuperuser - Creates a user account with all permissions(also known as superuser account).
django-admin remove_stale_contenttypes - removes stale content types (from deleted models) in your database.
django-admin clearsessions - Can be used to clean out expired sessions or as a cron job.

**What is Jinja templating?**

Jinja Templating is a very popular templating engine for Python, the latest version is Jinja2. 

Some of its features are:

Sandbox Execution - This is a sandbox (or a protected) framework for automating the testing process
HTML Escaping - It provides automatic HTML Escaping as <, >, & characters have special values in templates and if using a regular text, these symbols can lead to XSS Attacks which Jinja deals with automatically.
Template Inheritance
Generates HTML templates much faster than default engine
Easier to debug as compared to the default engine.

----

**11. What are Django URLs?**

URLs are one of the most important parts of a web application and Django provides you with an elegant way to design your own custom URLs with help of its module known as URLconf (URL Configuration). The basic functionality of this python module is to 
You can design your own URLs in Django in the way you like and then map them to the python function (View function). These URLs can be static as well as dynamic. These URLs as present in the urls.py where they are matched with the equivalent view function. 

Basic Syntax:

from django.urls import path
from . import views
urlpatterns = [
   path('data/2020/', views.data_2020),
   path('data/<int:year>/', views.data_year)
]

----

**12. What is the difference between a project and an app in Django?**

In simple words Project is the entire Django application and an app is a module inside the project that deals with one specific use case. 
For eg, payment system(app) in the eCommerce app(Project).

----

**13. What are different model inheritance styles in the Django?**

Abstract Base Class Inheritance: Used when you only need the parent class to hold information that you don’t want to write for each child model.
Multi-Table Model Inheritance:  Used when you are subclassing an existing model and need each model to have its own table in the database.
Proxy Model Inheritance:  Used when you want to retain the model's field while altering the python level functioning of the model.
Intermediate Django Interview Questions

----

**14. What are Django Signals?**

Whenever there is a modification in a model, we may need to trigger some actions. 
Django provides an elegant way to handle these in the form of signals. The signals are the utilities that allow us to associate events with actions. We can implement these by developing a function that will run when a signal calls it.

List of built-in signals in the models:

Signals	Description
django.db.models.pre_init &
django.db.models.post_init	Sent before or after a models’s _init_() method is called
django.db.models.signals.pre_save & django.db.models.signals.post_save	Sent before or after a model’s save() method is called
django.db.models.signals.pre_delete &
django.db.models.signals.post_delete	Sent before or after a models’ delete() method or queryset delete() method is called
django.db.models.signals.m2m_changed	Sent when a ManyToManyField is changed
django.core.signals.request_started &
django.core.signals.request_finished	Sent when an HTTP request is started or finished

----

**15. Explain the caching strategies in the Django?**

Caching refers to the technique of storing the output results when they are processed initially so that next time when the same results are fetched again, instead of processing again those already stored results can be used, which leads to faster accessing as well us less resource utilization. Django provides us with a robust cache system that is able to store dynamic web pages so that these pages don’t need to be evaluated again for each request. 

Some of the caching strategies in Django are listed below:

Strategy	Description
Memcached	A memory-based cache server is the fastest and most efficient
FileSystem Caching	Values of the cache are stored as separate files in a serialized order
Local-memory Caching	This is used as the default cache strategy by Django if you haven’t set anything. It is per-process as well as thread-safe.
Database Caching 	Cache data will be stored in the database and works very well if you have a fast and well-indexed DB server.

----

**16. Explain user authentication in Django?**

Django comes with a built-in user authentication system, which handles objects like users, groups, user-permissions, and few cookie-based user sessions. Django User authentication not only authenticates the user but also authorizes him.

The system consists and operates on these objects:

Users
Permissions
Groups
Password Hashing System
Forms Validation
A pluggable backend system

----

**17. How to configure static files?**

Ensure that django.contrib.staticfiles is added to your INSTALLED_APPS

In your settings file. define STATIC_URL for ex.

STATIC_URL = '/static/'

In your Django templates, use the static template tag to create the URL for the given relative path using the configured STATICFILES_STORAGE.

{% load static %}
<img src="{% static 'my_sample/abcxy.jpg' %}" alt="ABC image">
Store your static files in a folder called static in your app. For example my_sample/static/my_sample/abcxy.jpg

----

**18. Explain Django Response lifecycle?**

Whenever a request is made to a web page, Django creates an HttpRequest object that contains metadata about the request. After that Django loads the particular view, passing the HttpRequest as the first argument to the view function. Each view will be returning an HttpResponse object.
On the big picture following steps occur when a request is received by Django:

First of the Django settings.py file is loaded which also contain various middleware classes (MIDDLEWARES)
The middlewares are also executed in the order in which they are mentioned in the MIDDLEWAREST
From here on the request is now moved to the URL Router, who simply gets the URL path from the request and tries to map with our given URL paths in the urls.py. 
As soon as it has mapped, it will call the equivalent view function, from where an equivalent response is generated
The response also passes through the response middlewares and send back to the client/browser.

----

**19. What databases are supported by Django?**

PostgreSQL and MySQL, SQLite and Oracle. Apart from these, Django also supports databases such as ODBC, Microsoft SQL Server, IBM DB2, SAP SQL Anywhere, and Firebird using third-party packages. Note: Officially Django doesn’t support any no-SQL databases.

----

**20. What's the use of a session framework?**

Using the session framework, you can easily store and retrieve arbitrary data based on the pre-site-visitors. It stores data on the server-side and takes care of the process of sending and receiving cookies. These cookies just consist of a session ID, not the actual data itself unless you explicitly use a cookie-based backend.

----

**21. What’s the use of Middleware in Django?**

Middleware is something that executes between the request and response. In simple words, you can say it acts as a bridge between the request and response. Similarly In Django when a request is made it moves through middlewares to views and data is passed through middleware as a response. 

----

**22. What is context in the Django?**

Context is a dictionary mapping template variable name given to Python objects in Django. This is the general name, but you can give any other name of your choice if you want.

----

**23. What is django.shortcuts.render function?**

When a view function returns a webpage as HttpResponse instead of a simple string, we use render(). Render function is a shortcut function that lets the developer easily pass the data dictionary with the template. This function then combines the template with a data dictionary via templating engine. Finally, this render() returns as HttpResponse with the rendered text, which is the data returned by models. Thus, Django render() bypasses most of the developer’s work and lets him use different template engines.
The basic syntax:
render(request, template_name, context=None, content_type=None, status=None, using=None)
The request is the parameter that generates the response. The template name is the HTML template used, whereas the context is a dict of the data passed on the page from the python. You can also specify the content type, the status of the data you passed, and the render you are returning.

----

**24. What’s the significance of the settings.py file?**

As the name suggests this file stores the configurations or settings of our Django project, like database configuration, backend engines, middlewares, installed applications, main URL configurations, static file addresses, templating engines, main URL configurations, security keys, allowed hosts, and much more.

----

**25. How to view all items in the Model?**

ModelName.objects.all()

----

**26. How to filter items in the Model?**

ModelName.objects.filter(field_name=”term”)

----

**27. How to use file-based sessions?**

To use the same, you need to set the SESSION_ENGINE settings to "django.contrib.sessions.backends.file"

----

**28. What is mixin?**

Mixin is a type of multiple inheritances wherein you can combine behaviors and attributes of more than one parent class. It provides us with an excellent way to reuse code from multiple classes. One drawback of using these mixins is that it becomes difficult to analyze what a class is doing and which methods to override in case of its code being too scattered between multiple classes.

----

**29. What is Django Field Class?**

'Field' refers to an abstract class that represents a column in the database table. 
The Field class is just a subclass of RegisterLookupMixin. In Django, these fields are used to create database tables (db_types()) which are used to map Python types to the database using get_prep_value() and the other way round using from_db_value() method. Therefore, fields are fundamental pieces in different Django APIs such as models and querysets.

----

**30. Why is permanent redirection not a good option?**

Permanent redirection is used only when you don’t want to lead visitors to the old URLs. The response of the permanent redirections is cached by the browser so when you try to redirect to something else it will cause issues. Since this is a browser-side operation if your user wants to move to a new page it will load the same page.

----

**31. Difference between Django OneToOneField and ForeignKey Field?**

Both of them are of the most common types of fields used in Django. The only difference between these two is that ForeignKey field consists of on_delete option along with a model’s class because it’s used for many-to-one relationships while on the other hand, the OneToOneField, only carries out a one-to-one relationship and requires only the model’s class.

----

**32. How can you combine multiple QuerySets in a View?**

Initially, Concatenating QuerySets into lists is believed to be the easiest approach. Here’s an example of how to do that:
from itertools import chain
result_list = list(chain(model1_list, model2_list, model3_list))

----

**33. How to get a particular item in the Model?**

ModelName.objects.get(id=”term”)
Note: If there are no results that match the query, get() will raise a DoesNotExist exception. If more than one item matches the given get() query. In this case, it’ll raise MultipleObjectsReturned, which is also an attribute of the model class itself.

----

**34. How to obtain the SQL query from the queryset?**

print(queryset.query)

----

**35. What are the ways to customize the functionality of the Django admin interface?**

There are multiple ways to customize the functionality of the Django admin interface. You can piggyback on top of an add/change form that’s automatically generated by Django, you can add JavaScript modules using the js parameter. This parameter is basically a list of URLs that point to the JavaScript modules that are to be included in your project within a script tag. You can also write views for the admin if you want.

----

**36. Difference between select_related and prefetch_related?**

Though both the functions are used to fetch the related fields on a model but their functioning is bit different from each other. In simple words, select_related uses a foreign key relationship, i.e. using join on the query itself while on the prefetch_related there is a separate lookup and the joining on the python side. Let’s try to illustrate this via an example:

from django.db import models
class Country(models.Model):
    country_name = models.CharField(max_length=5)
class State(models.Model):
    state_name = models.CharField(max_length=5)
    country = model.ForeignKey(Country)
>> states = State.objects.select_related(‘country’).all()
>> for state in states:
…   print(state.state_name)

```sql
SELECT state_id, state_name, country_name FROM State INNER JOIN Country ON (State.country_id = Country.id)
```
>> country = Country.objects.prefetch_related(‘state’).get(id=1)
>> for state in country.state.all():
…   print(state.state_name)
```Query Executed
SELECT id, country_name FROM country WHERE id=1;
SELECT state_id, state_name WHERE State WHERE country_id IN (1);
```

----

**Explain Q objects in Django ORM?**

Q objects are used to write complex queries, as in filter() functions just `AND` the conditions while if you want to `OR` the conditions you can use Q objects. Let’s see an example:

```python
from django.db import models
from django.db.models import Q
>> objects = Models.objects.get(
   Q(tag__startswith='Human'),
   Q(category=’Eyes’) | Q(category=’Nose’)
)
```

```sql
SELECT * FROM Model WHERE tag LIKE ‘Human%’ AND (category=’Eyes’ OR category=’Nose’)
```

----

**What are Django exceptions?**

In addition to the standard Python exceptions, Django raises of its own exceptions.List of the exceptions
by Django (https://docs.djangoproject.com/en/3.1/ref/exceptions/)
 
*Important Resources:*
- Django Projects
- Node.js vs Django
- Flask Vs Django

----

**Which of these exceptions are related to the MyModel.objects.get(id=’123’)?**


- Http404
- DatabaseError
- MyModel.DoesNotExist
- IntegrityError

----

**Which of these databases are not by default supported by Django?**

- Postgres
- Mysql
- Sqlite
- Mongodb

----

**Which file is responsible for the configurations of the Django applications?**

- settings.py
- manage.py
- wsgi.py
- app.py

----

**Django is based on which architecture?**

- MVT
- MVC
- MVTT
- MVP

----

**Which is the default port for the Django development server?**

- 8080
- 8081
- 8000
- 9000

----

**What is the use of the post_delete signal in Django?**

- Sent before a model’s save() method is called
- Sent after a model’s save() method is called
- Sent before a model’s delete() method is called
- Sent after a model’s delete() method is called

----

**Django is written in which programming language?**

- PHP
- Python
- Java
- C++

# https://www.interviewbit.com/django-interview-questions/

# https://quescol.com/interview-preparation/python-coding-question

**Write a program to reverse an integer in Python?**

```python
#!/usr/bin/python3 // run with system Python
#!/usr/bin/env python3 // run with dev version
# -*- coding: utf-8 -*-

def reverse_integer(num):
    reversed_num = 0
    is_negative = False

    if num < 0:
        is_negative = True
        num *= -1

    while num > 0:
        remainder = num % 10
        reversed_num = (reversed_num * 10) + remainder
        num //= 10

    if is_negative:
        reversed_num *= -1

    return reversed_num

def main():
    num = 12345
    reversed_num = reverse_integer(num)
    print(f"The reversed number of {num} is {reversed_num}")

if __name__ == '__main__':
    main()
```

----

**Write a program in Python to check whether an integer is armstrong number or not?**

```python
#!/usr/bin/python3 // run with system Python
#!/usr/bin/env python3 // run with dev version
# -*- coding: utf-8 -*-

def is_armstrong(number):
    # determine the number of digits
    num_of_digits = len(str(number))
    # initialize the sum variable to 0
    sum = 0
    # loop through each digit and raise it to the power of the number of digits and add it to the sum
    for digit in str(number):
        sum += int(digit) ** num_of_digits
    # check if the sum is equal to the original number
    if sum == number:
        return True
    else:
        return False

def main():
    print(is_armstrong(153)) # True
    print(is_armstrong(371)) # True
    print(is_armstrong(9474)) # True
    print(is_armstrong(9475)) # False

if __name__ == '__main__':
    main()
```

----

**Write a program in Python to print the Fibonacci series using iterative method?**

```python
def fibonacci(n):
    a, b = 0, 1
    for i in range(n):
        print(a)
        a, b = b, a + b

# test the function
n_terms = 10
print(f"The first {n_terms} terms of Fibonacci series are:")
fibonacci(n_terms)
```

----

**Write a program in Python to print the Fibonacci series using recursive method?**

```python
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return (fibonacci(n-1) + fibonacci(n-2))

n_terms = int(input("Enter the number of terms for Fibonacci series: "))

if n_terms <= 0:
    print("Please enter a positive integer.")
else:
    print("Fibonacci series:")
    for i in range(n_terms):
        print(fibonacci(i), end=" ")
```

----

**Write a program in Python to check whether a number is palindrome or not using iterative method?**

```python
def is_palindrome(num):
    temp = num
    reverse_num = 0
    
    while num > 0:
        digit = num % 10
        reverse_num = (reverse_num * 10) + digit
        num = num // 10
    
    if temp == reverse_num:
        return True
    else:
        return False

# example usage
print(is_palindrome(12321))  # True
print(is_palindrome(12345))  # False
```

----

**Write a program in Python to check whether a number is palindrome or not using recursive method?**

```python
def is_palindrome(num):
    if len(str(num)) <= 1:
        return True
    else:
        if str(num)[0] == str(num)[-1]:
            return is_palindrome(str(num)[1:-1])
        else:
            return False
 
num = int(input("Enter a number: "))
if is_palindrome(num):
    print(num, "is a palindrome number")
else:
    print(num, "is not a palindrome number")
```

----

**Write a program in Python to find greatest among three integers?**

```python
a = int(input("Enter the first number: "))
b = int(input("Enter the second number: "))
c = int(input("Enter the third number: "))

if a > b and a > c:
    print("The greatest number is:", a)
elif b > a and b > c:
    print("The greatest number is:", b)
else:
    print("The greatest number is:", c)
```

----

**Write a program in Python to check if a number is binary?**

```python
def is_binary(num):
    for digit in str(num):
        if digit != '0' and digit != '1':
            return False
    return True

# example usage
print(is_binary(101010)) # True
print(is_binary(12345)) # False
```

----

**Write a program in Python to find sum of digits of a number using recursion?**

```python
def sum_of_digits(n):
    if n == 0:
        return 0
    else:
        return (n % 10) + sum_of_digits(n // 10)

num = int(input("Enter a number: "))
print("Sum of digits of", num, "is", sum_of_digits(num))
```

----

**Write a program in Python to swap two numbers without using third variable?**

```python
# program to swap two numbers without using third variable

a = 5
b = 10

print("Before swapping: a =", a, "b =", b)

# swapping
a = a + b
b = a - b
a = a - b

print("After swapping: a =", a, "b =", b)
```

----

**Write a program in Python to swap two numbers using third variable?**

```python
# take input from the user
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))

# print the values before swapping
print("Before swapping - num1 =", num1, ", num2 =", num2)

# swap the numbers using a third variable
temp = num1
num1 = num2
num2 = temp

# print the values after swapping
print("After swapping - num1 =", num1, ", num2 =", num2)
```

----

**Write a program in Python to find prime factors of a given integer?**

```python
def is_prime(num):
    """
    Function to check if a number is prime or not.
    """
    if num < 2:
        return False
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            return False
    return True

def prime_factors(num):
    """
    Function to find the prime factors of a number.
    """
    factors = []
    i = 2
    while num > 1:
        if num % i == 0:
            if is_prime(i):
                factors.append(i)
                num = num / i
            else:
                i += 1
        else:
            i += 1
    return factors

# Take input from the user
num = int(input("Enter a number: "))

# Find the prime factors of the number
factors = prime_factors(num)

# Print the prime factors
if not factors:
    print(f"{num} has no prime factors.")
else:
    print(f"The prime factors of {num} are:", end=" ")
    for factor in factors:
        print(factor, end=" ")

```

**Write a program in Python to add two integer without using arithmetic operator?**

```python
def add_without_arithmetic(a, b):
    while b != 0:
        # carry contains common set bits of a and b
        carry = a & b

        # sum of bits of a and b where at least one of the bits is not set
        a = a ^ b

        # carry is shifted by one so that adding it to a gives the required sum
        b = carry << 1

    return a
```

----

**Write a program in Python to find given number is perfect or not?**

```python
def is_perfect(num):
    sum_divisors = 0
    for i in range(1, num):
        if num % i == 0:
            sum_divisors += i
    return sum_divisors == num

num = int(input("Enter a number: "))
if is_perfect(num):
    print(num, "is a perfect number")
else:
    print(num, "is not a perfect number")
```

----

**Python Program to find the Average of numbers with explanations?**

```python
n = int(input("Enter the number of elements: "))
num_list = []

# take input from user and store it in the list
for i in range(n):
    num = int(input("Enter element {}: ".format(i+1)))
    num_list.append(num)

# calculate the sum of all the elements in the list
sum_of_elements = sum(num_list)

# calculate the average
average = sum_of_elements/n

print("Average of numbers is: ", round(average, 2))
```

----

**Python Program to calculate factorial using iterative method?**

```python
def factorial(n):
    fact = 1
    for i in range(1, n+1):
        fact *= i
    return fact

# example usage
n = 5
print("Factorial of", n, "is", factorial(n))
```

----

**Python Program to calculate factorial using recursion?**

```python
def factorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial(n-1)

num = int(input("Enter a number: "))
if num < 0:
    print("Factorial of negative number doesn't exist.")
else:
    print(f"Factorial of {num} is {factorial(num)}")
```

----

**Python Program to check a given number is even or odd?**

```python
num = int(input("Enter a number: "))
if num % 2 == 0:
    print(num, "is even")
else:
    print(num, "is odd")
```

----

**Python program to print first n Prime Number with explanation?**

```python
n = int(input("Enter the value of n: "))

# loop through numbers from 2 to n+1
for i in range(2, n+1):
    is_prime = True
    
    # loop through numbers from 2 to i-1
    for j in range(2, i):
        if i % j == 0:
            is_prime = False
            break
    
    if is_prime:
        print(i)
```

----

**on Program to print Prime Number in a given range?**

```python
lower = int(input("Enter lower range: "))
upper = int(input("Enter upper range: "))

print("Prime numbers between", lower, "and", upper, "are:")

for num in range(lower, upper + 1):
    # prime numbers are greater than 1
    if num > 1:
        for i in range(2, num):
            if (num % i) == 0:
                break
        else:
            print(num)
```

----

**Python Program to find Smallest number among three?**

```python
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
num3 = float(input("Enter third number: "))

if num1 <= num2 and num1 <= num3:
    smallest = num1
elif num2 <= num1 and num2 <= num3:
    smallest = num2
else:
    smallest = num3

print("The smallest number is:", smallest)
```

----

**Python program to calculate the power using the POW method?**

```python
base = 2
exponent = 3
result = pow(base, exponent)
print("The result of {0} raised to the power of {1} is {2}".format(base, exponent, result))
```

----

**Python Program to calculate the power without using POW function.(using for loop)?**

```python
def power(base, exponent):
    result = 1
    for i in range(exponent):
        result *= base
    return result

# Example usage:
print(power(2, 3)) # Output: 8
print(power(5, 4)) # Output: 625
```

----

**Python Program to calculate the power without using POW function.(using while loop)?**

```python
def power(base, exponent):
    result = 1
    while exponent > 0:
        result *= base
        exponent -= 1
    return result
```

----

**Python Program to calculate the square of a given number?**

```python
num = float(input("Enter a number: "))
square = num ** 2
print("The square of", num, "is", square)
```

----

**Python Program to calculate the cube of a given number?**

```python
def cube(num):
    """
    This function takes a number as input and returns the cube of the number.
    """
    return num ** 3

# Example usage
print(cube(2))  # Output: 8
print(cube(5))  # Output: 125
```

----

**Python Program to calculate the square root of a given number?**

```python
import math

num = float(input("Enter a number: "))

if num < 0:
    print("Please enter a positive number.")
else:
    sqrt = math.sqrt(num)
    print("The square root of", num, "is", sqrt)
```

----

**Python program to calculate LCM of given two numbers?**

```python
def lcm(a, b):
    # find the greater number
    if a > b:
        greater = a
    else:
        greater = b

    while True:
        if greater % a == 0 and greater % b == 0:
            lcm = greater
            break
        greater += 1

    return lcm

# Example usage
print(lcm(4, 6)) # Output: 12
```

----

**Python Program to find GCD or HCF of two numbers?**

```python
def gcd(a, b):
    if b == 0:
        return a
    else:
        return gcd(b, a % b)

# Example usage
print(gcd(48, 18)) # Output: 6
```

----

**Python Program to find GCD of two numbers using recursion?**

```python

```

----

**Python Program to Convert Decimal Number into Binary?**

```python
def decimal_to_binary(decimal):
    binary = ""
    while decimal > 0:
        remainder = decimal % 2
        binary = str(remainder) + binary
        decimal = decimal // 2
    return binary
```

----

**Python Program to convert Decimal number to Octal number?**

```python
def decimal_to_octal(decimal):
    octal = ""
    while decimal > 0:
        remainder = decimal % 8
        octal = str(remainder) + octal
        decimal = decimal // 8
    return octal
```

----

**Python Program to check the given year is a leap year or not?**

```python
def is_leap_year(year):
    if year % 4 == 0:
        if year % 100 == 0:
            if year % 400 == 0:
                return True
            else:
                return False
        else:
            return True
    else:
        return False
```

----

**Python Program to convert Celsius to Fahrenheit?**

```python
def celsius_to_fahrenheit(celsius):
    # Celsius to Fahrenheit formula: F = (C * 9/5) + 32
    fahrenheit = (celsius * 9/5) + 32
    return fahrenheit
```

----

**Python Program to convert Fahrenheit to Celsius?**

```python
def fahrenheit_to_celsius(fahrenheit):
    # Celsius to Fahrenheit formula: C = (F - 32) * 5/9
    celsius = (fahrenheit - 32) * 5/9
    return celsius
```

----

**Python program to calculate Simple Interest with explanation?**

```python
def calculate_simple_interest(principal, rate, time):
    # Simple Interest formula: SI = P * R * T / 100
    simple_interest = (principal * rate * time) / 100
    return simple_interest
```

----

**Python Coding Questions on String**

1. Write a Python program to find the first non-repeating character in a string.
1. Write a Python program to count the number of words in a sentence.
1. Write a Python program to check if a string contains only digits.
1. Write a Python program to count the occurrences of each word in a sentence.
1. Write a Python program to find the most frequent word in a sentence.
1. Write a Python program to reverse the words in a sentence.
1. Write a Python program to check if a string is a palindrome.
1. Write a Python program to check if a string is an anagram of another string.
1. Write a Python program to remove all the vowels from a string.
1. Write a Python program to replace all occurrences of a substring with another substring in a given string.


----

**Python program to remove given character from String?**

```python
def remove_char(s, char):
    # Replace all occurrences of the character with an empty string
    return s.replace(char, '')
```

----

**Program to count occurrence of a given characters in string?**

```python
def count_char(s, char):
    count = 0
    for c in s:
        if c == char:
            count += 1
    return count
```

----

**Python Program to check if two Strings are Anagram?**

```python
def are_anagrams(s1, s2):
    # Remove any non-alphanumeric characters and convert to lowercase
    s1 = ''.join(e for e in s1 if e.isalnum()).lower()
    s2 = ''.join(e for e in s2 if e.isalnum()).lower()
    # Check if the sorted strings are equal
    return sorted(s1) == sorted(s2)
```

----

**Python program to check a String is palindrome or not?**

```python
def is_palindrome(s):
    # Remove any non-alphanumeric characters and convert to lowercase
    s = ''.join(e for e in s if e.isalnum()).lower()
    # Check if the string is equal to its reverse
    return s == s[::-1]
```

**Python program to check given character is vowel or consonant?**

```python
def check_vowel(char):
    vowels = ['a', 'e', 'i', 'o', 'u']
    if char.lower() in vowels:
        print("The character is a vowel.")
    else:
        print("The character is a consonant.")
```

----

**Python program to check given character is digit or not?**

```python
def check_digit(char):
    if char.isdigit():
        print("The character is a digit.")
    else:
        print("The character is not a digit.")
```

----

**Python program to check given character is digit or not using isdigit() method?**

```python
def check_digit(char):
    if char.isdigit():
        print("The character is a digit.")
    else:
        print("The character is not a digit.")
```

----

**Python program to replace the string space with a given character?**

```python
def replace_space(string, char):
    # initialize an empty string to store the result
    result = ''
    
    # loop through each character in the string
    for i in range(len(string)):
        # if the character is a space, replace it with the given character
        if string[i] == ' ':
            result += char
        else:
            result += string[i]
    
    # return the result string
    return result
```

----

**Python program to replace the string space with a given character using replace() method?**

```python
def replace_space(string, char):
    # use the replace() method to replace spaces with the given character
    new_string = string.replace(' ', char)
    
    # return the new string
    return new_string
```

----

**Python program to convert lowercase char to uppercase of string?**

```python
def convert_lowercase(string):
    # initialize an empty string to store the result
    result = ''
    
    # loop through each character in the string
    for char in string:
        # if the character is a lowercase letter, convert it to uppercase
        if char.islower():
            result += char.upper()
        else:
            result += char
    
    # return the result string
    return result
```

----

**Python program to convert lowercase vowel to uppercase in string?**

```python
def convert_vowels(string):
    # define a list of vowels
    vowels = ['a', 'e', 'i', 'o', 'u']
    
    # initialize an empty string to store the result
    result = ''
    
    # loop through each character in the string
    for char in string:
        # if the character is a vowel and lowercase, convert it to uppercase
        if char.lower() in vowels:
            result += char.upper()
        else:
            result += char
    
    # return the result string
    return result
```

----

**Python program to delete vowels in a given string?**

```python
def delete_vowels(string):
    # define a list of vowels
    vowels = ['a', 'e', 'i', 'o', 'u']
    
    # initialize an empty string to store the result
    result = ''
    
    # loop through each character in the string
    for char in string:
        # if the character is not a vowel, add it to the result
        if char.lower() not in vowels:
            result += char
    
    # return the result string
    return result
```

----

**Python program to count Occurrence Of Vowels & Consonants in a String?**

```python
def count_vowels_consonants(string):
    # define lists of vowels and consonants
    vowels = ['a', 'e', 'i', 'o', 'u']
    consonants = ['b', 'c', 'd', 'f', 'g', 'h', 'j', 'k', 'l', 'm', 'n', 'p', 'q', 'r', 's', 't', 'v', 'w', 'x', 'y', 'z']
    
    # initialize counters for vowels and consonants
    vowel_count = 0
    consonant_count = 0
    
    # loop through each character in the string and count its occurrence
    for char in string.lower():
        if char in vowels:
            vowel_count += 1
        elif char in consonants:
            consonant_count += 1
    
    # return the count of vowels and consonants as a tuple
    return (vowel_count, consonant_count)
```

----

**Python program to print the highest frequency character in a String?**

```python
def highest_frequency_char(string):
    # create a dictionary to store the frequency of each character
    frequency = {}
    
    # loop through each character in the string and count its frequency
    for char in string:
        if char in frequency:
            frequency[char] += 1
        else:
            frequency[char] = 1
    
    # find the character with the highest frequency
    max_frequency = 0
    max_char = ''
    for char, freq in frequency.items():
        if freq > max_frequency:
            max_frequency = freq
            max_char = char
    
    # return the character with the highest frequency
    return max_char
```

----

**Python program to replace first occurrence of vowel With '-' in String?**

```python
def replace_first_vowel(string):
    # create a list of vowels
    vowels = ['a', 'e', 'i', 'o', 'u']
    
    # loop through each character in the string
    for i in range(len(string)):
        # if the character is a vowel, replace it with '-'
        if string[i].lower() in vowels:
            string = string[:i] + '-' + string[i+1:]
            break
    
    # return the resulting string
    return string
```

----

**Python program to count alphabets, digits and special characters?**

```python
def remove_whitespace(input_string):
    new_string = ""
    for char in input_string:
        if char == " ":
            new_string = new_string + char.replace( " ","" )
        else:
            new_string = new_string + char

    return new_string
```

----

**Python program to separate characters in a given string?**

```python
def separate_string(input_string):
    new_string = ""
    for char in input_string:
        new_string = new_string + f"{char} "

    return new_string
```

----

**Python program to remove blank space from string?**

```python

```

----

**Python program to concatenate two strings using join() method?**

```python
def concat_strings(str1, str2):
    # use the join() method to concatenate the two strings
    result = ''.join([str1, str2])
    
    # return the concatenated string
    return result
```

----

**Python program to concatenate two strings without using join() method?**

```python
def concat_strings(str1, str2):
    # create an empty string to store the result
    result = ""
    
    # loop through each character in the first string and add it to the result string
    for char in str1:
        result += char
    
    # loop through each character in the second string and add it to the result string
    for char in str2:
        result += char
    
    # return the result string
    return result
```

----

**Python program to remove repeated character from string?**

```python
def remove_repeated(string):
    # create an empty set to store unique characters
    unique_chars = set()
    
    # create an empty string to store the result
    result = ""
    
    # loop through each character in the string
    for char in string:
        # if the character is not already in the set, add it to the set and the result string
        if char not in unique_chars:
            unique_chars.add(char)
            result += char
    
    # return the result string
    return result
```

----

**Python program to calculate sum of integers in string?**

```python
def sum_of_integers(string):
    # initialize a sum variable to keep track of the total sum
    total_sum = 0
    
    # loop through each character in the string
    for char in string:
        # if the character is a digit, add its integer value to the total sum
        if char.isdigit():
            total_sum += int(char)
    
    # return the total sum
    return total_sum

```

----

**Python program to print all non repeating character in string?**

```python
def print_non_repeating(string):
    # create an empty dictionary to count the frequency of each character
    char_counts = {}
    
    # loop through each character in the string and count its frequency
    for char in string:
        if char in char_counts:
            char_counts[char] += 1
        else:
            char_counts[char] = 1
    
    # loop through each character in the string and print it if it appears only once
    for char in string:
        if char_counts[char] == 1:
            print(char)
```

----

**Python program to copy one string to another string?**

```python
def copy_string(source, destination):
    # loop through each character in the source string
    for i in range(len(source)):
        # copy the character to the corresponding position in the destination string
        destination[i] = source[i]
```

----

**Python Program to sort characters of string in ascending order?**

```python
def sort_string_asc(string):
    # convert the string to a list of characters
    chars = list(string)
    
    # sort the characters in ascending order
    chars.sort()
    
    # convert the sorted list of characters back to a string
    sorted_string = "".join(chars)
    
    # return the sorted string
    return sorted_string
```

----

**Python Program to sort character of string in descending order?**

```python
def sort_string_desc(string):
    # convert the string to a list of characters
    chars = list(string)
    
    # sort the characters in descending order
    chars.sort(reverse=True)
    
    # convert the sorted list of characters back to a string
    sorted_string = "".join(chars)
    
    # return the sorted string
    return sorted_string
```

----

**Write a program in Python for, In array 1-100 numbers are stored, one number is missing how do you find it?**

```python
def find_missing(arr):
    # create a set of all numbers from 1 to 100
    all_nums = set(range(1, 101))
    
    # create a set of numbers in the array
    arr_nums = set(arr)
    
    # find the difference between the two sets
    missing_nums = all_nums - arr_nums
    
    # return the missing number
    return missing_nums.pop()
```

----

**Write a program in Python for, In a array 1-100 multiple numbers are duplicates, how do you find it?**

```python
def find_duplicates(arr):
    # create an empty dictionary to store counts of each number
    counts = {}
    
    # loop through the array and count occurrences of each number
    for num in arr:
        if num in counts:
            counts[num] += 1
        else:
            counts[num] = 1
    
    # loop through the dictionary and print numbers that appear more than once
    for num, count in counts.items():
        if count > 1:
            print(num, "appears", count, "times")
```

----

**Write a program in Python for, How to find all pairs in array of integers whose sum is equal to given number?**

```python
def find_pairs(arr, target):
    # initialize an empty dictionary to store pairs
    pairs = {}
    
    # loop through the array and check for pairs that add up to the target
    for i in range(len(arr)):
        for j in range(i + 1, len(arr)):
            if arr[i] + arr[j] == target:
                pairs[(arr[i], arr[j])] = True
    
    # print the pairs that add up to the target
    if len(pairs) == 0:
        print("No pairs found.")
    else:
        for pair in pairs.keys():
            print(pair)
my_array = [2, 4, 6, 8, 10]
target_sum = 12
find_pairs(my_array, target_sum) #
```

----

**Write a program in Python for, How to compare two array is equal in size or not?**

```python
def compare_arrays(arr1, arr2):
    # check if the length of both arrays is equal
    if len(arr1) == len(arr2):
        print("The two arrays are equal in size")
    else:
        print("The two arrays are not equal in size")
```

----

**Write a program in Python to find largest and smallest number in array?**

```python
def find_min_max(arr):
    # initialize variables to hold the minimum and maximum numbers
    minimum = maximum = arr[0]
    
    # loop through the array and update the minimum and maximum variables
    for i in range(1, len(arr)):
        if arr[i] < minimum:
            minimum = arr[i]
        elif arr[i] > maximum:
            maximum = arr[i]
    
    # return the minimum and maximum numbers
    return (minimum, maximum)
```

----

**Write a program in Python to find second highest number in an integer array?**

```python
def second_highest(arr):
    # initialize variables to hold the highest and second highest numbers
    highest = arr[0]
    second_highest = float('-inf')
    
    # loop through the array and update the highest and second highest variables
    for i in range(1, len(arr)):
        if arr[i] > highest:
            second_highest = highest
            highest = arr[i]
        elif arr[i] > second_highest and arr[i] != highest:
            second_highest = arr[i]
    
    # return the second highest number
    return second_highest
```

----

**Write a program in Python to find top two maximum number in array?**

```python
def top_two_max_numbers(arr):
    # initialize variables to hold the first and second largest numbers
    largest = arr[0]
    second_largest = arr[1] if arr[1] < arr[0] else arr[1]
    
    # loop through the array and update the largest and second largest variables
    for i in range(2, len(arr)):
        if arr[i] > largest:
            second_largest = largest
            largest = arr[i]
        elif arr[i] > second_largest:
            second_largest = arr[i]
    
    # return the largest and second largest numbers
    return (largest, second_largest)
```

----

**Write a program in Python to remove duplicate elements form array?**

```python
def remove_duplicates(arr):
    # create an empty list to store unique elements
    unique_list = []
    
    # loop through each element in the array
    for elem in arr:
        # if the element is not already in the unique list, add it
        if elem not in unique_list:
            unique_list.append(elem)
    
    # return the unique list
    return unique_list
```

----

**Python program to find top two maximum number in array?**

```python
def top_two_max(arr):
    max1 = max2 = float('-inf')
    for i in arr:
        if i > max1:
            max2 = max1
            max1 = i
        elif i > max2:
            max2 = i
    return max1, max2

# Example usage
arr = [5, 10, 3, 8, 20, 12]
max1, max2 = top_two_max(arr)
print("Top two maximum numbers in array:", max1, max2)
```

----

**Python program to print array in reverse Order?**

```python
def print_reverse(arr):
    for i in range(len(arr) - 1, -1, -1):
        print(arr[i], end=' ')

# Example usage
arr = [1, 2, 3, 4, 5]
print("Original array:", arr)
print("Array printed in reverse order:", end=' ')
print_reverse(arr)
```

----

**Python program to reverse an Array in two ways?**

```python
def reverse_array(arr):
    # Method 1: Using a loop and swapping the first and last elements
    start_index = 0
    end_index = len(arr) - 1
    while end_index > start_index:
        arr[start_index], arr[end_index] = arr[end_index], arr[start_index]
        start_index += 1
        end_index -= 1
    
    # Method 2: Using slicing to reverse the array
    # arr = arr[::-1]  # Alternative method using slicing
    
    return arr

# Example usage
arr = [1, 2, 3, 4, 5]
print("Original array:", arr)
print("Reversed array using method 1:", reverse_array(arr))
print("Reversed array using method 2:", reverse_array(arr[::-1]))
```

----

**Python Program to calculate length of an array?**

```python
def array_length(arr):
    return len(arr)

# Example usage
arr = [1, 2, 3, 4, 5]
print("Length of array:", array_length(arr))
```

----

**Python program to insert an element at end of an Array?**

```python
def insert_end(arr, elem):
    arr.append(elem)
    return arr

# Example usage
arr = [1, 2, 3, 4, 5]
print("Original array:", arr)
arr = insert_end(arr, 6)
print("Array after inserting element 6 at end:", arr)
```

----

**Python program to insert element at a given location in Array?**

```python
def insert_element(arr, elem, index):
    arr.insert(index, elem)
    return arr

# Example usage
arr = [1, 2, 3, 4, 5]
print("Original array:", arr)
arr = insert_element(arr, 6, 2)
print("Array after inserting element 6 at index 2:", arr)
```

----

**Python Program to delete element at end of Array?**

```python
def delete_end(arr):
    arr.pop()
    return arr

# Example usage
arr = [1, 2, 3, 4, 5]
print("Original array:", arr)
arr = delete_end(arr)
print("Array after deleting element at end:", arr)
```

----

**Python Program to delete given element from Array?**

```python
def delete_element(arr, elem):
    arr = [x for x in arr if x != elem]
    return arr

# Example usage
arr = [1, 2, 3, 4, 5, 3]
print("Original array:", arr)
arr = delete_element(arr, 3)
print("Array after deleting all occurrences of 3:", arr)
```

----

**Python Program to delete element from array at given index?**

```python
def delete_element(arr, index):
    if index < 0 or index >= len(arr):
        print("Invalid index!")
        return arr
    else:
        del arr[index]
        return arr

# Example usage
arr = [1, 2, 3, 4, 5]
print("Original array:", arr)
arr = delete_element(arr, 2)
print("Array after deleting element at index 2:", arr)
```

----

**Python Program to find sum of array elements?**

```python
def sum_of_array(arr):
    sum = 0
    for i in arr:
        sum += i
    return sum

# Example usage
arr = [1, 2, 3, 4, 5]
print("The sum of the array elements is:", sum_of_array(arr))
```

----

**Python Program to print all even numbers in array?**

```python
def print_even_numbers(arr):
    for i in arr:
        if i % 2 == 0:
            print(i)

# Example usage
arr = [1, 2, 3, 4, 5, 6, 7, 8, 9]
print("The even numbers in the array are:")
print_even_numbers(arr)
```

----

**Python Program to print all odd numbers in array?**

```python
def print_odd_numbers(arr):
    for i in arr:
        if i % 2 != 0:
            print(i)

# Example usage
arr = [1, 2, 3, 4, 5, 6, 7, 8, 9]
print("The odd numbers in the array are:")
print_odd_numbers(arr)

```

----

**Python program to perform left rotation of array elements by two positions?**

```python
def left_rotate(arr):
    n = len(arr)
    temp = arr[2:n] + arr[0:2]
    return temp

# Example usage
arr = [1, 2, 3, 4, 5]
rotated_arr = left_rotate(arr)
print("The original array is", arr)
print("The rotated array is", rotated_arr)
```

----

**Python program to perform right rotation in array by 2 positions?**

```python
def right_rotate(arr):
    n = len(arr)
    temp = arr[n-2:n] + arr[:n-2]
    return temp

# Example usage
arr = [1, 2, 3, 4, 5]
rotated_arr = right_rotate(arr)
print("The original array is", arr)
print("The rotated array is", rotated_arr)
```

----

**Python Program to merge two arrays?**

```python
def merge_arrays(arr1, arr2):
    merged_arr = arr1 + arr2
    return sorted(merged_arr)

# Example usage
arr1 = [1, 2, 3, 4, 5]
arr2 = [6, 7, 8, 9, 10]
merged = merge_arrays(arr1, arr2)
print("The merged array is", merged)
```

----

**Python Program to find highest frequency element in array?**

```python
from collections import Counter

def find_highest_frequency(arr):
    freq_count = Counter(arr)
    return freq_count.most_common(1)[0][0]

# Example usage
arr = [1, 2, 3, 4, 2, 2, 3, 4, 4, 4]
highest_freq = find_highest_frequency(arr)
print("The highest frequency element in", arr, "is", highest_freq)
```

----

**Python Program to find sum of digit of number using recursion?**

```python
def digit_sum(n):
    if n == 0:
        return 0
    else:
        return (n % 10) + digit_sum(n // 10)

# Example usage
num = 12345
sum = digit_sum(num)
print("The sum of the digits of", num, "is", sum)
```

----

**Python Program to Create and Traverse Singly linked list?**

```python
# Define a Node class to represent a single node in the linked list
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

# Define a LinkedList class to represent the entire linked list
class LinkedList:
    def __init__(self):
        self.head = None

    # Add a new node to the end of the list
    def append(self, data):
        new_node = Node(data)
        if self.head is None:
            self.head = new_node
        else:
            current_node = self.head
            while current_node.next is not None:
                current_node = current_node.next
            current_node.next = new_node

    # Traverse the list and print out each node's data
    def traverse(self):
        current_node = self.head
        while current_node is not None:
            print(current_node.data, end=" ")
            current_node = current_node.next

# Example usage
linked_list = LinkedList()
linked_list.append(1)
linked_list.append(2)
linked_list.append(3)
linked_list.append(4)
linked_list.append(5)
linked_list.traverse()
```

----

**Python program to insert a node in linked list?**

```python
class Node:
    def __init__(self, data=None):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None

    def insert_at_beginning(self, data):
        new_node = Node(data)
        new_node.next = self.head
        self.head = new_node

    def print_list(self):
        current_node = self.head
        while current_node:
            print(current_node.data, end=' ')
            current_node = current_node.next
        print()

# Example usage
my_list = LinkedList()
my_list.insert_at_beginning(3)
my_list.insert_at_beginning(5)
my_list.insert_at_beginning(7)
my_list.print_list() # Output: 7 5 3
```

----

**n):**

```python
    if n <= 1:
        return False
    for i in range(2, int(n**0.5)+1):
        if n % i == 0:
            return False
    return True

# Example usage
n = 17
if is_prime(n):
    print(f"{n} is a prime number")
else:
    print(f"{n} is not a prime number")
```

----

**Write a program in Python to reverse a singly linked list?**

```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None

    def add_node(self, data):
        new_node = Node(data)
        if self.head is None:
            self.head = new_node
        else:
            current = self.head
            while current.next:
                current = current.next
            current.next = new_node

    def reverse_list(self):
        prev_node = None
        current_node = self.head
        while current_node:
            next_node = current_node.next
            current_node.next = prev_node
            prev_node = current_node
            current_node = next_node
        self.head = prev_node

    def print_list(self):
        current = self.head
        while current:
            print(current.data, end=' ')
            current = current.next
        print()

# Example usage
linked_list = LinkedList()
linked_list.add_node(1)
linked_list.add_node(2)
linked_list.add_node(3)
linked_list.add_node(4)
print("Original linked list:")
linked_list.print_list()
print("Reversed linked list:")
linked_list.reverse_list()
linked_list.print_list()
```

----

**n):**

```python
    """
    Checks if a given number is prime or not
    """
    if n <= 1:
        return False
    elif n <= 3:
        return True
    elif n % 2 == 0 or n % 3 == 0:
        return False
    i = 5
    while i * i <= n:
        if n % i == 0 or n % (i + 2) == 0:
            return False
        i += 6
    return True

# Example usage
print(is_prime(5))   # True
print(is_prime(10))  # False
```

----

**Python Program to search an element in singly linked list?**

```python
class Node:
    """
    Class representing a node in a singly linked list
    """
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    """
    Class representing a singly linked list
    """
    def __init__(self):
        self.head = None

    def add_node(self, data):
        """
        Adds a new node to the linked list
        """
        new_node = Node(data)
        new_node.next = self.head
        self.head = new_node

    def search(self, x):
        """
        Searches for an element in the linked list
        """
        current = self.head
        while current is not None:
            if current.data == x:
                return True
            current = current.next
        return False

# Example usage
my_list = LinkedList()
my_list.add_node(3)
my_list.add_node(7)
my_list.add_node(1)
my_list.add_node(8)

print(my_list.search(1))   # True
print(my_list.search(5))   # False
```

----

**n):**

```python
    """
    Checks if a given number is prime or not
    """
    if n <= 1:
        return False
    elif n <= 3:
        return True
    elif n % 2 == 0 or n % 3 == 0:
        return False
    i = 5
    while i * i <= n:
        if n % i == 0 or n % (i + 2) == 0:
            return False
        i += 6
    return True

# Example usage
print(is_prime(5))   # True
print(is_prime(10))  # False

```

----

**Linked list Deletion in Python: At beginning, End, Given location?**

```python
# In this program, we define a Node class that represents a single node in the linked list, and a LinkedList
# class that contains the methods for appending nodes, printing the list, and deleting nodes at the
# beginning, end, or a given position.

# To delete a node at the beginning of the list, we simply set the head of the list to the next node in
# the list. To delete a node at the end of the list, we iterate over the list until we reach the second
# to last node, and then set its next pointer to None. To delete a node at a given position, we iterate
# over the list until we reach the desired position, and then set the next pointer of the previous node
# to the next pointer of the current node, effectively removing the current node from the list.

# Finally, we use an example usage of the linked list class to create a linked list with five nodes,
# print the list, and then delete a node at the beginning, end, and a given position, printing
# the list after each deletion.
class Node:
    def __init__(self, data=None):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None

    def append(self, data):
        new_node = Node(data)
        if self.head is None:
            self.head = new_node
            return
        last_node = self.head
        while last_node.next:
            last_node = last_node.next
        last_node.next = new_node

    def print_list(self):
        current_node = self.head
        while current_node:
            print(current_node.data, end=" -> ")
            current_node = current_node.next
        print("None")

    def delete_at_beginning(self):
        if self.head is None:
            return
        self.head = self.head.next

    def delete_at_end(self):
        if self.head is None:
            return
        if self.head.next is None:
            self.head = None
            return
        current_node = self.head
        while current_node.next.next:
            current_node = current_node.next
        current_node.next = None

    def delete_at_pos(self, pos):
        if pos < 0 or self.head is None:
            return
        if pos == 0:
            self.head = self.head.next
            return
        current_node = self.head
        previous_node = None
        count = 0
        while current_node and count != pos:
            previous_node = current_node
            current_node = current_node.next
            count += 1
        if current_node:
            previous_node.next = current_node.next

# example usage
linked_list = LinkedList()
linked_list.append(1)
linked_list.append(2)
linked_list.append(3)
linked_list.append(4)
linked_list.append(5)

linked_list.print_list()

# delete node at beginning
linked_list.delete_at_beginning()
linked_list.print_list()

# delete node at end
linked_list.delete_at_end()
linked_list.print_list()

# delete node at position 2
linked_list.delete_at_pos(2)
linked_list.print_list()

```

----

**gram, we define a function called is_prime that takes an integer n as input and returns True if n is a**

```python
# prime number, and False otherwise.

# The function first checks if the input number is less than 2, since 1 and 0 are not prime. If n is greater than or
# equal to 2, it checks all integers from 2 up to the square root of n to see if they divide n evenly. If any of
# these integers divide n evenly, then n is not prime and the function returns False. Otherwise, the function
# returns True since n is prime.

# Finally, we use an example usage of the function to check if the number 17 is prime. If the function returns
# True, we print that 17 is prime, otherwise we print that it's not prime.
def is_prime(n):
    if n < 2:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True

# example usage
n = 17
if is_prime(n):
    print(f"{n} is a prime number")
else:
    print(f"{n} is not a prime number")

```

----

**Write a program in Python to find 3rd element of Linked List from last in single pass?**

```python
# In this program, we define a Node class that represents a single node in the linked list, and a LinkedList class that contains
# the methods for appending nodes, printing the list, and finding the 3rd element from the last.

# To find the 3rd element from the last, we use three pointers: first, second, and third. We first move the third pointer
# to the third node from the beginning. Then we move all three pointers together until the third pointer reaches the end
# of the list. At this point, the second pointer will be pointing to the 3rd element from the end of the list, so we
# return its data.
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None
        
    def append(self, data):
        new_node = Node(data)
        if self.head is None:
            self.head = new_node
            return
        last_node = self.head
        while last_node.next:
            last_node = last_node.next
        last_node.next = new_node
        
    def print_list(self):
        current_node = self.head
        while current_node:
            print(current_node.data)
            current_node = current_node.next
            
    def find_third_last(self):
        first = self.head
        second = self.head
        third = self.head
        
        for i in range(3):
            if third:
                third = third.next
                
        while third:
            first = second
            second = second.next
            third = third.next
            
        return first.data
        
linked_list = LinkedList()
linked_list.append(1)
linked_list.append(2)
linked_list.append(3)
linked_list.append(4)
linked_list.append(5)

linked_list.print_list()

third_last = linked_list.find_third_last()
print("The 3rd element from the last is:", third_last)
```

----

**Write a program to check if a number is a prime number?**

```python
    if num <= 1:
        return False

    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True

# Example usage
num = 17
if is_prime(num):
    print(f"{num} is a prime number")
else:
    print(f"{num} is not a prime number")
```

----

**Write a program in Python to find middle element of a linked list in single pass?**

```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None

    def append(self, data):
        new_node = Node(data)
        if self.head is None:
            self.head = new_node
            return
        last_node = self.head
        while last_node.next:
            last_node = last_node.next
        last_node.next = new_node

    def find_middle_element(self):
        slow_pointer = self.head
        fast_pointer = self.head

        while fast_pointer is not None and fast_pointer.next is not None:
            slow_pointer = slow_pointer.next
            fast_pointer = fast_pointer.next.next

        return slow_pointer.data

# creating linked list
linked_list = LinkedList()
linked_list.append(1)
linked_list.append(2)
linked_list.append(3)
linked_list.append(4)
linked_list.append(5)

# find the middle element
middle_element = linked_list.find_middle_element()

print("Middle element:", middle_element) # Output: 3
```

# https://quescol.com/interview-preparation/python-coding-question
