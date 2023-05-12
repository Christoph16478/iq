# https://www.simplilearn.com/tutorials/cpp-tutorial/cpp-interview-questions 

**What is the difference between C and C++?**

C
C++

C is a procedure-oriented programming language.
C++ is a partially object-oriented programming language.

It follows a top-down approach.
It follows a bottom-up approach.

C doesn’t support function or operator overloading.
C++ supports function as well as function overloading.

C language doesn’t support virtual and friend function
C++ language supports both virtual and friend functions.

C language has 32 keywords.
C++ language contains 52 keywords.

----

**What are classes and objects in C++?**

A class is like a blueprint of an object. It is a user-defined data type with data members and member
functions and is defined with the keyword class.

You define objects as an instance of a class. Once it creates the object, then it can operate on both data members and member functions.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class MyClass { // The class
public: // Access specifier
    int myNum; // Attribute (int variable)
    string myString; // Attribute (string variable)
};

int main()
{
    MyClass myObj; // Create an object of MyClass

    // Access attributes and set values
    myObj.myNum = 15;
    myObj.myString = "Some text";

    // Print attribute values
    cout << myObj.myNum << "\n";
    cout << myObj.myString;
    return 0;
}
```

**What are access modifiers?**

You use access modifiers to define accessibility for the class members. It defines how to access the members of the class outside the class scope.

There are three types of access modifiers:

- Private

```c++
// C++ program to demonstrate private
// access modifier

#include<iostream>
using namespace std;

class Circle
{
	// private data member
	private:
		double radius;
	
	// public member function
	public:
		double compute_area()
		{ // member function can access private
			// data member radius
			return 3.14*radius*radius;
		}
	
};

// main function
int main()
{
	// creating object of the class
	Circle obj;
	
	// trying to access private data member
	// directly outside the class
	obj.radius = 1.5;
	
	cout << "Area is:" << obj.compute_area();
	return 0;
}
```

- Public

```c++
// C++ program to demonstrate public
// access modifier

#include<iostream>
using namespace std;

// class definition
class Circle
{
	public:
		double radius;
		
		double compute_area()
		{
			return 3.14*radius*radius;
		}
	
};

// main function
int main()
{
	Circle obj;
	
	// accessing public datamember outside class
	obj.radius = 5.5;
	
	cout << "Radius is: " << obj.radius << "\n";
	cout << "Area is: " << obj.compute_area();
	return 0;
}
```

- Protected

```c++
// C++ program to demonstrate
// protected access modifier
#include <bits/stdc++.h>
using namespace std;

// base class
class Parent
{
	// protected data members
	protected:
	int id_protected;
	
};

// sub class or derived class from public base class
class Child : public Parent
{
	public:
	void setId(int id)
	{
		
		// Child class is able to access the inherited
		// protected data members of base class
		
		id_protected = id;
		
	}
	
	void displayId()
	{
		cout << "id_protected is: " << id_protected << endl;
	}
};

// main function
int main() {
	
	Child obj1;
	
	// member function of the derived class can
	// access the protected data members of the base class
	
	obj1.setId(81);
	obj1.displayId();
	return 0;
}
```

**Difference between equal to (==) and assignment operator(=)?**

The equal to operator == checks whether two values are equal or not. If equal, then it’s true; otherwise, it will return false.

The assignment operator = allots the value of the right-side expression to the left operand.

**What is the difference between a while loop and a do-while loop?**

while
do-while

The while loop verifies the condition; if it’s true, then it iterates the loop till the condition becomes false.
The do-while loop first iterates the loop body once, then it checks for the condition.

while - Syntax:

```c++
while (condition)
{
	statements  
}
```

do-while - Syntax:   

```c++
do
{
	statements     
}
while(condition);
```

If the condition is false in a while loop, then not a single statement will execute inside the loop.
If the condition in a do-while loop is false, then the body will also execute once.

----

**What is the size of the int data type?**

- 4 bytes (true, int)
- 1 byte
- 8 bytes
- 2 bytes

----

**Which among the following operators cannot be overloaded?**
- -:
- +:
- ?:  operator cannot be overloaded because it is not syntactically possible.
- %:

----

**What among these is used to return the number of characters in the string?**

- Size
- Length
- Both size and length: are used to return the number of characters in the string.
- Name

----

**Discuss the difference between prefix and postfix?**

In prefix (++i), first, it increments the value, and then it assigns the value to the expression.

In postfix (i++), it assigns the value to the expression, and then it increments the variable's value. 

----

**Can you compile a program without the main function?**

Yes, you can compile a program without the main function, but you cannot run or execute the program because the main() function is the entry
point, from where all the execution begins. And without the entry point, then you can execute the program.

----

**What is std in C++?**

- std is a standard class in C++ (true)
- std is a standard file reading header
- std is a standard header file
- std is a standard namespace

----

**What are the four different data types in C++?**

- Primitive/Basic: Char, int, short, float, double, long, bool, etc.
- Derived: Array, pointer, etc.
- Enumeration: Enum
- User-defined: Structure, class, etc.

----

**How is struct different from class?**

Structure
Class

Its members are public by default.
Its members are private by default.

The default access specifiers are public when deriving a struct from a class/struct. 
The default access specifiers are private when deriving a class. 

----

**What do you understand about polymorphism in C++?**

The term polymorphism refers to the presence of multiple forms. Polymorphism usually occurs when there is a hierarchy of classes that are linked by inheritance.
C++ polymorphism means that depending on the type of object that invokes the function, a different function will be executed.

----

**Compare compile time and runtime polymorphism?**

Compile-time Polymorphism
Runtime Polymorphism

The method to be executed is known at compile time. And the call is resolved by the compiler.
The method to be executed is known at run time. The compiler does not resolve the call.

Provides quicker execution because it is known at the compile time.
Provides slower execution because it is known at the run time.

Achieved by operation or function overloading.
Achieved by function overriding. 

Prepare Yourself to Answer All Questions!
Automation Testing Masters ProgramEXPLORE PROGRAMPrepare Yourself to Answer All Questions!

----

**What is a constructor in C++?**

In C++, a function Object is a particular "MEMBER FUNCTION" that shares the same title as the class it belongs to and is
used to initialize specific values to an object's data members. 

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class student {
    int no;
public:
    student()
    {
        cout << "Enter the RollNo:";
        cin >> no;
    }

    void display()
    {
        cout << endl << no << "\t";
    }
};

int main()
{
    student s; // constructor gets called automatically when
               // we create the object of the class
    s.display();
    return 0;
}
```

----

**What is a virtual function?**

A member function in the base class redefined in a derived class is a virtual function. It is declared using the virtual keyword. It ensures that the correct function is called
for an object, irrespective of the type of reference/pointer used for the function call. Virtual functions are mainly used for runtime polymorphism.  

----

**What do you understand about friend class and friend function?**

Like a friend function, a friend class can access personal and guarded variables of the type in which it is declared. All member functions for classes specified as
friends to another class are friend functions for the friend class.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class Node {
private:
    int key;
    Node* next;
    /* Other members of Node Class */
    // Now class LinkedList can
    // access private members of Node
    friend class LinkedList;
};

int main()
{
    
}
```

----

**What are the three different types of C++ access specifiers?**

- Public: All member functions and data members are accessible outside the class.
- Protected: All member functions and data members are accessible within the class and to the derived class.
- Private: All member functions and data members cannot be accessed outside the class. 

----

**What is an abstraction in C++?**

Abstraction means displaying the essential details to the user while hiding the irrelevant or particular
details that you don’t want to show to a user. It is of two types:
- Control abstraction
- Data abstraction

----

**What are destructors in C++?**

A destructor member function is instantly called when an object exits its scope or is specifically deleted by a call to delete.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class X {
public:
    // Constructor for class X
    X();
    // Destructor for class X
    ~X();
};

int main()
{
    
}
```

----

**Is it possible to overload a deconstructor? Give reasons for your answer?**

No, it is impossible as destructors do not take arguments or return anything. There has to be only one empty destructor per class. It should have a void parameter list.  

----

**What is an abstract class? When is it used?**

An abstract class is a class whose objects cannot be created. It serves as a parent for the derived classes. Placing a pure virtual function in the class makes it an abstract class. 

----

**What do you understand about static members and static member functions?**

A variable in a class declared as static has its space allocated for the lifetime of the program. Regardless of the number of objects of that class
created, there is only a single copy of the static member. The same static member is accessible to all the objects of that class.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class A
{
public:
    A()
    {
        cout << "A's Constructor Called " << endl;
    }
};

class B
{
    static A a;
public:
    B()
    {
        cout << "B's Constructor Called " << endl;
    }
};

int main()
{
    B b;
    return 0;
}
```

A static member function can be called even if no class objects exist. It is accessed using only the class name and the scope resolution operator (::).  

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

// C++ Program to demonstrate
// static member in a class

#include <iostream>
#include <string>

using namespace std;

class Student {
public:
    // static member
    static int total;

    // Constructor called
    Student() { total += 1; }
};

int Student::total = 0;

int main()
{
    // Student 1 declared
    Student s1;
    cout << "Number of students:" << s1.total << endl;

    // Student 2 declared
    Student s2;
    cout << "Number of students:" << s2.total << endl;

    // Student 3 declared
    Student s3;
    cout << "Number of students:" << s3.total << endl;
    return 0;
}
```

----

**What is the C++ OOPs concept?**

__OOPs concept in C++:__                                                                               

- Object: Anything that exists physically in the real world is called an object.
- Class: The collection of objects is called class.
- Inheritance: Properties of parent class inherited into child class is known as inheritance.
- Polymorphism: It is the ability to exist in more than one form.
- Encapsulation: Binding of code and data together into a single unit.
- Abstraction: Hiding internal details and showing functionality to the user.

----

**When is void() return type used?**

You use the void() return type when you don’t want to return any value. It specifies that the function doesn’t return a value.
A function with a void return type completes its task and then returns the control to the caller.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

void fun()
{
    cout << "Hello";
    // We can write return in void
    return;
}

int main()
{
    fun();
    return 0;
}
```

----

**What is call by value and call by reference in C++?**

In the call by value method, you pass the copies of actual parameters to the function's formal parameters. This means if there is any change in the values inside the function, then that change will not affect the actual values.

In the call-by-reference method, the reference or address of actual parameters is sent to the function's formal parameters. This means any change in values inside the function will be reflected in the actual values.

----

**What is an [inline function?](https://www.geeksforgeeks.org/inline-functions-cpp/)**

An inline function when called expands in line. When you call this function, the whole code of the inline function gets inserted or substituted at the inline function call.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

inline int cube(int s) { return s * s * s; }

int main() {
	cout << "The cube of 3 is: " << cube(3) << "\n";
	return 0;
}
```

----

**What are pointers in C++?**

Pointers are the variables that store the memory address of another variable. The type of the variable must correspond with the type of pointer.

Syntax: type *name

30. What is a scope resolution operator?
A scope resolution operator is represented as ::

This operator is used to associate function definition to a particular class.

The scope operator is used for the following purposes:

To access a global variable when you have a local variable with the same name.
To define a function outside the class.
Unleash a High-paying Automation Testing Job!
Automation Testing Masters ProgramEXPLORE PROGRAMUnleash a High-paying Automation Testing Job!
31. What should be the output of the following C++ program?
InterviewQuestions_Example3

01
02
012
011
3 - 012, the value of i is 0 and i % 5 is equal to 0, so x is displayed and incremented and i is also incremented, then 1 % 5 is not zero, so the condition is not met. Similarly, the process will repeat till 4 % 5 because 5 % 5 is zero. So the value of x is one and gets incremented to two. Then, the process will repeat for 6,7,8,9, but 10  % 10 will be zero again, and the value of x is printed, which is 2.

32. What is a constructor?
A constructor is defined as a member function that is invoked whenever you create an object; it has the same name as that of the class.

There are two types of constructors:

Default constructor: This auto-generated constructor doesn’t take any arguments.
Parameterized constructor: In this constructor, it can pass arguments.
33. Define operator overloading and function overloading.
An example of compile-time polymorphism is operator overloading. It is the concept of modifying an existing C++ operator without altering its original meaning. 

Let us take an example for this 

class A

{

};

int main()

{

      A a1,a2,a3;

      a3= a1 + a2;

      return 0;

}

34. How to input strings in C++ with spaces?
InterviewQuestions_Example4

35. Discuss the difference between new and malloc
new
malloc
new is an operator

malloc() is a function

It calls the constructor

The malloc function doesn’t call the constructor

There is no need to specify memory size while using new()

You have to specify the memory size

new operator can be overloaded

malloc() can never be overloaded

36. What is operator overloading?
Operator overloading is a mechanism in which a special meaning is given to an operator.

For example, you can overload the ‘+’ operator in a class-like string to concatenate two strings by only using ‘+.’

Create and Showcase Your Portfolio from Scratch!
Caltech PGP Full Stack DevelopmentEXPLORE PROGRAMCreate and Showcase Your Portfolio from Scratch!
37. What is the output of the below C++ program?
InterviewQuestions_Example5.

0 3
0 8
0 6
0 2
3 - 0 6. In enum, the element's value is one greater than the previous element. The value of blue is 0 by default, and the value of green is five, so the value of GREAT will become six automatically.

38. What among these is used to return the number of characters in the string?
Size

Length

Both size and length

Name

3 - Both size and length are used to return the number of characters in the string

39. Which among the following statements is correct about the program given below?
InterviewQuestions_Example7.

The output will be 7
The output will be 14
The output will be 0
The output will be 1
1 - Output will be 7.  Pointer p has the memory address of x, and you display the pointer with a dereference operator that will display the value 7.

40. Which among the following statements is correct about the program given below?
InterviewQuestions_Example8.

The output will be 245
The output will be 222
The output will be 4810
The output will be 4812
3 - Output will be 4810, because you are passing the references of the function here.

Become an Automation Test Engineer in 11 Months!
Automation Testing Masters ProgramEXPLORE PROGRAMBecome an Automation Test Engineer in 11 Months!
41. What is a friend function?
You can define a friend function as a function that can access private, public and protect members of the class. You declare the friend function with the help of the friend keyword. You declare this function inside the class.

42. Which of the following will give the size of object or type?
sizeof
malloc
realloc
calloc
1 - The sizeof operator is used to give the size of object or type

43. Which of the following is not a member of a class?
Static function
Virtual function
Const function
Friend function
4 - Among the following, friend function is not a member of the class

44. What is STL?
STL stands for standard template library. It is a library of container templates that provide generic classes and functions.

STL components are containers, algorithms, iterators, and function objects.

InterviewQuestions_Example13




Now, have a look at some advanced-level C++ Interview Questions.

C++ Interview Questions For Experienced
These C++ Interview Questions test your application skills in C++ and explore practical problems that might be posed to you in a C++ interview.

45. How to write a program to check if a number is a palindrome or not?
InterviewQuestions_Example9.

Front or Back-End Development? Learn It All!
Caltech Coding BootcampEXPLORE PROGRAMFront or Back-End Development? Learn It All!
46. What is a copy constructor?
A copy function is a member function that uses another object from the same class to initialize a new thing. A copy function is, to put it simply, a function that produces an object by initializing it with a different object of the same class that has already been constructed.

#include <iostream>  

using namespace std;  

class A  

{  

   Public:  

    int x;  

    A(int a) // parameterized constructor.  

    {  

      x=a;  

    }  

    A(A &i) // copy constructor  

    {  

        x = i.x;  

    }  

};  

int main()  

{  

  A a1(20); // Calling the parameterized constructor.  

 A a2(a1); // Calling the copy constructor.  

 cout<<a2.x;  

  return 0;  

}  

47. Write a program to find the factorial of a number?
InterviewQuestions_Example2

48. What is inheritance?
Inheritance is the mechanism in which you can create a new class i.e. child class from the existing class i.e. parent class. This child class is also known as a derived class and the parent class is also called Base class. 

InterviewQuestions_Example12.

49. What is Abstraction?
Abstraction can be defined as a technique in which you only show functionality to the user i.e., the details that you want the user to see, hiding the internal details or implementation details.

50. What should be the output of the below code?
InterviewQuestions_Example10.

5
4
7
6
4 - 6, Ternary operator is used, the value of a is less than b which violates the condition that is why 6 is the answer. 

Automation Test Engineer Master's Program
To learn about the automation of web applicationsEXPLORE COURSEAutomation Test Engineer Master's Program
51. How to find the frequency of a number in C++?
InterviewQuestions_Example6.

52. What should be the output of the below code?
InterviewQuestions_Example11.

1010
1001
11
1000
1 - 1010, the value of j is incremented to 11, then j value is added to 100 but not assigned, and at last the value of j i.e 11 is added to 999 which gives us 1010.

53. What should be the correct statement about string objects in C++?
String objects should necessarily be terminated by a null character
String objects have a static size
String objects have a dynamic size
String objects use extra memory than required 
3 - String objects have a dynamic size.

Here's How to Land a Top Software Developer Job
Full Stack Development-MEANEXPLORE PROGRAMHere's How to Land a Top Software Developer Job
54. How is a shallow copy different from a deep copy?
Shallow Copy
Deep Copy
It stores the references of objects to the original memory address.

It makes a fresh and separate copy of an entire object and its unique memory address.

Faster

Comparatively slower

It reflects changes made to the new/copied object in the original object.

It doesn’t reflect changes made to the new/copied object in the original object.

55. How are virtual functions different from pure virtual functions?
A virtual function is a base class member function that a derived class can modify. A member function of a base class that is a pure virtual function must be defined in the derived type; otherwise, the derived class will become abstract as well.

class

interface Woocommerce{    

void print();    

}    

class Bat implements Woo{    

public void print(){System.out.println("Woo!");}    

public static void main(String args[]){    

Bat obj = new Bat();    

obj.print();    

 }    

} 

56. Class D is derived from a base class B. If creating an object of type D, what order will the constructors of these classes get called?
The derived class consists of two parts: the base part and the derived part. C++ constructs derived objects in phases. The process begins with constructing the most-base class (at the top of the inheritance tree), followed by each child class construction in order, and then the most-child class. Thus, first, the Constructor of class B will be called, and then the constructor of class D. 

57. Can a virtual function be called from a constructor?
A virtual process may be called a function Object, but exercise caution. It might perform differently than expected. The virtual call mechanism in a function Object is disabled since overriding from derived classes hasn't happened yet. Building blocks are used to create objects, "base before derived."

class Dog{

void make(){

System.out.println("labrador");

}

}

public class Big extends Dog{

void make(){

System.out.println("Big Dog labrador ");

}

public static void main(String args[]){

Dog ob1 = new Big();

ob1.make();

}

}

58. What are void pointers?
In C, a void pointer has no connection to any particular data type. It designates a location for specific data within the storage. This indicates that it is pointing to a variable's address. It also goes by the name "general purpose pointer."

#include <iostream>

using namespace std;

int main()

{

int a = 10;

char b = 'x';

void* p = &a; // void pointer holds address of int 'a'

p = &b; // void pointer holds address of char 'b'

}

59. What is this pointer in C++?
A class, struct, or union form only has access to this pointer within non-static member variables. The arrow shows the object for which the member function is called. 

string food = "Pizza"; // A food variable of type string

string* ptr = &food; // A pointer variable, with the name ptr, that stores the address of food

// Output the value of food (Pizza)

cout << food << "\n";

// Output the memory address of food (0x6dfed4)

cout << &food << "\n";

// Output the memory address of food with the pointer (0x6dfed4)

cout << ptr << "\n";

60. How would you deallocate and allocate memory in C++?
The heap is used in C to allocate dynamic memory, and these functions are part of the standard library. Malloc() and free are the two important dynamic memory operations (). The size of the desired memory area in bytes is the only parameter accepted by the malloc() function. 

#include <iostream>

#include <cstdlib>

#include <cstring>

using namespace std;

int main() {

  char *user;

  user = (char *) malloc(25);

  strcpy(user, "Jane_Eyre");

  cout << "User Name = " << user << " " << &user << endl;

  free(user);

}

</https://www.simplilearn.com/tutorials/cpp-tutorial/cpp-interview-questions>

<https://www.interviewbit.com/cpp-interview-questions/>

1. What are the different data types present in C++?
The 4 data types in C++ are given below:

Primitive Datatype(basic datatype). Example- char, short, int, float, long, double, bool, etc.
Derived datatype. Example- array, pointer, etc.
Enumeration. Example- enum
User-defined data types. Example- structure, class, etc.
logo
Practice Problems
Solve these problems to ace this concept
Variable and Types
Medium
29.49 Mins
Solve

2. What is the difference between C and C++?
The main difference between C and C++ are provided in the table below:

C	C++
C is a procedure-oriented programming language.	C++ is an object-oriented programming language.
C does not support data hiding.	Data is hidden by encapsulation to ensure that data structures and operators are used as intended.
C is a subset of C++	C++ is a superset of C.
Function and operator overloading are not supported in C	Function and operator overloading is supported in C++
Namespace features are not present in C	Namespace is used by C++, which avoids name collisions.
Functions can not be defined inside structures.	Functions can be defined inside structures.
calloc() and malloc() functions are used for memory allocation and free() function is used for memory deallocation.	new operator is used for memory allocation and deletes operator is used for memory deallocation.
3. What are class and object in C++?
A class is a user-defined data type that has data members and member functions. Data members are the data variables and member functions are the functions that are used to perform operations on these variables.

An object is an instance of a class. Since a class is a user-defined data type so an object can also be called a variable of that data type.

A class is defined as-

class A{
private:
 int data;
public:
 void fun(){

 }
};

Class and Object in C++
For example, the following is a class car that can have properties like name, color, etc. and they can have methods like speed().

logo
Practice Problems
Solve these problems to ace this concept
Classes and Objects
Medium
21.28 Mins
Solve

You can download a PDF version of Cpp Interview Questions.

Download PDF

4. What is the difference between struct and class?
In C++ a structure is the same as a class except for a few differences like security. The difference between struct and class are given below:

Structure	Class
Members of the structure are public by default.	Members of the class are private by default.
When deriving a struct from a class/struct, default access specifiers for base class/struct are public.	When deriving a class, default access specifiers are private.
5. What is operator overloading?
Operator Overloading is a very essential element to perform the operations on user-defined data types. By operator overloading we can modify the default meaning to the operators like +, -, *, /, <=, etc. 

For example -

The following code is for adding two complex number using operator overloading-

class complex{
private:
 float r, i;
public:
 complex(float r, float i){
  this->r=r;
  this->i=i;
 }
 complex(){}
 void displaydata(){
  cout<<”real part = “<<r<<endl;
  cout<<”imaginary part = “<<i<<endl;
 }
 complex operator+(complex c){
  return complex(r+c.r, i+c.i);
 }
};
int main(){
complex a(2,3);
complex b(3,4);
complex c=a+b;
c.displaydata();
return 0;
}
6. What is polymorphism in C++?
Polymorphism in simple means having many forms. Its behavior is different in different situations. And this occurs when we have multiple classes that are related to each other by inheritance.

For example, think of a base class called a car that has a method called car brand(). Derived classes of cars could be Mercedes, BMW, Audi - And they also have their own implementation of a cars

The two types of polymorphism in c++ are:

Compile Time Polymorphism
Runtime Polymorphism

Polymorphism in C++
logo
Practice Problems
Solve these problems to ace this concept
Polymorphism
Medium
12.58 Mins
Solve

7. Explain constructor in C++
The constructor is a member function that is executed automatically whenever an object is created. Constructors have the same name as the class of which they are members so that compiler knows that the member function is a constructor. And no return type is used for constructors.

Example:

class A{
 private:
  int val;
 public:
  A(int x){             //one argument constructor
   val=x;
  }
  A(){                    //zero argument constructor
  }
}
int main(){
 A a(3);     

 return 0;
}
8. Tell me about virtual function
Virtual function is a member function in the base class that you redefine in a derived class. A virtual function is declared using the virtual keyword. When the function is made virtual, C++ determines which function is to be invoked at the runtime based on the type of the object pointed by the base class pointer.

logo
Practice Problems
Solve these problems to ace this concept
Runtime Polymorphism (Virtual Functions)
Medium
28.32 Mins
Solve

9. Compare compile time polymorphism and Runtime polymorphism
The main difference between compile-time and runtime polymorphism is provided below:

Compile-time polymorphism	Run time polymorphism
In this method, we would come to know at compile time which method will be called. And the call is resolved by the compiler.	In this method, we come to know at run time which method will be called. The call is not resolved by the compiler.
It provides fast execution because it is known at the compile time.	It provides slow execution compared to compile-time polymorphism because it is known at the run time.
It is achieved by function overloading and operator overloading.	It can be achieved by virtual functions and pointers.
Example -

int add(int a, int b){
      return a+b;
}
int add(int a, int b, int c){
      return a+b+c;
}

int main(){
    cout<<add(2,3)<<endl;
    cout<<add(2,3,4)<<endl;


     return 0;
}
 

Example -

class A{
     public:
          virtual void fun(){
               cout<<"base ";
          }
};
class B: public A{
     public:
          void fun(){
               cout<<"derived ";
          }
};
int main(){
     A *a=new B;
     a->fun();

     return 0;
}
10. What do you know about friend class and friend function?
A friend class can access private, protected, and public members of other classes in which it is declared as friends.

Like friend class, friend function can also access private, protected, and public members. But, Friend functions are not member functions.

For example -

class A{
 private:
  int data_a;
 public:
  A(int x){
   data_a=x;
  }
  friend int fun(A, B);
}
class B{
 private:
  int data_b;
 public:
  A(int x){
   data_b=x;
  }
  friend int fun(A, B);
}
int fun(A a, B b){
 return a.data_a+b.data_b;
}
int main(){
 A a(10);
 B b(20);
 cout<<fun(a,b)<<endl;
 return 0;
}
Here we can access the private data of class A and class B.

11. What are the C++ access specifiers?
In C++ there are the following access specifiers:

Public: All data members and member functions are accessible outside the class.

Protected: All data members and member functions are accessible inside the class and to the derived class.

Private: All data members and member functions are not accessible outside the class.

12. Define inline function
If a function is inline, the compiler places a copy of the code of that function at each point where the function is called at compile time. One of the important advantages of using an inline function is that it eliminates the function calling overhead of a traditional function.

13. What is a reference in C++?
A reference is like a pointer. It is another name of an already existing variable. Once a reference name is initialized with a variable, that variable can be accessed by the variable name or reference name both.

For example-

int x=10;
int &ref=x;           //reference variable
If we change the value of ref it will be reflected in x. Once a reference variable is initialized it cannot refer to any other variable. We can declare an array of pointers but an array of references is not possible.

14. What do you mean by abstraction in C++?
Abstraction is the process of showing the essential details to the user and hiding the details which we don’t want to show to the user or hiding the details which are irrelevant to a particular user.

15. Is deconstructor overloading possible? If yes then explain and if no then why?
No destructor overloading is not possible. Destructors take no arguments, so there’s only one way to destroy an object. That’s the reason destructor overloading is not possible.

16. What do you mean by call by value and call by reference?
In call by value method, we pass a copy of the parameter is passed to the functions. For these copied values a new memory is assigned and changes made to these values do not reflect the variable in the main function.

In call by reference method, we pass the address of the variable and the address is used to access the actual argument used in the function call. So changes made in the parameter alter the passing argument.

17. What is an abstract class and when do you use it?
A class is called an abstract class whose objects can never be created. Such a class exists as a parent for the derived classes. We can make a class abstract by placing a pure virtual function in the class.

18. What are destructors in C++?
A constructor is automatically called when an object is first created. Similarly when an object is destroyed a function called destructor automatically gets called. A destructor has the same name as the constructor (which is the same as the class name) but is preceded by a tilde.

Example:

class A{
 private:
  int val;
 public:
  A(int x){           
   val=x;
  }
  A(){                
  }
  ~A(){                  //destructor
  }
}
int main(){
 A a(3);     
 return 0;
}
19. What are the static members and static member functions?
When a variable in a class is declared static, space for it is allocated for the lifetime of the program. No matter how many objects of that class have been created, there is only one copy of the static member. So same static member can be accessed by all the objects of that class.

A static member function can be called even if no objects of the class exist and the static function are accessed using only the class name and the scope resolution operator ::

20. Explain inheritance
Inheritance is the process of creating new classes, called derived classes, from existing classes. These existing classes are called base classes. The derived classes inherit all the capabilities of the base class but can add new features and refinements of their own.

Example-


Inheritance in C++
Class Bus, Class Car, and Class Truck inherit the properties of Class Vehicle.

The most important thing about inheritance is that it permits code reusability.

C++ Interview Questions For Experienced
21. What is a copy constructor?
A copy constructor is a member function that initializes an object using another object of the same class.

Example-

class A{
int x,y;
A(int x, int y){
 this->x=x;
 this->y=y;
}

};
int main(){
A a1(2,3);
A a2=a1;     //default copy constructor is called
return 0;
}
We can define our copy constructor. If we don’t define a copy constructor then the default copy constructor is called.

22. What is the difference between shallow copy and deep copy?
The difference between shallow copy and a deep copy is given below:

Shallow Copy	Deep Copy
Shallow copy stores the references of objects to the original memory address.	Deep copy makes a new and separate copy of an entire object with its unique memory address.
Shallow copy is faster.	Deep copy is comparatively slower.
Shallow copy reflects changes made to the new/copied object in the original object.	Deep copy doesn’t reflect changes made to the new/copied object in the original object
23. What is the difference between virtual functions and pure virtual functions?
A virtual function is a member function in the base class that you redefine in a derived class. It is declared using the virtual keyword.

Example-

class base{
public:
 virtual void fun(){

 }
};
A pure virtual function is a function that has no implementation and is declared by assigning 0. It has no body.

Example-

class base{
public:
 virtual void fun()=0;
};
Here, = sign has got nothing to do with the assignment, and value 0 is not assigned to anything. It is used to simply tell the compiler that a function will be pure and it will not have anybody.

24. If class D is derived from a base class B. When creating an object of type D in what order would the constructors of these classes get called?
The derived class has two parts, a base part, and a derived part.  When C++ constructs derived objects, it does so in phases. First, the most-base class(at the top of the inheritance tree) is constructed. Then each child class is constructed in order until the most-child class is constructed last. 
So the first Constructor of class B will be called and then the constructor of class D will be called.

During the destruction exactly reverse order is followed. That is destructor starts at the most-derived class and works its way down to base class.
So the first destructor of class D will be called and then the destructor of class B will be called.

25. Can we call a virtual function from a constructor?
Yes, we can call a virtual function from a constructor. But the behavior is a little different in this case. When a virtual function is called, the virtual call is resolved at runtime. It is always the member function of the current class that gets called. That is the virtual machine doesn’t work within the constructor.

For example-

class base{
 private:
  int value;
 public:
  base(int x){
   value=x;
  }
  virtual void fun(){
   
  }
}

class derived{
 private:
  int a;
 public:
  derived(int x, int y):base(x){
   base *b;
   b=this;
   b->fun();      //calls derived::fun()
  }
  void fun(){
   cout<<”fun inside derived class”<<endl;
  }
}
26. What are void pointers?
A void pointer is a pointer which is having no datatype associated with it. It can hold addresses of any type.

For example-

void *ptr; 
char *str;
p=str;                // no error 
str=p;                // error because of type mismatch
We can assign a pointer of any type to a void pointer but the reverse is not true unless you typecast it as

str=(char*) ptr;
27. What is this pointer in C++?
The member functions of every object have a pointer named this, which points to the object itself. The value of this is set to the address of the object for which it is called. It can be used to access the data in the object it points to.

Example

class A{
 private:
  int value;
 public:
  void setvalue(int x){
   this->value=x; 
  }
};

int main(){
 A a;
 a.setvalue(5);
 return 0;
}
28. How do you allocate and deallocate memory in C++?
The new operator is used for memory allocation and deletes operator is used for memory deallocation in C++.

For example-

int value=new int;  		//allocates memory for storing 1 integer
delete value;          		// deallocates memory taken by value

int *arr=new int[10];    	//allocates memory for storing 10 int
delete []arr;              	// deallocates memory occupied by arr
Additional Resources

Practice Coding

C++ MCQ

C++ Tutorials

C Interview Questions

Difference Between C and C++

Difference Between C++ and Java

Online C++ Compiler

Features of C++

C++ Coding Questions
1.
Which operator can not be overloaded in C++?


+

::

*

++
2.
What will be the output of the following C++ program:

#include<iostream>
using namespace std;
int main(){
int a=1;
cout<<(a++)*(++a)<<endl;
return 0;
}

1

6

2

3
3.
What will be the value of x in the following C++ program

#include<iostream>
using namespace std;
int main(){
int a=1;
int x=(a++)++;
cout<<x<<endl;
return 0;
}

Compile Time Error

3

1

2
4.
What is an abstract class?


Class declared with abstract keyword

Class which has exactly one virtual function

Class which hash at least one pure virtual function

None of the above
5.
Consider the following C++ program

#include<iostream>
using namespace std;
class A{
public:
virtual void a()=0;
A(){
 cout<<"A ";
}
};
class B: public A
{
public:
B(){
 cout<<"B ";
} 
};

int main(){
A *a=new B();

return 0;
}
What will be output?


A B

B A

Compile-time error

None of the above
6.
What is the size of void in C++?


0

1

2

4
7.
If a base class and derived class each include a member function with the same name. Function from which class will be called if called by an object of the derived class


Member function of the base class

Member function of the derived class

Depend on the parameter

None of the above
8.
Memory used by an array is


Contiguous

Non-contiguous

Not determined

None of the above
9.
Which of the following statement is correct?


An object is an instance of the class

A friend function can access private members of a class

Members of the class are private by default

All of the above

</https://www.interviewbit.com/cpp-interview-questions/>

<https://www.javatpoint.com/cpp-interview-questions>

1) What is C++?
C++ is an object-oriented programming language created by Bjarne Stroustrup. It was released in 1985.

C++ is a superset of C with the major addition of classes in C language.

Initially, Stroustrup called the new language "C with classes". However, after sometime the name was changed to C++. The idea of C++ comes from the C increment operator ++.


2) What are the advantages of C++?
C++ doesn't only maintains all aspects from C language, it also simplifies memory management and adds several features like:

C++ is a highly portable language means that the software developed using C++ language can run on any platform.
C++ is an object-oriented programming language which includes the concepts such as classes, objects, inheritance, polymorphism, abstraction.
C++ has the concept of inheritance. Through inheritance, one can eliminate the redundant code and can reuse the existing classes.
Data hiding helps the programmer to build secure programs so that the program cannot be attacked by the invaders.
Message passing is a technique used for communication between the objects.
C++ contains a rich function library.
3) What is the difference between C and C++?
Following are the differences between C and C++:

C	C++
C language was developed by Dennis Ritchie.	C++ language was developed by Bjarne Stroustrup.
C is a structured programming language.	C++ supports both structural and object-oriented programming language.
C is a subset of C++.	C++ is a superset of C.
In C language, data and functions are the free entities.	In the C++ language, both data and functions are encapsulated together in the form of a project.
C does not support the data hiding. Therefore, the data can be used by the outside world.	C++ supports data hiding. Therefore, the data cannot be accessed by the outside world.
C supports neither function nor operator overloading.	C++ supports both function and operator overloading.
In C, the function cannot be implemented inside the structures.	In the C++, the function can be implemented inside the structures.
Reference variables are not supported in C language.	C++ supports the reference variables.
C language does not support the virtual and friend functions.	C++ supports both virtual and friend functions.
In C, scanf() and printf() are mainly used for input/output.	C++ mainly uses stream cin and cout to perform input and output operations.
4) What is the difference between reference and pointer?
Following are the differences between reference and pointer:

Reference	Pointer
Reference behaves like an alias for an existing variable, i.e., it is a temporary variable.	The pointer is a variable which stores the address of a variable.
Reference variable does not require any indirection operator to access the value. A reference variable can be used directly to access the value.	Pointer variable requires an indirection operator to access the value of a variable.
Once the reference variable is assigned, then it cannot be reassigned with different address values.	The pointer variable is an independent variable means that it can be reassigned to point to different objects.
A null value cannot be assigned to the reference variable.	A null value can be assigned to the reference variable.
It is necessary to initialize the variable at the time of declaration.	It is not necessary to initialize the variable at the time of declaration.
5) What is a class?
The class is a user-defined data type. The class is declared with the keyword class. The class contains the data members, and member functions whose access is defined by the three modifiers are private, public and protected. The class defines the type definition of the category of things. It defines a datatype, but it does not define the data it just specifies the structure of data.

You can create N number of objects from a class.


6) What are the various OOPs concepts in C++?
The various OOPS concepts in C++ are:

C++ Interview Questions
Class:
The class is a user-defined data type which defines its properties and its functions. For example, Human being is a class. The body parts of a human being are its properties, and the actions performed by the body parts are known as functions. The class does not occupy any memory space. Therefore, we can say that the class is the only logical representation of the data.

The syntax of declaring the class:


class student  
{  
//data members;  
//Member functions  
}  
Object:
An object is a run-time entity. An object is the instance of the class. An object can represent a person, place or any other item. An object can operate on both data members and member functions. The class does not occupy any memory space. When an object is created using a new keyword, then space is allocated for the variable in a heap, and the starting address is stored in the stack memory. When an object is created without a new keyword, then space is not allocated in the heap memory, and the object contains the null value in the stack.

class Student  
{  
//data members;  
//Member functions  
}  
The syntax for declaring the object:

Student s = new Student();  
Inheritance:
Inheritance provides reusability. Reusability means that one can use the functionalities of the existing class. It eliminates the redundancy of code. Inheritance is a technique of deriving a new class from the old class. The old class is known as the base class, and the new class is known as derived class.

Syntax

class derived_class :: visibility-mode base_class;   
Note: The visibility-mode can be public, private, protected.
Encapsulation:
Encapsulation is a technique of wrapping the data members and member functions in a single unit. It binds the data within a class, and no outside method can access the data. If the data member is private, then the member function can only access the data.


Abstraction:
Abstraction is a technique of showing only essential details without representing the implementation details. If the members are defined with a public keyword, then the members are accessible outside also. If the members are defined with a private keyword, then the members are not accessible by the outside methods.

Data binding:
Data binding is a process of binding the application UI and business logic. Any change made in the business logic will reflect directly to the application UI.

Polymorphism:
Polymorphism means multiple forms. Polymorphism means having more than one function with the same name but with different functionalities. Polymorphism is of two types:


Static polymorphism is also known as early binding.
Dynamic polymorphism is also known as late binding.
7) What are the different types of polymorphism in C++?
Polymorphism: Polymorphism means multiple forms. It means having more than one function with the same function name but with different functionalities.

Polymorphism is of two types:

C++ Interview Questions
Runtime polymorphism
Runtime polymorphism is also known as dynamic polymorphism. Function overriding is an example of runtime polymorphism. Function overriding means when the child class contains the method which is already present in the parent class. Hence, the child class overrides the method of the parent class. In case of function overriding, parent and child class both contains the same function with the different definition. The call to the function is determined at runtime is known as runtime polymorphism.

Let's understand this through an example:

#include <iostream>  
using namespace std;  
class Base  
{  
    public:  
    virtual void show()  
    {  
        cout<<"javaTpoint";  
     }  
};  
class Derived:public Base  
{  
    public:  
    void show()  
    {  
        cout<<"javaTpoint tutorial";  
    }  
};  
  
int main()  
{  
    Base* b;  
    Derived d;  
    b=&d;  
    b->show();  
                return 0;  
}  
Output:

javaTpoint tutorial
Compile time polymorphism
Compile-time polymorphism is also known as static polymorphism. The polymorphism which is implemented at the compile time is known as compile-time polymorphism. Method overloading is an example of compile-time polymorphism.

Method overloading: Method overloading is a technique which allows you to have more than one function with the same function name but with different functionality.

Method overloading can be possible on the following basis:

The return type of the overloaded function.
The type of the parameters passed to the function.
The number of parameters passed to the function.
Let's understand this through an example:


#include <iostream>  
using namespace std;  
class Multiply  
{  
   public:  
   int mul(int a,int b)  
   {  
       return(a*b);  
   }  
   int mul(int a,int b,int c)  
   {  
       return(a*b*c);  
  }  
 };  
int main()  
{  
    Multiply multi;  
    int res1,res2;  
    res1=multi.mul(2,3);  
    res2=multi.mul(2,3,4);  
    cout<<"\n";  
    cout<<res1;  
    cout<<"\n";  
    cout<<res2;  
    return 0;  
}  
Output:

6
24
In the above example, mul() is an overloaded function with the different number of parameters.
8) Define namespace in C++.
The namespace is a logical division of the code which is designed to stop the naming conflict.
The namespace defines the scope where the identifiers such as variables, class, functions are declared.
The main purpose of using namespace in C++ is to remove the ambiguity. Ambiquity occurs when the different task occurs with the same name.
For example: if there are two functions exist with the same name such as add(). In order to prevent this ambiguity, the namespace is used. Functions are declared in different namespaces.
C++ consists of a standard namespace, i.e., std which contains inbuilt classes and functions. So, by using the statement "using namespace std;" includes the namespace "std" in our program.
Syntax of namespace:
namespace namespace_name  
{  
 //body of namespace;  
}  
Syntax of accessing the namespace variable:

namespace_name::member_name;  
Let's understand this through an example:

#include <iostream>  
using namespace std;  
namespace addition  
{  
    int a=5;  
    int b=5;  
    int add()  
    {  
        return(a+b);  
    }  
}  
  
int main() {  
int result;  
result=addition::add();  
cout<<result;  
return 0;  
}  
Output:

10
9) Define token in C++.
A token in C++ can be a keyword, identifier, literal, constant and symbol.


10) Who was the creator of C++?
Bjarne Stroustrup.

11) Which operations are permitted on pointers?
Following are the operations that can be performed on pointers:

Incrementing or decrementing a pointer: Incrementing a pointer means that we can increment the pointer by the size of a data type to which it points.
There are two types of increment pointers:

1. Pre-increment pointer: The pre-increment operator increments the operand by 1, and the value of the expression becomes the resulting value of the incremented. Suppose ptr is a pointer then pre-increment pointer is represented as ++ptr.

Let's understand this through an example:

#include <iostream>  
using namespace std;  
int main()  
{  
int a[5]={1,2,3,4,5};  
int *ptr;  
ptr=&a[0];  
cout<<"Value of *ptr is : "<<*ptr<<"\n";  
cout<<"Value of *++ptr : "<<*++ptr;  
return 0;  
}  
Output:

Value of *ptr is : 1
Value of *++ptr : 2
2. Post-increment pointer: The post-increment operator increments the operand by 1, but the value of the expression will be the value of the operand prior to the incremented value of the operand. Suppose ptr is a pointer then post-increment pointer is represented as ptr++.

Let's understand this through an example:

#include <iostream>  
using namespace std;  
int main()  
{  
int a[5]={1,2,3,4,5};  
int *ptr;  
ptr=&a[0];  
cout<<"Value of *ptr is : "<<*ptr<<"\n";  
cout<<"Value of *ptr++ : "<<*ptr++;  
return 0;  
}  
Output:

Value of *ptr is : 1
Value of *ptr++ : 1
Subtracting a pointer from another pointer: When two pointers pointing to the members of an array are subtracted, then the number of elements present between the two members are returned.
12) Define 'std'.
Std is the default namespace standard used in C++.

13) Which programming language's unsatisfactory performance led to the discovery of C++?
C++was discovered in order to cope with the disadvantages of C.

14) How delete [] is different from delete?
Delete is used to release a unit of memory, delete[] is used to release an array.

15) What is the full form of STL in C++?
STL stands for Standard Template Library.

16) What is an object?
The Object is the instance of a class. A class provides a blueprint for objects. So you can create an object from a class. The objects of a class are declared with the same sort of declaration that we declare variables of basic types.

17) What are the C++ access specifiers?
The access specifiers are used to define how to functions and variables can be accessed outside the class.

There are three types of access specifiers:

Private: Functions and variables declared as private can be accessed only within the same class, and they cannot be accessed outside the class they are declared.
Public: Functions and variables declared under public can be accessed from anywhere.
Protected: Functions and variables declared as protected cannot be accessed outside the class except a child class. This specifier is generally used in inheritance.
18) What is Object Oriented Programming (OOP)?
OOP is a methodology or paradigm that provides many concepts. The basic concepts of Object Oriented Programming are given below:

Classes and Objects: Classes are used to specify the structure of the data. They define the data type. You can create any number of objects from a class. Objects are the instances of classes.

Encapsulation: Encapsulation is a mechanism which binds the data and associated operations together and thus hides the data from the outside world. Encapsulation is also known as data hiding. In C++, It is achieved using the access specifiers, i.e., public, private and protected.

Abstraction: Abstraction is used to hide the internal implementations and show only the necessary details to the outer world. Data abstraction is implemented using interfaces and abstract classes in C++.

Some people confused about Encapsulation and abstraction, but they both are different.


Inheritance: Inheritance is used to inherit the property of one class into another class. It facilitates you to define one class in term of another class.

19) What is the difference between an array and a list?
An Array is a collection of homogeneous elements while a list is a collection of heterogeneous elements.
Array memory allocation is static and continuous while List memory allocation is dynamic and random.
In Array, users don't need to keep in track of next memory allocation while In the list, the user has to keep in track of next location where memory is allocated.
20) What is the difference between new() and malloc()?
new() is a preprocessor while malloc() is a function.
There is no need to allocate the memory while using "new" but in malloc() you have to use sizeof().
"new" initializes the new memory to 0 while malloc() gives random value in the newly allotted memory location.
The new() operator allocates the memory and calls the constructor for the object initialization and malloc() function allocates the memory but does not call the constructor for the object initialization.
The new() operator is faster than the malloc() function as operator is faster than the function.
21) What are the methods of exporting a function from a DLL?
There are two ways:

By using the DLL's type library.
Taking a reference to the function from the DLL instance.
22) Define friend function.
Friend function acts as a friend of the class. It can access the private and protected members of the class. The friend function is not a member of the class, but it must be listed in the class definition. The non-member function cannot access the private data of the class. Sometimes, it is necessary for the non-member function to access the data. The friend function is a non-member function and has the ability to access the private data of the class.

To make an outside function friendly to the class, we need to declare the function as a friend of the class as shown below:

class sample  
{  
   // data members;  
 public:  
friend void abc(void);  
};  
Following are the characteristics of a friend function:

The friend function is not in the scope of the class in which it has been declared.
Since it is not in the scope of the class, so it cannot be called by using the object of the class. Therefore, friend function can be invoked like a normal function.
A friend function cannot access the private members directly, it has to use an object name and dot operator with each member name.
Friend function uses objects as arguments.
Let's understand this through an example:

#include <iostream>  
using namespace std;  
class Addition  
{  
 int a=5;  
 int b=6;  
 public:  
 friend int add(Addition a1)  
 {  
     return(a1.a+a1.b);  
 }  
};  
int main()  
{  
int result;  
Addition a1;  
 result=add(a1);  
 cout<<result;  
return 0;  
}  
Output:

11
23) What is a virtual function?
A virtual function is used to replace the implementation provided by the base class. The replacement is always called whenever the object in question is actually of the derived class, even if the object is accessed by a base pointer rather than a derived pointer.
A virtual function is a member function which is present in the base class and redefined by the derived class.
When we use the same function name in both base and derived class, the function in base class is declared with a keyword virtual.
When the function is made virtual, then C++ determines at run-time which function is to be called based on the type of the object pointed by the base class pointer. Thus, by making the base class pointer to point different objects, we can execute different versions of the virtual functions.
Rules of a virtual function:

The virtual functions should be a member of some class.
The virtual function cannot be a static member.
Virtual functions are called by using the object pointer.
It can be a friend of another class.
C++ does not contain virtual constructors but can have a virtual destructor.
24) When should we use multiple inheritance?
You can answer this question in three manners:

Never
Rarely
If you find that the problem domain cannot be accurately modeled any other way.
25) What is a destructor?
A Destructor is used to delete any extra resources allocated by the object. A destructor function is called automatically once the object goes out of the scope.

Rules of destructor:

Destructors have the same name as class name and it is preceded by tilde.
It does not contain any argument and no return type.
26) What is an overflow error?
It is a type of arithmetical error. It happens when the result of an arithmetical operation been greater than the actual space provided by the system.

27) What is overloading?
When a single object behaves in many ways is known as overloading. A single object has the same name, but it provides different versions of the same function.
C++ facilitates you to specify more than one definition for a function name or an operator in the same scope. It is called function overloading and operator overloading respectively.
Overloading is of two types:
C++ Interview Questions
1. Operator overloading: Operator overloading is a compile-time polymorphism in which a standard operator is overloaded to provide a user-defined definition to it. For example, '+' operator is overloaded to perform the addition operation on data types such as int, float, etc.

Operator overloading can be implemented in the following functions:

Member function
Non-member function
Friend function
Syntax of Operator overloading:

Return_type classname :: Operator Operator_symbol(argument_list)  
{  
      // body_statements;  
}  
2. Function overloading: Function overloading is also a type of compile-time polymorphism which can define a family of functions with the same name. The function would perform different operations based on the argument list in the function call. The function to be invoked depends on the number of arguments and the type of the arguments in the argument list.

28) What is function overriding?
If you inherit a class into a derived class and provide a definition for one of the base class's function again inside the derived class, then this function is called overridden function, and this mechanism is known as function overriding.

29) What is virtual inheritance?
Virtual inheritance facilitates you to create only one copy of each object even if the object appears more than one in the hierarchy.

30) What is a constructor?
A Constructor is a special method that initializes an object. Its name must be same as class name.

31) What is the purpose of the "delete" operator?
The "delete" operator is used to release the dynamic memory created by "new" operator.

32) Explain this pointer?
This pointer holds the address of the current object.

33) What does Scope Resolution operator do?
A scope resolution operator(::) is used to define the member function outside the class.

34) What is the difference between delete and delete[]?
Delete [] is used to release the array of allocated memory which was allocated using new[] whereas delete is used to release one chunk of memory which was allocated using new.

35) What is a pure virtual function?
The pure virtual function is a virtual function which does not contain any definition. The normal function is preceded with a keyword virtual. The pure virtual function ends with 0.

Syntax of a pure virtual function:

virtual void abc()=0;   //pure virtual function.  
Let's understand this through an example:

#include<iostream>  
using namespace std;  
class Base  
{  
    public:  
    virtual void show()=0;  
};  
  
class Derived:public Base  
{  
    public:  
    void show()  
    {  
        cout<<"javaTpoint";  
    }  
};  
int main()  
{  
    Base* b;  
    Derived d;  
    b=&d;  
    b->show();  
    return 0;  
}  
Output:

javaTpoint
36) What is the difference between struct and class?
Structures	class
A structure is a user-defined data type which contains variables of dissimilar data types.	The class is a user-defined data type which contains member variables and member functions.
The variables of a structure are stored in the stack memory.	The variables of a class are stored in the heap memory.
We cannot initialize the variables directly.	We can initialize the member variables directly.
If access specifier is not specified, then by default the access specifier of the variable is "public".	If access specifier is not specified, then by default the access specifier of a variable is "private".
The instance of a structure is a "structure variable".	
Declaration of a structure:
struct structure_name
{
   // body of structure;
} ;
Declaration of class:
class class_name
{
   // body of class;
} 
A structure is declared by using a struct keyword.	The class is declared by using a class keyword.
The structure does not support the inheritance.	The class supports the concept of inheritance.
The type of a structure is a value type.	The type of a class is a reference type.
37) What is a class template?
A class template is used to create a family of classes and functions. For example, we can create a template of an array class which will enable us to create an array of various types such as int, float, char, etc. Similarly, we can create a template for a function, suppose we have a function add(), then we can create multiple versions of add().

The syntax of a class template:

template<class T>  
class classname  
{  
  // body of class;  
};  
Syntax of a object of a template class:

classname<type> objectname(arglist);  
38) What is the difference between function overloading and operator overloading?
Function overloading: Function overloading is defined as we can have more than one version of the same function. The versions of a function will have different signature means that they have a different set of parameters.

Operator overloading: Operator overloading is defined as the standard operator can be redefined so that it has a different meaning when applied to the instances of a class.

39) What is a virtual destructor?
A virtual destructor in C++ is used in the base class so that the derived class object can also be destroyed. A virtual destructor is declared by using the ~ tilde operator and then virtual keyword before the constructor.

Note: Constructor cannot be virtual, but destructor can be virtual.
Let's understand this through an example

Example without using virtual destructor
#include <iostream>  
using namespace std;  
class Base  
{  
    public:  
    Base()  
    {  
        cout<<"Base constructor is called"<<"\n";  
    }  
    ~Base()  
    {  
        cout<<"Base class object is destroyed"<<"\n";  
    }  
};  
class Derived:public Base  
{  
    public:  
    Derived()  
    {  
        cout<<"Derived class constructor is called"<<"\n";  
    }  
    ~Derived()  
    {  
        cout<<"Derived class object is destroyed"<<"\n";  
    }  
};  
int main()   
{  
  Base* b= new Derived;  
  delete b;  
  return 0;  
    
}  
Output:


Base constructor is called
Derived class constructor is called
Base class object is destroyed
In the above example, delete b will only call the base class destructor due to which derived class destructor remains undestroyed. This leads to the memory leak.

Example with a virtual destructor
#include <iostream>  
using namespace std;  
class Base  
{  
    public:  
    Base()  
    {  
        cout<<"Base constructor is called"<<"\n";  
    }  
    virtual ~Base()  
    {  
        cout<<"Base class object is destroyed"<<"\n";  
    }  
};  
class Derived:public Base  
{  
    public:  
    Derived()  
    {  
        cout<<"Derived class constructor is called"<<"\n";  
    }  
    ~Derived()  
    {  
        cout<<"Derived class object is destroyed"<<"\n";  
    }  
};  
int main()   
{  
  Base* b= new Derived;  
  delete b;  
  return 0;  
    
}  

</https://www.javatpoint.com/cpp-interview-questions>

<https://www.geeksforgeeks.org/cpp-interview-questions/>

1. What is C++? What are the advantages of C++?
C++ is an object-oriented programming language that was introduced to overcome the jurisdictions where C was lacking. By object-oriented we mean that it works with the concept of polymorphism, inheritance, abstraction, encapsulation, object, and class.

Advantages of C++:

C++ is an OOPs language that means the data is considered as objects.
C++ is a multi-paradigm language; In simple terms, it means that we can program the logic, structure, and procedure of the program.
Memory management is a key feature in C++ as it enables dynamic memory allocation
It is a Mid-Level programming language which means it can develop games, desktop applications, drivers, and kernels
To read more, refer to the article – What are the advantages of C++?


2. What are the different data types present in C++?
data types in C++
Different types of data types in C++

For more information, refer to C++ data types 

3. Define ‘std’?
‘std’ is also known as Standard or it can be interpreted as a namespace. The command “using namespace std” informs the compiler to add everything under the std namespace and inculcate them in the global namespace. This all inculcation of global namespace benefits us to use “cout” and “cin” without using “std::_operator_”.

For more information, refer to namespace and std.

4. What are references in C++?
When a variable is described as a reference it becomes an alias of the already existing variable. In simple terms, a referenced variable is another named variable of an existing variable keeping in mind that changes made in the reference variable will be reflected in the already existing variable. A reference variable is preceded with a ‘&’ symbol.

Syntax:

int GFG = 10;

// reference variable
int& ref = GFG;
For more information, refer to references in C++

5. What do you mean by Call by Value and Call by Reference?
In this programming language to call a function we have 2 methods: Call by Value and Call by Reference

Call by Value

Call by Reference


A copy of a variable is passed.	A variable itself is passed fundamentally.
Calling a function by sending the values by copying variables.	Calling a function by sending the address of the passed variable.
The changes made in the function are never reflected outside the function on the variable. In short, the original value is never altered in Call by Value.	The changes made in the functions can be seen outside the function on the passed function. In short, the original value is altered in Call by reference.
Passed actual and formal parameters are stored in different memory locations. Therefore, making Call by Value a little memory insufficient 	Passed actual and formal parameters are stored in the same memory location. Therefore, making Call by Reference a little more memory efficient.
For information, refer to the difference between call by value and call by reference

6. Define token in C++
A token is the smallest individual element of a program that is understood by a compiler. A token comprises the following:

Keywords – That contain a special meaning to the compiler
Identifiers – That hold a unique value/identity 
Constants – That never change their value throughout the program 
Strings – That contains the homogenous sequence of data 
Special Symbols – They have some special meaning and cannot be used for another purpose; eg: [] () {}, ; * = # 
Operators – Who perform operations on the operand
For more information, refer to Tokens in C++

7. What is the difference between C and C++?
C

C++

It is a procedural programming language. In simple words, it does not support classes and objects	It is a mixture of both procedural and object-oriented programming languages. In simple words, it supports classes and objects.
It does not support any OOPs concepts like polymorphism, data abstraction, encapsulation, classes, and objects.	It supports all concepts of data 
It does not support Function and Operator Overloading	It supports Function and Operator Overloading respectively
It is a function-driven language	It is an object-driven language
For more information, refer to Difference between C and C++

8. What is the difference between struct and class?
Struct

Class

Members of the struct are always by default public mode	Members of the class can be in private, protected, and public modes.
Structure does not support inheritance.	Classes do support the concept of inheritance.
Structures are of the value type. They only hold value in memory.	Classes are of reference type. It holds a reference of an object in memory.
The memory in structures is stored as stacks	The memory in classes is stored as heaps.
For more information, refer to the Difference between struct and class.

9. What is the difference between reference and pointer?
Reference

Pointer

The value of a reference cannot be reassigned	The value of a pointer can be reassigned
It can never hold a null value as it needs an existing value to become an alias of                     	It can hold or point at a null value and be termed as a nullptr or null pointer
It cannot work with arrays	It can work with arrays
To access the members of class/struct it uses a ‘ . ‘	To access the members of class/struct it uses a ‘ -> ‘ 
The memory location of reference can be accessed easily or it can be used directly	The memory location of a pointer cannot be accessed easily as we have to use a dereference ‘ * ‘ 
For more information, refer to the Difference between reference and pointer

10. What is the difference between function overloading and operator overloading?
Function Overloading

Operator Overloading

It is basically defining a function in numerous ways such that there are many ways to call it or in simple terms you have multiple versions of the same function	It is basically giving practice of giving a special meaning to the existing meaning of an operator or in simple terms redefining the pre-redefined meaning                          
Parameterized Functions are a good example of Function Overloading as just by changing the argument or parameter of a function you make it useful for different purposes 	Polymorphism is a good example of an operator overloading as an object of allocations class can be used and called by different classes for different purposes
Example of Function Overloading:

int GFG(int X, int Y);
int GFG(char X, char Y);
Example of Operator Overloading:

int GFG() = X() + Y();
int GFG() = X() – Y();
For more information, refer to Operator Overloading and Function Overloading

11. What is the difference between an array and a list?
Arrays

Lists

Array are contiguous memory locations of homogenous data types stored in a fixed location or size.    	Lists are classic individual elements that are linked or connected to each other with the help of pointers and do not have a fixed size.
Arrays are static in nature.	Lists are dynamic in nature
Uses less memory than linked lists.	Uses more memory as it has to store the value and the pointer memory location
For more information, refer to Arrays Vs List

12: What is the difference between a while loop and a do-while loop?
While Loop

do-while Loop

While loop is also termed an entry-controlled loop	The do-while loop is termed an exit control loop
If the condition is not satisfied the statements inside the loop will not execute                                  	Even if the  condition is not satisfied the statements inside the loop will execute for at least one time
Example of a while loop:

while(condition) 

{statements to be executed;};

Example of a do-while loop:

do {

statements to be executed;

} while(condition or expression);

For more information, refer to the Difference between while and do-while loop

13. Discuss the difference between prefix and postfix?
prefix

postfix

It simply means putting the operator before the operand	It simply means putting the operator after the operand
It executes itself before ‘; ‘ 	 It executes itself after ‘; ‘ 
Associativity of prefix ++ is right to left	Associativity of postfix ++ is left to right
For more information, refer to the Difference between prefix and postfix

14. What is the difference between new and malloc()?
new

malloc()

new is an operator which performs an operation   	malloc is a function that returns and accepts values
new calls the constructors	malloc cannot call a constructor
new is faster than malloc as it is an operator	malloc is slower than new as it is a function
new returns the exact data type	malloc returns void*
For more information, refer to Difference between new and malloc()

15. What is the difference between virtual functions and pure virtual functions?
Virtual Function

Pure Virtual Function

A Virtual Function is a member function of a base class that can be redefined in another derived class.	A Pure Virtual Function is a member function of a base class that is only declared in a base class and defined in a derived class to prevent it from becoming an abstract class.
A virtual Function has its definition in its respective base class.              	There is no definition in Pure Virtual Function and is initialized with a pure specifier (= 0).
The base class has a virtual function that can be represented or instanced; In simple words, its object can be made.	A base class having pure virtual function becomes abstract that cannot be represented or instanced; In simple words, it means its object cannot be made.
 For more information, refer to the Difference between virtual functions and pure virtual functions

16. What are classes and objects in C++?
A class is a user-defined data type where all the member functions and data members are tailor-made according to demands and requirements in addition to which these all can be accessed with the help of an object. To declare a user-defined data type we use a keyword class.

An object is an instance of a class and an entity with value and state; In simple terms, it is used as a catalyst or to represent a class member. It may contain different parameters or none.

Note: A class is a blueprint that defines functions which are used by an object.

For more information, refer to this What are classes and objects

17. What is Function Overriding?
When a function of the same name, same arguments or parameters, and same return type already present/declared in the base class is used in a derived class is known as Function Overriding. It is an example of Runtime Polymorphism or Late Binding which means the overridden function will be executed at the run time of the execution.

For more information, refer to Function Overriding in C++

18. What are the various OOPs concepts in C++?
Classes: It is a user-defined datatype
Objects: It is an instance of a class
Abstraction: It is a technique of showing only necessary details
Encapsulation: Wrapping of data in a single unit
Inheritance: The capability of a class to derive properties and characteristics from another class
Polymorphism: Polymorphism is known as many forms of the same thing
For more information, refer to Various OOPs concepts in C++

19. Explain inheritance
The capability or ability of a class to derive properties and characteristics from another class is known as inheritance. In simple terms, it is a system or technique of reusing and extending existing classes without modifying them.

For more information, refer to Inheritance

20. When should we use multiple inheritance?
Multiple inheritances mean that a derived class can inherit two or more base/parent classes. It is useful when a derived class needs to combine numerous attributes/contracts and inherit some, or all, of the implementation from these attributes/contracts. To take a real-life example consider your Parents where Parent A is your DAD Parent B is your MOM and Chid C is you.

multiple inheritances
Multiple Inheritances

For more information, refer to Multiple Inheritance.

21. What is virtual inheritance?
Virtual inheritance is a technique that ensures only one copy of a base class’s member variables is inherited by grandchild-derived classes. Or in simple terms, virtual inheritance is used when we are dealing with a situation of multiple inheritances but want to prevent multiple instances of the same class from appearing in the inheritance hierarchy.

22. What is polymorphism in C++?
Polymorphism is known as many forms of the same thing. In simple terms, we can say that Polymorphism is the ability to display a member function in multiple forms depending on the type of object that calls them. 

In other words, we can also say that a man can be an employee to someone, a son of someone, a father of someone, and a husband of someone; this is how polymorphism can be projected in real life.

There is 2 type of polymorphism:

Compile Time Polymorphism
Function Overloading
Operator Overloading
Run Time Polymorphism
Function Overriding
Virtual Function
To know more about it, refer to Polymorphism 

23. What are the different types of polymorphism in C++?
There is 2 type of polymorphism

Compile Time Polymorphism or Static Binding

This type of polymorphism is achieved during the compile time of the program which results in it making a bit faster than Run time. Also, Inheritance is not involved in it. It is comprised of 2 further techniques:

Function Overloading: When there are multiple functions with the same name but different parameters then this is known as function overloading.

// same name different arguments
int GFG() { }
int GFG(int a) { }
float GFG(double a) { }
int GFG(int a, double b) { }
Operator Overloading: It is basically giving practice of giving a special meaning to the existing meaning of an operator or in simple terms redefining the pre-redefined meaning

class GFG {
  // private and other modes
  statements
  public
       returnType operator symbol (arguments) {
           statements
       } 
    statements
};
   

Run-Time Polymorphism or Late Binding

Run-time polymorphism takes place when functions are invoked during run time. 
 
Function Overriding: Function overriding occurs when a base class member function is redefined in a derived class with the same arguments and return type.


// C++ program to demonstrate 
// Function overriding
#include <iostream>
using namespace std;
class GFG {
    public:
    virtual void display() {
        cout<<"Function of base class"<<endl;
    }
};
class derived_GFG : public GFG {
    public:
    void show() {
        cout<<"Function of derived class"<<endl;
    }
};
int main() {
  derived_GFG dg;
  dg.show();
  return 0;
}
Output:

Function of derived class
For more information, refer to Different types of Polymorphism

24. Compare compile-time polymorphism and Runtime polymorphism
Compile-Time Polymorphism

Runtime Polymorphism

It is also termed static binding and early binding.	It is also termed Dynamic binding and Late binding.
It is fast because execution is known early at compile time.	It is slow as compared to compile-time because execution is known at runtime.
It is achieved by function overloading and operator overloading.	It is achieved by virtual functions and function overriding.
For more information, refer to Compile-time polymorphism and Runtime polymorphism

25. Explain the constructor in C++.
A constructor is a special type of member function of a class, whose name is the same as that of the class by whom it is invoked and initializes value to the object of a class. 

There are 3 types of constructors:

A. Default constructor: It is the most basic type of constructor which accepts no arguments or parameters. Even if it is not called the compiler calls it automatically when an object is created.

Example:

class Class_name
{
public:
 Class_name()
 {
 cout<<"I am a default constructor";
 }
};
B. Parameterized constructor: It is a type of constructor which accepts arguments or parameters. It has to be called explicitly by passing values in the arguments as these arguments help initialize an object when it is created. It also has the same name as that of the class. 

Also, It is used to overload constructors.

Example:


// CPP program to demonstrate
// parameterized constructors
#include <iostream>
using namespace std;
class GFG {
private:
    int x, y;
public:
    // Parameterized Constructor
    GFG(int x1, int y1)
    {
        x = x1;
        y = y1;
    }
    int getX() { return x; }
    int getY() { return y; }
};
int main()
{
    // Constructor called
    GFG G(10, 15);
    // Access values assigned by constructor
    cout << "G.x = " << G.getX() << ", G.y = " << G.getY();
    return 0;
}
Output

G.x = 10, G.y = 15
C. Copy Constructor: A copy constructor is a member function that initializes an object using another object of the same class. Also, the Copy constructor takes a reference to an object of the same class as an argument.

Example:


Sample(Sample& t) 
{
  id = t.id;
}
For more information, refer to Constructors 

26. What are destructors in C++?
Destructors are members of functions in a class that delete an object when an object of the class goes out of scope. Destructors have the same name as the class preceded by a tilde (~) sign. Also, destructors follow a down-to-top approach, unlike constructors which follow a top-to-down.

Syntax:

~constructor_name(); // tilde sign signifies that it is a destructor
For more information, refer to Destructor.

27. What is a virtual destructor?
When destroying instances or objects of a derived class using a base class pointer object, a virtual destructor is invoked to free up memory space allocated by the derived class object or instance.

Virtual destructor guarantees that first the derived class’ destructor is called. Then the base class’s destructor is called to release the space occupied by both destructors in the inheritance class which saves us from the memory leak. It is advised to make your destructor virtual whenever your class is polymorphic.

For more information, refer to Virtual Destructor

28. Is destructor overloading possible? If yes then explain and if no then why?
The simple answer is NO we cannot overload a destructor. It is mandatory to only destructor per class in C++. Also to mention, Destructor neither take arguments nor they have a parameter that might help to overload.

C++ Interview Questions – Intermediate Level
29. Which operations are permitted on pointers?
Pointers are the variables that are used to store the address location of another variable. Operations that are permitted to a pointer are:

Increment/Decrement of a Pointer
Addition and Subtraction of integer to a pointer
Comparison of pointers of the same type
30. What is the purpose of the “delete” operator?
The delete operator is used to delete/remove all the characteristics/properties from an object by deallocating its memory; furthermore, it returns true or false in the end. In simple terms, it destroys or deallocates array and non-array(pointer) objects which are created by new expressions.

int GFG = new int[100];
// uses GFG for deletion
delete [] GFG;
For more information, refer to Delete operator

31. How delete [] is different from delete?
delete[]

delete

It is used for deleting a whole array	It is used to delete only one single pointer
It is used for deleting the objects of new[]; By this, we can say that delete[] is used to delete an array of objects	It is used for deleting the objects of new; By this, we can say that delete is used to delete a single object
It can call as many destructors it wants	It can only call the destructor of a class once
32. What do you know about friend class and friend function?
A friend class is a class that can access both the protected and private variables of the classes where it is declared as a friend.

Example of friend class:


class Class_1st {
   // ClassB is a friend class of ClassA
   friend class Class_2nd;
   statements;
}
  
class Class_2nd {
   statements;
}
A friend function is a function used to access the private, protected, and public data members or member functions of other classes. It is declared with a friend keyword. The advantage of a friend function is that it is not bound to the scope of the class and once it is declared in a class, furthermore to that, it cannot be called by an object of the class; therefore it can be called by other functions. Considering all the mentioned points we can say that a friend function is a global function.

Example of friend function:

class GFG {
    statements;
    friend dataype function_Name(arguments);
    statements;
}
  
OR 
  
class GFG{
     statements'
     friend int divide(10,5);
     statements;
}
For more information, refer to the friend function and friend class

33. What is an Overflow Error?
Overflow Error occurs when the number is too large for the data type to handle. In simple terms, it is a type of error that is valid for the defined but exceeds used the defined range where it should coincide/lie. 

For example, the range of int data type is –2,147,483,648 to 2,147,483,647 and if we declare a variable of size 2,247,483,648 it will generate a overflow error.

34. What does the Scope Resolution operator do?
A scope resolution operator is denoted by a ‘::‘ symbol. Just like its name this operator resolves the barrier of scope in a program. A scope resolution operator is used to reference a member function or a global variable out of their scope furthermore to which it can also access the concealed variable or function in a program.

Scope Resolution is used for numerous amounts of tasks:

To access a global variable when there is a local variable with the same name
To define the function outside the class
In case of multiple inheritances
For namespace
For more information, refer to Scope resolution operator

35. What are the C++ access modifiers?
The access restriction specified to the class members( whether it is member function or data member) is known as access modifiers/specifiers. 

Access Modifiers are of 3 types:

Private – It can neither be accessed nor be viewed from outside the class 
Protected – It can be accessed if and only if the accessor is the derived class
Public – It can be accessed or be viewed from outside the class 
For more information, refer to Access Modifiers

36. Can you compile a program without the main function?
Yes, it is absolutely possible to compile a program without a main(). For example Use Macros that defines the main


// C++ program to demonstrate the
// a program without main()
#include <stdio.h>
#define fun main
int fun(void)
{
    printf("Geeksforgeeks");
    return 0;
}
For more information, refer to Can you compile a program without the main function

37. What is STL?
STL is known as Standard Template Library, it is a library that provides 4 components like container, algorithms, and iterators.
 


C++ STL

For more information, refer to STL in C++

38. Define inline function. Can we have a recursive inline function in C++?
An inline function is a form of request not an order to a compiler which results in the inlining of our function to the main function body. An inline function can become overhead if the execution time of the function is less than the switching time from the caller function to called function. To make a function inline use the keyword inline before and define the function before any calls are made to the function.

Inline Function
Inline Function Explanation

Syntax:

inline data_type function_name()
{
Body;
}
The answer is No; It cannot be recursive.

An inline function cannot be recursive because in the case of an inline function the code is merely placed into the position from where it is called and does not maintain a piece of information on the stack which is necessary for recursion.

Plus, if you write an inline keyword in front of a recursive function, the compiler will automatically ignore it because the inline is only taken as a suggestion by the compiler.

For more information, refer to Inline Function

39. What is an abstract class and when do you use it?
An abstract class is a class that is specifically designed to be used as a base class. An abstract class contains at least one pure virtual function. You declare a pure virtual function by using a pure specifier(= 0) in the declaration of a virtual member function in the class declaration

You cannot use an abstract class as a parameter type, a function return type, or the type of an explicit conversion, nor can you declare an object of an abstract class. However, it can be used to declare pointers and references to an abstract class. 

An abstract class is used if you want to provide a common, implemented functionality among all the implementations of the component. Abstract classes will allow you to partially implement your class, whereas interfaces would have no implementation for any members whatsoever. In simple words, Abstract Classes are a good fit if you want to provide implementation details to your children but don’t want to allow an instance of your class to be directly instantiated.

40. What are the static data members and static member functions?
The static data member of a class is a normal data member but preceded with a static keyword. It executes before main() in a program and is initialized to 0 when the first object of the class is created. It is only visible to a defined class but its scope is of a lifetime.

Syntax:

static Data_Type Data_Member;  
The static member function is the member function that is used to access other static data members or other static member functions. It is also defined with a static keyword. We can access the static member function using the class name or class objects.

Syntax:

classname::function name(parameter);
C++ Interview Questions – Expert Level
41. What is the main use of the keyword “Volatile”?
Just like its name, things can change suddenly and unexpectantly; So it is used to inform the compiler that the value may change anytime. Also, the volatile keyword prevents the compiler from performing optimization on the code. It was intended to be used when interfacing with memory-mapped hardware, signal handlers, and machine code instruction.

For more information, refer to this Volatile

42. Define storage class in C++ and name some
Storage class is used to define the features(lifetime and visibility) of a variable or function. These features usually help in tracing the existence of a variable during the runtime of a program.

Syntax:

storage_class var_data_type var_name; 
Some types of storage classes:


Examples of storage class

For more information, refer to Storage Class

43. What is a mutable storage class specifier? How can they be used?
Just like its name, the mutable storage class specifier is used only on a class data member to make it modifiable even though the member is part of an object declared as const. Static or const, or reference members cannot use the mutable specifier. When we declare a function as const, this pointer passed to the function becomes const.

44. Define the Block scope variable. 
So the scope of a variable is a region where a variable is accessible. There are two scope regions, A global and block or local. 

A block scope variable is also known as a local scope variable. A variable that is defined inside a function (like main) or inside a block (like loops and if blocks) is a local variable. It can be used ONLY inside that particular function/block in which it is declared. a block-scoped variable will not be available outside the block even if the block is inside a function.

For more information, refer to Scope of a variable

45. What is the function of the keyword “Auto”?
The auto keyword may be used to declare a variable with a complex type in a straightforward fashion. You can use auto to declare a variable if the initialization phrase contains templates, pointers to functions, references to members, etc. With type inference capabilities, we can spend less time having to write out things the compiler already knows. As all the types are deduced in the compiler phase only, the time for compilation increases slightly but it does not affect the runtime of the program. 

For more information, refer to Auto in C++

46.  Define namespace in C++.
Namespaces enable us to organize named items that would otherwise have global scope into smaller scopes, allowing us to give them namespace scope. This permits program parts to be organized into distinct logical scopes with names. The namespace provides a place to define or declare identifiers such as variables, methods, and classes. 

Or we could say that A namespace is a declarative zone that gives the identifiers (names of types, functions, variables, and so on) within it a scope. Namespaces are used to arrange code into logical categories and to avoid name clashes, which might happen when you have many libraries in your code base.

For more information, refer to Namespace in C++

47. When is void() return type used?
The void keyword, when used as a function return type, indicates that the function does not return a value. When used as a parameter list for a function, void indicates that the function takes no parameters. Non-Value Returning functions are also known as void functions. They’re called “void” since they’re not designed to return anything. True, but only partially. We can’t return values from void functions, but we can certainly return something. Although void functions have no return type, they can return values.

For more information, refer to Void return type.

48. What is the difference between shallow copy and deep copy?
Shallow Copy

Deep Copy

In Shallow copy, a copy of the original object is stored and only the reference address is finally copied. In simple terms, Shallow copy duplicates as little as possible	In Deep copy, the copy of the original object and the repetitive copies both are stored. In simple terms, Deep copy duplicates everything
A shallow copy of a collection is a copy of the collection structure, not the elements. With a shallow copy, two collections now share individual elements.	A deep copy of a collection is two collections with all of the elements in the original collection duplicated.
A shallow copy is faster	Deep copy is comparatively slower.
For more information, refer to Shallow copy VS Deep Copy 

49. Can we call a virtual function from a constructor?
Yes, we can call a virtual function from a constructor. But it can throw an exception of overriding.

50. What are void pointers?
Just like its name a void pointer is a pointer that is not associated with anything or with any data type. Nevertheless, a void pointer can hold the address value of any type and can be converted from one data type to another.

For more, information refers to Void Pointer in C++

</https://www.geeksforgeeks.org/cpp-interview-questions/>

<https://www.toptal.com/c-plus-plus/interview-questions>

Is there a difference between class and struct?

View answer

2.
What will the line of code below print out and why?

#include <iostream>

int main(int argc, char **argv)
{
    std::cout << 25u - 50;
    return 0;
}
View answer




3.
What is the error in the code below and how should it be corrected?

my_struct_t *bar;
/* ... do stuff, including setting bar to point to a defined my_struct_t object ... */
memset(bar, 0, sizeof(bar));
View answer



Apply to Join Toptal's Development Network

and enjoy reliable, steady, remote Freelance C++ Developer Jobs

4.
What will i and j equal after the code below is executed? Explain your answer.

int i = 5;
int j = i++;
View answer




5.
Assuming buf is a valid pointer, what is the problem in the code below? What would be an alternate way of implementing this that would avoid the problem?

size_t sz = buf->size();
while ( --sz >= 0 )
{
	/* do something */
}
View answer



6.
Consider the two code snippets below for printing a vector. Is there any advantage of one vs. the other? Explain.

Option 1:

vector vec;
/* ... .. ... */
for (auto itr = vec.begin(); itr != vec.end(); itr++) {
	itr->print();
}
Option 2:

vector vec;
/* ... .. ... */
for (auto itr = vec.begin(); itr != vec.end(); ++itr) {
	itr->print();
}
View answer


7.
Implement a template function IsDerivedFrom() that takes class C and class P as template parameters. It should return true when class C is derived from class P and false otherwise.

View answer

8.
Implement a template boolean IsSameClass() that takes class A and B as template parameters. It should compare class A and B and return false when they are different classes and true if they are the same class.

View answer
9.
Is it possible to have a recursive inline function?

View answer

10.
What is the output of the following code:

#include <iostream>

class A {
public:
    A() {}
    ~A() {
        throw 42;
    }
};

int main(int argc, const char * argv[]) {
    try {
        A a;
        throw 32;
    } catch(int a) {
        std::cout << a;
    }
}
View answer

11.
You are given library class Something as follows:

class Something {
public:
    Something() {
        topSecretValue = 42;
    }
    bool somePublicBool;
    int somePublicInt;
    std::string somePublicString;
private:
    int topSecretValue;
};
Implement a method to get topSecretValue for any given Something* object. The method should be cross-platform compatible and not depend on sizeof (int, bool, string).

View answer



12.
Implement a void function F that takes pointers to two arrays of integers (A and B) and a size N as parameters. It then populates B where B[i] is the product of all A[j] where j != i.

For example: If A = {2, 1, 5, 9}, then B would be {45, 90, 18, 10}.

View answer



13.
When you should use virtual inheritance?

View answer



14.
What is the output of the following code:

#include <iostream>

int main(int argc, const char * argv[]) {
    int a[] = {1, 2, 3, 4, 5, 6};
    std::cout << (1 + 3)[a] - a[0] + (a + 1)[2];
}
View answer






15.
What is the output of the following code:

#include <iostream>

class Base {
    virtual void method() {std::cout << "from Base" << std::endl;}
public:
    virtual ~Base() {method();}
    void baseMethod() {method();}
};

class A : public Base {
    void method() {std::cout << "from A" << std::endl;}
public:
    ~A() {method();}
};

int main(void) {
    Base* base = new A;
    base->baseMethod();
    delete base;
    return 0;
}
View answer


16.
How many times will this loop execute? Explain your answer.

unsigned char half_limit = 150;

for (unsigned char i = 0; i < 2 * half_limit; ++i)
{
    // do something;
}
View answer



17.
How can you make sure a C++ function can be called as e.g. void foo(int, int) but not as any other type like void foo(long, long)?

View answer



18.
What is the problem with the following code?

class A
{
public:
A() {}
~A(){}
};

class B: public A
{
public:
B():A(){}
~B(){}
};

int main(void)
{
  A* a = new B();
  delete a;
}
View answer


19.
What is a storage class?

View answer



20.
How can a C function be called in a C++ program?

View answer

21.
What will be the output of the following program?

#include <iostream>

struct A
{
    int data[2];

    A(int x, int y) : data{x, y} {}
    virtual void f() {}
};

int main(int argc, char **argv)
{
    A a(22, 33);

    int *arr = (int *) &a;
    std::cout << arr[2] << std::endl;

    return 0;
}
View answer

22.
Are you allowed to have a static const member function? Explain your answer.

View answer

23.
Explain the volatile and mutable keywords.

View answer


24.
C++ supports multiple inheritance. What is the “diamond problem” that can occur with multiple inheritance? Give an example.

View answer

</https://www.toptal.com/c-plus-plus/interview-questions>

<https://hackr.io/blog/cpp-interview-questions>

Basic C++ Level Interview Questions
1. What is C++?
C++ is a computer programming language that is a superset of C, with additional features. 


2. Does C++ make use of OOPS? 
Yes, it does. An Object-Oriented Programming System is a paradigm that includes concepts such as data binding, polymorphism, and inheritance, among others.

3. What is a Class?
A class is a user-defined data type that is at the center of OOP. It reflects different entities, attributes, and actions.

4. What is an object?
An object is an instance of the class. An object can have fields, methods, and constructors.

5. What is encapsulation?
Encapsulation is the process of binding together the data and functions in a class. It is applied to prevent direct access to the data for security reasons. The functions of a class are applied for this purpose.

6. What is abstraction?
An abstraction in C++ is hiding the internal implementations and displaying only the required details.

For example, when you send an important message through email, at that time, only writing and clicking the send option is used. This outcome is just the success message that is displayed to confirm that your email has been sent. However, the process followed in transferring the data through email is not displayed because it is of no use to you.

7. What is inheritance?
C++ allows classes to inherit some of the commonly used state and behavior from other classes. This process is known as inheritance.

8. What is the access specifier and what are the types?
An access specifier determines how the class members, i.e., functions and variables, will be accessed outside the class's scope. 



There are three types of access specifiers in C++:

Private: Such class members can’t be accessed outside the class in which they are declared and are only accessible within the same class. Even child classes are disabled to access private members of its parent class.
Protected: In addition to the class in which they are declared, the child classes can access its parent class's protected members.
Public: Class members declared as public can be accessed throughout the program.
9. What is a namespace?
 A namespace is used for resolving the name conflict of the identifier, which is accomplished by placing them under various namespaces.

10. What is a class template?
A class template is a name given to the generic class. The use of the keyword template is made for defining a class template.

11. What is the function of the keyword “Volatile”?
"Volatile" is a function that helps in declaring that the particular variable is volatile and thereby directs the compiler to change the variable externally- this way, the compiler optimization on the variable reference can be avoided.

12. What is a storage class?
A storage class in C++ specifically resembles the scope of symbols, including the variables, functions, etc. Some of the storage class names in C++ include mutable, auto, static, extern, register, etc.

13. What is an Inline Function? Is it possible to ignore inlining?
In order to reduce the function call overhead, C++ offers inline functions. As the name suggests, an inline function is expanded in line when it is called.

As soon as the inline function is called, the whole code of the same gets either inserted or substituted at the particular point of the inline function call. The substitution is completed by the C++ compiler at compile time. Small inline functions might increase program efficiency.

The syntax of a typical inline function is:

Inline return-type function-name(parameters)
{
// Function code goes here
}

As the inlining is a request, not a command, the compiler can ignore it.

14. Can we have a recursive inline function in C++?
Even though it is possible to call an inline function from within itself in C++, the compiler may not generate the inline code. This is so because the compiler won’t determine the depth of the recursion at the compile time.

Nonetheless, a compiler with a good optimizer is able to inline recursive calls until some depth is fixed at compile time and insert non-recursive calls at compile time for the cases when the actual depth exceeds run time.

15. What is the ‘this’ pointer?
The ‘this’ pointer is a constant pointer, and it holds the memory address of the current object. It passes as a hidden argument to all the nonstatic member function calls. It is available as a local variable within the body of all the nonstatic functions.

As static member functions can be called even without any object, i.e., with the class name, the ‘this’ pointer is not available for them.

16. What are the most important differences between C and C++?
C++ supports references while C doesn’t.
Features like friend functions, function overloading, inheritance, templates, and virtual functions are inherent to C++. These are not available in the C programming language.
In C, exception handling is taken care of in the traditional if-else style. On the other hand, C++ offers support for exception handling at the language level.
Mainly used input and output in C are scanf() and printf(), respectively. In C++, cin is the standard input stream while cout serves as the standard output stream.
While C is a procedural programming language, C++ provides support for both procedural and object-oriented programming approaches.
17. Why do we need the Friend class and function?
Sometimes, there is a need for allowing a particular class to access private or protected members of a class. The solution is a friend class, which can access the protected and private members of the class in which it is declared as a friend.

Similar to the friend class, a friend function is able to access private and protected class members. A friend function can either be a global function or a method of some class.

Some important points about friend class and friend function:

Friendship is not inherited.
Friendship isn’t mutual, i.e., if some class called riend is a friend of some other class called NotAFriend, then it doesn’t automatically become a friend of the Friend class.
The total number of friend classes and friend functions should be limited in a program as the overabundance of the same might lead to a depreciation of the concept of encapsulation of separate classes, which is an inherent and desirable quality of object-oriented programming.
18. What is Operator Overloading?
Operating overloading is when operators have different implementations depending on the arguments passed. It is a type of polymorphism.

19. What is Polymorphism?


Polymorphism is the ability of a variable, function, or object to take on multiple forms. 

Intermediate Level Interview Questions
20. Explain vTable and vptr.
vTable is a table containing function pointers. Every class has a vTable. vptr is a pointer to vTable. Each object has a vptr. In order to maintain and use vptr and vTable, the C++ compiler adds additional code at two places:

In every constructor – This code sets vptr:
Of the object being created
To point to vTable of the class
Code with the polymorphic functional call – At every location where a polymorphic call is made, the compiler inserts code in order to first look for vptr using the base class pointer or reference. The vTable of a derived class can be accessed once the vptr is successfully fetched. The address of the derived class function show() is accessed and called using the vTable.
21. How is function overloading different from operator overloading?
Function overloading allows two or more functions with different types and number of parameters to have the same name. On the other hand, operator overloading allows for redefining the way an operator works for user-defined types.


22. Is it possible for a C++ program to be compiled without the main() function?
Yes, it is possible. However, as the main() function is essential for the execution of the program, the program will stop after compiling and will not execute.

23. What is a destructor?
A destructor is the member function of the class. It has the same name as the class name and is also prefixed with a tilde symbol. It can be executed automatically whenever an object loses its scope. A destructor cannot be overloaded, and it has the only form without the parameters.

24. What is the default constructor?
The compiler provides a constructor to every class in case the provider does not offer the same. This is when the programmer provides the constructor with no specific parameters - this is called a default constructor. The code for default constructor can be displayed in the following example.

// Cpp program to illustrate the
// concept of Constructors
#include <iostream>
using namespace std;
class construct {
public:
   int a, b;
   // Default Constructor
   construct()
   {
       a = 10;
       b = 20;
   }
};
int main()
{
   // Default constructor called automatically
   // when the object is created
   construct c;
   cout << "a: " << c.a << endl
        << "b: " << c.b;
   return 1;
}
25. Can we provide one default constructor for our class?
No, we cannot provide one default constructor for our class. When a variable in the class type is set to null, it means that it was never initialized and the outcomes will be zero.

26. What is the main difference between the keyword struct and class?
The keyword struct is used for resembling public members by default, while the keyword class is used for resembling private members by default.

27. What is the output of the following program?
#include <iostream>
using namespace std;
int main() 
{
 int numbers[5], sum = 0;
 cout << "Enter 5 numbers: ";
 for (int i = 0; i < 5; ++i) 
 {
 cin >> numbers[i];
 sum += numbers[i];
 }
 cout << "Sum = " << sum << endl; 
 return 0;
}
The program will ask the user to enter 5 numbers and then present with their sum. For instance,

Enter 5 numbers: 22

25

32

46

66

Sum = 191

28. Explain Virtual Functions and Runtime Polymorphism in C++ with an example.
Any function when accompanying the virtual keyword exhibits the behavior of a virtual function. Unlike normal functions that are called in accordance with the type of pointer or reference used, virtual functions are called as per the type of the object pointed or referred.

In simple terms, virtual functions resolve at runtime, not anytime sooner. Use of virtual functions could also be understood as writing a C++ program leveraging the concept of runtime polymorphism. Things essential to writing a virtual function in C++ are:

A base class
A derived class
A function with the same name in both the classes i.e. the base class and the derived class
A pointer or reference of base class type that points or refers, respectively to an object of the derived class
An example demonstrating the use of virtual functions (or runtime polymorphism at play) is:

#include <iostream>
 using namespace std;
 class Base { 
 public: 
 virtual void show() { cout<<" In Base \n"; } 
 };
 class Derived: public Base { 
 public: 
 void show() { cout<<"In Derived \n"; } 
 }; 
 
 int main(void) { 
 Base *bp = new Derived; 
 bp->show(); // <- Runtime Polymorphism in Action
 return 0;
}

In the aforementioned program bp is a pointer of type Base. A call to bp->show() calls show() function of the Derived class. This is because bp points to an object of the Derived class.

29. What differences separate structure from a class in C++?
There are two important distinctions between a class and a structure in C++. These are:

When deriving a structure from a class or some other structure, the default access specifier for the base class or structure is public. On the contrary, the default access specifier is private when deriving a class.
While the members of a structure are public by default, the members of a class are private by default
30. What is a static member?
Denoted by the static keyword, a static member is allocated storage, in the static storage area, only once during the program lifetime. Some important facts pertaining to the static members are:

Any static member function can’t be virtual
Static member functions don’t have ‘this’ pointer
The const, const volatile, and volatile declaration aren’t available for static member functions
31. What is the Reference variable?
The reference variable in C++ is the name given to the existing variables. The variable name and reference variable point share the same memory location in C++, which helps in updating the original variable using the reference variable. The code can be displayed in the following example.

#include<iostream>
using namespace std;
int main()
{
 int x = 10;
 // ref is a reference to x.
 int& ref = x;
 // Value of x is now changed to 20
 ref = 20;
 cout << "x = " << x << endl ;
 // Value of x is now changed to 30
 x = 30;
 cout << "ref = " << ref << endl ;
 return 0;
}
Advanced C++ Interview Questions
32. Explain the Copy Constructor.
A member function that initializes an object using another object of the same class is known as a copy constructor in C++. They can also be made private. A call to the copy constructor can happen in any of the following 4 scenarios when:

The compiler generates a temporary object
An object is constructed or based on some another object of the same class
An object of the class is returned by value
An object of the class is passed (i.e., to a function) by value as an argument
The general function prototype for the Copy Constructor is:

ClassName (const ClassName &old_obj);

Point(int x1, int y1) { x=x1; y=y1;}

Point(const Point &p2) { x=p2.x; y=p2.y; }

33. Take a look at the following two code examples for printing a vector. Is there any advantage of using one over the other?
Sample Code 1:
vector vec;
/* ... .. ... */
for (auto itr = vec.begin(); itr != vec.end(); itr++) {
 itr->print();
}
Sample Code 2:
vector vec;
/* ... .. ... */
for (auto itr = vec.begin(); itr != vec.end(); ++itr) {
 itr->print();
}
Though both codes will generate the same output, sample code 2 is a more performant option. This is due to the fact that the post-increment ‘itr++’ operator is more expensive than the pre-increment ‘++itr’ operator.

The post-increment operator generates a copy of the element before proceeding with incrementing the element and returning the copy. Moreover, most compilers will automatically optimize sample code 1 by converting it implicitly into sample code 2.

34. Write a program that stores and displays the GPA (Grade Point Average) of a certain number of students, and you need to store and display it using C++. 
#include<iostream>
using namespace std;
int main()
{
 int num;
 cout << "Enter the total number of students: ";
 cin >> num;
 float* ptr;
 ptr = new float[num];
 cout << "Enter the GPA of students." << endl;
 for (int i = 0; i < num; ++i)
 {
 cout << "Student" << i + 1 << ": ";
 cin >> *(ptr + i);
 }
 cout << "\nDisplaying GPA of students." << endl;
 for (int i = 0; i < num; ++i) {
 cout << "Student" << i + 1 << " :" << *(ptr + i) << endl;
 }
 delete [] ptr;
return 0;

}

35. What is a mutable storage class specifier? How can they be used?
A mutable storage class specifier is applied only to the class's non-static and non-constant member variable. It is used for altering the constant class object's member by declaring it. This can be done by using a storage class specifier.

36. What are the differences between a shallow copy and a deep copy?
The differences between a shallow copy and a deep copy are:

Shallow Copy

Deep Copy

Allows memory dumping on a bit-by-bit basis from one object to another

Allows the copy field, which is done by field from one object to another.

Reflects changes made to the new/copied object in the original object. 

Doesn't reflect changes made to the new/copied object in the original object.

37. What is an Abstract class?
An abstract class in C++ is referred to as the base class, which has at least one pure virtual function. In such a function, a person cannot instantiate an abstract class. This way, a pure virtual function is defined by using a pure specifier which is equal to zero during the declaration of the virtual member function in the class declaration. The code sample can be displayed as follows in example.

// An abstract class
class Test
{
// Data members of class
public:
// Pure Virtual Function
virtual void show() = 0;
/* Other members */
};
38. What are the functions of the scope resolution operator?
The functions of the scope resolution operator include the following.

It helps resolve the scope of various global variables.
It helps associate the function with the class when it is defined outside the class.
The code of the scope resolution operator can be displayed as follows.

#include <iostream>
using namespace std;
int my_var = 0;
int main(void) {
int my_var = 0;
::my_var = 1; // set global my_var to 1
my_var = 2; // setlocal my_var to 2
cout << ::my_var << ", " << my_var;
return 0;
}
39. What is a token?
A token is a name given to the various functions in C++ programs. Examples of tokens include a keyword, symbol, string literal, identifier, constant, etc. The following example explains these:

asm      bool    catch      class
const_cast   delete dynamic_cast   explicit
export   false   friend         inline
mutable  namespace   new operator
private  protected   public reinterpret_cast
static_cast  template this       throw
true     try     typeid     typename
using    virtual wchar_t
40. What is the ‘diamond problem’ that occurs with multiple inheritance in C++? 
The diamond problem in C++ represents the inability of the programming language to support hybrid inheritance using multiple and hierarchical inheritance.

Suppose we have a university with some faculty members and some graduate students. A simple inheritance scheme in this scenario might have different types of people in different roles. However, all of them inherit from the same Person class.

The Person class defines an abstract getRole() method that would then be overridden by its subclasses in order to return the correct role type. Things up to this point are simple. However, if we wish to model the role of a TA or Teaching Assistant then things get more complex.

A Teaching Assistant is both a student and a faculty member. The problem generates an inheritance diagram resembling a diamond, hence the name, diamond problem.

Which getRole() implementation should the Teaching Assistant inherit? Graduate Student or the Faculty Member? A potential answer might be to have the Teaching Assistant class override the getRole() method and return a newly-defined role, say TA.

However, such an answer would also be far from complete as it will hide the fact that a teaching assistant is both a faculty member and a graduate student.

</https://hackr.io/blog/cpp-interview-questions>

<https://www.tutorialspoint.com/cplusplus/cpp_interview_questions.htm>

What is the full form of OOPS?
Object Oriented Programming System.

What is a class?
Class is a blue print which reflects the entities attributes and actions. Technically defining a class is designing an user defined data type.

What is an object?
An instance of the class is called as object.

List the types of inheritance supported in C++.
Single, Multilevel, Multiple, Hierarchical and Hybrid.

What is the role of protected access specifier?
If a class member is protected then it is accessible in the inherited class. However, outside the both the private and protected members are not accessible.

What is encapsulation?
The process of binding the data and the functions acting on the data together in an entity (class) called as encapsulation.

What is abstraction?
Abstraction refers to hiding the internal implementation and exhibiting only the necessary details.

What is inheritance?
Inheritance is the process of acquiring the properties of the exiting class into the new class. The existing class is called as base/parent class and the inherited class is called as derived/child class.

Explain the purpose of the keyword volatile.
Declaring a variable volatile directs the compiler that the variable can be changed externally. Hence avoiding compiler optimization on the variable reference.

What is an inline function?
A function prefixed with the keyword inline before the function definition is called as inline function. The inline functions are faster in execution when compared to normal functions as the compiler treats inline functions as macros.

What is a storage class?
Storage class specifies the life or scope of symbols such as variable or functions.

Mention the storage classes names in C++.
The following are storage classes supported in C++

auto, static, extern, register and mutable

What is the role of mutable storage class specifier?
A constant class object’s member variable can be altered by declaring it using mutable storage class specifier. Applicable only for non-static and non-constant member variable of the class.

Distinguish between shallow copy and deep copy.
Shallow copy does memory dumping bit-by-bit from one object to another. Deep copy is copy field by field from object to another. Deep copy is achieved using copy constructor and or overloading assignment operator.

What is a pure virtual function?
A virtual function with no function body and assigned with a value zero is called as pure virtual function.

What is an abstract class in C++?
A class with at least one pure virtual function is called as abstract class. We cannot instantiate an abstract class.

What is a reference variable in C++?
A reference variable is an alias name for the existing variable. Which mean both the variable name and reference variable point to the same memory location. Therefore updation on the original variable can be achieved using reference variable too.

What is role of static keyword on class member variable?
A static variable does exit though the objects for the respective class are not created. Static member variable share a common memory across all the objects created for the respective class. A static member variable can be referred using the class name itself.

Explain the static member function.
A static member function can be invoked using the class name as it exits before class objects comes into existence. It can access only static members of the class.

Name the data type which can be used to store wide characters in C++.
wchar_t

What are/is the operator/operators used to access the class members?
Dot (.) and Arrow ( -> )

Can we initialize a class/structure member variable as soon as the same is defined?
No, Defining a class/structure is just a type definition and will not allocated memory for the same.

What is the data type to store the Boolean value?
bool, is the new primitive data type introduced in C++ language.

What is function overloading?
Defining several functions with the same name with unique list of parameters is called as function overloading.

What is operator overloading?
Defining a new job for the existing operator w.r.t the class objects is called as operator overloading.

Do we have a String primitive data type in C++?
No, it’s a class from STL (Standard template library).

Name the default standard streams in C++.
cin, cout, cerr and clog.

Which access specifier/s can help to achive data hiding in C++?
Private & Protected.

When a class member is defined outside the class, which operator can be used to associate the function definition to a particular class?
Scope resolution operator (::)

What is a destructor? Can it be overloaded?
A destructor is the member function of the class which is having the same name as the class name and prefixed with tilde (~) symbol. It gets executed automatically w.r.t the object as soon as the object loses its scope. It cannot be overloaded and the only form is without the parameters.

What is a constructor?
A constructor is the member function of the class which is having the same as the class name and gets executed automatically as soon as the object for the respective class is created.

What is a default constructor? Can we provide one for our class?
Every class does have a constructor provided by the compiler if the programmer doesn’t provides one and known as default constructor. A programmer provided constructor with no parameters is called as default constructor. In such case compiler doesn’t provides the constructor.

Which operator can be used in C++ to allocate dynamic memory?
‘new’ is the operator can be used for the same.

What is the purpose of ‘delete’ operator?
‘delete’ operator is used to release the dynamic memory which was created using ‘new’ operator.

Can I use malloc() function of C language to allocate dynamic memory in C++?
Yes, as C is the subset of C++, we can all the functions of C in C++ too.

Can I use ‘delete’ operator to release the memory which was allocated using malloc() function of C language?
No, we need to use free() of C language for the same.

What is a friend function?
A function which is not a member of the class but still can access all the member of the class is called so. To make it happen we need to declare within the required class following the keyword ‘friend’.

What is a copy constructor?
A copy constructor is the constructor which take same class object reference as the parameter. It gets automatically invoked as soon as the object is initialized with another object of the same class at the time of its creation.

Does C++ supports exception handling? If so what are the keywords involved in achieving the same.
C++ does supports exception handling. try, catch & throw are keyword used for the same.

Explain the pointer – this.
This, is the pointer variable of the compiler which always holds the current active object’s address.

What is the difference between the keywords struct and class in C++?
By default the members of struct are public and by default the members of the class are private.

Can we implement all the concepts of OOPS using the keyword struct?
Yes.

What is the block scope variable in C++?
A variable whose scope is applicable only within a block is said so. Also a variable in C++ can be declared anywhere within the block.

What is the role of the file opening mode ios::trunk?
If the file already exists, its content will be truncated before opening the file.

What is the scope resolution operator?
The scope resolution operator is used to

Resolve the scope of global variables.
To associate function definition to a class if the function is defined outside the class.
What is a namespace?
A namespace is the logical division of the code which can be used to resolve the name conflict of the identifiers by placing them under different name space.

What are command line arguments?
The arguments/parameters which are sent to the main() function while executing from the command line/console are called so. All the arguments sent are the strings only.

What is a class template?
A template class is a generic class. The keyword template can be used to define a class template.

How can we catch all kind of exceptions in a single catch block?
The catch block with ellipses as follows

catch(…) 
{
}
What is keyword auto for?
By default every local variable of the function is automatic (auto). In the below function both the variables ‘i’ and ‘j’ are automatic variables.

void f() 
{
   int i;
  
   auto int j;
}
NOTE − A global variable can’t be an automatic variable.

What is a static variable?
A static local variables retains its value between the function call and the default value is 0. The following function will print 1 2 3 if called thrice.

void f() 
{ 
   static int i; 
   
   ++i; 
   printf(“%d “,i); 
}
If a global variable is static then its visibility is limited to the same source code.

What is the purpose of extern storage specifier.
Used to resolve the scope of global symbol

#include <iostream>

using namespace std;	
main() {
   extern int i;
      
   cout<<i<<endl;
}
int i = 20;
What is the meaning of base address of the array?
The starting address of the array is called as the base address of the array.

When should we use the register storage specifier?
If a variable is used most frequently then it should be declared using register storage specifier, then possibly the compiler gives CPU register for its storage to speed up the look up of the variable.

Can a program be compiled without main() function?
Yes, it can be but cannot be executed, as the execution requires main() function definition.

Where an automatic variable is stored?
Every local variable by default being an auto variable is stored in stack memory

What is a container class?
A class containing at least one member variable of another class type in it is called so.

What is a token?
A C++ program consists of various tokens and a token is either a keyword, an identifier, a constant, a string literal, or a symbol.

What is a preprocessor?
Preprocessor is a directive to the compiler to perform certain things before the actual compilation process begins.

What are command line arguments?
The arguments which we pass to the main() function while executing the program are called as command line arguments. The parameters are always strings held in the second argument (below in args) of the function which is array of character pointers. First argument represents the count of arguments (below in count) and updated automatically by operating system.

main( int count, char *args[]) {
}
What are the different ways of passing parameters to the functions? Which to use when?
Call by value − We send only values to the function as parameters. We choose this if we do not want the actual parameters to be modified with formal parameters but just used.

Call by address − We send address of the actual parameters instead of values. We choose this if we do want the actual parameters to be modified with formal parameters.

Call by reference − The actual parameters are received with the C++ new reference variables as formal parameters. We choose this if we do want the actual parameters to be modified with formal parameters.

What is reminder for 5.0 % 2?
Error, It is invalid that either of the operands for the modulus operator (%) is a real number.

Which compiler switch to be used for compiling the programs using math library with g++ compiler?
Opiton –lm to be used as > g++ –lm <file.cpp>

Can we resize the allocated memory which was allocated using ‘new’ operator?
No, there is no such provision available.

Who designed C++ programming language?
Bjarne Stroustrup.

Which operator can be used to determine the size of a data type/class or variable/object?
sizeof

How can we refer to the global variable if the local and the global variable names are same?
We can apply scope resolution operator (::) to the for the scope of global variable.

What are valid operations on pointers?
The only two permitted operations on pointers are

Comparision ii) Addition/Substraction (excluding void pointers)

What is recursion?
Function calling itself is called as recursion.

What is the first string in the argument vector w.r.t command line arguments?
Program name.

What is the maximum length of an identifier?
Ideally it is 32 characters and also implementation dependent.

What is the default function call method?
By default the functions are called by value.

What are available mode of inheritance to inherit one class from another?
Public, private & protected

What is the difference between delete and delete[]?
Delete[] is used to release the array allocated memory which was allocated using new[] and delete is used to release one chunk of memory which was allocated using new.

Does an abstract class in C++ need to hold all pure virtual functions?
Not necessarily, a class having at least one pure virtual function is abstract class too.

Is it legal to assign a base class object to a derived class pointer?
No, it will be error as the compiler fails to do conversion.

What happens if an exception is thrown outside a try block?
The program shall quit abruptly.

Are the exceptions and error same?
No, exceptions can be handled whereas program cannot resolve errors.

What is function overriding?
Defining the functions within the base and derived class with the same signature and name where the base class’s function is virtual.

Which function is used to move the stream pointer for the purpose of reading data from stream?
seekg()

Which function is used to move the stream pointer for the purpose of writing data from stream?
seekp()

Are class functions taken into consideration as part of the object size?
No, only the class member variables determines the size of the respective class object.

Can we create and empty class? If so what would be the size of such object.
We can create an empty class and the object size will be 1.

What is ‘std’?
Default namespace defined by C++.

What is the full form of STL?
Standard template library

What is ‘cout’?
cout is the object of ostream class. The stream ‘cout’ is by default connected to console output device.

What is ‘cin’?
cin is the object of istream class. The stream ‘cin’ is by default connected to console input device.

What is the use of the keyword ‘using’?
It is used to specify the namespace being used in.

If a pointer declared for a class, which operator can be used to access its class members?
Arrow (->) operator can be used for the same

What is difference between including the header file with-in angular braces < > and double quotes “ “
If a header file is included with in < > then the compiler searches for the particular header file only with in the built in include path. If a header file is included with in “ “, then the compiler searches for the particular header file first in the current working directory, if not found then in the built in include path

S++ or S = S+1, which can be recommended to increment the value by 1 and why?
S++, as it is single machine instruction (INC) internally.

What is the difference between actual and formal parameters?
The parameters sent to the function at calling end are called as actual parameters while at the receiving of the function definition called as formal parameters.

What is the difference between variable declaration and variable definition?
Declaration associates type to the variable whereas definition gives the value to the variable.

Which key word is used to perform unconditional branching?
goto.

Is 068 a valid octal number?
No, it contains invalid octal digits.

What is the purpose of #undef preprocessor?
It will be used to undefine an existing macro definition.

Can we nest multi line comments in a C++ code?
No, we cannot.

What is a virtual destructor?
A virtual destructor ensures that the objects resources are released in the reverse order of the object being constructed w.r.t inherited object.

What is the order of objects destroyed in the memory?
The objects are destroyed in the reverse order of their creation.

What is a friend class?
A class members can gain accessibility over other class member by placing the class declaration prefixed with the keyword ‘friend’ in the destination class.

</https://www.tutorialspoint.com/cplusplus/cpp_interview_questions.htm>

<https://www.interviewkickstart.com/interview-questions/cpp-interview-questions-for-experienced-developers>
Q1. Why would you choose C++ over other programming languages?
The following prominent advantages of C++ make it software developers' choice:

It is a portable language and can allow developers to run it on any platform and operating system.
It has abundant function libraries.
C++ supports inheritance, polymorphism, and friend functions.
Data hiding in C++ language provides additional data security.
Learn how C++ is different from the C programming language. 

Q2. What do you understand about scopes in C++?
This is one of the most commonly asked C++ interview questions and answers. The area wherein the variable is active is referred to as scope. Thus, you can declare, define, and use the variable in scope. C++ has the following two types of scopes:

Local scope: When a variable is declared inside the block of code and remains active only inside that block, it is said to be in a local scope and is accessible outside the block.
Global scope: When a variable is declared at the top of the program, it is in a global scope and is accessible throughout the program.
Q3. What tokens does the C++ language support? 
C++ supports the following types of tokens:

Keyword
Constant
Identifier
Literal
Symbol
Q4. How is the assignment operator ( = ) different from the equal to operator ( == )?
The assignment operator ( = ) assigns the value to the variable and is sometimes used in complex equations.

The 'equal to' operator ( == ) is an equality operator used to compare two values. It returns true if they are equal; else, it returns false.

Q5. Explain comments in context with C++?
Comments are the source code that the compiler ignores, and they are not a part of programs. The purpose of comments is to inform the programmer about additional information. It provides details about the source code. There are two types of comments in C++:

Single line comment: It uses "//"for commenting, and the compiler ignores everything after "//"in the line.
Multiline comment or block comment: It uses “ /* ” “ */ “ for commenting and the compiler ignores everything between “ /* “ “ */ “.
Q6. What is containership?
It is one of the most important C++ interview questions and answers concepts. You can contain an object of one class into another, and that object will be a member of the other class. This relationship between classes wherein one class contains the object of another class is referred to as containership. 

Q7. What is data hiding?
The process of hiding elements of a program's code from object members is called data hiding. It ensures controlled data access and objects integrity. It also prevents unintentional or intended changes to the program.

Q8. What is the use of getline in C++?
The C++ getline() is a standard library in-built function and it is defined in the <string.h> header file. It allows accepting and reading single and multiple lines. 

Q9. What is a singleton design pattern?
Design patterns are reusable solutions that you can apply to recurring Object-Oriented Design problems. Singleton design patterns fall under the category of Creational Design Patterns. This pattern helps design a class with a maximum of a single instance at any time. It cannot be instantiated further. 

The concept of a singleton design pattern can be applied to creating a logger or hardware interface class. 

Q10. What operators cannot be overloaded?
The following operators cannot be overloaded:

?: – conditional operator
.* – dereferencing operator
sizeof – sizeof operator
:: – scope resolution operator
. – Dot operator
-> – member dereferencing operator
Q11. What do you understand about RTTI?
RTTI stands for Run-time type information. This mechanism gives information about an object's data type at runtime. It is available only for classes that have at least one virtual function. You can determine the type of an object during program runtime execution.

Q12. What is the sparse matrix?
An array of elements wherein many elements have a value of zero is called a sparse matrix. For instance, if you are given a matrix with several elements and the number of zeroes is more than half the elements of the matrix, then it is a sparse matrix.

Q13. What do you understand about smart pointers in C++?
Smart pointers are employed in garbage collection to ensure no memory leaks. If you use smart pointers, you need not call delete for any memory allocated dynamically as it is automatically deallocated. You can implement smart pointers in C++11 and higher versions. C++11 has the following four kinds of smart pointers:

auto_ptr
unique_ptr
shared_ptr 
weak_ptr.
Q14. What is the role of this pointer and void pointer?
This pointer: The 'this pointer' is present in the member functions of every object. It points to the object itself and can be used to access the object's data. 

Void pointer: A pointer that has no data type associated with it is called a void pointer. You can assign any type of pointer to a void pointer, but the reverse isn't true unless you use it as follows

str=(char*) ptr;.

Q15. What do you understand about pure virtual functions?
A virtual function is a member function in the base class that can be redefined in a derived class. It can be declared using the virtual keyword. On the contrary, a pure virtual function has no implementation. It has no body and is declared by assigning 0. 

Q16. Is it possible to call a virtual function from a constructor?
Yes, you can call a virtual function from a constructor. However, the behavior differs in that case. When you call a virtual function, the virtual call is resolved at runtime. The virtual machine does not work within the constructor.

Take a look at some more C++ Interview Questions and Answers to prepare better.

Frequently Asked C++ Interview Questions for Experienced Professionals
You should be prepared for advanced C++ interview questions and answers if you are applying for senior roles. Although interview rounds of senior positions have mostly programming and behavioral questions, you will also be asked a few advanced theoretical questions. Take a look at this list of questions to brush up on the crucial C++ concepts.

What is a copy constructor in C++?
How is modularity introduced in C++?
What is the difference between method overloading and method overriding?
What is the size of an empty class in C++?
Explain the following concepts in C++:
Inheritance 
Abstraction
Encapsulation 
Polymorphism
Friend Function
Data Binding
Virtual Function
Access Specifiers
Overloading
Destructor
Constructor
C++ Programming Interview Questions for Practice
Coding rounds are often a part of technical interviews wherein you must solve problems on data structures and algorithms. To ace C++ programming interview questions, you must have a good command of the language and diligent practice. The following topics are important for coding questions:

Arrays, strings, and linked lists
Sorting algorithms — quicksort, merge sort, heap sort, etc.
Hash tables and queues
Recursion
Trees and graphs
Graph algorithms, including greedy algorithms
Dynamic programming 
Here are a few C++ coding questions for practice:

Write a program in C++ to print the first non-repeated character in the given string.
Write a program in C++ to find duplicate numbers in a given array that contains multiple duplicates.
Write a program to print the date in dd/mm/yy format.
How would you check if a given linked list contains a cycle? Also, find the initial node of the cycle.
Write a program to reverse a singly linked list without recursion. 
How would you implement a binary search tree? 
Write a program to traverse a given binary tree in preorder without recursion.
How would you implement a merge sort algorithm? 
You can check out the Problems Page for more C++ interview questions and answers to practice for technical interviews.  

FAQs on C++ Interview Questions and Answers
Q1. How do I prepare for C++ interview questions and answers?

You should begin your preparation by brushing up on core programming concepts and move on to practicing programming problems. You can also enroll in mock interviews and practice mocks with hiring managers who are closely acquainted with the FAANG companies' interview process. Learn important tips on how to prepare for C++ interviews here.

Q2. What topics are important for C++ interview questions and answers?

You should be prepared for questions on crucial C++ concepts, including methods, events in C++, lists, inheritance, polymorphism, abstraction, data binding, and commands to crack the most challenging C++ interview questions and answers.

Q3. Can I use C++ for the FAANG company's coding interviews?

Yes, you can use C++ in coding interview rounds. Top tech companies, including Microsoft, LinkedIn, PayPal, and Amazon, list C++ as one of their main programming languages for coding interviews. C++ has become one of the most sought-after skills in modern developers at FAANG+ companies. 

Q4. What positions am I eligible for with C++ programming skills?

You can make a career in the following roles with C++ programming skills: Junior/Senior Programmer, Software Developer, Quality Analyst, Game Programmer, Software Developer Engineer, C++ Analyst, and Programming Architect.

Q5. What is the average salary of C++ developers in the US?

The average base salary of a C++ developer is $116,987 per annum in the United States. You can expect a higher salary in US cities like Orlando, New York, and San Francisco (Source: Indeed.com). The salary increases according to your experience and based on your performance. The higher the experience, the higher the salary will be.

Gear Up for Your Next Tech Interview
Preparing for technical interviews, especially the challenging ones, steers you on the path to becoming a better software professional with improved coding, problem-solving, and behavioral skills. You become more confident at taking and cracking interviews. 

At Interview Kickstart, we've trained thousands of coding engineers, software developers, and data scientists to land dream offer at the biggest companies, including Google, Facebook, Amazon, Apple, Microsoft, and Netflix. Check out some reviews to know more.

Sign up now to uplevel your career!

‍</https://www.interviewkickstart.com/interview-questions/cpp-interview-questions-for-experienced-developers>

<https://www.softwaretestinghelp.com/cpp-interview-questions/>

Q #1) What is the basic structure of a C++ program?

Answer: The basic structure of a C++ program is shown below:

#include<iostream.h>
int main()
{
                cout<<”Hello,World!”;
                return 0;
}
The first line that begins with “#” is a preprocessor directive. In this case, we are using include as a directive which tells the compiler to include a header while “iostream.h” will be used for basic input/output later in the program.

The next line is the “main” function that returns an integer. The main function is the starting point of execution for any C++ program. Irrespective of its position in the source code file, the contents of the main function are always executed first by the C++ compiler.

In the next line, we can see open curly braces that indicate the start of a block of code. After this, we see the programming instruction or the line of code that uses the count which is the standard output stream (its definition is present in iostream.h).

This output stream takes a string of characters and prints it to a standard output device. In this case, it is, “Hello, World!”. Please note that each C++ instruction ends with a semicolon (;), which is very much necessary, and omitting it will result in compilation errors.

Before closing the braces}, we see another line “return 0;”. This is the returning point to the main function.

Every C++ program will have a basic structure as shown above with a preprocessor directive, the main function declaration followed by a block of code, and then a returning point to the main function which indicates successful execution of the program.

Q #2) What are the Comments in C++?

Answer: Comments in C++ are simply a piece of source code ignored by the compiler. They are only helpful for a programmer to add a description or additional information about their source code.

In C++ there are two ways to add comments:

//single-line comment
/* block comment */
The first type will discard everything after the compiler encounters “//”. In the second type, the compiler discards everything between “/*” and “*/”.

Variables, Data Types, And Constants
Q #3) Difference between Declaration and Definition of a variable.

Answer: The declaration of a variable is merely specifying the data type of a variable and the variable name. As a result of the declaration, we tell the compiler to reserve the space for a variable in the memory according to the data type specified.

Example:

int Result;
char c;
int a,b,c;
All the above are valid declarations. Also, note that as a result of the declaration, the value of the variable is undetermined.

Whereas, a definition is an implementation/instantiation of the declared variable where we tie up appropriate value to the declared variable so that the linker will be able to link references to the appropriate entities.

From the above Example,

Result = 10;

C = ‘A’;

These are valid definitions.

Q #4) Comment on the Local and Global scope of a variable.

Answer: The scope of a variable is defined as the extent of the program code within which the variable remains active i.e. it can be declared, defined, or worked with.

There are two types of scope in C++:

Local Scope: A variable is said to have a local scope or is local when it is declared inside a code block. The variable remains active only inside the block and is not accessible outside the code block.
Global Scope: A variable has a global scope when it is accessible throughout the program. A global variable is declared on top of the program before all the function definitions.
Example:

#include <iostream.h>
Int globalResult=0; //global variable
int main()
{
Int localVar = 10; //local variable.
….. 
 
}
Q #5) What is the precedence when there are a Global variable and a Local variable in the program with the same name?

Answer: Whenever there is a local variable with the same name as that of a global variable, the compiler gives precedence to the local variable.

Example:

#include <iostream.h>
 int globalVar = 2;
int main()
{
 int globalVar = 5;
 cout<<globalVar<<endl;
}
The output of the above code is 5. This is because, although both the variables have the same name, the compiler has given preference to the local scope.

Q #6) When there are a Global variable and a Local variable with the same name, how will you access the global variable?

Answer: When there are two variables with the same name but different scopes, i.e. one is a local variable and the other is a global variable, the compiler will give preference to a local variable.

In order to access the global variable, we make use of a “scope resolution operator (::)”. Using this operator, we can access the value of the global variable.

Example:

#include<iostream.h>
int x= 10;
int main()
{
 int x= 2;
 cout<<”Global Variable x = “<<::x;
 cout<<”\nlocal Variable x= “<<x;
}
Output:

Global Variable x = 10
local Variable x= 2

Q #7) How many ways are there to initialize an int with a Constant?

Answer: There are two ways:

The first format uses traditional C notation.
int result = 10;
The second format uses the constructor notation.
int result (10);
Constants
Q #8) What is a Constant? Explain with an example.

Answer: A constant is an expression that has a fixed value. They can be divided into integer, decimal, floating-point, character, or string constants depending on their data type.

Apart from the decimal, C++ also supports two more constants i.e. octal (to the base 8) and hexadecimal (to the base 16) constants.

Examples of Constants:

75 //integer (decimal)
0113 //octal
0x4b //hexadecimal
3.142 //floating point
‘c’ //character constant
“Hello, World” //string constant
Note: When we have to represent a single character, we use single quotes and when we want to define a constant with more than one character, we use double quotes.

Q #9) How do you define/declare constants in C++?


Answer: In C++, we can define our own constants using the #define preprocessor directive.

#define Identifier value

Example:

#include<iostream.h>
#define PI 3.142
int main ()
{
                 float radius =5, area;
                 area = PI * r * r;
                 cout<<”Area of a Circle = “<<area;
}
Output: Area of a Circle = 78.55

As shown in the above example, once we define a constant using #define directive, we can use it throughout the program and substitute its value.

We can declare constants in C++ using the “const” keyword. This way is similar to that of declaring a variable, but with a const prefix.

Examples of declaring a constant

const int pi = 3.142;
const char c = “sth”;
const zipcode = 411014;

In the above examples, whenever the type of a constant is not specified, the C++ compiler defaults it to an integer type.

Operators
Q #10) Comment on Assignment Operator in C++.

Answer: The assignment operator in C++ is used to assign a value to another variable.

a = 5;

This line of code assigns the integer value 5 to variable a.

The part at the left of the =operator is known as an lvalue (left value) and the right as rvalue (right value). Lvalue must always be a variable whereas the right side can be a constant, a variable, the result of an operation, or any combination of them.

The assignment operation always takes place from the right to left and never at the inverse.

One property which C++ has over the other programming languages is that the assignment operator can be used as the rvalue (or part of an rvalue) for another assignment.

Example:

a = 2 + (b = 5);

is equivalent to:

b = 5;
a = 2 + b;

This means, first assign 5 to variable b and then assign to a, the value 2 plus the result of the previous expression of b(that is 5), leaving a with a final value of 7.

Thus, the following expression is also valid in C++:

a = b = c = 5;

assign 5 to variables a, b and c.

Q #11) What is the difference between equal to (==) and Assignment Operator (=)?

Answer: In C++, equal to (==) and assignment operator (=) are two completely different operators.

Equal to (==) is an equality relational operator that evaluates two expressions to see if they are equal and returns true if they are equal and false if they are not.

The assignment operator (=) is used to assign a value to a variable. Hence, we can have a complex assignment operation inside the equality relational operator for evaluation.

Q #12) What are the various Arithmetic Operators in C++?

Answer: C++ supports the following arithmetic operators:

+ addition
– subtraction
* multiplication
/ division
% module
Let’s demonstrate the various arithmetic operators with the following piece of code.

Example:

#include <iostream.h>
int main ()
{
              int a=5, b=3;
cout<<”a + b = “<<a+b;
cout<”\na – b =”<<a-b;
cout<<”\na * b =”<<a*b;
cout<<”\na / b =”<<a/b;
cout<<”\na % b =“<<a%b;
 
return 0;
 }
Output:

a + b = 8
a – b =2
a * b =15
a / b =2
a % b=1

As shown above, all the other operations are straightforward and the same as actual arithmetic operations, except the modulo operator which is quite different. Modulo operator divides a and b and the result of the operation is the remainder of the division.

Q #13) What are the various Compound Assignment Operators in C++?

Answer: Following are the Compound assignation operators in C++:

+=, -=, *=, /=, %=, >>=, <<=, &=, ^=,|=

The compound assignation operator is one of the most  important features of C++ language which allow us to change the value of a variable with one of the basic operators:

Example:

value += increase; is equivalent to value = value + increase;
if base_salary is a variable of type int.
               int base_salary = 1000;
               base_salary += 1000; #base_salary = base_salary + 1000
               base_salary *= 5; #base_salary = base_salary * 5;
Q #14) State the difference between Pre and Post Increment/Decrement Operations.

Answer: C++ allows two operators i.e ++ (increment) and –(decrement), that allow you to add 1 to the existing value of a variable and subtract 1 from the variable respectively. These operators are in turn, called increment (++) and decrement (–).

Example:

a=5;
a++;

The second statement, a++, will cause 1 to be added to the value of a. Thus a++ is equivalent to

a = a+1; or
a += 1;

A unique feature of these operators is that we can prefix or suffix these operators with the variable. Hence, if a is a variable and we prefix the increment operator it will be

++a;

This is called Pre-increment. Similarly, we have pre-decrement as well.

If we prefix the variable a with an increment operator, we will have,

a++;

This is the post-increment. Likewise, we have post-decrement too.

The difference between the meaning of pre and post depends upon how the expression is evaluated and the result is stored.

In the case of the pre-increment/decrement operator, the increment/decrement operation is carried out first, and then the result is passed to an lvalue. Whereas for post-increment/decrement operations, the lvalue is evaluated first and then increment/decrement is performed accordingly.

Example:

a = 5; b=6;
++a;       #a=6
b–;         #b=6
–a;         #a=5
b++;      #6

I/O through Console
Q #15) What are the Extraction and Insertion operators in C++? Explain with examples.

Answer: In the iostream.h library of C++, cin, and cout is the two data streams that are used for input and output respectively. Cout is normally directed to the screen and cin is assigned to the keyboard.

“cin” (extraction operator): By using overloaded operator >> with cin stream, C++ handles the standard input.

int age;
cin>>age;
As shown in the above example, an integer variable ‘age’ is declared and then it waits for cin (keyboard) to enter the data. “cin” processes the input only when the RETURN key is pressed.

“cout” (insertion operator): This is used in conjunction with the overloaded << operator. It directs the data that followed it into the cout stream.

Example:

cout<<”Hello, World!”;
 cout<<123;
Control Structures And Functions
Control Structures And Loops
Q #16) What is the difference between a while and a do while loop? Explain with examples.

Answer: The format of the while loop in C++ is:

While (expression)
{statements;}

The statement block under while is executed as long as the condition in the given expression is true.

Example:

#include <iostream.h>
 int main()
{
               int n;
               cout<<”Enter the number : “;
               cin>>n;
              while(n>0)
              {
                              cout<<” “<<n;
                              --n;
              }
              cout<<”While loop complete”;
 }
In the above code, the loop will directly exit if n is 0. Thus in the while loop, the terminating condition is at the beginning of the loop and if it’s fulfilled, no iterations of the loop are executed.

Next, we consider the do-while loop.

The general format of do-while is:

do {statement;} while(condition);

Example:

#include<iostream.h>
int main()
{
               int n;
               cout<<”Enter the number : “;
               cin>>n;
               do {
                          cout<<n<<”,”;
                          --n;
                     }while(n>0);
                    cout<<”do-while complete”;
}
In the above code, we can see that the statement inside the loop is executed at least once as the loop condition is at the end. These are the main differences between the while and the do-while.

In the case of the while loop, we can directly exit the loop at the beginning, if the condition is not met whereas in the do-while loop we execute the loop statements at least once.

Functions
Q #17) What do you mean by ‘void’ return type?

Answer: All functions should return a value as per the general syntax.

However, in case, if we don’t want a function to return any value, we use “void” to indicate that. This means that we use “void” to indicate that the function has no return value or it returns “void”.

Example:

void myfunc()
{
                         Cout<<”Hello,This is my function!!”;
}
int main()
{
myfunc();
return 0;
}
Q #18) Explain Pass by Value and Pass by Reference.

Answer: While passing parameters to the function using “Pass by Value”, we pass a copy of the parameters to the function.

Hence, whatever modifications are made to the parameters in the called function are not passed back to the calling function. Thus the variables in the calling function remain unchanged.

Example:

void printFunc(int a,int b,int c)
{
                  a *=2;
                  b *=2;
                  c *=2;
}
 
int main()
 
{
 
                 int x = 1,y=3,z=4;
                 printFunc(x,y,z);
                 cout<<”x = “<<x<<”\ny = “<<y<<”\nz = “<<z;
}
Output:

x=1
y=3
z=4

As seen above, although the parameters were changed in the called function, their values were not reflected in the calling function as they were passed by value.

However, if we want to get the changed values from the function back to the calling function, then we use the “Pass by Reference” technique.

To demonstrate this we modify the above program as follows:

void printFunc(int& a,int& b,int& c)
{
                              a *=2;
                              b *=2;
                              c *=2;
}
  int main()
{
                  int x = 1,y=3,z=4;
                  printFunc(x,y,z);
                   cout<<”x = “<<x<<”\ny = “<<y<<”\nz = “<<z;
}
Output:
x=2
y=6
z=8

As shown above, the modifications done to the parameters in the called functions are passed to the calling function when we use the “Pass by reference” technique. This is because using this technique we do not pass a copy of the parameters but we actually pass the variable’s reference itself.

Q #19) What are Default Parameters? How are they evaluated in the C++ function?

Answer: A default Parameter is a value that is assigned to each parameter while declaring a function.

This value is used if that parameter is left blank while calling the function. To specify a default value for a particular parameter, we simply assign a value to the parameter in the function declaration.

If the value is not passed for this parameter during the function call, then the compiler uses the default value provided. If a value is specified, then this default value is stepped on and the passed value is used.

Example:

int multiply(int a, int b=2)
{
              int r;
              r = a * b;
              return r;
} 
  
int main()
 {
  
             Cout<<multiply(6);
             Cout<<”\n”;
             Cout<<multiply(2,3);
 }
Output:

12
6

As shown in the above code, there are two calls to the multiply function. In the first call, only one parameter is passed with a value. In this case, the second parameter is the default value provided. But in the second call, as both the parameter values are passed, the default value is overridden and the passed value is used.

Q #20) What is an Inline function in C++?

Answer: Inline function is a function that is compiled by the compiler as the point of calling the function and the code is substituted at that point. This makes compiling faster. This function is defined by prefixing the function prototype with the keyword “inline”.

Such functions are advantageous only when the code of the inline function is small and simple. Although a function is defined as Inline, it is completely compiler dependent to evaluate it as inline or not.

Advanced-Data Structure
Arrays
Q #21) Why are arrays usually processed with for loop?

Answer: Array uses the index to traverse each of its elements.

If A is an array then each of its elements is accessed as A[i]. Programmatically, all that is required for this to work is an iterative block with a loop variable i that serves as an index (counter) incrementing from 0 to A.length-1.

This is exactly what a loop does and this is the reason why we process arrays using for loops.

Q #22) State the difference between delete and delete[].

Answer: “delete[]” is used to release the memory allocated to an array that was allocated using new[]. “delete” is used to release one chunk of memory which was allocated using new.

Q #23) What is wrong with this code?

T *p = new T[10];
delete p;

Answer: The above code is syntactically correct and will compile fine.

The only problem is that it will just delete the first element of the array. Though the entire array is deleted, only the destructor of the first element will be called and the memory for the first element is released.

Q #24) What’s the order in which the objects in an array are destructed?

Answer: Objects in an array are destructed in the reverse order of construction: First constructed, last destructed.

In the following Example, the order for destructors will be a[9], a[8], …, a[1], a[0]:

voiduserCode()
{
                 Car a[10];
                  ...
}
Pointers
Q #25) What is wrong with this code?

T *p = 0;
delete p;

Answer: In the above code, the pointer is a null pointer. Per the C++ 03 standard, it’s perfectly valid to call delete on a NULL pointer. The delete operator would take care of the NULL check internally.

Q #26) What is a Reference Variable in C++?

Answer: A reference variable is an alias name for the existing variable. This means that both the variable name and the reference variable point to the same memory location. Hence, whenever the variable is updated, the reference is updated too.

Example:

int a=10;
 int& b = a;
Here, b is the reference of a.

Suggested reading =>> Most Common Data Structure Interview Questions

Storage Classes
Q #27) What is a Storage Class? Mention the Storage Classes in C++.

Answer: Storage class determines the life or scope of symbols such as variables or functions.

C++ supports the following storage classes:

Auto
Static
Extern
Register
Mutable
Q #28) Explain the Mutable Storage class specifier.

Answer: The variable of a constant class object’s member cannot be changed. However, by declaring the variables as “mutable”, we can change the values of these variables.

Q #29) What is the keyword auto for?

Answer: By default, every local variable of the function is automatic i.e. auto. In the below function both the variables ‘i’ and ‘j’ are automatic variables.

void f()
 {
 int i; 
 auto int j;
 }
NOTE: A global variable is not an automatic variable.

Q #30) What is a Static Variable?

Answer: A static variable is a local variable that retains its value across the function calls. Static variables are declared using the keyword “static”. Numeric variables which are static have the default value as zero.

The following function will print 1 2 3 if called thrice.

void f()
{
static int i;
++i;
printf(“%d “,i);
}
If a global variable is static, then its visibility is limited to the same source code.

Q #31) What is the purpose of the Extern Storage Specifier?

Answer: “Extern” specifier is used to resolve the scope of a global symbol.

#include <iostream >
 using nam espace std;
 main()
 {
extern int i;
 cout<<i<<endl;
 }
 int i=20;
In the above code, “i” can be visible outside the file where it is defined.


Q #32) Explain Register Storage Specifier.

Answer: “Register” variable should be used whenever the variable is used. When a variable is declared with a “register” specifier, then the compiler gives a CPU register for its storage to speed up the lookup of the variable.

Q #33) When to use “const” reference arguments in a function?

Answer: Using “const” reference arguments in a function is beneficial in several ways:

“const” protects from programming errors that could alter data.
As a result of using “const”, the function is able to process both const and non-const actual arguments, which is not possible when “const” is not used.
Using a const reference will allow the function to generate and use a temporary variable in an appropriate manner.
Structure & User-Defined Data Types
Q #34) What is a Class?

Answer: Class is a user-defined data type in C++. It can be created to solve a particular kind of problem. After creation, the user is not required to know the details of the working of a class.

In general, class acts as a blueprint of a project and can include various parameters and functions or actions operating on these parameters. These are called the members of the class.

Q #35) Difference between Class and Structure.

Answer:

Structure: In C language, the structure is used to bundle different types of data types together. The variables inside a structure are called the members of the structure. These members are by default public and can be accessed by using the structure name followed by a dot operator and then the member name.

Class: Class is a successor of the Structure. C++ extends the structure definition to include the functions that operate on its members. By default all the members of the class are private.

Object-Oriented Programming With C++
Classes, Constructors, Destructors
Q #36) What is Namespace?

Answer: Namespace allows us to group a set of global classes, objects, and/or functions under a specific name.

The general form to use namespaces is:

namespace identifier { namespace-body }

Where identifier is any valid identifier and the namespace-body is the set of classes, objects, and functions that are included within the namespace. Namespaces are especially useful in cases where there is a possibility for more than one object to have the same name, resulting in name clashes.

Q #37) What is the use of a ‘using’ declaration?

Answer: Using Declaration is used to refer to a name from the namespace without the scope resolution operator.

Q #38) What is Name Mangling?

Answer: C++ compiler encodes the parameter types with function/method into a unique name. This process is called name mangling. The inverse process is called demangling.

Example:

A::b(int, long) const is mangled as ‘b__C3Ail’.

For a constructor, the method name is left out.

That is A:: A(int, long) const is mangled as ‘C3Ail’.

Q #39) What is the difference between an Object and a Class?

Answer: Class is a blueprint of a project or problem to be solved and consists of variables and methods. These are called the members of the class. We cannot access methods or variables of the class on its own unless they are declared static.

In order to access the class members and put them to use, we should create an instance of a class which is called an Object. The class has an unlimited lifetime whereas an object has a limited lifespan only.

Q #40) What are the various Access Specifiers in C++?

Answer: C++ supports the following access specifiers:

Public: Data members and functions are accessible outside the class.
Private: Data members and functions are not accessible outside the class. The exception is the usage of a friend class.
Protected: Data members and functions are accessible only to the derived classes.
Example:

Describe PRIVATE, PROTECTED, and PUBLIC along with their differences and give examples.

class A{
             int x; int y;
             public int a;
             protected bool flag;
             public A() : x(0) , y(0) {} //default (no argument) constructor
 };
 
 main(){
  
A MyObj;
  
MyObj.x = 5; // Compiler will issue a ERROR as x is private
  
int x = MyObj.x; // Compiler will issue a compile ERROR MyObj.x is private
  
 MyObj.a = 10; // no problem; a is public member
 int col = MyObj.a; // no problem
  
 MyObj.flag = true; // Compiler will issue a ERROR; protected values are read only
 bool isFlag = MyObj.flag; // no problem
Q #41) What is a Constructor and what is it called?

Answer: Constructor is a member function of the class having the same name as the class. It is mainly used for initializing the members of the class. By default constructors are public.

There are two ways in which the constructors are called:

Implicitly: Constructors are implicitly called by the compiler when an object of the class is created. This creates an object on a Stack.
Explicit Calling: When the object of a class is created using new, constructors are called explicitly. This usually creates an object on a Heap.
Example:

class A{
 int x; int y; 
 public A() : x(0) , y(0) {} //default (no argument) constructor
 };
 main()
 {
                    A Myobj; // Implicit Constructor call. In order to allocate memory on stack,
                                    //the default constructor is implicitly called.
                  A * pPoint = new A(); // Explicit Constructor call. In order to allocate
                                                  //memory on HEAP we call the default constructor.
 }
Q #42) What is a COPY CONSTRUCTOR and when is it called?

Answer: A copy constructor is a constructor that accepts an object of the same class as its parameter and copies its data members to the object on the left part of the assignment. It is useful when we need to construct a new object of the same class.

Example:

class A{
             int x; int y;
             public int color;
             public A() : x(0) , y(0) {} //default (no argument) constructor
             public A( const A& ) ;
};
A::A( const A & p )
{
              this->x = p.x;
              this->y = p.y;
              this->color = p.color;
}
main()
{
            A Myobj;
            Myobj.color = 345;
            A Anotherobj = A( Myobj ); // now Anotherobj has color = 345
}
Q #43) What is a Default Constructor?

Answer: A default constructor is a constructor that either has no arguments or if there are any, then all of them are default arguments.

Example:

class B {
 public: B (int m = 0) : n (m) {} int n;
 }; 
 int main(int argc, char *argv[])
{
 B b; return 0;
 } 
Q #44) What is a Conversion Constructor?

Answer: It is a constructor that accepts one argument of a different type. Conversion constructors are mainly used for converting from one type to another.

Q #45) What is an Explicit Constructor?

Answer: A conversion constructor is declared with the explicit keyword. The compiler does not use an explicit constructor to implement an implied conversion of types. Its purpose is reserved explicitly for construction.

Q #46) What is the role of the Static keyword for a class member variable?

Answer: The static member variable shares a common memory across all the objects created for the respective class. We need not refer to the static member variable using an object. However, it can be accessed using the class name itself.

Q #47) Explain the Static Member Function.

Answer: A static member function can access only the static member variable of the class. Same as the static member variables, a static member function can also be accessed using the class name.

Q #48) What’s the order in which the local objects are destructed?

Answer: Consider following a piece of code:

Class A{
 ….
 };
 int main()
 {
 A a;
 A b;
 ...
 }
In the main function, we have two objects created one after the other. They are created in order, first a then b. But when these objects are deleted or if they go out of scope, the destructor for each will be called in the reverse order in which they were constructed.

Hence, the destructor of b will be called first followed by a. Even if we have an array of objects, they will be destructed in the same way in the reverse order of their creation.

Overloading
Q #49) Explain Function Overloading and Operator Overloading.

Answer: C++ supports OOPs concept Polymorphism which means “many forms”.

In C++ we have two types of polymorphism, i.e. Compile-time polymorphism, and Run-time polymorphism. Compile-time polymorphism is achieved by using an Overloading technique. Overloading simply means giving additional meaning to an entity by keeping its base meaning intact.

C++ supports two types of overloading:

Function Overloading:

Function overloading is a technique that allows the programmer to have more than one function with the same name but a different parameter list. In other words, we overload the function with different arguments i.e. be it the type of arguments, number of arguments, or the order of arguments.

Function overloading is never achieved on its return type.

Operator Overloading:

This is yet another type of compile-time polymorphism that is supported by C++. In operator overloading, an operator is overloaded, so that it can operate on the user-defined types as well as the operands of the standard data type. But while doing this, the standard definition of that operator is kept intact.

For Example, an Addition operator (+) that operates on numerical data types can be overloaded to operate on two objects just like an object of a complex number class.

Q #50) What is the difference between Method Overloading and Method Overriding in C++?

Answer: Method overloading is having functions with the same name but different argument lists. This is a form of compile-time polymorphism.

Method overriding comes into the picture when we rewrite the method that is derived from a base class. Method overriding is used while dealing with run-time polymorphism or virtual functions.

Q #51) What is the difference between a Copy Constructor and an Overloaded Assignment Operator?

Answer: A copy constructor and an overloaded assignment operator basically serve the same purpose i.e. assigning the content of one object to another. But still, there is a difference between the two.

Example:

complex c1,c2;
c1=c2; //this is assignment
complex c3=c2; //copy constructor
In the above example, the second statement c1 = c2 is an overloaded assignment statement.

Here, both c1 and c2 are already existing objects and the contents of c2 are assigned to the object c1. Hence, for an overloaded assignment statement both the objects need to be created already.

Next statement, complex c3 = c2 is an example of the copy constructor. Here, the contents of c2 are assigned to a new object c3, which means the copy constructor creates a new object every time when it executes.

Q #52) Name the Operators that cannot be Overloaded.

Answer: 

sizeof – sizeof operator
. – Dot operator
.* – dereferencing operator
-> – member dereferencing operator
:: – scope resolution operator
?: – conditional operator
Q #53) Function can be overloaded based on the parameter which is a value or a reference. Explain if the statement is true.

Answer: False. Both, Passing by value and Passing by reference look identical to the caller.

Q #54) What are the benefits of Operator Overloading?

Answer: By overloading standard operators on a class, we can extend the meaning of these operators, so that they can also operate on the other user-defined objects.

Function overloading allows us to reduce the complexity of the code and make it more clear and readable as we can have the same function names with different argument lists.

Inheritance
Q #55) What is Inheritance?

Answer: Inheritance is a process by which we can acquire the characteristics of an existing entity and form a new entity by adding more features to it.

In terms of C++, inheritance is creating a new class by deriving it from an existing class so that this new class has the properties of its parent class as well as its own.

Q #56) What are the advantages of Inheritance?

Answer: Inheritance allows code re-usability, thereby saving time on code development.

By inheriting, we make use of bug-free high-quality software that reduces future problems.

Q #57) Does C++ support Multilevel and Multiple Inheritances?

Answer: Yes.

Q #58) What are Multiple Inheritances (virtual inheritance)? What are its advantages and disadvantages?

Answer: In multiple inheritances, we have more than one base classes from which a derived class can inherit. Hence, a derived class takes the features and properties of more than one base class.

For Example, a class driver will have two base classes namely, employee and a person because a driver is an employee as well as a person. This is advantageous because the driver class can inherit the properties of the employee as well as the person class.

But in the case of an employee and a person, the class will have some properties in common. However, an ambiguous situation will arise as the driver class will not know the classes from which the common properties should be inherited. This is the major disadvantage of multiple inheritances.

Q #59) Explain the ISA and HASA class relationships. How would you implement each?

Answer: “ISA” relationship usually exhibits inheritance as it implies that a class “ISA” specialized version of another class. For Example, An employee ISA person. That means an Employee class is inherited from the Person class.

Contrary to “ISA”, “HASA” relationship depicts that an entity may have another entity as its member or a class has another object embedded inside it.

So taking the same example of an Employee class, the way in which we associate the Salary class with the employee is not by inheriting it but by including or containing the Salary object inside the Employee class. “HASA” relationship is best exhibited by containment or aggregation.

Q #60) Does a derived class inherit or doesn’t inherit?

Answer: When a derived class is constructed from a particular base class, it basically inherits all the features and ordinary members of the base class. But there are some exceptions to this rule. For instance, a derived class does not inherit the base class’s constructors and destructors.

Each class has its own constructors and destructors. The derived class also does not inherit the assignment operator of the base class and friends of the class. The reason is that these entities are specific to a particular class and if another class is derived or if it is the friend of that class, then they cannot be passed on to them.

Polymorphism
Q #61) What is Polymorphism?

Answer: The basic idea behind polymorphism is in many forms. In C++, we have two types of Polymorphism:

(i) Compile-time Polymorphism

In compile-time polymorphism, we achieve many forms by overloading. Hence, we have an Operator overloading and function overloading. (We have already covered this above)

(ii) Run-time Polymorphism

This is the polymorphism for classes and objects. General idea is that a base class can be inherited by several classes. A base class pointer can point to its child class and a base class array can store different child class objects.

This means, that an object reacts differently to the same function call. This type of polymorphism can use a virtual function mechanism.

Q #62) What are Virtual Functions?

Answer: A virtual function allows the derived classes to replace the implementation provided by the base class.

Whenever we have functions with the same name in the base as well as the derived class, there arises an ambiguity when we try to access the child class object using a base class pointer. As we are using a base class pointer, the function that is called is the base class function with the same name.

To correct this ambiguity we use the keyword “virtual” before the function prototype in the base class. In other words, we make this polymorphic function Virtual. By using a Virtual function, we can remove the ambiguity and we can access all the child class functions correctly using a base class pointer.

Q #63) Give an example of Run-time Polymorphism/Virtual Functions.

Answer:

class SHAPE{
                  public virtual Draw() = 0; //abstract class with a pure virtual method
 };
 class CIRCLE: public SHAPE{
                  public int r;
                  public Draw() { this->drawCircle(0,0,r); }
 };
class SQUARE: public SHAPE{
               public int a;
               public Draw() { this->drawSquare(0,0,a,a); }
 };
 
 int main()
 {
                SHAPE shape1*;
                SHAPE shape2*;
  
                CIRCLE c1;
                SQUARE s1;
  
               shape1 = &c1;
              shape2 = &s1;
             cout<<shape1->Draw(0,0,2);
             cout<<shape2->Draw(0,0,10,10);
 }
In the above code, the SHAPE class has a pure virtual function and is an abstract class (which cannot be instantiated). Each class is derived from SHAPE implementing the Draw () function in its own way.

Further, each Draw function is virtual so that when we use a base class (SHAPE) pointer each time with the object of the derived classes (Circle and SQUARE), then appropriate Draw functions are called.

Q #64) What do you mean by Pure Virtual Functions?

Answer: A Pure Virtual Member Function is a member function in which the base class forces the derived classes to override. Normally this member function has no implementation. Pure virtual functions are equated to zero.

Example:

class Shape { public: virtual void draw() = 0; };
A base class that has a pure virtual function as its member can be termed an “Abstract class”. This class cannot be instantiated and it usually acts as a blueprint that has several sub-classes with further implementation.

Q #65) What are Virtual Constructors/Destructors?

Answer:

Virtual Destructors: When we use a base class pointer pointing to a derived class object and use it to destroy it, then instead of calling the derived class destructor, the base class destructor is called.

Example:

Class A{
              ….
              ~A();
};
Class B:publicA{
               …
               ~B();
};
B b;
A a = &b;
delete a;
As shown in the above example, when we say delete a the destructor is called but it’s actually the base class destructor. This gives rise to the ambiguity that all the memory held by b will not be cleared properly.

This problem can be solved by using the “Virtual Destructor” concept.

What we do is, we make the base class constructor “Virtual” so that all the child class destructors also become virtual and when we delete the object of the base class pointing to the object of the derived class, the appropriate destructor is called and all the objects are properly deleted.

This is shown as follows:

Class A{
              ….
              virtual ~A();
};
Class B:publicA{
               …
               ~B();
};
B b;
A a = &b;
delete a;
Virtual constructor: Constructors cannot be virtual. Declaring a constructor as a virtual function is a syntax error.

Friend
Q #66) What is a friend function?

Answer: C++ class does not allow its private and protected members to be accessed outside the class. But this rule can be violated by making use of the “Friend” function.

As the name itself suggests, the friend function is an external function that is a friend of the class. For the friend function to access the private and protected methods of the class, we should have a prototype of the friend function with the keyword “friend” included inside the class.

Q #67) What is a friend class?

Answer: Friend classes are used when we need to override the rule for private and protected access specifiers so that two classes can work closely with each other.

Hence, we can have a friend class to be a friend of another class. This way, friend classes can keep private, inaccessible things the way they are.

When we have a requirement to access the internal implementation of a class (private member) without exposing the details by making the public, we go for friend functions.

Advanced C++
Templates
Q #68) What is a template?

Answer: Templates allow creating functions that are independent of data type (generic) and can take any data type as parameters and return value without having to overload the function with all the possible data types. Templates nearly fulfill the functionality of a macro.

Its prototype is any of the following ones:

template <class identifier> function_declaration;

template <typename identifier> function_declaration;

The only difference between both prototypes is the use of keyword class or typename. Their basic functionality of being generic remains the same.

Exception Handling
Q #69) What is Exception Handling? Does C++ support Exception Handling?

Answer: Yes C++ supports exception handling.

We cannot ensure that code will execute normally at all times. There can be certain situations that might force the code written by us to malfunction, even though it’s error-free. This malfunctioning of code is called an Exception.

When an exception has occurred, the compiler has to throw it so that we know an exception has occurred. When an exception has been thrown, the compiler has to ensure that it is handled properly, so that the program flow continues or terminates properly. This is called the handling of an exception.

Thus in C++, we have three keywords i.e. try, throw, and catch which are in exception handling.

The general syntax for exception block is:

try{
 …. 
 # Code that is potentially about to throw exception goes here
 ….
 throw exception;
 }
 catch(exception type) {
 …
 #code to handle exception goes here
 }
As shown above, the code that might potentially malfunction is put under the try block. When code malfunctions, an exception is thrown. This exception is then caught under the catch block and is handled i.e. appropriate action is taken.

Q #70) Comment on C++ standard exceptions?

Answer: C++ supports some standard exceptions that can be caught if we put the code inside the try block. These exceptions are a part of the base class “std:: exception”. This class is defined in the C++ header file <exception>.

A few Examples of Exceptions supported by this class include:

bad_alloc – thrown by ‘new’

runtime_error – thrown for runtime errors

bad_typeid – thrown by type id

Introduction to Standard Template Library
Q #71) What is a Standard Template Library (STL)? What are the various types of STL Containers?

Answer: A Standard Template Library (STL) is a library of container templates approved by the ANSI committee for inclusion in the standard C++ specification. We have various types of STL containers depending on how they store the elements.

Queue, Stack – These are the same as traditional queue and stack and are called adaptive containers.
Set, Map – These are basically containers that have key/value pairs and are associative in nature.
Vector, deque – These are sequential in nature and have similarities to arrays.
Q #72) What is an Iterator class?

Answer: In C++ a container class is a collection of different objects.

If we need to traverse through this collection of objects, we cannot do it using simple index variables. Hence, we have a special class in STL called an Iterator class which can be used to step through the contents of the container class.

The various categories of iterators include input iterators, output iterators, forward iterators, bidirectional iterators, random access, etc.

Q #73) What is the difference between an External Iterator and an Internal Iterator? Describe an advantage of the External Iterator.

Answer: An internal iterator is implemented with member functions of the class that has items to step through.

An external iterator is implemented as a separate class that can be bound to the object that has items to step through. The basic advantage of an External iterator is that it’s easy to implement as it is implemented as a separate class.

Secondly, as it’s a different class, many iterator objects can be active simultaneously.

</https://www.softwaretestinghelp.com/cpp-interview-questions/>

<https://interviewsansar.com/category/cplusplus-advanced-interview-questions-and-answers/>

C++ Technical Interview Question on polymorphism in oops

Write a complete class stating function overriding feature in C++
Show the function call in main program.
Explain the concept of function overriding.
Take example of drawing multiple shapes e.g. circle and rectangle etc.
Interviewer Intent:

You know the concept and syntax of function overriding in C++
you can write class and program.
If you follow best coding practice and the things you care when write the code.
NOTE: As per question criteria, we will write code using interface, but, to describe the concept a basic example will be covered first.

Answer:

Function overriding concept is run time polymorphism in oops, in which functions get resolved on run time using VTABLE (Virtual table) by compiler.

If we have definition /declaration of a function in base class and want to have a definition of same function name in derive class and want to call derived function using base class pointer, then we need to override function. It’s simple, just we must make base class function virtual. for example,
Example if base class has a function definition:

class A{
public:
	virtual void foo(){
		cout<<" Base::A";
	}
};
class B:public A{
public:
	void foo(){
		cout<<" Derived::B"; } }; int main() { A *p = new B(); p->foo();
	delete p;
	
	return 0;
}

Example if base class has a function declaration(Interface):

Recommended to read C++ Interface and Pure virtual function.

//Interface
class IShape{
public:
	virtual void draw()=0;
};

//Derived class
class Circle:public IShape{
public:
	void draw();
};

//define the function
void Circle::draw(){

	cout<<"Circle"<<endl; } int main() { IShape *s = new Circle(); s->draw();
	delete s;
	
	return 0;
}

As a best practice, what we have taken care of in above program so for? Here are the points

We have used interface not a class to maintain loose coupling.
We have deallocated the dynamically allocated memory.
But, still we have missed one important point i.e. we should have written virtual destructor in the above base class to maintain the hierarchy of destructor call.

You can read here constructor and destructor call order in inheritance in C++. ( In short, constructor gets called from the base to derived class, and destructor call order is vice versa).


In the current program, derived class that is “Circle” class destructor will not be called, as we have not written virtual destructor in base class. Here is the example and output in which derived class destructor is not called.

In the above program lets write destructors in base class and derived class

//Interface
class IShape{
public:

	virtual void draw()=0;
		//destructor
	~IShape(){
		cout<<"Base destructor"<<endl;
	}
};

//Derived class
class Circle:public IShape{
public:
	void draw();

	//destructor
	~Circle(){
		cout<<"Circle destructor"<<endl;
	}
};

//define the function
void Circle::draw(){

	cout<<"Circle"<<endl;
}

Output:

Circle
Base destructor

But, if we make base class destructor virtaul as virtual ~IShape()then derived class destructor will also be called and output will be as below in reverse order(derived to base)

Circle
Circle destructor
Base destructor

There is no harm if we have not written virtual destructor, but, a pain comes at later point in a large project, if some other programmer comes and deallocate memory consuming resources in the destructor of derived class. A memory leak will happen and it may take huge time identifying that at run time. so, as a best practice we should write virtual destructor in base class too.

You can read virtual destructor in C++ with example in detail.

How to delete array of objects in C++? Proof by C++ code for proper deletion
Posted in C++ AdvancedBy rsinghPosted on April 26, 2017Tagged delete array of pointers in C++
Answer includes how to delete array of objects in C++ created dynamically with C++ code example with proof. In other words, delete array of pointers to objects in c++.

Interview Question: Write C++ code to create an array of objects using new keyword and delete these objects. Also, proof that all the objects are deleted properly.

Answer:

We know that when we create an object of a class dynamically from heap memory using new keyword, then we must delete it explicitly to avoid memory leaks in C++ programs after we are done with its operations.

Let’s take below class Pen as an example.

class Pen {
  
public:
      Pen() { 
         cout << "Constructor..." <<endl; 
      }
		
      ~Pen() { 
         cout << "Destructor...!" <<endl; 
      }
	  void write(){
		  cout << "Writing...!" <<endl; 
	  }
};

Below is an example, how we create an object of the class Pen dynamically and delete it after we are done with operations.

int main()
{
	//create an object dynamically
   Pen* pen = new Pen();
   pen->write();//operations
   
   delete pen;//de-allocate the memory
   
   return 0;
}
How to create array of objects of a class in C?
Let’s see how we create an array of objects in below C++ program example. In this example, we will create array of 3 objects, perform operation and delete dynamic array of pointers properly.

int main()
{
	//create an array of objects
   Pen* pen = new Pen[3];

   pen[0].write();
   pen[1].write();
   pen[2].write();
   
   delete [] pen;//de-allocate array of objects

   return 0;
}

Output:

Constructor…
Constructor…
Constructor…
Writing…!
Writing…!
Writing…!
Destructor…!
Destructor…!
Destructor…!

Proof of proper deletion of array of objects in C++
First, note that if we create an object of a class and delete the object then class constructor and destructor will be called respectively.

In above example, we have created an array of 3 objects and delete it using statement delete [] pen; if we look at the output the class constructor and destructor were called 3 times each. means, we have deleted objects properly.


Now, If we delete the object using the statement “delete pen” ( This is general mistake a programmer make) then the destructor will be called only once and for rest 2 objects destructor will not be called and program will crash. and this will proof that objects are not deleted properly.


Lets see the output if we use statement “delete pen”

int main()
{
	//create an array of objects
   Pen* pen = new Pen[3];

   pen[0].write();
   pen[1].write();
   pen[2].write();
   
   //this is not a prper way to delete
   //array of objects
   delete pen;

   return 0;
}

Output:

Constructor…
Constructor…
Constructor…
Writing…!
Writing…!
Writing…!
Destructor…!

and then program will crash at run time.

Conclusion:
In C++, single object of a class created dynamically is deleted using statement “delete pointer” and array of objects are deleted using statement “delete [ ] pointer”.

How to stop class inheritance in C++ with condition that object creation should be allowed
Posted in C++ AdvancedBy rsinghPosted on April 11, 2017Tagged C# inheritance, C++ stop inheritance
Answer includes multiple solutions to stop or prevent class inheritance in C++ with condition that object creation of the class should be allowed with C++ program example and explanation.

Interview Question: I want to stop a class to be inherited and allow to create an object of the class. Design a solution for this problem statement. Give as many solutions as you can.

Answer:
We can apply 3 solutions to prevent a class to be inherited in C++ where object creations will be allowed.

Solution-1: Use the final keyword (from C++11)
In the below example, we’ve made the Unique class final. So, it’ll not be inherited by any class.

If you try to inherit it, the compiler will flash an error that “a final class cannot be used as a base class“.


Note that you can create an object of the final class as show in the main() method here.


#include <iostream>
using namespace std;

 class Unique final {

 public:
	 void display() {
		 cout << "My unique class" << endl;
	 }
};

 //class Derived : Unique {
	// YOUR GET ERROR HERE if you inherit the Unique class
	// class Unique - a final class cannot be used as
	// a base class.
 //};

int main() {

	// you can create an object of the final class 
	Unique ob;
	ob.display(); 
	
	return 0;
}
Solution-2: Make the constructor of the class private and write a static function in the class that create object and return it to users.
Here is the C++ program example, in which constructor of the class named Unique is private and have written one static function, that is GetInstance() that create object and returns to user i.e. main() function.

So, the below program will fulfil the criteria mentioned in the question.

Note that if a class has its constructor private then neither an object of it can be created nor it can be inherited by any class.

So, if we try to derive a new class from it then compiler will throw an error stating that private constructor of the class is inaccessible at the compile time itself.

Since, we’ve prevented a class to be inherited by making the class constructor private. So, an object will also not be created of this class.


But, we want to allow an object of the class to be created. To solve this problem,

we can have a static function in the class that is called by class name without creating an object. And this function will create the class object, and return to users or main program.


Here is the complete working program that’ll satisfy the above criteria.

C++ Code Example:
“Unique” class cannot be inherited but object of it can be created.

#include<iostream>
using namespace std;

class Unique{
private:
	//Make constructor private
	Unique(){}

public:
	//Create a static fuction that
	//returns object of the class
	static Unique*  GetInstance(){

		return new Unique();
	}	
	void Display(){

		cout<<" My Unique Class"<<endl; } }; int main(){ Unique *u = Unique::GetInstance(); u->Display();		
	
	return 0;
}

If we try to derive a class from Unique class (example below) compiler will throw an error stating that private constructor of Unique class is inaccessible at compile time itself.

class Derived:public Unique{
public:
	Derived(){
		cout<<"Derived constructor"<<endl;
	}

public:
	void Display(){
		cout<<" My Derived Class"<<endl;
	}
};

Solution-3: Create a dummy class having a private constructor and make the class friend of dummy class and extend the class virtually from dummy class.
Below is the C++ program example that will not allow Unique class to be inherited. But, allow object creation of the Unique class.

When we create the object of the Unique class, it will access and call the private constructor of the dummy class StopInheritance, Because the Unique class is friend of the dummy class.

Note that if a class is friend of another class then it can access private data of that class.

Recommend to read the order of constructor and destructor call in C++ inheritance relationship if you are not familiar with calling orders.

So, we can create an object of the Unique class. But, if we derive a class from the Unique class and create an object of derived class, then it will directly try to access the constructor of dummy class because the Unique class has inherited it virtually.


And since the derived class is not a friend of the dummy class, it cannot access the private constructor resulting in a compiler error.

#include<iostream>
using namespace std;

//dummy class
class StopInheritance{

private:
	//make constructor private
	StopInheritance(){
	}

	//make Unique class a friend of it
	friend class Unique;
};

class Unique:virtual StopInheritance
{
public:	
	Unique(){
		cout<<"Class";
	}
	void Display(){

		cout<<" My Unique Class"<<endl;
	}
};

class Derived:public Unique{
public:
	void Display(){

		cout<<" My derived Class"<<endl;
	}
};
int main(){	
	
	Derived obj;
	obj.Display();

	return 0;
}

What is Advantage and Use of THIS pointer in C++ – Scenarios?
Posted in C++ AdvancedBy rsinghPosted on February 27, 2017Tagged this pointer use
Answer includes uses and advantage of the this pointer in C++ programming with multiple scenarios where the this pointer is used.

Sceranio-1: Internal use of this pointer as an argument to a function.
Wherever an object calls a class member function, then the compiler internally passes a “this” pointer to the member function internally.

For example,

In the below class Car, we have a “SetModel” member function that receives one argument i.e. car model.

In fact, besides the model parameter, one more argument is passed to the set model function internally, and that is the “this” pointer.

class Car{
	int model;
public:
	void SetModel(int model){		
		this->model = model;
	}
};

int main(){

	int modelNumber = 1024;
	Car obj;
	//On calling function using class obj
	//THIS pointer is also passed internally besides
	//model number paramer.
	obj.SetModel(modelNumber);

	return 0;
}

You can Read in detail: “this” pointer internal working in C++.

Scenario-2: Use “this” pointer to assign value of the function’s parameter to a class member variable correctly
In the below code example,

the class member variable “ modle”, and the parameter “modle” in the function SetModel(int model) are of the same name.

class Car{
	int model;
public:
	void SetModel(int model){		
		this->model = model;
	}
};

Even though if we write model=model in the SetModel function instead of this->model = model; the compiler will throw no error and everything would seems fine at the compile time, but when you run the program, you’ll get garbage value.

Scenario-3: In a large code base of a function, identifying the class member variable is easy
Assume a function of a class or multiple functions uses the class fields and they have very large and complex code base, then

it’s easy for a programmer to identify the class fields. Specially when a maintenance or modification is done within it.

class Car{
	int model;
public:
	void SetModel(int m){
		// do something;


		this->model = m;
	}
};

Can we use THIS Pointer in static function – Reason in C++?
Posted in C++ AdvancedBy rsinghPosted on February 27, 2017Tagged this pointer static functin c++
We cannot use THIS pointer in static function of a class in C++ program.

Reason: Whenever we call a class non-static member function using class object then THIS pointer is also passed to the function as a parameter internally and this is why a non-static member function of a class know that on which class object it is being called in case of multiple objects creation of the class.

Recommended: How does “this” pointer in C++ work internally?

But, static function of a class is not associated with class object. So, THIS pointer is not passed to a static function as an internal parameter. So, a static function does not understand THIS pointer inside its body.


If we compile below class, compiler with throw an error i.e. static functions do not have this pointer.

class Printer{
	static int a;
public:
	static void print(){
		//Error static funtions do not have 
		//this pointer.
		this->a; 
	}
};

This is why static member function cannot have this pointer in C++ language.

C++ Public access specifier instead of Private – What is bad?
Posted in C++ AdvancedBy rsinghPosted on August 25, 2016
Interview Question: A class is having private data members and that is by design and expected. Question is, if we write C++ public access specifier instead of private for that data members then what issue we can face in a C++ program?

If you want to know access specifiers in C++ programming,  read another interview question on: access specifiers in C++ and use of C++ access specifiers .

Answer: Wrongly placed specifiers may create a huge pain in maintenance or finding bugs for changed behavior of a large C++ project.


In a simple program it may not be noticeable. But, in a large program where tons of classes and tons of functions are there, it may be difficult to find issues. So, we need to keep focus when using access specifiers in C++ software projects.


Let’s take a simple C++ code example . If we use public access specifier instead of private for data members in a class,  compiler is not going to complain and programs work fine.  However, it may lead to an issue unknowingly.


In below C++ program, there is a class called Insurance and it contains a data member “float sum” and the value of “sum” has been initialize to 5.0. There is another class TaxCalculator which is using the value of sum variable to calculate the tax with formula float tax = obj.getSum()*10/100;. Expected answer for this program is 0.5.

But assume, by mistake, if some programmer changed its value in TaxCalculator class that is sum=100, may be to solve other problems. Then value of tax will become 10 that was not expected. So, we have to be careful  with choosing access specifiers for members and functions.

class Insurance{
public:	
	int year;
	float sum;
public:
	Insurance(){
		this->sum =5.0;
	}
	float getSum(){
		return sum;
	}
};

class TaxCalculator{

	Insurance obj;
public:
	TaxCalculator(){
		obj.sum = 100;
	}
	float getTax(){
		float tax = obj.getSum()*10/100;		
		return tax;
	}

};


int main(){
	//Access to public functions 
	TaxCalculator tc;
	cout<< "Tax="<<tc.getTax();
	
	return 0;
}

Use of Public Private and Protected access specifiers in C++?
Posted in C++ AdvancedBy rsinghPosted on August 23, 2016Tagged C++ Public Private and Protected modifiers, What is access specifier in C++
Answer: Use of public private and protected access specifiers in C++ is to control the access/visibility of member data and functions out of a class.

It all depends upon requirement when we design a class, what access level to fields and member functions, we want to provide in a class with the use of public private and protected specifiers.

use of public private and protected access specifiers
Use of private access specifier in C++:
Use private specifier for data and functions of a class that are not supposed to be exposed outside of a class.

As a good class design, a class should have all data members private in a class and class’s functions should use these member data.


If we have to provide access to data members of a class to another class or program e.g. main (), we should not make it public or protected, but we should provide it using an interface i.e. public methods to access from outside of a class.


In below C++ class, all member fields are private. Let’s say, we want to allow another class to set or get the value of sum, then we should have public method getSum() and setSum() etc.

class Insurance{
private:
	float sum;
	int year;
	
public:
	float getSum(){
		return sum;
	}
	void setSum(float sum){
		this->sum = sum;
	}	
};
int main(){

	Insurance obj;
	
	obj.setSum(5.0);
	cout<<obj.getSum();	

	return 0;
}

All the internal functions of a class that is used in class itself and public exposer of internal functions not required, then make them private. Only make function public which is supposed to be accessed from outside of a class.

Use of Public access specifier in C++:
Expose only required member functions to out of a class. So, it can be accessed from anywhere from another class or program.

class Insurance{
private:	
	int year;
	float sum;
	
public:
	float getSum(){
		return sum;
	}
	void setSum(float sum){
		this->sum = sum;
	}	
};


int main(){
	//Access to public functions 
	Insurance iobj;	
	vobj.getSum();
	return 0;
}

Use of Protected access specifier in C++:
Use protected specifier if you want to allow access of data and member functions to child class only in inheritance.

In below program, data member “sum” and displaySum() function are protected and only available to child class. If we call them in main() program, compiler will flash an error i.e. protected member can’t be accessed.

class Insurance{
private:	
	int year;
protected:
	float sum;
	void displaySum(){
		cout<<"sum="<<sum; } public: float getSum(){ return sum; } void setSum(float sum){ this->sum = sum;
	}	
};

class VehicleInsurance:public Insurance{

public:

	VehicleInsurance(){
		sum = 100.00;//can access protected member
		displaySum();//access protected function
	}

};

int main(){
	
	VehicleInsurance vobj;

	//vobj.sum = 12;//Error can't access protected member
	//vobj.displaySum();//Error can't access protected function
	vobj.getSum();// public fucntin OK
	return 0;
}

Also, use of public private and protected access specifiers in C++ is in inheritance hierarchy that is how we want to inherit the base class. For example

class VehicleInsurance:public Insurance{
}
class VehicleInsurance:private Insurance{
}
class VehicleInsurance:protected Insurance{
}

Use of public instead of private may lead you in great pain. How? Read hear another interview question: what is issue on using public specifier in place of private in C++ classes?

Use of Public Private and Protected access specifiers in C++?
Posted in C++ AdvancedBy rsinghPosted on August 23, 2016Tagged C++ Public Private and Protected modifiers, What is access specifier in C++
Answer: Use of public private and protected access specifiers in C++ is to control the access/visibility of member data and functions out of a class.

It all depends upon requirement when we design a class, what access level to fields and member functions, we want to provide in a class with the use of public private and protected specifiers.

use of public private and protected access specifiers
Use of private access specifier in C++:
Use private specifier for data and functions of a class that are not supposed to be exposed outside of a class.


As a good class design, a class should have all data members private in a class and class’s functions should use these member data.

If we have to provide access to data members of a class to another class or program e.g. main (), we should not make it public or protected, but we should provide it using an interface i.e. public methods to access from outside of a class.


In below C++ class, all member fields are private. Let’s say, we want to allow another class to set or get the value of sum, then we should have public method getSum() and setSum() etc.

class Insurance{
private:
	float sum;
	int year;
	
public:
	float getSum(){
		return sum;
	}
	void setSum(float sum){
		this->sum = sum;
	}	
};
int main(){

	Insurance obj;
	
	obj.setSum(5.0);
	cout<<obj.getSum();	

	return 0;
}

All the internal functions of a class that is used in class itself and public exposer of internal functions not required, then make them private. Only make function public which is supposed to be accessed from outside of a class.

Use of Public access specifier in C++:
Expose only required member functions to out of a class. So, it can be accessed from anywhere from another class or program.

class Insurance{
private:	
	int year;
	float sum;
	
public:
	float getSum(){
		return sum;
	}
	void setSum(float sum){
		this->sum = sum;
	}	
};


int main(){
	//Access to public functions 
	Insurance iobj;	
	vobj.getSum();
	return 0;
}

Use of Protected access specifier in C++:
Use protected specifier if you want to allow access of data and member functions to child class only in inheritance.


In below program, data member “sum” and displaySum() function are protected and only available to child class. If we call them in main() program, compiler will flash an error i.e. protected member can’t be accessed.

class Insurance{
private:	
	int year;
protected:
	float sum;
	void displaySum(){
		cout<<"sum="<<sum; } public: float getSum(){ return sum; } void setSum(float sum){ this->sum = sum;
	}	
};

class VehicleInsurance:public Insurance{

public:

	VehicleInsurance(){
		sum = 100.00;//can access protected member
		displaySum();//access protected function
	}

};

int main(){
	
	VehicleInsurance vobj;

	//vobj.sum = 12;//Error can't access protected member
	//vobj.displaySum();//Error can't access protected function
	vobj.getSum();// public fucntin OK
	return 0;
}

Also, use of public private and protected access specifiers in C++ is in inheritance hierarchy that is how we want to inherit the base class. For example

class VehicleInsurance:public Insurance{
}
class VehicleInsurance:private Insurance{
}
class VehicleInsurance:protected Insurance{
}

Use of public instead of private may lead you in great pain. How? Read hear another interview question: what is issue on using public specifier in place of private in C++ classes?

What if memory allocation using new fails in C++ how to handle
Posted in C++ AdvancedBy rsinghPosted on July 23, 2016Tagged Handle memory allocation failure in C++
Interview Question on memory allocation failure in C++: when you do memory allocation using new in C++ and it fails then what are issues? In another words, when you allocate memory on heap using new operator, how do you handle memory allocation using new in C++ failure? What is issue when you don’t handle it?

The answer for this technical interview question i.e. if C++ new fails to allocate memory will include 2 techniques to handle dynamic memory allocation using new failure in C++.


Answer: When we allocate memory from heap dynamically in a C++ program using new operator,  the program crashes when memory is not available, or the system is not able to allocate memory to a program, as it throws an exception. So, to prevent program crash, we need to handle the exception when memory allocation fails.

Techniques to handle bad allocation exception in C++ program:
Using Try Catch Block with std::bad_alloc exception
We need to put the memory allocation code using new operator in try catch block. Below C++ program catches exception when it is thrown on memory allocation failure.

#include <iostream>
using namespace std;

int main(){

	//Try to allocate very huge amount of memory
	//so memory allocation fails.
	long CHUNK_SIZE = 0x7fffffff;

	//Allocate memory dynamically using "new" 
	// using try catch block

	try {
		char *ptr = new char[CHUNK_SIZE];
		//on exception below line will not be printed.
		//and control will go in catch block.
		cout<<"Memory allocation Successful"<<endl;
	}
	catch (const bad_alloc& e) {

		cout << "Allocation failed: " << e.what() << '\n';
		//handle error
	}		

	return 0;
}

Using no_throw version of “new” i.e. new(std::nothrow)
Rather than simply using new operator for memory allocation in C++, we need to use no throw version of “new” as it handle the exception and there is no program crash.

#include <iostream>
using namespace std;

int main(){

	//Try to allocate very huge amount of memory
	//so memory allocation fails.
	long CHUNK_SIZE = 0x7fffffff;

	//Allocate memory dynamically using "new" with
	//"nothrow" version of new
	char *ptr = new(std::nothrow) char[CHUNK_SIZE];
	
	//Chek ptr if it contains the valild address of
	//allocated memory
	if (ptr)
	{
		cout<<"Memory allocation Successful"<<endl;
		//do operations
	}  
	else{
		cout << "Memory allocation fails" << endl;
	}      

	return 0;
}

When to use RTTI – Dynamic_cast in C++
Posted in C++ AdvancedBy rsinghPosted on June 2, 2016Tagged c++ dynamic_cast use
When to use RTTI (Run Time Type Information) dynamic_cast in C++ is frequently asked c++ technical interview question. Answer to this question will cover multiple scenarios where we can use dynamic_cast in C++ program.

Answer:

Scenarios – Use of Dynamic_cast in C++ program:
Situation 1- When we need to call a specialized member function of child class that’s not available to the base class in inheritance hierarchy. Polymorphism breaks down here but sometimes we get this situation.  Below, class B contains specialized funcB() function.

class A {
public:	
	virtual void func() { }
};


class B : public A {
public:
	void func()}

	//Specialized function to B class
	void funcB(){}
};

What if we need to call specialized funcB() using base class pointer like below program. Dynamic cast operator, Part of RTTI in C++ comes into picture to type cast from base to child class.

//A* arg: base class pointer that can have
//any child classes object.
void f(A* arg) {
 
//down cast from base pointer to derive pointer
//as, base class pointer does not understand 
//specialized function of derived class.
B* bp = dynamic_cast<B*>(arg);	
 
  if (bp)
  {   	
		bp->func();
		bp->func2();// ok
  }  
  else{
	  //Call respective class function
    arg->func();
  }
};

Situation 2 – We want to override a function from base class that is not virtual and we can’t make it virtual as base class is sitting in a library and it can’t be modified.

So, overriding is not possible. If we use statements for below program, A* ptr = new B(), ptr->func2(); always base call method will be called as its not virtual in base class. But we want to call child class func2() method.


Then we need to use dynamic_cast operator to type cast base pointer to child pointer to call child’s class method.

//We cannot touch base class A but can be inherited. 
class A {
public:	
	virtual void func() { printf("Class A :func()\n"); }
	        void func2(){ printf("Class A :func2()\n"); }//Not virtual 
};


class B : public A {
public:
	void func() { printf("Class B :func()\n"); }

	//Want to override func2 but can't func2 is not virtual in base class.
	
	//if we use base class pointer with B object, base class func2 function will be called.
	
	//Can't make class A:func2 virtual as it is in a library- binary form.
	
	//only option is RTTI to access it via base class pointer in client code.
	void func2(){ printf("Class B :func2()\n"); }
};

Complete Example: Situation-1: Call specialized member function of a child class using dynamic_cast RTTI in C++.
#include
#include
using namespace std;


class A {
public:	
	virtual void func() { printf("Class A :func()\n"); }
};


class B : public A {
public:
	void func() { printf("Class B :func()\n"); }

	//Specialized function to B class
	void funcB(){ printf("Class B :funcB()\n"); }
};

int main()
{
	A* ap = new B();
 	//Call funcB() function of class B using base pointer A
//	ap->funcB();//Compiler error as funcB() is not a member of Animal	

	//Now use dymaic cast to convert base pointer to derived pointer i.e. A to B.
	B* bp = dynamic_cast<B*>(ap);
	
	if (bp)
	{
		bp->funcB();
	}
	

return 0;
}

Complete Example: Situation-2: Call child class method if it is not virtual in base class in C++

#include
#include
using namespace std;


class A {
public:	
	virtual void func() { printf("Class A :func()\n"); }
	        void func2(){ printf("Class A :func2()\n"); }//Not virtual 
};


class B : public A {
public:
	void func() { printf("Class B :func()\n"); }
	
	void func2(){ printf("Class B :func2()\n"); }
};

class C : public A {
public:
	void func() { printf("Class C :func()\n"); }	
};


//-----Client code------
void f(A* arg) {

	//call 
  B* bp = dynamic_cast<B*>(arg);	
 
  //Call Specific class B function.
  if (bp)
  {   	
		bp->func();
		bp->func2();
  }  
  else{
	  //Call respective class function
    arg->func();
  }
};

int main()
{
	A* ap1 = new B(); 
	f(ap1);


	//operate C object
	A* ap2 = new C();
	f(ap2);

return 0;
}

Writing Smart Pointer in C++ for a Specific Class
Posted in C++ AdvancedBy rsinghPosted on April 28, 2016Tagged c++ smart pointer example
What is smart pointer and implementation of Smart pointer in C++. This simple smart pointer implementation in C++ is asked in technical interview to know if we know the concept of smart pointer and able to implement it.

Answer: 

Smart pointers are a pointers that get de-allocated by itself, when it goes out of scope and we don’t need to to delete it manually. Generally , in C++ programming we use new and delete to allocate and deallocate memory dynamically / at run time.

When we use “new” to allocate memory, the programmer is responsible to free the memory using delete keyword. Where as this is not the case of smart pointers. In fact, smart pointers are objects which store pointers to dynamically allocated objects.


Lets see a simple example to create a smart pointer class.


Consider a class called “Car” having a method Run () as shown below. We will create a smart pointer for this class named CarSP. This smart pointer in C++ program will handle automatic deallocation of memory i.e. for Car object allocated dynamically.

Car Class :

//Car class for which we have to implement
// a Smart pointer.
class Car{

public:
	void Run(){
		cout<<"Car Running..."<<"\n";
	}
};

Implementation of Smart pointer in C++
In CarSP  smart pointer class, we’ll have a field Car *sp, that hold the pointer of Car object. In the destructor of CarSP, we will write code to delete object of Car class.

To call the function of car class we have to overload arrow operator -> operator, that returns pointer of object Car. Note that After overloading -> only we would be able to use -> on class CarSP that act as a pointer.

Smart pointer class and testing code
//Smart pointer for class Car
class CarSP{

	Car * sp;

public:
	//Initialize Car pointer when Car 
	//object is createdy dynamically
	CarSP(Car * cptr):sp(cptr)
	{
	}

	// Smart pointer destructor that will de-allocate
	//The memory allocated by Car class.
	~CarSP(){		
		printf("Deleting dynamically allocated car object\n");
		delete sp;
	}

	//Overload -> operator that will be used to 
	//call functions of class car
	Car* operator-> ()
	{    
		return sp;
	}
};


//Test
int main(){

	//Create car object and initialize to smart pointer
	CarSP ptr(new Car());
	ptr->Run();

	//Memory allocated for car will be deleted
	//Once it goes out of scope.
	return 0;
}



</https://interviewsansar.com/category/cplusplus-advanced-interview-questions-and-answers/>
