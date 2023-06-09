# https://www.simplilearn.com/tutorials/cpp-tutorial/cpp-interview-questions 

## **What are widely used applications of C++?**

1. *Systems Programming:* C++ was designed with systems programming in mind. It provides low-level control over hardware resources and memory management, making it an ideal choice for developing operating systems, device drivers, embedded systems, and other performance-critical applications.

2. *Game Development:* C++ is extensively used in the game development industry due to its efficiency and performance. Game engines like Unreal Engine and Unity use C++ as their primary language. C++ allows developers to optimize game code, work closely with hardware resources, and achieve high-performance graphics rendering.

3. *High-Performance Computing:* C++ is often used in high-performance computing (HPC) applications where speed and efficiency are critical. Its ability to directly manipulate memory and perform low-level optimizations allows developers to write code that can efficiently leverage multicore processors and exploit parallelism.

4. *Graphics and Visualization:* C++ is commonly used in graphics and visualization applications. Libraries like OpenGL and DirectX provide efficient graphics rendering capabilities, and tools like OpenCV offer image processing and computer vision functions. C++ enables developers to create interactive and visually rich applications, including computer-aided design (CAD), virtual reality (VR), and computer graphics rendering.

5. *Networking and Communication:* C++ is frequently used in networking and communication applications. Its low-level control over memory and efficient performance make it suitable for building network protocols, server applications, and real-time communication systems. C++ libraries like Boost.Asio provide powerful networking capabilities.

6. *Financial and Trading Systems:* C++ is prevalent in the financial industry, where speed and reliability are crucial. Trading systems, algorithmic trading platforms, and high-frequency trading applications often utilize C++ for its low latency and high-performance capabilities.

7. *Scientific Computing and Simulations:* C++ is used in scientific computing and simulations, particularly when performance is a primary concern. Computational physics, computational chemistry, and simulations involving complex mathematical models benefit from C++'s ability to optimize performance-critical code.

8. *Embedded Systems:* C++ is widely used in embedded systems development. Its ability to work closely with hardware, manage limited resources efficiently, and provide deterministic behavior makes it suitable for programming microcontrollers, robotics, IoT devices, and other embedded applications.

----

## **What are useful resources?**

* [History of C++](https://en.cppreference.com/w/cpp/language/history)

* [Current status](https://isocpp.org/std/status)

* [JTC1/SC22/WG21 - The C++ Standards Committee - ISOCPP](https://www.open-std.org/jtc1/sc22/wg21/)
* [News, Status & Discussion about Standard C++](https://isocpp.org/)

* [C++ Core Guidelines](https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md)

* [C++ Reference](https://en.cppreference.com/w/cpp)

* [C++ StdLib](http://www.cppstdlib.com/)

* [C++ Standard Library Headers](https://en.cppreference.com/w/cpp/header)

* [Cplusplus conference](https://cppcon.org/)

* C++ detailed infos on certain topics
  * [Declaring namespaces and namespace members](https://learn.microsoft.com/en-us/cpp/cpp/namespaces-cpp?view=msvc-170)
  * [Enumerationsklasse (C++/CLI und C++/CX)](https://learn.microsoft.com/de-de/cpp/extensions/enum-class-cpp-component-extensions?view=msvc-170)
  * [Function templates](https://cplusplus.com/doc/oldtutorial/templates/#:~:text=Function%20templates%20are%20special%20functions,be%20achieved%20using%20template%20parameters.)
  * [Predefined macros](https://learn.microsoft.com/en-us/cpp/preprocessor/predefined-macros?view=msvc-170)
  * [Source code organization (C++ Templates)](https://learn.microsoft.com/en-us/cpp/cpp/source-code-organization-cpp-templates?view=msvc-170)
  * [Writing OS Independent Code in C/C++](https://www.geeksforgeeks.org/writing-os-independent-code-cc/)
  * [Awesome CPP](https://github.com/fffaraz/awesome-cpp)

* [CMake - Reference Documentation](https://cmake.org/documentation/)
    * [CMake Tutorial](https://cmake.org/cmake/help/latest/guide/tutorial/)
    * [Mastering CMake](https://cmake.org/cmake/help/book/mastering-cmake/)
    * [https://github.com/dev-cafe/cmake-cookbook](CMake Cookbook)

----

## **What is the difference between C and C++?**

| C | C++ |
| ----- | ------ |
| C is a procedure-oriented programming language. | C++ is a partially object-oriented programming language. |
| It follows a top-down approach. | It follows a bottom-up approach. |
| C doesn’t support function or operator overloading. | C++ supports function as well as function overloading. |
| C language doesn’t support virtual and friend function | C++ language supports both virtual and friend functions. |
| C language has 32 keywords. | C++ language contains 52 keywords. |

----

## **What is the bottom-up approach mentioned in connection with C++?**

When we say that C++ follows a "bottom-up" approach, we are referring to the language's design philosophy and the way it handles program execution.

In a bottom-up approach:

*Low-level Control:* C++ allows developers to have fine-grained control over the hardware and system resources. It provides features like direct memory manipulation, pointer arithmetic, and low-level access to system functions. This level of control enables developers to optimize code for efficiency, performance, and resource utilization.

*Emphasis on Efficiency:* C++ prioritizes efficiency and performance. It allows developers to write code that executes quickly and uses system resources efficiently. The language provides features like inline assembly, manual memory management, and the ability to work with hardware resources directly. These features enable developers to fine-tune their code for maximum efficiency.

Close to the Machine:* C++ is considered a "close-to-the-machine" language. It allows developers to write code that operates at a low level, close to the underlying hardware. This proximity to the machine allows for precise *control over memory, processor registers, and hardware devices. C++ code can directly interact with memory addresses, manage hardware interrupts, and access system-level functionality.

*Modularity and Reusability:* While C++ provides low-level control, it also supports modular programming and code reuse. The language offers features like classes, objects, and libraries that facilitate the creation of reusable and maintainable code. Developers can build higher-level abstractions on top of low-level components, creating a layered and modular code structure.

*Flexible and Versatile:* C++ is a versatile language that supports various programming paradigms, including procedural, object-oriented, and generic programming. It allows developers to choose the level of abstraction that suits their needs, making it suitable for a wide range of applications.

It is important to note that while C++ provides low-level control, it also offers high-level abstractions and programming paradigms. This combination allows developers to work at different levels of abstraction and choose the most appropriate approach for their specific requirements.

----

## **What are classes and objects in C++?**

A class is like a blueprint of an object. It is a user-defined data type with data members and member
functions and is defined with the keyword class.

You define objects as an instance of a class. Once it creates the object, then it can operate on both data members and member functions.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class MyClass
{ // The class
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

----

## **What are access modifiers?**

You use access modifiers to define accessibility for the class members. It defines how to access the members of the class outside the class scope.

There are three types of access modifiers:

- Private

```c++
// C++ program to demonstrate private
// access modifier

#include <iostream>

using namespace std;

class Circle
{
	// private data member
	private:
		double radius;
	
	// public member function
	public:
		double compute_area() // member function can access private
		{ 
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
int main()
{
	Child obj1;
	
	// member function of the derived class can
	// access the protected data members of the base class
	obj1.setId(81);
	obj1.displayId();
	
    return 0;
}
```

## **Difference between equal to (==) and assignment operator(=)?**

The equal to operator == checks whether two values are equal or not. If equal, then it’s true; otherwise, it will return false.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>

using namespace std;

int main()
{
	cout << boolalpha  // For printing true and false as true and false in case of a bool result
		<< "The true expression 3 != 2 yields: "
		<< (3 != 2) << endl
		<< "The false expression 20 == 10 yields: "
		<< (20 == 10) << endl;
}

// Output:
// The true expression 3 != 2 yields: true
// The false expression 20 == 10 yields: false
```

The assignment operator = allots the value of the right-side expression to the left operand.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>

using namespace std;

int main()
{
    int a = 3, b = 2;

    if (a < b)
    {
        cout << a << " is less than " << b;
    }
    else if (a > b)
    {
        cout << a << " is greater than " << b;
    }
    
    return 0;
}

// Output:
// 3 is greater than 2
```

----

## **What is the difference between a while loop and a do-while loop?**

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

## **What is the size of the int data type?**

- 4 bytes (true, int)
- 1 byte
- 8 bytes
- 2 bytes

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>

using namespace std;

int main()
{
	cout << "size of datatype int : " << sizeof(int) << endl;
}

// Output:
// size of datatype int : 4
```

----

## **Which among the following operators cannot be overloaded?**

- -:
- +:
- ?:  operator cannot be overloaded because it is not syntactically possible.
- %:

```c++
// TestApplication.cpp : Example of overlaoding the + operator.
//

#include <iostream>
#include <string>

using namespace std;

class Box
{
    double length; // Length of a box
    double breadth; // Breadth of a box
    double height; // Height of a box

public:
    double getVolume(void)
    {
        return length * breadth * height;
    }

    void setLength(double len)
    {
        length = len;
    }

    void setBreadth(double bre)
    {
        breadth = bre;
    }

    void setHeight(double hei)
    {
        height = hei;
    }

    // Overload + operator to add two Box objects.
    Box operator+(const Box& b)
    {
        Box box;
        box.length = this->length + b.length;
        box.breadth = this->breadth + b.breadth;
        box.height = this->height + b.height;
        return box;
    }
};

int main()
{
    Box Box1;                // Declare Box1 of type Box
    Box Box2;                // Declare Box2 of type Box
    Box Box3;                // Declare Box3 of type Box
    double volume = 0.0;     // Store the volume of a box here

    // box 1 specification
    Box1.setLength(6.0);
    Box1.setBreadth(7.0);
    Box1.setHeight(5.0);

    // box 2 specification
    Box2.setLength(12.0);
    Box2.setBreadth(13.0);
    Box2.setHeight(10.0);

    // volume of box 1
    volume = Box1.getVolume();
    cout << "Volume of Box1 : " << volume << endl;

    // volume of box 2
    volume = Box2.getVolume();
    cout << "Volume of Box2 : " << volume << endl;

    // Add two object as follows:
    Box3 = Box1 + Box2;

    // volume of box 3
    volume = Box3.getVolume();
    cout << "Volume of Box3 : " << volume << endl;

    return 0;
}

// Output:
// Volume of Box1 : 210
// Volume of Box2 : 1560
// Volume of Box3 : 5400
```

----

## **What among these is used to return the number of characters in the string?**

- Size
- Length
- Both size and length: are used to return the number of characters in the string.
- Name

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

int main()
{
	string str1 = "hello";
	cout << str1 << ":" << str1.length();

	cout << "\n" << endl;

	const char* str2 = "hello";
	cout << str2 << ":" << strlen(str2);
}

// Output:
// hello:5
// 
// hello:5
```

----

## **Discuss the difference between prefix and postfix?**

In prefix (++i), first, it increments the value, and then it assigns the value to the expression.

In postfix (i++), it assigns the value to the expression, and then it increments the variable's value. 

```c++
// TestApplication.cpp : Demonstrate difference between prefixes and postfixes.
//

#include <iostream>
#include <string>

using namespace std;

int main()
{
	int x = 3, y, z;
	y = x++;
	z = ++x;
	cout << x << ", " << y << ", " << z;
	return 0;
}

// Output:
// 5, 3, 5
```

----

## **Can you compile a program without the main function?**

Yes, you can compile a program without the main function, but you cannot run or execute the program because the `main()` function is the entry
point, from where all the execution begins. And without the entry point, then you can execute the program.

----

## **What is std in C++?**

- std is a standard class in C++ (true)
- std is a standard file reading header
- std is a standard header file
- std is a standard namespace

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>
#include <stdio.h>

using namespace std;

namespace n1
{
    int x = 2;
    // Function to display the message
    // for namespace n1
    void fun()
    {
        cout << "This is fun() of n1" << endl;
    }
}

namespace n2
{
    int x = 5;
    // Function to display the message
    // for namespace n2
    void fun()
    {
        cout << "This is fun() of n2" << endl;
    }
}

int main()
{
    // The methods and variables called
    // using scope resolution(::)
    cout << n1::x << endl;
    n1::fun();

    cout << n2::x << endl;
    n2::fun();

    return 0;
}

// Output:
// 2
// This is fun() of n1
// 5
// This is fun() of n2
```

----

## **What are the four different data types in C++?**

- __Primitive/Basic:__ `Char`, `int`, `short`, `float`, `double`, `long`, `bool`, etc.
- __Derived:__ `Array`, `pointer`, etc.
- __Enumeration:__ `Enum`
- __User-defined:__ `Structure`, `class`, etc.

----

## **How is [struct different from class?](https://www.geeksforgeeks.org/structure-vs-class-in-cpp/)**

Structure
Class

Its members are public by default.
Its members are private by default.

The default access specifiers are public when deriving a struct from a class/struct. 
The default access specifiers are private when deriving a class. 

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class Test1
{
    // x is private
    int x1;
};

struct Test2
{
    // x is public
    int x2;
};

int main()
{
    Test1 t1;
    // t1.x1 = 20; // x1 is private

    Test2 t2;
    t2.x2 = 20;
    cout << t2.x2 << endl; // works because x2 is public
}

// Output:
// 20
```

----

## **What do you understand about polymorphism in C++?**

The term polymorphism refers to the presence of multiple forms. Polymorphism usually occurs when there is a hierarchy
of classes that are linked by inheritance. C++ polymorphism means that depending on the type of object that invokes
the function, a different function will be executed.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

// Base class
class Animal
{
public:
    void animalSound()
    {
        cout << "The animal makes a sound \n";
    }
};

// Derived class
class Pig : public Animal
{
public:
    // animalSound method gets overwritten
    void animalSound()
    {
        cout << "The pig says: wee wee \n";
    }
};

// Derived class
class Dog : public Animal
{
public:
    // animalSound method gets overwritten
    void animalSound()
    {
        cout << "The dog says: bow wow \n";
    }
};

int main()
{
    Animal myAnimal;
    Pig myPig;
    Dog myDog;

    myAnimal.animalSound();
    myPig.animalSound();
    myDog.animalSound();
    return 0;
}

// Output:
// The animal makes a sound
// The pig says: wee wee
// The dog says: bow wow
```

----

## **Compare compile time and runtime polymorphism?**

Compile-time Polymorphism
Runtime Polymorphism

The method to be executed is known at compile time. And the call is resolved by the compiler.
The method to be executed is known at run time. The compiler does not resolve the call.

Provides quicker execution because it is known at the compile time.
Provides slower execution because it is known at the run time.

Achieved by operation or function overloading.
Achieved by function overriding. 

- Compile-time Polymorphism

Compile-time polymorphism in C++ is achieved through the use of function overloading and templates. It allows different functions or templates to be selected and called based on the types of the arguments known at compile time. This form of polymorphism is resolved by the compiler during the compilation process.

Here are two common mechanisms for achieving compile-time polymorphism in C++:

1. Function Overloading:

Function overloading enables you to define multiple functions with the same name but different parameter lists. The compiler determines the appropriate function to call based on the types and/or number of arguments provided. The function signature (name and parameter list) is used to differentiate between the overloaded functions.

```c++
void print(int num)
{
    std::cout << "Integer: " << num << std::endl;
}

void print(double num)
{
    std::cout << "Double: " << num << std::endl;
}

int main()
{
    print(10);       // Calls print(int)
    print(3.14);     // Calls print(double)
    return 0;
}
```

In the above example, the print() function is overloaded with different parameter types (int and double). The appropriate function is selected based on the type of argument passed during the function call.

2. Templates:

Templates allow you to write generic code that can be used with different types. Templates are instantiated by the compiler for each specific type used, and the generated code is type-specific. This is known as template specialization.

```c++
template <typename T>
void print(T num)
{
    std::cout << "Value: " << num << std::endl;
}

int main()
{
    print(10);       // Instantiates print<int>(int)
    print(3.14);     // Instantiates print<double>(double)
    print("Hello");  // Instantiates print<const char*>(const char*)
    return 0;
}
```

In this example, the print() function is a template function that can accept any type. The compiler generates the appropriate code for each type used at the call site. This allows for flexibility and code reuse.

Both function overloading and templates provide mechanisms for compile-time polymorphism in C++. The selection of the appropriate function or template specialization is determined at compile time based on the static type information available.

- Run-time Polymorphism

Runtime polymorphism in C++ is achieved through the use of virtual functions and inheritance. It allows objects of different derived classes to be treated as objects of their common base class, and the appropriate function is called based on the actual type of the object at runtime. This form of polymorphism is resolved dynamically during program execution.

Here's how you can achieve runtime polymorphism in C++:

1. Inheritance:
Inheritance allows you to define a base class and derive multiple classes from it. The derived classes inherit the properties and behaviors of the base class. In the context of runtime polymorphism, the base class typically contains virtual functions that can be overridden by the derived classes.

```c++
class Shape
{
public:
    virtual void draw()
    {
        // Default implementation or do nothing
    }
};

class Circle : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a circle." << std::endl;
    }
};

class Rectangle : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a rectangle." << std::endl;
    }
};

int main()
{
    Shape* shape1 = new Circle();
    Shape* shape2 = new Rectangle();

    shape1->draw();   // Calls Circle::draw()
    shape2->draw();   // Calls Rectangle::draw()

    delete shape1;
    delete shape2;
    
    return 0;
}
```

In this example, the Shape class is the base class, and the Circle and Rectangle classes are derived from it. The draw() function in the base class is declared as virtual, indicating that it can be overridden by derived classes. The Circle and Rectangle classes provide their own implementations of the draw() function.

2. Polymorphic Pointers and References:
Polymorphic pointers or references are used to refer to objects of derived classes through a pointer or reference of their base class type. This allows for dynamic dispatch of virtual functions based on the actual type of the object being pointed to or referenced.

```c++
void processShape(Shape* shape)
{
    shape->draw();   // Calls the appropriate draw() function based on the actual object type
}

int main()
{
    Circle circle;
    Rectangle rectangle;

    processShape(&circle);     // Calls Circle::draw()
    processShape(&rectangle);  // Calls Rectangle::draw()

    return 0;
}
```

In this example, the processShape() function takes a pointer to a Shape object. It can accept objects of derived classes since they are implicitly converted to a pointer of their base class type. The draw() function is called inside processShape(), and the appropriate implementation is determined based on the actual object type.

Runtime polymorphism in C++ allows for dynamic dispatch of virtual functions, enabling different behaviors based on the actual type of the object at runtime. This is useful in scenarios where you have a collection of objects of different types but want to treat them uniformly through their common base class interface.

----

## **What is a constructor in C++?**

In C++, a function Object is a particular "MEMBER FUNCTION" that shares the same title as the class it belongs to and is
used to initialize specific values to an object's data members. 

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class student
{
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

## **What is a virtual function?**

A member function in the base class redefined in a derived class is a virtual function. It is declared using
the virtual keyword. It ensures that the correct function is called for an object, irrespective of the type of
reference/pointer used for the function call. Virtual functions are mainly used for runtime polymorphism.  

```c++
// C++ program to illustrate
// concept of Virtual Functions

#include <iostream>
using namespace std;

class base
{
public:
	virtual void print()
    {
        cout << "print base class\n";
    }

	void show()
    {
        cout << "show base class\n";
    }
};

class derived : public base
{
public:
	void print()
    {
        cout << "print derived class\n";
    }

	void show()
    {
        cout << "show derived class\n";
    }
};

int main()
{
	base* bptr;
	derived d;
	bptr = &d;

	// Virtual function, binded at runtime
	bptr->print();

	// Non-virtual function, binded at compile time
	bptr->show();

	return 0;
}
```

----

## **What do you understand about friend class and friend function?**

Like a friend function, a friend class can access personal and guarded variables of the type in which it is declared. All member functions for classes specified as
friends to another class are friend functions for the friend class.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class Node
{
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

## **What are the three different types of C++ access specifiers?**

- Public: All member functions and data members are accessible outside the class.
- Protected: All member functions and data members are accessible within the class and to the derived class.
- Private: All member functions and data members cannot be accessed outside the class. 

----

## **What is an abstraction in C++?**

Abstraction means displaying the essential details to the user while hiding the irrelevant or particular
details that you don’t want to show to a user. It is of two types:
- Control abstraction
- Data abstraction

```c++
// C++ Program to Demonstrate the
// working of Abstraction
#include <iostream>
using namespace std;

class implementAbstraction
{
private:
	int a, b;

public:
	// method to set values of
	// private members
	void set(int x, int y)
	{
		a = x;
		b = y;
	}

	void display()
	{
		cout << "a = " << a << endl;
		cout << "b = " << b << endl;
	}
};

int main()
{
	implementAbstraction obj;
	obj.set(10, 20);
	obj.display();
	return 0;
}
```

----

## **What are destructors in C++?**

A destructor member function is instantly called when an object exits its scope or is specifically deleted by a call to delete.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class X
{
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

## **Is it possible to overload a deconstructor? Give reasons for your answer?**

No, it is impossible as destructors do not take arguments or return anything. There has to be only one empty destructor per class. It should have a void parameter list.  

----

## **What is an abstract class? When is it used?**

An abstract class is a class whose objects cannot be created. It serves as a parent for the derived classes. Placing a pure virtual function in the class makes it an abstract class. 

----

## **What do you understand about static members and static member functions?**

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

A static member function can be called even if no class objects exist. It is accessed using only the class name and the scope resolution operator ```::```.  

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

// C++ Program to demonstrate
// static member in a class

#include <iostream>
#include <string>

using namespace std;

class Student
{
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

## **What is the C++ OOPs concept?**

__OOPs concept in C++:__                                                                               

- Object: Anything that exists physically in the real world is called an object.
- Class: The collection of objects is called class.
- Inheritance: Properties of parent class inherited into child class is known as inheritance.
- Polymorphism: It is the ability to exist in more than one form.
- Encapsulation: Binding of code and data together into a single unit.
- Abstraction: Hiding internal details and showing functionality to the user.

----

## **When is void() return type used?**

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

## **What is call by value and call by reference in C++?**

In the call by value method, you pass the copies of actual parameters to the function's formal parameters. This means
if there is any change in the values inside the function, then that change will not affect the actual values.

```c++
#include <iostream>

using namespace std;
 
// function declaration
void swap(int x, int y);

// function definition to swap the values.
void swap(int x, int y)
{
   int temp;

   temp = x; /* save the value of x */
   x = y;    /* put y into x */
   y = temp; /* put x into y */
  
   return;
}

int main()
{
   // local variable declaration:
   int a = 100;
   int b = 200;
 
   cout << "Before swap, value of a :" << a << endl;
   cout << "Before swap, value of b :" << b << endl;
 
   // calling a function to swap the values.
   swap(a, b);
 
   cout << "After swap, value of a :" << a << endl;
   cout << "After swap, value of b :" << b << endl;
 
   return 0;
}
```

In the call-by-reference method, the reference or address of actual parameters is sent to the function's formal parameters.
This means any change in values inside the function will be reflected in the actual values.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

// function declaration
void swap(int &x, int &y);

// function definition to swap the values.
void swap(int &x, int &y)
{
   int temp;
   temp = x; /* save the value at address x */
   x = y; /* put y into x */
   y = temp; /* put x into y */
  
   return;
}

// For now, let us call the function swap() by passing values by reference as in the following example −

int main()
{
   // local variable declaration:
   int a = 100;
   int b = 200;
 
   cout << "Before swap, value of a :" << a << endl;
   cout << "Before swap, value of b :" << b << endl;

   /* calling a function to swap the values using variable reference.*/
   swap(a, b);

   cout << "After swap, value of a :" << a << endl;
   cout << "After swap, value of b :" << b << endl;
 
   return 0;
}

```

----

## **What is an [inline function?](https://www.geeksforgeeks.org/inline-functions-cpp/)**

An inline function when called expands in line. When you call this function, the whole code of the inline function gets inserted or substituted at the inline function call.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

inline int cube(int s)
{
    return s * s * s;
}

int main()
{
	cout << "The cube of 3 is: " << cube(3) << "\n";
	return 0;
}
```

----

## **What are pointers in C++?**

Pointers are the variables that store the memory address of another variable. The type of the variable must correspond with the type of pointer.

Syntax: type *name

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

int main()
{
    string food = "Pizza"; // A food variable of type string
    string* ptr = &food; // A pointer variable, with the name ptr, that stores the address of food

    // Output the value of food (Pizza)
    cout << food << "\n";

    // Output the memory address of food (0x6dfed4)
    cout << &food << "\n";

    // Output the memory address of food with the pointer (0x6dfed4)
    cout << ptr << "\n";
}

// Output:
// Pizza
// 0000007CD02FF528
// 0000007CD02FF528
```

----

## **What is a scope resolution operator?**

A scope resolution operator is represented as `::`

This operator is used to associate function definition to a particular class.

The scope operator is used for the following purposes:
- To access a global variable when you have a local variable with the same name.
- To define a function outside the class.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>
#include <stdio.h>

using namespace std;

// Define a namespace
namespace MyNamespace
{
    int value = 5;
    
    void printValue()
    {
        std::cout << "Value from MyNamespace: " << value << std::endl;
    }
}

// Define a class
class MyClass
{
public:
    static int value;

    static void printValue()
    {
        std::cout << "Value from MyClass: " << value << std::endl;
    }
};

// Define the static member variable outside the class
int MyClass::value = 10;

int main()
{
    // Accessing namespace member using scope resolution operator
    std::cout << "Value from namespace: " << MyNamespace::value << std::endl;
    MyNamespace::printValue();

    // Accessing class member using scope resolution operator
    std::cout << "Value from class: " << MyClass::value << std::endl;
    MyClass::printValue();

    return 0;
}

// Output:
// Value from namespace: 5
// Value from MyNamespace: 5
// Value from class: 10
// Value from MyClass: 10
```

----

## **What is a constructor?**

A constructor is defined as a member function that is invoked whenever you create an object; it has the same name as that of the class.

There are two types of constructors:
- Default constructor: This auto-generated constructor doesn’t take any arguments.
- Parameterized constructor: In this constructor, it can pass arguments.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class MyClass
{ // The class
public: // Access specifier
    MyClass()
    { // Constructor
        cout << "Hello World!";
    }
};

int main()
{
    MyClass myObj;    // Create an object of MyClass (this will call the constructor)
    return 0;
}

// Output:
// Hwllo World!
```

----

## **Define operator overloading and function overloading?**

An example of compile-time polymorphism is operator overloading.
It is the concept of modifying an existing C++ operator without
altering its original meaning. 

Let us take an example for this 

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

class A
{
};

int main()
{
    A a1, a2, a3;
    // a3 = a1 + a2;
    return 0;
}
```

----

## **How to input strings in C++ with spaces?**

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>
#include <stdio.h>

using namespace std;

int main()
{
    std::string input;

    std::cout << "Enter a sentence: ";
    std::getline(std::cin, input);

    std::cout << "You entered: " << input << std::endl;

    return 0;
}
```

----

## **Discuss the difference between new and malloc?**

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

----

## **What is operator overloading?**

Operator overloading is a mechanism in which a special meaning is given to an operator.

For example, you can overload the `+`-operator in a class-like string to concatenate two strings by only using ‘+.’

----

## **What is a friend function?**

You can define a friend function as a function that can access private, public and protect members of the class. You declare the
friend function with the help of the friend keyword. You declare this function inside the class.

```c++
#include <iostream>
 
using namespace std;
 
class Box
{
   double width;
   
   public:
      friend void printWidth( Box box );
      void setWidth( double wid );
};

// Member function definition
void Box::setWidth( double wid )
{
   width = wid;
}

// Note: printWidth() is not a member function of any class.
void printWidth( Box box )
{
   /* Because printWidth() is a friend of Box, it can
   directly access any member of this class */
   cout << "Width of box : " << box.width <<endl;
}
 
// Main function for the program
int main()
{
   Box box;
 
   // set box width without member function
   box.setWidth(10.0);
   
   // Use friend function to print the wdith.
   printWidth( box );
 
   return 0;
}
```

----

## **Which of the following will give the size of object or type?**

The sizeof operator is used to give the size of object or type.

----

## **Which of the following is not a member of a class?**

- Static function
- Virtual function
- Const function
- Friend function

Among the following, friend function is not a member of the class

----

## **What is STL?**

STL stands for standard template library. It is a library of container templates that provide generic classes and functions.

STL components are containers, algorithms, iterators, and function objects.

----

## **How to write a program to check if a number is a palindrome or not?**

```c++
#include <iostream>

using namespace std;

bool is_palindrome(int num)
{
    int reversed_num = 0;
    int temp_num = num;
    while (temp_num > 0) {
        int digit = temp_num % 10;
        reversed_num = (reversed_num * 10) + digit;
        temp_num /= 10;
    }

    return (reversed_num == num);
}

int main()
{
    int num;
    cout << "Enter a number: ";
    cin >> num;
    if (is_palindrome(num)) {
        cout << num << " is a palindrome" << endl;
    } else {
        cout << num << " is not a palindrome" << endl;
    }

    return 0;
}
```

----

## **What is a copy constructor?**

A copy function is a member function that uses another object from the same class to initialize a new thing. A copy
function is, to put it simply, a function that produces an object by initializing it with a different object of the
same class that has already been constructed.

```c++
// TestApplication.cpp : Copy constructor example.
//

#include <iostream>  

using namespace std;

class A
{
public:
    int x;

    A(int a) // parameterized constructor.  
    {
        x = a;
    }

    A(A& i) // copy constructor  
    {
        x = i.x;
    }
};

int main()
{
    A a1(20); // Calling the parameterized constructor.  
    A a2(a1); // Calling the copy constructor.  
    cout << a2.x;
    return 0;
}

// Output:
// 20
```

----

## **Write a program to find the factorial of a number?**

```c++
#include <iostream>

using namespace std;

int factorial(int n)
{
    if (n == 0 || n == 1)
    {
        return 1;
    }
    else
    {
        return n * factorial(n-1);
    }
}

int main()
{
    int n;
    cout << "Enter a number: ";
    cin >> n;
    cout << "Factorial of " << n << " is " << factorial(n) << endl;
    return 0;
}
```

----

## **What is inheritance?**

Inheritance is the mechanism in which you can create a new class i.e. child class from the existing class
i.e. parent class. This child class is also known as a derived class and the parent class is also called Base class. 

----

## **What is Abstraction?**

Abstraction can be defined as a technique in which you only show functionality to the
user i.e., the details that you want the user to see, hiding the internal details or implementation details.

----

## **How to find the frequency of a number in C++?**

```c++
#include <iostream>

using namespace std;

int frequency(int arr[], int n, int x)
{
    int count = 0;
    for (int i = 0; i < n; i++)
    {
        if (arr[i] == x)
        {
            count++;
        }
    }
    
    return count;
}

int main()
{
    int arr[] = {1, 2, 3, 4, 5, 2, 3, 2};
    int n = sizeof(arr) / sizeof(arr[0]);
    int x = 2;
    int freq = frequency(arr, n, x);
    cout << "Frequency of " << x << " is " << freq << endl;
    return 0;
}
```

----

## **What should be the correct statement about string objects in C++?**

- String objects should necessarily be terminated by a null character
- String objects have a static size
- String objects have a dynamic size (true)
- String objects use extra memory than required 

----

## **How is a shallow copy different from a deep copy?**

Shallow Copy
Deep Copy

It stores the references of objects to the original memory address.
It makes a fresh and separate copy of an entire object and its unique memory address.

Faster
Comparatively slower

It reflects changes made to the new/copied object in the original object.
It doesn’t reflect changes made to the new/copied object in the original object.

----

## **How are virtual functions different from pure virtual functions?**

A virtual function is a base class member function that a derived class can modify. A member function of a base class that
is a pure virtual function must be defined in the derived type; otherwise, the derived class will become abstract as well.

*Virtual Function:*

A virtual function is a member function of a class that can be overridden in derived classes.
It is declared using the virtual keyword in the base class.
The base class provides a default implementation for the virtual function, which can be overridden by derived classes to provide their specific implementation.
A virtual function can have an implementation in the base class, and it can also be declared as = 0 to make it a pure virtual function.
A virtual function in the base class can be called using a pointer or reference to the base class, and the derived class's implementation will be invoked dynamically at runtime.
Here's an example that demonstrates the usage of a virtual function:

```c++
#include <iostream>

class Shape
{
public:
    virtual void draw()
    {
        std::cout << "Drawing a shape." << std::endl;
    }
};

class Circle : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a circle." << std::endl;
    }
};

int main()
{
    Shape* shape = new Circle();
    shape->draw();  // Output: Drawing a circle.
    delete shape;
    
    return 0;
}
```

In this example, the Shape class has a virtual function draw(), which provides a default implementation for drawing a shape. The Circle class derives from Shape and overrides the draw() function to provide its specific implementation for drawing a circle.

In the main() function, we create a pointer of type Shape* that points to a Circle object. When we call the draw() function through the base class pointer, the derived class's implementation is invoked dynamically at runtime, and the output is "Drawing a circle."

*Pure Virtual Function:*

A pure virtual function is a virtual function that is declared in the base class but does not have any implementation in the base class.
It is declared using the virtual keyword and followed by = 0 in the base class.
The base class cannot be instantiated because it contains a pure virtual function, making it an abstract class.
Derived classes must override the pure virtual function and provide their specific implementation.
Pure virtual functions define an interface that derived classes must adhere to.

```c++
#include <iostream>

class Animal {
public:
    virtual void makeSound() const = 0;  // Pure virtual function
};

class Dog : public Animal {
public:
    void makeSound() const override {
        std::cout << "Woof!" << std::endl;
    }
};

int main() {
    // Animal* animal = new Animal();  // Error: Cannot instantiate abstract class

    Animal* dog = new Dog();
    dog->makeSound();  // Output: Woof!

    delete dog;
    return 0;
}
```

In this example, the Animal class has a pure virtual function makeSound(), which does not provide any implementation. The Dog class derives from Animal and overrides the makeSound() function to provide its specific implementation for making the sound of a dog.

Since the Animal class contains a pure virtual function, it cannot be instantiated. However, we can create a pointer of type Animal* that points to a Dog object. When we call the makeSound() function through the base class pointer, the derived class's implementation is invoked, and the output is "Woof!"

Pure virtual functions allow for defining an interface or base behavior

----

## **Class D is derived from a base class B. If creating an object of type D, what order will the constructors of these classes get called?**

The derived class consists of two parts: the base part and the derived part. C++ constructs derived objects in phases. The process begins with
constructing the most-base class (at the top of the inheritance tree), followed by each child class construction in order, and then the
most-child class. Thus, first, the Constructor of class B will be called, and then the constructor of class D. 

----

## **Can a virtual function be called from a constructor?**

A virtual process may be called a function Object, but exercise caution. It might perform differently than expected. The virtual call mechanism in a function Object is disabled since overriding from derived classes hasn't happened yet. Building blocks are used to create objects, "base before derived."

```c++
class Animal
{
public:
    virtual void makeSound() const = 0;  // Pure virtual function

    void eat()
    {
        std::cout << "The animal is eating." << std::endl;
    }
};

class Dog : public Animal
{
public:
    void makeSound() const override
    {
        std::cout << "The dog barks." << std::endl;
    }
};

class Cat : public Animal
{
public:
    void makeSound() const override
    {
        std::cout << "The cat meows." << std::endl;
    }
};

int main()
{
    // Animal animal;   // Error: Cannot instantiate an abstract class
    Dog dog;
    Cat cat;

    dog.makeSound();   // Calls Dog::makeSound()
    cat.makeSound();   // Calls Cat::makeSound()

    dog.eat();         // Calls Animal::eat()
    cat.eat();         // Calls Animal::eat()

    return 0;
}
```

----

In this example, the Animal class is an abstract class because it contains a pure virtual function makeSound(). The makeSound() function is declared with = 0 at the end, indicating that it has no implementation in the base class. The derived classes, Dog and Cat, must provide their own implementations for the makeSound() function to become concrete classes.

----

## **What are void pointers?**

In C, a void pointer has no connection to any particular data type. It designates a location for specific data within the storage.
This indicates that it is pointing to a variable's address. It also goes by the name "general purpose pointer."

```c++
#include <iostream>
#include <string>
#include <stdio.h>
#include <math.h>
#include <stdbool.h>

using namespace std;

int main()
{
    int a = 10;
    char b = 'x';
    void* p = &a; // void pointer holds address of int 'a'
    p = &b; // void pointer holds address of char 'b'
}
```

----

## **What is this pointer in C++?**

A class, struct, or union form only has access to this pointer within non-static member variables. The arrow shows the object for which the member function is called. 

```c++
// TestApplication.cpp : Pointer example.
//

#include <iostream>
#include <string>
#include <stdio.h>
#include <math.h>
#include <stdbool.h>

using namespace std;

int main()
{
	string food = "Pizza"; // A food variable of type string
	string* ptr = &food; // A pointer variable, with the name ptr, that stores the address of food
	// Output the value of food (Pizza)
	cout << food << "\n";
	// Output the memory address of food (0x6dfed4)
	cout << &food << "\n";
	// Output the memory address of food with the pointer (0x6dfed4)
	cout << ptr << "\n";
}
```

----

## **How would you deallocate and allocate memory in C++?**

The heap is used in C to allocate dynamic memory, and these functions are part of the standard library. Malloc() and free are the
two important dynamic memory operations (). The size of the desired memory area in bytes is the only parameter accepted by the malloc() function. 

```c++
// TestApplication.cpp : Deallocate and allocate memory.
//

#include <iostream>
#include <string>
#include <stdio.h>
#include <math.h>
#include <stdbool.h>
#include <cstdlib>
#include <cstring>

using namespace std;

int main()
{
	char* user;
	user = (char*)malloc(25);
	strcpy(user, "Jane_Eyre");
	cout << "User Name = " << user << " " << &user << endl;
	free(user);
}
```

# https://www.simplilearn.com/tutorials/cpp-tutorial/cpp-interview-questions

# https://www.interviewbit.com/cpp-interview-questions

## **What are the different data types present in C++?**

The 4 data types in C++ are given below:

- Primitive Datatype(basic datatype). Example- char, short, int, float, long, double, bool, etc.
- Derived datatype. Example- array, pointer, etc.
- Enumeration. Example- enum
- User-defined data types. Example- structure, class, etc.

## **What will be the output of the following C++ program:**

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

int main()
{
	int a = 1;
	cout << (a++) * (++a) << endl;
	return 0;
}

// Output:
// 4
```

----

## **What will be the value of x in the following C++ program?**

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>

using namespace std;

int main()
{
	int a = 1;
	int x = (a++)++;
	cout << x << endl;
}

// Output:
// Compile Time Error
// Severity	Code	Description	Project	File	Line	Suppression State
// Error (active)	E0137	expression must be a modifiable lvalue	TestApplication	C:\Users\chris\OneDrive\Desktop\Christoph16478_github\.GITIGNORE\TestApplication\TestApplication\TestApplication.cpp	12	
```

----

## **What is an abstract class?**

An interface describes the behavior or capabilities of a C++ class without committing to a particular implementation of that class.

The C++ interfaces are implemented using abstract classes and these abstract classes should not be confused with data abstraction
which is a concept of keeping implementation details separate from associated data.

```c++
#include <iostream>
 
using namespace std;

// Base class
class Shape
{
public:
    // pure virtual function providing interface framework.
    virtual int getArea() = 0;
    void setWidth(int w)
    {
        width = w;
    }

    void setHeight(int h)
    {
        height = h;
    }

protected:
    int width;
    int height;
};

// Derived classes
class Rectangle : public Shape
{
public:
    int getArea()
    {
        return (width * height);
    }
};

class Triangle : public Shape
{
public:
    int getArea()
    {
        return (width * height) / 2;
    }
};

int main(void)
{
    Rectangle Rect;
    Triangle  Tri;

    Rect.setWidth(5);
    Rect.setHeight(7);

    // Print the area of the object.
    cout << "Total Rectangle area: " << Rect.getArea() << endl;

    Tri.setWidth(5);
    Tri.setHeight(7);

    // Print the area of the object.
    cout << "Total Triangle area: " << Tri.getArea() << endl;

    return 0;
}
```

----

## **Consider the following C++ program?**

What will be output?
A B
B A
Compile-time error
None of the above

```c++
#include <iostream>

using namespace std;

class A
{
public:
	virtual void a() = 0;
	A()
	{
		cout << "A ";
	}
};

class B : public A
{
public:
	B()
	{
		cout << "B ";
	}
};

int main() {
	A* a = new B();
	return 0;
}

// Output
// Compile-time error
```

----

## **What is the size of void in C++?**

The size of void pointer varies system to system. If the system is 16-bit, size of void pointer is 2 bytes.
If the system is 32-bit, size of void pointer is 4 bytes. If the system is 64-bit, size of void pointer is 8 bytes.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>
#include <stdio.h>

using namespace std;

int main()
{	
	void* ptr;
	printf("The size of pointer value : %d", sizeof(ptr));
	return 0;
} 
```

----

## **Which of the following statement is correct?**

- An object is an instance of the class (true)
- A friend function can access private members of a class (true)
- Members of the class are private by default
- All of the above

# https://www.interviewbit.com/cpp-interview-questions

# https://www.javatpoint.com/cpp-interview-questions

## **Define namespace in C++?**

The namespace is a logical division of the code which is designed to stop the naming conflict.
The namespace defines the scope where the identifiers such as variables, class, functions are declared.
The main purpose of using namespace in C++ is to remove the ambiguity. Ambiquity occurs when the different task occurs with the same name.
For example: if there are two functions exist with the same name such as add(). In order to prevent this ambiguity, the namespace is used. Functions are declared in different namespaces.
C++ consists of a standard namespace, i.e., std which contains inbuilt classes and functions. So, by using the statement "using namespace std;" includes the namespace "std" in our program.

Syntax of namespace:

```c++
namespace namespace_name  
{
    // body of namespace;  
}
```

Syntax of accessing the namespace variable:

```c++
namespace_name::member_name;
```

Let's understand this through an example:

```c++
// TestApplication.cpp : Nemsapce example.
//

#include <iostream>
#include <string>
#include <stdio.h>
#include <math.h>
#include <stdbool.h>
#include <cstdlib>
#include <cstring>

using namespace std;

namespace addition
{
    int a = 5;
    int b = 5;
    
    int add()
    {
        return(a + b);
    }
}

int main()
{
    int result;
    result = addition::add();
    cout << result;
    return 0;
}

// Output:
// 10
```

----
    
## **Define token in C++?**

A token in C++ can be a keyword, identifier, literal, constant and symbol.

Examples: 

__1. Identifiers:__

Identifiers are names given to variables, functions, classes, or other entities in a program. They consist of a sequence of letters, digits, and underscores. They must begin with a letter or an underscore. Examples of 

```c++
int age;
double pi;
class MyClass;
```

__2. Keywords:__

Keywords are reserved words in C++ that have a specific meaning and cannot be used as identifiers. Examples of keywords:

```c++
int
double
class
if
else

```

__3. Constants:__

Constants represent fixed values that do not change during the execution of a program. They can be of various types, such as integer, floating-point, character, or string constants. Examples of constants:

```c++
42        // Integer constant
3.14      // Floating-point constant
'a'       // Character constant
"Hello"   // String constant

```

__4. Operators:__

Operators perform operations on operands and produce a result. Examples of operators:

```c++
+   // Addition operator
-   // Subtraction operator
*   // Multiplication operator
/   // Division operator
=   // Assignment operator
```

__5. Punctuation Symbols:__

Punctuation symbols are used for grouping, separating, and terminating statements or expressions. Examples of punctuation symbols:

```c++
;    // Semicolon
,    // Comma
.    // Dot (used for member access)
()   // Parentheses
{}   // Braces
```

----

## **Who was the creator of C++?**

Bjarne Stroustrup.

----

## **hich operations are permitted on pointers?**

Following are the operations that can be performed on pointers:

Incrementing or decrementing a pointer: Incrementing a pointer means that we can increment the pointer by the size of a data type to which it points.
There are two types of increment pointers:

__1. Pre-increment pointer:__

The pre-increment operator increments the operand by 1, and the value of the expression becomes the resulting value of the incremented.
Suppose ptr is a pointer then pre-increment pointer is represented as ++ptr.

Let's understand this through an example:

```c++
#include <iostream>  

using namespace std;

int main()
{
    int a[5] = { 1,2,3,4,5 };
    int* ptr;
    ptr = &a[0];
    cout << "Value of *ptr is : " << *ptr << "\n";
    cout << "Value of *++ptr : " << *++ptr;
    return 0;
}

// Output:
// Value of *ptr is : 1
// Value of *++ptr : 2
```

__2. Post-increment pointer:__

The post-increment operator increments the operand by 1, but the value of the expression will be the value of the operand
prior to the incremented value of the operand. Suppose ptr is a pointer then post-increment pointer is represented as ptr++.

Let's understand this through an example:

```c++
#include <iostream>  

using namespace std;  

int main()
{
	int a[5] = { 1,2,3,4,5 };
	int* ptr;
	ptr = &a[0];
	cout << "Value of *ptr is : " << *ptr << "\n";
	cout << "Value of *ptr++ : " << *ptr++;
	return 0;
}

// Output:
// Value of *ptr is : 1
// Value of *ptr++ : 1
// Subtracting a pointer from another pointer: When two pointers pointing to the members of an array are subtracted, then the number of elements present between the two members are returned.
```

----

## **Define 'std'?**

Std is the default namespace standard used in C++.

----

## **Which programming language's unsatisfactory performance led to the discovery of C++?**

C++ was discovered in order to cope with the disadvantages of C.

----

## **How delete[] is different from delete?**

Delete is used to release a unit of memory, delete[] is used to release an array.

*1. delete:*

The delete operator is used to deallocate memory that was allocated for a single object using the new operator. It calls the destructor of the object being deleted and frees the memory occupied by that object.

```c++
int* singleNumber = new int;
// Use singleNumber...
delete singleNumber;  // Deallocate memory for a single integer
```

*2. delete[]:*

The delete[] operator is used to deallocate memory that was allocated for an array of objects using the new[] operator. It calls the destructors of all the objects in the array (in reverse order) and frees the memory occupied by the entire array.

```c++
int* numbers = new int[5];
// Use numbers...
delete[] numbers;  // Deallocate memory for an array of integers
```

It is important to note that using delete instead of delete[] (or vice versa) for deallocating dynamically allocated arrays can lead to undefined behavior. When allocating memory for an array with new[], you must deallocate it with delete[], and when allocating memory for a single object with new, you must deallocate it with delete.

----

## **What is the full form of STL in C++?**

STL stands for Standard Template Library.

----

## **What is an object?**

The Object is the instance of a class. A class provides a blueprint for objects. So you can create an object from a class. The objects of
a class are declared with the same sort of declaration that we declare variables of basic types.

----

## **What are the C++ access specifiers?**

The access specifiers are used to define how to functions and variables can be accessed outside the class.

There are three types of access specifiers:
- Private: Functions and variables declared as private can be accessed only within the same class, and they cannot be accessed outside the class they are declared.
- Public: Functions and variables declared under public can be accessed from anywhere.
- Protected: Functions and variables declared as protected cannot be accessed outside the class except a child class. This specifier is generally used in inheritance.

----

## **What is Object Oriented Programming (OOP)?**

OOP is a methodology or paradigm that provides many concepts. The basic concepts of Object Oriented Programming are given below:

*Classes and Objects:* Classes are used to specify the structure of the data. They define the data type. You can create any number
of objects from a class. Objects are the instances of classes.

*Encapsulation:* Encapsulation is a mechanism which binds the data and associated operations together and thus hides the data
from the outside world. Encapsulation is also known as data hiding. In C++, It is achieved using the access specifiers,
i.e., public, private and protected.

```c++
#include <iostream>
#include <string>

class Person
{
private:
    std::string name;
    int age;

public:
    // Setter methods
    void setName(const std::string& newName)
    {
        name = newName;
    }

    void setAge(int newAge)
    {
        age = newAge;
    }

    // Getter methods
    std::string getName() const
    {
        return name;
    }

    int getAge() const
    {
        return age;
    }
};

int main()
{
    Person person;

    person.setName("John");
    person.setAge(30);

    std::cout << "Name: " << person.getName() << std::endl;
    std::cout << "Age: " << person.getAge() << std::endl;

    return 0;
}
```

*Abstraction:* Abstraction is used to hide the internal implementations and show only the necessary details to the outer world.
Data abstraction is implemented using interfaces and abstract classes in C++.

Some people confused about Encapsulation and abstraction, but they both are different.

```c++
#include <iostream>

// Abstract class
class Shape
{
public:
    virtual double getArea() const = 0;  // Pure virtual function

    virtual void print() const
    {
        std::cout << "This is a shape." << std::endl;
    }
};

// Concrete classes derived from the Shape class
class Circle : public Shape
{
private:
    double radius;

public:
    Circle(double radius) : radius(radius)
    {
    }

    double getArea() const override
    {
        return 3.14 * radius * radius;
    }

    void print() const override
    {
        std::cout << "This is a circle." << std::endl;
    }
};

class Rectangle : public Shape
{
private:
    double length;
    double width;

public:
    Rectangle(double length, double width) : length(length), width(width)
    {
    }

    double getArea() const override
    {
        return length * width;
    }

    void print() const override
    {
        std::cout << "This is a rectangle." << std::endl;
    }
};

int main()
{
    Circle circle(5.0);
    Rectangle rectangle(4.0, 6.0);

    // Using polymorphic behavior
    Shape* shape1 = &circle;
    Shape* shape2 = &rectangle;

    shape1->print();  // Calls Circle::print()
    std::cout << "Area: " << shape1->getArea() << std::endl;

    shape2->print();  // Calls Rectangle::print()
    std::cout << "Area: " << shape2->getArea() << std::endl;

    return 0;
}
```

*Inheritance:* Inheritance is used to inherit the property of one class into another class. It facilitates you to define one class in term of another class.

```c++
#include <iostream>
#include <string>

// Base class
class Vehicle
{
protected:
    std::string brand;

public:
    Vehicle(const std::string& brand) : brand(brand)
    {
    }

    void honk()
    {
        std::cout << "Beep beep!" << std::endl;
    }
};

// Derived class
class Car : public Vehicle
{
private:
    int numWheels;

public:
    Car(const std::string& brand, int numWheels) : Vehicle(brand), numWheels(numWheels)
    {
    }

    void drive()
    {
        std::cout << "Driving a car with " << numWheels << " wheels." << std::endl;
    }
};

// Derived class
class Bicycle : public Vehicle
{
private:
    int numGears;

public:
    Bicycle(const std::string& brand, int numGears) : Vehicle(brand), numGears(numGears)
    {
    }

    void pedal()
    {
        std::cout << "Pedaling a bicycle with " << numGears << " gears." << std::endl;
    }
};

int main() {
    Car car("Toyota", 4);
    Bicycle bicycle("Giant", 18);

    car.honk();        // Inherited from Vehicle
    car.drive();       // Defined in Car

    bicycle.honk();    // Inherited from Vehicle
    bicycle.pedal();   // Defined in Bicycle

    return 0;
}
```

----

## **What is the difference between an array and a list?**

An Array is a collection of homogeneous elements while a list is a collection of heterogeneous elements.
Array memory allocation is static and continuous while List memory allocation is dynamic and random.
In Array, users don't need to keep in track of next memory allocation while In the list, the user has to keep in track of next location where memory is allocated.

----

## **What is the difference between new() and malloc()?**

new() is a preprocessor while malloc() is a function.

There is no need to allocate the memory while using "new" but in malloc() you have to use sizeof().

"new" initializes the new memory to 0 while malloc() gives random value in the newly allotted memory location.

The new() operator allocates the memory and calls the constructor for the object initialization and malloc() function allocates the memory but does not call the constructor for the object initialization.

The new() operator is faster than the malloc() function as operator is faster than the function.

----

## **What are the methods of exporting a function from a DLL?**

There are two ways:
- By using the DLL's type library.
- Taking a reference to the function from the DLL instance.

----

## **Define friend function?**

Friend function acts as a friend of the class. It can access the private and protected members of the class. The friend function is not a member of the class,
but it must be listed in the class definition. The non-member function cannot access the private data of the class. Sometimes, it is necessary for the non-member
function to access the data. The friend function is a non-member function and has the ability to access the private data of the class.

To make an outside function friendly to the class, we need to declare the function as a friend of the class as shown below:

```c++
class sample  
{  
// data members;  
public:  
    friend void abc(void);  
};  
```

Following are the characteristics of a friend function:

The friend function is not in the scope of the class in which it has been declared. Since it is not in the scope of the class, so it cannot be
called by using the object of the class. Therefore, friend function can be invoked like a normal function. A friend function cannot access the
private members directly, it has to use an object name and dot operator with each member name. Friend function uses objects as arguments.

Let's understand this through an example:

```c++
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

// Output:
// 11
```

----

## **What is virtual inheritance?**

Virtual inheritance facilitates you to create only one copy of each object even if the object appears more than one in the hierarchy.

```c++
#include <iostream>

// Base class
class Animal
{
public:
    void eat()
    {
        std::cout << "Animal is eating." << std::endl;
    }
};

// Intermediate base class with virtual inheritance
class Mammal : public virtual Animal
{
public:
    void walk()
    {
        std::cout << "Mammal is walking." << std::endl;
    }
};

// Intermediate base class with virtual inheritance
class Bird : public virtual Animal
{
public:
    void fly()
    {
        std::cout << "Bird is flying." << std::endl;
    }
};

// Derived class inheriting from Mammal and Bird
class Bat : public Mammal, public Bird
{
public:
    void feedYoungOnMilk()
    {
        std::cout << "Bat is feeding its young on milk." << std::endl;
    }
};

int main()
{
    Bat bat;

    bat.eat();            // Resolves ambiguity by using virtual inheritance from Animal
    bat.walk();           // Inherited from Mammal
    bat.fly();            // Inherited from Bird
    bat.feedYoungOnMilk(); // Defined in Bat

    return 0;
}
```

----

## **What is polymorphism in C++?**

Polymorphism is known as many forms of the same thing. In simple terms, we can say that Polymorphism is the ability to display a member
function in multiple forms depending on the type of object that calls them. 

In other words, we can also say that a man can be an employee to someone, a son of someone, a father of someone, and a husband of someone;this is how polymorphism can be projected in real life.

There is 2 type of polymorphism:

- Compile Time Polymorphism
    - Function Overloading
    - Operator Overloading
- Run Time Polymorphism
    - Function Overriding
    - Virtual Function

Examples are provided above in this document

----

## **What are the different types of polymorphism in C++?**

There is 2 type of polymorphism:

__Compile Time Polymorphism or Static Binding__

This type of polymorphism is achieved during the compile time of the program which results in it making a bit faster than Run time. Also, Inheritance is not involved in it. It is comprised of 2 further techniques:

Function Overloading: When there are multiple functions with the same name but different parameters then this is known as function overloading.

```c++
// same name different arguments
int GFG()
{  
}

int GFG(int a)
{
}

float GFG(double a)
{
}

int GFG(int a, double b)
{
}

Operator Overloading:

It is basically giving practice of giving a special meaning to the existing meaning of an operator or in simple terms redefining the pre-redefined meaning

class GFG
{
    // private and other modes
    statements

    public:
        returnType operator symbol (arguments)
        {
            statements
        }
    statements
};
```   

__Run-Time Polymorphism or Late Binding__

Run-time polymorphism takes place when functions are invoked during run time. 
 
Function Overriding:

Function overriding occurs when a base class member function is redefined in a derived class with the same arguments and return type.

```c++
// C++ program to demonstrate 
// Function overriding

#include <iostream>

using namespace std;

class GFG
{
    public:
    virtual void display()
    {
        cout<<"Function of base class"<<endl;
    }
};

class derived_GFG : public GFG
{
    public:
    void show()
    {
        cout<<"Function of derived class"<<endl;
    }
};

int main()
{
    derived_GFG dg;
    dg.show();
    return 0;
}
// Output:
// Function of derived class
// For more information, refer to Different types of Polymorphism
```

----

## **Compare compile-time polymorphism and Runtime polymorphism?**

| Compile-Time | Polymorphism Runtime Polymorphism |
| ------------ | --------------------------- |
| It is also termed static binding and early binding. | It is also termed Dynamic binding and Late binding. |
| It is fast because execution is known early at compile time. | It is slow as compared to compile-time because execution is known at runtime. |
| It is achieved by function overloading and operator overloading. | It is achieved by virtual functions and function overriding. |
| For more information | refer to Compile-time polymorphism and Runtime polymorphism |

----

## **Explain the constructor in C++?**

A constructor is a special type of member function of a class, whose name is the same as that of the class by whom it is invoked and initializes
value to the object of a class. 

There are 3 types of constructors:

__A. Default constructor:__

It is the most basic type of constructor which accepts no arguments or parameters. Even if it is not called the compiler
calls it automatically when an object is created.

Example:

```c++
class Class_name
{
public:
    Class_name()
    {
        cout << "I am a default constructor" << endl;
    }
};
```

__B. Parameterized constructor:__

It is a type of constructor which accepts arguments or parameters. It has to be called explicitly by
passing values in the arguments as these arguments help initialize an object when it is created. It also has the same name as that of the class. 

Also, It is used to overload constructors.

Example:

```c++
// CPP program to demonstrate
// parameterized constructors
#include <iostream>

using namespace std;

class GFG
{
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

// Output
// G.x = 10, G.y = 15
```

__C. Copy Constructor:__

A copy constructor is a member function that initializes an object using another object of the same class. Also,
the Copy constructor takes a reference to an object of the same class as an argument.

Example:

```c++
Sample(Sample& t) 
{
    id = t.id;
}
```

----

## **Which operations are permitted on pointers?**

Pointers are the variables that are used to store the address location of another variable. Operations that are permitted to a pointer are:
- Increment/Decrement of a Pointer
- Addition and Subtraction of integer to a pointer
- Comparison of pointers of the same type

----

## **Define inline function. Can we have a recursive inline function in C++?**

An inline function is a form of request not an order to a compiler which results in the inlining of our function to the main function
body. An inline function can become overhead if the execution time of the function is less than the switching time from the caller function
to called function. To make a function inline use the keyword inline before and define the function before any calls are made to the function.

- Inline Function
- Inline Function Explanation

Syntax:

```c++
inline data_type function_name()
{
    Body;
}
```

The answer is No; It cannot be recursive.

An inline function cannot be recursive because in the case of an inline function the code is merely placed into the position from where it
is called and does not maintain a piece of information on the stack which is necessary for recursion.

Plus, if you write an inline keyword in front of a recursive function, the compiler will automatically ignore it because the inline is only taken as a suggestion by the compiler.

For more information, refer to Inline Function

----

## **What is an abstract class and when do you use it?**

An abstract class is a class that is specifically designed to be used as a base class. An abstract class contains at least one pure virtual function. You declare a pure virtual
function by using a pure specifier(= 0) in the declaration of a virtual member function in the class declaration

You cannot use an abstract class as a parameter type, a function return type, or the type of an explicit conversion, nor can you declare an object of an abstract class.
However, it can be used to declare pointers and references to an abstract class. 

An abstract class is used if you want to provide a common, implemented functionality among all the implementations of the component. Abstract classes will allow you to
partially implement your class, whereas interfaces would have no implementation for any members whatsoever. In simple words, Abstract Classes are a good fit if you want
to provide implementation details to your children but don’t want to allow an instance of your class to be directly instantiated.

```c++
#include <iostream>

// Abstract base class
class Shape
{
public:
    virtual double getArea() const = 0;  // Pure virtual function

    void print() const
    {
        std::cout << "This is a shape." << std::endl;
    }
};

// Derived class
class Circle : public Shape
{
private:
    double radius;

public:
    Circle(double radius) : radius(radius)
    {
    }

    double getArea() const override
    {
        return 3.14 * radius * radius;
    }

    void print() const override
    {
        std::cout << "This is a circle." << std::endl;
    }
};

// Derived class
class Rectangle : public Shape
{
private:
    double length;
    double width;

public:
    Rectangle(double length, double width) : length(length), width(width)
    {
    }

    double getArea() const override
    {
        return length * width;
    }

    void print() const override
    {
        std::cout << "This is a rectangle." << std::endl;
    }
};

int main()
{
    Circle circle(5.0);
    Rectangle rectangle(4.0, 6.0);

    // Using polymorphic behavior
    Shape* shape1 = &circle;
    Shape* shape2 = &rectangle;

    shape1->print();  // Calls Circle::print()
    std::cout << "Area: " << shape1->getArea() << std::endl;

    shape2->print();  // Calls Rectangle::print()
    std::cout << "Area: " << shape2->getArea() << std::endl;

    return 0;
}
```

In this example, the Shape class is an abstract class because it contains a pure virtual function getArea(). The pure virtual function is declared using = 0 at the end, indicating that it has no implementation in the base class. The Circle and Rectangle classes are derived from the Shape class and provide their own implementations for the getArea() function.

Note that attempting to instantiate an object of the abstract class Shape directly will result in a compilation error. The abstract class serves as a common interface for the derived classes and provides a way to achieve polymorphic behavior through pointer or reference variables.

----

## **What is the main use of the keyword "Volatile"?**

Just like its name, things can change suddenly and unexpectantly; So it is used to inform the compiler that the value may change anytime. Also, the volatile
keyword prevents the compiler from performing optimization on the code. It was intended to be used when interfacing with memory-mapped hardware, signal
handlers, and machine code instruction.

For more information, refer to this Volatile

```c++
#include <iostream>

int main()
{
    volatile int counter = 0;

    while (counter < 10)
    {
        std::cout << "Counter: " << counter << std::endl;
        counter++;
    }

    return 0;
}
```

In this example, the variable counter is declared as volatile. This indicates to the compiler that the value of counter can change unexpectedly, and the compiler should not make assumptions about its value during optimization. This is important when dealing with variables that can be modified by hardware, interrupts, or other external factors.

By using the volatile keyword, you ensure that the value of counter is read from memory each time it is accessed within the while loop, rather than relying on a cached value. This ensures that any changes to counter from external sources are taken into account.

It's worth noting that the volatile keyword should be used carefully and only when necessary. It is typically used when dealing with hardware registers, multi-threaded environments, or when interacting with memory-mapped I/O devices. In most cases, regular variables are sufficient for general programming needs.

----

## **Define storage class in C++ and name some**

Storage class is used to define the features(lifetime and visibility) of a variable or function. These features usually help in tracing the existence of a variable during the runtime of a program.

Syntax:

```c++
storage_class var_data_type var_name; 
```

Some types of storage classes:

Examples of storage class

```c++
#include <iostream>

void incrementCount()
{
    static int count = 0;  // Static variable

    count++;
    std::cout << "Count: " << count << std::endl;
}

int main() {
    for (int i = 0; i < 5; i++)
    {
        incrementCount();
    }

    return 0;
}
```

In this example, the incrementCount() function contains a static variable count. When the function is called multiple times, the count variable retains its value between invocations.

The static storage class has the following characteristics:

- The static variable is initialized only once, during the first execution of the function.
- The variable retains its value between function calls.
- The scope of the variable is limited to the block or function in which it is defined.
- The lifetime of the variable is throughout the program execution.

In the example above, the count variable is incremented and printed on each function call, but its value is retained due to its static nature. This can be useful in scenarios where you need to maintain state or keep track of the number of times a function is called without using a global variable.

----

## **What is a mutable storage class specifier? How can they be used?**

Just like its name, the mutable storage class specifier is used only on a class data member to make it modifiable even though
the member is part of an object declared as const. Static or const, or reference members cannot use the mutable specifier.
When we declare a function as const, this pointer passed to the function becomes const.

----

## **Define the Block scope variable?**

So the scope of a variable is a region where a variable is accessible. There are two scope regions, A global and block or local. 

A block scope variable is also known as a local scope variable. A variable that is defined inside a function (like main) or inside a
block (like loops and if blocks) is a local variable. It can be used ONLY inside that particular function/block in which it is declared.
a block-scoped variable will not be available outside the block even if the block is inside a function.

For more information, refer to Scope of a variable

----

## **What is the function of the keyword “Auto”?**

The auto keyword may be used to declare a variable with a complex type in a straightforward fashion. You can use auto to declare a variable if the initialization phrase contains templates, pointers to functions, references to members, etc. With type inference capabilities, we can spend less time having to write out things the compiler already knows. As all the types are deduced in the compiler phase only, the time for compilation increases slightly but it does not affect the runtime of the program. 

----

## **Can we call a virtual function from a constructor?**

Yes, we can call a virtual function from a constructor. But it can throw an exception of overriding.

----

## **What are void pointers?**

Just like its name a void pointer is a pointer that is not associated with anything or with any data type. Nevertheless,
a void pointer can hold the address value of any type and can be converted from one data type to another.

# https://www.geeksforgeeks.org/cpp-interview-questions

# https://www.toptal.com/c-plus-plus/interview-questions

## **What will the line of code below print out and why?**

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>
#include <stdio.h>

using namespace std;

int main(int argc, char** argv)
{	
    std::cout << 25u - 50;
    return 0;
}

// Output:
// 4294967271
```

----

## **What is the error in the code below and how should it be corrected?**

```c++
my_struct_t *bar;
/* ... do stuff, including setting bar to point to a defined my_struct_t object ... */
memset(bar, 0, sizeof(bar));
```

Solution:

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>
#include <stdio.h>

using namespace std;

struct my_struct_t
{
};

int main()
{	
	my_struct_t* bar = nullptr;
	/* ... do stuff, including setting bar to point to a defined my_struct_t object ... */
	memset(bar, 0, sizeof(bar));
}
```

----

## **What will i and j equal after the code below is executed? Explain your answer?**

```c++
int i = 5;
std::out << i << std::endl;
int j = i++;
std::out << j << std::endl;

// Output:
// 5
// 6
```

----

## **Assuming buf is a valid pointer, what is the problem in the code below? What would be an alternate way of implementing this that would avoid the problem?**

```c++
size_t sz = buf->size();
while ( --sz >= 0 )
{
	/* do something */
}
```

Solution:

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>
#include <stdio.h>

using namespace std;

int main()
{	
	size_t sz = buf->size();
	while (sz > 0)
    // or
	// for (size_t i = buf->size(); i > 0; --i)
	{
		/* do something */
	}
}
```

----

## **Consider the two code snippets below for printing a vector. Is there any advantage of one vs. the other? Explain?**

```c++
// Option 1:
vector vec;
/* ... .. ... */
for (auto itr = vec.begin(); itr != vec.end(); itr++)
{
	itr->print();
}
```

```c++
// Option 2:
vector vec;
/* ... .. ... */
for (auto itr = vec.begin(); itr != vec.end(); ++itr)
{
	itr->print();
}
```

----

## **Implement a template function IsDerivedFrom() that takes class C and class P as template parameters. It should return true when class C is derived from class P and false otherwise.**

```c++
#include <iostream>

// Base class
class P
{
};

// Derived class
class C : public P
{
};

// Template function to check if C is derived from P
template<typename C, typename P>
bool IsDerivedFrom()
{
    return std::is_base_of<P, C>::value;
}

int main()
{
    std::cout << std::boolalpha;
    std::cout << "Is C derived from P? " << IsDerivedFrom<C, P>() << std::endl; // true
    std::cout << "Is P derived from C? " << IsDerivedFrom<P, C>() << std::endl; // false

    return 0;
}
```

In this example, we have two classes: P (base class) and C (derived class). The IsDerivedFrom() template function takes two template parameters, C and P. It uses the std::is_base_of type trait from the <type_traits> library to check if C is derived from P. The function returns true if C is derived from P, and false otherwise.

In the main() function, we demonstrate the usage of IsDerivedFrom() by checking if C is derived from P and if P is derived from C. The results are printed to the console using std::cout. In this case, IsDerivedFrom<C, P>() returns true because C is derived from P, while IsDerivedFrom<P, C>() returns false because P is not derived from C.

----

## **Implement a template boolean IsSameClass() that takes class A and B as template parameters. It should compare class A and B and return false when they are different classes and true if they are the same class.**

```c++
#include <iostream>

// Template function to check if A and B are the same class
template<typename A, typename B>
bool IsSameClass()
{
    return std::is_same<A, B>::value;
}

int main()
{
    std::cout << std::boolalpha;
    std::cout << "Is A the same class as B? " << IsSameClass<A, B>() << std::endl;  // false
    std::cout << "Is A the same class as A? " << IsSameClass<A, A>() << std::endl;  // true

    return 0;
}
```

In this example, we have two classes: A and B. The IsSameClass() template function takes two template parameters, A and B. It uses the std::is_same type trait from the <type_traits> library to compare the types of A and B. The function returns true if A and B are the same class, and false otherwise.

In the main() function, we demonstrate the usage of IsSameClass() by comparing A and B, as well as comparing A with itself. The results are printed to the console using std::cout. In this case, IsSameClass<A, B>() returns false because A and B are different classes, while IsSameClass<A, A>() returns true because A is the same class as itself.

----

## **Is it possible to have a recursive inline function?**

No, it is not possible to have a recursive inline function in C++.

Inline functions are expanded at the call site by the compiler, and they are intended for small, frequently used functions where the function call overhead can be eliminated. However, recursion requires the function to call itself, creating a loop of function calls. Inline functions do not support this kind of recursive behavior because the expansion of an inline function is done in a single step, and it does not allow for recursive calls.

If you need to implement recursion, you should use a regular (non-inline) function. The compiler will handle the recursive calls by pushing the necessary information onto the call stack.

----

## **What is the output of the following code:**

```c++
#include <iostream>

using namespace std;

class A
{
public:
    A()
    {
    }
    ~A()
    {
        throw 42;
    }
};

int main(int argc, const char* argv[])
{
    try
    {
        A a;
        throw 32;
    }
    catch (int a)
    {
        std::cout << a;
    }
}

// Output:
// Debug Error
```

----

## **You are given library class Something as follows:**

```c++
class Something
{
public:
    Something()
    {
        topSecretValue = 42;
    }

    bool somePublicBool;
    int somePublicInt;
    std::string somePublicString;

private:
    int topSecretValue;
};
```

----

## **Implement a method to get topSecretValue for any given Something* object. The method should be cross-platform compatible and not depend on sizeof (int, bool, string).**

```c++
#include <iostream>
#include <string>

// Base class
class Something
{
public:
    virtual ~Something() {}  // Virtual destructor for proper cleanup

    virtual std::string getTopSecretValue() const = 0;
};

// Derived class
class ConcreteSomething : public Something
{
private:
    std::string topSecretValue;

public:
    explicit ConcreteSomething(const std::string& value) : topSecretValue(value)
    {
    }

    std::string getTopSecretValue() const override
    {
        return topSecretValue;
    }
};

// Function to get the topSecretValue for any Something* object
std::string getTopSecretValue(const Something* something)
{
    return something->getTopSecretValue();
}

int main()
{
    Something* something = new ConcreteSomething("This is a top secret value");
    std::cout << "Top Secret Value: " << getTopSecretValue(something) << std::endl;
    delete something;  // Cleanup

    return 0;
}
```

----

## **Implement a void function F that takes pointers to two arrays of integers (A and B) and a size N as parameters. It then populates B where B[i] is the product of all A[j] where j != i.**

For example: If A = {2, 1, 5, 9}, then B would be {45, 90, 18, 10}.

```c++
#include <iostream>

void F(const int* A, int* B, int N)
{
    // Calculate the product of all elements in A
    int product = 1;
    for (int i = 0; i < N; i++)
    {
        product *= A[i];
    }

    // Populate B such that B[i] is the product of all A[j] where j != i
    for (int i = 0; i < N; i++)
    {
        B[i] = product / A[i];
    }
}

int main()
{
    const int N = 5;
    int A[N] = {2, 3, 4, 5, 6};
    int B[N] = {0};
    F(A, B, N);

    // Print the resulting array B
    for (int i = 0; i < N; i++)
    {
        std::cout << B[i] << " ";
    }

    std::cout << std::endl;

    return 0;
}
```

----

## **When you should use virtual inheritance?**

Virtual inheritance is a feature in C++ that allows multiple base classes to share a common base class, but with only a single copy of the common base class being inherited by the derived class. It is typically used in situations where the same base class is inherited by multiple paths in an inheritance hierarchy, which can cause problems with ambiguous base classes.

Here are some scenarios where virtual inheritance can be useful:

Diamond inheritance: This is a situation where a class inherits from two base classes that both inherit from a common base class. Without virtual inheritance, the derived class will have two copies of the common base class, which can lead to ambiguity when accessing members of the common base class. Virtual inheritance ensures that there is only one copy of the common base class, avoiding the ambiguity.

Base classes with overlapping member functions: If two or more base classes have member functions with the same name and signature, it can cause ambiguity when the derived class tries to call the function. Virtual inheritance ensures that there is only one copy of the function in the derived class, avoiding the ambiguity.

Separation of interface and implementation: Virtual inheritance can be used to separate the interface and implementation of a base class. The interface can be defined in a non-virtual base class, while the implementation can be defined in a virtual base class. This can make it easier to reuse the interface in different implementations without duplicating the interface code.

Shared resources: Virtual inheritance can be useful in situations where multiple base classes need to share a common resource, such as a mutex or a file handle. By using virtual inheritance to share a common base class, the derived class can ensure that there is only one copy of the shared resource, avoiding conflicts and reducing memory usage.

In general, virtual inheritance should be used sparingly, as it can add complexity to the inheritance hierarchy and make the code harder to understand and maintain. It should only be used when it is necessary to avoid problems with ambiguity or to share a common resource.

----

## **What is the output of the following code?**

```c++
// TestApplication.cpp.
//

#include <iostream>
#include <string>
#include <stdio.h>
#include <math.h>
#include <stdbool.h>
#include <cstdlib>
#include <cstring>

using namespace std;

int main(int argc, const char* argv[])
{
    int a[] = { 1, 2, 3, 4, 5, 6 };
    std::cout << (1 + 3)[a] - a[0] + (a + 1)[2];
}

// Output:
// 8
```

----

## **What is the output of the following code?**

```c++
#include <iostream>

class Base
{
    virtual void method()
    {
        std::cout << "from Base" << std::endl;
    }

public:
    virtual ~Base()
    {
        method();
    }

    void baseMethod()
    {
        method();
    }
};

class A : public Base
{
    void method()
    {
        std::cout << "from A" << std::endl;
    }

public:
    ~A()
    {
        method();
    }
};

int main(void)
{
    Base* base = new A;
    base->baseMethod();
    delete base;
    return 0;
}
```

----

## **How many times will this loop execute? Explain your answer?**

```c++
unsigned char half_limit = 150;

for (unsigned char i = 0; i < 2 * half_limit; ++i)
{
    // do something;
}

// Output:
// The loop iterates over the values of i starting from 0 and continuing as long as i is less than 2 * half_limit. Here, half_limit is assigned a value of 150.

// The condition i < 2 * half_limit sets the termination condition for the loop. Since half_limit is 150, the termination condition becomes i < 300, as 2 * half_limit equals 300.

// As a result, the loop will iterate as long as i is less than 300. The loop will start at i = 0 and increment i by 1 with each iteration until i reaches the value of 299. At that point, i will no longer be less than 300, and the loop will terminate.

// Therefore, the loop will execute 300 times: from i = 0 to i = 299.
```

----

## **How can you make sure a C++ function can be called as e.g. void foo(int, int) but not as any other type like void foo(long, long)?**

One way to make sure that a C++ function can only be called with a specific set of argument types is to use template specialization. Here's an example:

```c++
// Generic function template
template<typename T1, typename T2>
void foo(T1, T2)
{
    static_assert(sizeof(T1) == sizeof(int) && sizeof(T2) == sizeof(int), "foo() must be called with two int arguments");
    // Do something with the arguments
}

// Specialization for int arguments
template<>
void foo(int, int)
{
    // Do something specific to int arguments
}
```

In this example, we define a generic function template foo() that takes two template parameters of arbitrary types. The static_assert statement ensures that the size of the template arguments is equal to the size of an int, which restricts the function to only accept arguments of type int. We then define a specialization of the foo() template for arguments of type int, which can provide specific behavior for this case.

When foo() is called with two arguments of type int, the specialization will be used, and any other types will result in a compile-time error due to the static_assert statement. This ensures that foo() can only be called with the specified argument types.

Note that this approach relies on the size of the argument types being a specific value, which may not always be the case. In general, it is better to use more robust type-checking techniques, such as std::enable_if or concept constraints, to ensure that a function can only be called with specific argument types.

----

## **What is the problem with the following code?**

```c++
using namespace std;

class A
{
public:
	A()
    {
    }
	
    ~A()
    {
    }
};

class B : public A
{
public:
	B() :A()
    {
    }
	
    ~B()
    {
    }
};

int main(void)
{
	A* a = new B();
	delete a;
}
```

----

## **What is a storage class?**

In C++, a storage class defines the scope, lifetime, and visibility of variables or functions within a program. It specifies how the memory is allocated and managed for these entities. C++ provides several storage classes that determine the characteristics of variables or functions.

Here are the different storage classes in C++:

__auto:__ This is the default storage class for local variables. It is automatically assigned to variables declared within a block or function. The auto keyword is rarely used explicitly since it is the default behavior.

__register:__ This storage class is used to declare local variables that should be stored in a register instead of memory. It suggests the compiler to optimize access to these variables by keeping them in registers, but the decision ultimately lies with the compiler.

__static:__ The static storage class has different meanings depending on where it is used:

__For local variables:__ It preserves the value of a variable between function calls. The variable is initialized only once and retains its value throughout the program's execution.

__For global variables:__ It limits the scope of the variable to the file where it is declared. The variable is accessible only within that file, even if it is declared as extern in other files.

__For functions:__ It limits the visibility of the function to the file where it is declared. The function cannot be accessed from other files using the extern keyword.

__extern:__ The extern storage class is used to declare variables or functions that are defined in other files. It is typically used to provide access to variables or functions that are defined in one file and used in other files of a program.

__mutable:__ This storage class is applicable only to class member variables. It allows modifying a member variable even within a const member function.

__thread_local:__ Introduced in C++11, this storage class is used to declare variables that have a different instance for each thread. Each thread has its own copy of the variable, and the variable retains its value across function calls within the same thread.

Understanding storage classes helps you control the behavior, scope, and lifetime of variables and functions in your C++ programs, allowing for efficient memory management and controlling variable visibility across different parts of your code.

```c++
#include <iostream>

// Global variables
int globalVar = 5;
static int staticGlobalVar = 10;

// Function with static local variable
void countCalls()
{
    static int counter = 0;  // static local variable
    counter++;
    std::cout << "Function calls: " << counter << std::endl;
}

int main()
{
    // Automatic storage class (default)
    int localVar = 15;

    // Register storage class
    register int registerVar = 20;

    // Extern storage class
    extern int externalVar;

    std::cout << "Global variable: " << globalVar << std::endl;
    std::cout << "Static global variable: " << staticGlobalVar << std::endl;
    std::cout << "Local variable: " << localVar << std::endl;
    std::cout << "Register variable: " << registerVar << std::endl;
    std::cout << "External variable: " << externalVar << std::endl;

    countCalls();
    countCalls();
    countCalls();

    return 0;
}

// Definition of the external variable
int externalVar = 25;

// Output:
// Global variable: 5
// Static global variable: 10
// Local variable: 15
// Register variable: 20
// External variable: 25
// Function calls: 1
// Function calls: 2
// Function calls: 3
```

In this example, we have used various storage classes:

*Global variables (globalVar and staticGlobalVar):*
globalVar is a regular global variable accessible throughout the program. staticGlobalVar is a global variable with the static storage class. It limits the variable's visibility to the current file.

*Local variable (localVar):*
localVar is an automatic variable declared within the main() function. It is allocated and deallocated automatically when the function is called.

*Register variable (registerVar):*
RegisterVar is declared with the register storage class, suggesting the compiler to store it in a register for faster access.

*External variable (externalVar):*
externalVar is declared as an extern variable, meaning it is defined in another file. Here, we define it at the end of the program.

*Static local variable (counter):*
The countCalls() function contains a static local variable counter. It retains its value across multiple function calls and is initialized only once.

----

## **How can a C function be called in a C++ program?**

In C++, you can call a C function in a C++ program by using the extern "C" declaration to specify the C linkage for the function. The extern "C" declaration informs the C++ compiler to treat the enclosed code as C code, allowing you to call C functions from within a C++ program. Here's an example:

```c
// mylibrary.h
#ifndef MY_LIBRARY_H
#define MY_LIBRARY_H

int add(int a, int b);

#endif  // MY_LIBRARY_H

// mylibrary.c
#include "mylibrary.h"

int add(int a, int b)
{
    return a + b;
}
```

```c++
#include <iostream>

extern "C"
{
#include "mylibrary.h"
}

int main()
{
    int result = add(5, 3);
    std::cout << "Result: " << result << std::endl;

    return 0;
}
```

In this example, we have a simple C library consisting of mylibrary.h and mylibrary.c. The mylibrary.h file declares the add() function, and mylibrary.c defines the implementation of the add() function.

To call the add() function in a C++ program, we include mylibrary.h and use the extern "C" declaration before including the C header file. This tells the C++ compiler to use C linkage for the enclosed code.

In the main() function of the C++ code, we call the add() function as if it were a regular C++ function. The C++ compiler will recognize the extern "C" declaration and treat the function as a C function.

When you run this program, it will output:
makefile
Copy code
Result: 8
This demonstrates how you can call a C function from a C++ program by using the extern "C" declaration to specify the C linkage.

----

## **What will be the output of the following program?**

```c++
#include <iostream>

struct A
{
    int data[2];
    A(int x, int y) : data{x, y}
    {
    }

    virtual void f()
    {
    }
};

int main(int argc, char **argv)
{
    A a(22, 33);
    int *arr = (int *) &a;
    std::cout << arr[2] << std::endl;

    return 0;
}

// Output:
// 22
```

----

## **Are you allowed to have a static const member function? Explain your answer?**

No, it is not possible to have a static const member function in C++. The const qualifier is not applicable to member functions marked as static because static member functions are not associated with any particular object instance. The const qualifier is used to indicate that a member function does not modify the state of the object on which it is invoked. However, since static member functions are not tied to any specific object, the concept of constness does not apply to them.

In C++, the const qualifier can be applied to non-static member functions to indicate that these functions do not modify the state of the object on which they are invoked. This allows the compiler to perform additional optimizations and enforce immutability guarantees.

If you need a function to be both static and const in behavior, you can achieve similar functionality by declaring a regular non-member function as const. Non-member functions can be declared as const to indicate that they do not modify any global or static variables and have no side effects. By declaring a non-member function as static, it can be restricted to the file scope if desired.

----

## **Explain the volatile and mutable keywords.**

In C++, the volatile and mutable keywords are used to modify the behavior of variables. Here's an explanation of each keyword:

Volatile:

The volatile keyword is used to indicate that a variable may be modified by external entities that are not under the control of the program. It informs the compiler that the variable's value may change unexpectedly, and therefore, the compiler should not optimize or make assumptions about the variable.

When a variable is declared as volatile, the compiler generates code that always reads the variable from memory, even if it appears to be redundant. Similarly, any write to a volatile variable is guaranteed to be performed and not optimized away.

Common use cases for volatile variables include:
- Variables shared between multiple threads or interrupt service routines.
- Variables that are memory-mapped to hardware registers, where the register's value can change due to external factors.

Example:

```c++
volatile int externalVar;

int main()
{
    while (externalVar == 0)
    {
        // Code to handle the case when the variable changes unexpectedly
    }

    return 0;
}
```

In this example, externalVar is declared as volatile to indicate that its value can change externally. The while loop continuously checks the value of externalVar, even if it appears to be redundant, to ensure the program can handle unexpected changes.

mutable:
The mutable keyword is used in the context of class member variables to allow modification of the variable even within a const member function. By default, const member functions are not allowed to modify any member variables because they are intended to be read-only operations. However, when a member variable is marked as mutable, it can be modified within a const member function without violating the constness of the function.
Example:

```c++
class MyClass
{
public:
    mutable int mutableVar;

    void printValue() const
    {
        mutableVar = 10;  // Modifying a mutable member variable in a const member function
        std::cout << "Value: " << mutableVar << std::endl;
    }
};

int main()
{
    MyClass obj;
    obj.printValue();

    return 0;
}
```

In this example, mutableVar is declared as mutable within the MyClass class. The printValue() function is marked as const, but it can still modify the mutableVar member variable without violating the constness of the function.

The volatile and mutable keywords serve different purposes in C++:

volatile is used to indicate that a variable may change unexpectedly due to external factors.
mutable is used to allow modification of a member variable within a const member function.

----

## **C++ supports multiple inheritance. What is the "diamond problem" that can occur with multiple inheritance? Give an example.**

The "diamond problem" is a specific issue that can occur in languages that support multiple inheritance, including C++. It arises when a class inherits from two or more base classes that have a common base class themselves. This situation creates ambiguity and confusion for the derived class, leading to the diamond problem.

Let's consider an example to understand the diamond problem:

```c++
#include <iostream>

class Base
{
public:
    void display()
    {
        std::cout << "Base class" << std::endl;
    }
};

class DerivedA : public Base
{
public:
    void display() {
        std::cout << "DerivedA class" << std::endl;
    }
};

class DerivedB : public Base
{
public:
    void display()
    {
        std::cout << "DerivedB class" << std::endl;
    }
};

class DerivedAB : public DerivedA, public DerivedB
{
public:
    void display()
    {
        std::cout << "DerivedAB class" << std::endl;
    }
};

int main()
{
    DerivedAB obj;
    obj.display();

    return 0;
}
```

In this example, we have a base class Base and two derived classes DerivedA and DerivedB, both inheriting from Base. Then, we have a class DerivedAB that inherits from both DerivedA and DerivedB.

The diamond problem occurs when DerivedAB attempts to access a member or function that is inherited from Base through multiple paths. In this case, the display() function is the common member function inherited from Base.

When we create an object of DerivedAB and call the display() function, it leads to ambiguity. The compiler does not know which version of display() to invoke: the one inherited from DerivedA or the one inherited from DerivedB, as both paths lead to the Base class.

To resolve this ambiguity, we can use scope resolution to specify which version of display() to call:

```c++
class DerivedAB : public DerivedA, public DerivedB
{
public:
    void display()
    {
        DerivedA::display();
    }
};
```

By using DerivedA::display(), we explicitly specify that we want to call the display() function inherited from DerivedA.

The diamond problem in multiple inheritance occurs due to the potential ambiguity when two or more base classes share a common base class. It is important to carefully consider the design and potential conflicts when using multiple inheritance to avoid such issues.

# https://www.toptal.com/c-plus-plus/interview-questions

# https://hackr.io/blog/cpp-interview-questions

## **What is C++?**

C++ is a computer programming language that is a superset of C, with additional features. 

----

## **Does C++ make use of OOPS?**

Yes, it does. An Object-Oriented Programming System is a paradigm that includes concepts such as data binding, polymorphism, and inheritance, among others.

----

## **What is a Class?**

A class is a user-defined data type that is at the center of OOP. It reflects different entities, attributes, and actions.

```c++
class LivingBeing
{
public:
    void eating()
    {
        cout << "living being is eating" << endl;
    }
    
    void running()
    {
        cout << "living being is running" << endl;
    }
private:
};

// derived class
class Human : public LivingBeing // public, because it is about an public inheritance.
{
public:
    Human(string name)
    {
        name = n;
    }
    void speaking()
    {
        cout << "Human says hallo" << endl;
    }
private:
    string n;
};

// derived class
class Dog : public LivingBeing
{
public:
    Dog(string name)
    {
        name = n;
    }
    void barking()
    {
        cout << "woof woof" << endl;
    }
private:
    string n;
};
```

----

## **What is an object?**

An object is an instance of the class. An object can have fields, methods, and constructors.

```c++
#include <iostream>

// Class definition
class Circle
{
private:
    double radius;

public:
    // Constructor
    Circle(double r)
    {
        radius = r;
    }

    // Member function
    double calculateArea()
    {
        return 3.14159 * radius * radius;
    }
};

int main()
{
    // Create objects of class Circle
    Circle circle1(2.5);
    Circle circle2(3.8);

    // Access object's member function
    double area1 = circle1.calculateArea();
    double area2 = circle2.calculateArea();

    // Output the results
    std::cout << "Area of circle1: " << area1 << std::endl;
    std::cout << "Area of circle2: " << area2 << std::endl;

    return 0;
}

// Output:
// Area of circle1: 19.6349
// Area of circle2: 45.3899
```

----

## **What is encapsulation?**

Encapsulation is the process of binding together the data and functions in a class. It is applied to prevent direct access to the data for security reasons. The functions of a class are applied for this purpose.

```c++
#include <iostream>

class Circle
{
private:
    double radius;

public:
    void setRadius(double r)
    {
        radius = r;
    }

    double getArea() const
    {
        return 3.14159 * radius * radius;
    }
};

int main()
{
    Circle circle;
    circle.setRadius(2.5);
    double area = circle.getArea();
    std::cout << "Area of circle: " << area << std::endl;

    return 0;
}
```

----

## **What is abstraction?**

An abstraction in C++ is hiding the internal implementations and displaying only the required details.

For example, when you send an important message through email, at that time, only writing and clicking the send option is used. This outcome is just the success message that is displayed to confirm that your email has been sent. However, the process followed in transferring the data through email is not displayed because it is of no use to you.

```c++
#include <iostream>

// Abstract class
class Shape
{
public:
    // Pure virtual function
    virtual double calculateArea() const = 0;
};

// Concrete class implementing Shape
class Rectangle : public Shape
{
private:
    double length;
    double width;

public:
    Rectangle(double l, double w) : length(l), width(w)
    {
    }

    double calculateArea() const override
    {
        return length * width;
    }
};

int main()
{
    // Create objects of the concrete class
    Rectangle rectangle(5.0, 3.0);

    // Use the abstract interface
    double area = rectangle.calculateArea();
    std::cout << "Area of rectangle: " << area << std::endl;

    return 0;
}
```

----

## **What is inheritance?**

C++ allows classes to inherit some of the commonly used state and behavior from other classes. This process is known as inheritance.

```c++
#include <iostream>

// Base class
class Animal
{
public:
    void eat()
    {
        std::cout << "Animal is eating." << std::endl;
    }
};

// Derived class
class Dog : public Animal
{
public:
    void bark()
    {
        std::cout << "Dog is barking." << std::endl;
    }
};

int main()
{
    // Create an object of the derived class
    Dog dog;

    // Call member functions from the base and derived classes
    dog.eat();
    dog.bark();

    return 0;
}
```

## **What is a namespace?**

A namespace is used for resolving the name conflict of the identifier, which is accomplished by placing them under various namespaces.

```c++
#include <iostream>

// First namespace
namespace FirstNamespace
{
    void greet()
    {
        std::cout << "Hello from FirstNamespace!" << std::endl;
    }
}

// Second namespace
namespace SecondNamespace
{
    void greet()
    {
        std::cout << "Hello from SecondNamespace!" << std::endl;
    }
}

int main()
{
    FirstNamespace::greet();   // Call greet() from FirstNamespace
    SecondNamespace::greet();  // Call greet() from SecondNamespace

    return 0;
}
```

----

## **What is a class template?**

A class template is a name given to the generic class. The use of the keyword template is made for defining a class template.

In C++, a class template is a mechanism that allows you to define a generic class that can work with different data types. It enables you to create a blueprint for a class that can be customized to work with various types, providing flexibility and code reuse.

A class template is defined using the template keyword followed by a template parameter list, which specifies one or more template parameters. These parameters can be used as placeholders for the types or values that will be supplied when using the template.

Here's an example of a class template that represents a generic stack:

```c++
template <typename T>
class Stack
{
private:
    static const int MAX_SIZE = 100;
    T elements[MAX_SIZE];
    int top;

public:
    Stack() : top(-1)
    {
    }

    void push(const T& item)
    {
        if (top >= MAX_SIZE - 1)
        {
            std::cout << "Stack overflow!" << std::endl;
        }
        else
        {
            elements[++top] = item;
        }
    }

    T pop()
    {
        if (top < 0)
        {
            std::cout << "Stack is empty!" << std::endl;
            return T(); // Return a default-constructed value
        }
        else
        {
            return elements[top--];
        }
    }
};
```

In this example, the Stack class template is defined with a single template parameter T. The template parameter T represents the type of the elements that the stack will store. It can be any valid C++ type.

Inside the Stack class template, you can see how the template parameter T is used to define the data members and member functions of the class. For example, the elements array is of type T, allowing it to hold elements of the specified type.

You can then use the class template to create stack objects for different data types. Here's an example of using the Stack class template with integers and strings:

```c++
int main()
{
    Stack<int> intStack;
    intStack.push(10);
    intStack.push(20);
    intStack.push(30);

    Stack<std::string> stringStack;
    stringStack.push("Hello");
    stringStack.push("World");

    int poppedInt = intStack.pop();
    std::string poppedString = stringStack.pop();

    std::cout << "Popped int: " << poppedInt << std::endl;
    std::cout << "Popped string: " << poppedString << std::endl;

    return 0;
}
```

We then use the member functions of each stack object to push elements onto the stack and pop elements from the stack. The template parameter T is automatically deduced based on the data type used during object creation.

Class templates provide a powerful mechanism for creating reusable code that can work with different data types. They allow you to avoid duplicating code for similar classes and provide a way to create generic algorithms and data structures in C++.

----

## **What is the function of the keyword "Volatile"?**

"Volatile" is a function that helps in declaring that the particular variable is volatile and thereby directs the compiler to change the variable externally- this way, the compiler optimization on the variable reference can be avoided.

```c++
volatile int sensorValue;

void readSensor()
{
    while (true)
    {
        // Read sensor value from hardware
        int value = /* read value from hardware */;

        // Update the volatile variable
        sensorValue = value;
    }
}

void processSensor()
{
    while (true)
    {
        // Read the volatile variable
        int value = sensorValue;

        // Process the sensor value
        // ...
    }
}
```

----

## **What is a storage class?**

A storage class in C++ specifically resembles the scope of symbols, including the variables, functions, etc. Some of the storage class names in C++ include mutable, auto, static, extern, register, etc.

In C++, a storage class specifies the scope, lifetime, and visibility of variables or functions within a program. It determines how memory is allocated, initialized, and deallocated for variables and how functions are stored and accessed during program execution. C++ provides several storage classes that control these aspects.

Here are the main storage classes in C++:

__auto:__ This is the default storage class for local variables. It automatically allocates and deallocates memory for variables within a block or function. The auto keyword is rarely used explicitly, as it is the default behavior.

__register:__ This storage class suggests the compiler to store the variable in a CPU register for faster access. However, the decision to use a register is ultimately made by the compiler. The register keyword is rarely used explicitly, as modern compilers are efficient in optimizing register allocation.

__static:__ The static storage class is used to declare variables that are allocated memory once and persist throughout the program's execution. They retain their values between function calls. Static variables are initialized only once, and their memory is not deallocated when they go out of scope. Static variables have file scope if defined outside any function or block, and they have block scope if defined inside a function or block.

__extern:__ The extern storage class is used to declare variables or functions that are defined in another translation unit (source file). It is used to provide a declaration without allocating memory. When using extern, the actual definition of the variable or function is assumed to be elsewhere.

__mutable:__ This storage class is applicable only to non-static class members. It allows modifying a member variable of a const object. The mutable keyword is used to specify that a member variable can be changed even within a const member function.

NOTE: C++11 introduced the thread_local storage class, which allows the creation of thread-local variables.

Here's an example that demonstrates the usage of different storage classes in C++:

```c++
#include <iostream>

int globalVariable;  // Static storage duration, external linkage

void function()
{
    static int staticVariable;  // Static storage duration, internal linkage
    int localVariable;           // Automatic storage duration

    // Access and modify variables
    globalVariable++;
    staticVariable++;
    localVariable++;

    std::cout << "Global Variable: " << globalVariable << std::endl;
    std::cout << "Static Variable: " << staticVariable << std::endl;
    std::cout << "Local Variable: " << localVariable << std::endl;
}

int main()
{
    globalVariable = 10;

    for (int i = 0; i < 3; i++)
    {
        function();
    }

    return 0;
}
```

In this example, we have a global variable (globalVariable) with static storage duration and external linkage. Inside the function(), we have a static local variable (staticVariable) with static storage duration and internal linkage, and a local variable (localVariable) with automatic storage duration.

The globalVariable and staticVariable retain their values between function calls because of their static storage duration. The localVariable is allocated and deallocated on each invocation of the function due to its automatic storage duration.

When running this program, the output will be:

```c++
// Global Variable: 11
// Static Variable: 1
// Local Variable: 1
// Global Variable: 12
// Static Variable: 2
// Local Variable: 1
// Global Variable: 13
// Static Variable: 3
// Local Variable: 1
```

----

## **What is an Inline Function? Is it possible to ignore inlining?**

In order to reduce the function call overhead, C++ offers inline functions. As the name suggests, an inline function is expanded in line when it is called.

As soon as the inline function is called, the whole code of the same gets either inserted or substituted at the particular point of the inline function call. The substitution is completed by the C++ compiler at compile time. Small inline functions might increase program efficiency.

The syntax of a typical inline function is:

```c++
Inline return-type function-name(parameters)
{
    // Function code goes here
}
```

As the inlining is a request, not a command, the compiler can ignore it.

----

## **Can we have a recursive inline function in C++?**

Even though it is possible to call an inline function from within itself in C++, the compiler may not generate the inline code. This is so because the compiler won’t determine the depth of the recursion at the compile time.

Nonetheless, a compiler with a good optimizer is able to inline recursive calls until some depth is fixed at compile time and insert non-recursive calls at compile time for the cases when the actual depth exceeds run time.

----

## **What is the ‘this’ pointer?**

The 'this' pointer is a constant pointer, and it holds the memory address of the current object. It passes as a hidden argument to all the nonstatic member function calls. It is available as a local variable within the body of all the nonstatic functions.

As static member functions can be called even without any object, i.e., with the class name, the 'this' pointer is not available for them.

----

## **What are the most important differences between C and C++?**

C++ supports references while C doesn’t. Features like friend functions, function overloading, inheritance, templates, and virtual functions are inherent to C++. These are not available in the C programming language.

In C, exception handling is taken care of in the traditional if-else style. On the other hand, C++ offers support for exception handling at the language level.

Mainly used input and output in C are scanf() and printf(), respectively. In C++, cin is the standard input stream while cout serves as the standard output stream.

While C is a procedural programming language, C++ provides support for both procedural and object-oriented programming approaches.

----

## **Why do we need the Friend class and function?**

Sometimes, there is a need for allowing a particular class to access private or protected members of a class. The solution is a friend class, which can access the protected and private members of the class in which it is declared as a friend.

Similar to the friend class, a friend function is able to access private and protected class members. A friend function can either be a global function or a method of some class.

Some important points about friend class and friend function:

Friendship is not inherited.
Friendship isn’t mutual, i.e., if some class called riend is a friend of some other class called NotAFriend, then it doesn’t automatically become a friend of the Friend class.
The total number of friend classes and friend functions should be limited in a program as the overabundance of the same might lead to a depreciation of the concept of encapsulation of separate classes, which is an inherent and desirable quality of object-oriented programming.

----

## **What is Operator Overloading?**

Operating overloading is when operators have different implementations depending on the arguments passed. It is a type of polymorphism.

----

## **What is Polymorphism?**

Polymorphism is the ability of a variable, function, or object to take on multiple forms.

```c++
#include <iostream>

class Shape
{
public:
    virtual void draw()
    {
        std::cout << "Drawing a shape." << std::endl;
    }
};

class Circle : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a circle." << std::endl;
    }
};

class Rectangle : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a rectangle." << std::endl;
    }
};

int main()
{
    Shape* shape1 = new Circle();
    Shape* shape2 = new Rectangle();

    shape1->draw();  // Calls Circle::draw()
    shape2->draw();  // Calls Rectangle::draw()

    delete shape1;
    delete shape2;

    return 0;
}
```

----

## **Explain vTable and vptr?**

vTable is a table containing function pointers. Every class has a vTable. vptr is a pointer to vTable. Each object has a vptr. In order to maintain and use vptr and vTable, the C++ compiler adds additional code at two places:

In every constructor – This code sets vptr:
Of the object being created
To point to vTable of the class
Code with the polymorphic functional call – At every location where a polymorphic call is made, the compiler inserts code in order to first look for vptr using the base class pointer or reference. The vTable of a derived class can be accessed once the vptr is successfully fetched. The address of the derived class function show() is accessed and called using the vTable.

```c++
#include <iostream>

class Shape
{
public:
    virtual void draw()
    {
        std::cout << "Drawing a shape." << std::endl;
    }
};

class Circle : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a circle." << std::endl;
    }
};

int main() {
    Shape* shape = new Circle();
    shape->draw();  // Calls Circle::draw()

    delete shape;

    return 0;
}
```

In this example, we have a base class Shape with a virtual function draw(). The Circle class is derived from Shape and overrides the draw() function.

When the main() function is executed, a Circle object is created and assigned to a Shape pointer. The shape->draw() call invokes the draw() function based on the actual object type at runtime. This is possible because the Shape object contains a vptr that points to the vtable, and the vtable contains the correct function address for the Circle class.

The vptr and vtable mechanism ensures that the correct function is called based on the actual object type, even when accessing the object through a base class pointer or reference.

It's important to note that the usage of vtable and vptr is implementation-dependent and may vary across different compilers and platforms. However, the concept of vtable and vptr is fundamental to achieving dynamic polymorphism in C++ through virtual functions.

----

## **How is function overloading different from operator overloading?**

Function overloading and operator overloading are two distinct features in C++ that allow multiple definitions of functions or operators with different parameters or behaviors. Here are the differences between the two:

*Purpose:*

Function Overloading: Function overloading enables you to define multiple functions with the same name but different parameter lists. It allows you to provide different implementations of a function for different argument types or numbers.
Operator Overloading: Operator overloading allows you to redefine the behavior of an operator when it is used with user-defined types. It allows you to define how operators, such as +, -, *, /, =, etc., work with your custom types.

*Syntax:*

Function Overloading: Function overloading is achieved by declaring multiple functions with the same name but different parameters. The functions can have different return types, but the parameter lists must differ in terms of the number, type, or order of parameters.
Operator Overloading: Operator overloading is done by defining functions with special names that correspond to specific operators. For example, to overload the + operator, you define a function named operator+ in the class.

*Invocation:*

Function Overloading: Functions are invoked by their name, and the compiler selects the appropriate function based on the argument types used during the function call. The selection is made at compile time.
Operator Overloading: Operators are invoked using the operator symbol and the objects on which they operate. For example, if you overload the + operator for a custom class, you can use the + operator directly between two objects of that class.

*Return Type:*

Function Overloading: Functions with the same name can have different return types. The return type is not considered during function overloading resolution.
Operator Overloading: The return type of an overloaded operator is determined by the operator itself. For example, the + operator typically returns the sum of two objects of the class.

*Limitations:*

Function Overloading: Function overloading is limited to functions with different parameter lists. You cannot overload functions based solely on their return type or the presence of const qualifiers.
Operator Overloading: Operator overloading has certain constraints and limitations on which operators can be overloaded and how they can be overloaded. For example, you cannot create new operators or change the precedence of operators.

Here's an example to illustrate the differences between function overloading and operator overloading:

```c++
#include <iostream>

class MyClass
{
public:
    void process(int value)
    {
        std::cout << "Processing integer: " << value << std::endl;
    }

    void process(double value)
    {
        std::cout << "Processing double: " << value << std::endl;
    }

    MyClass operator+(const MyClass& other)
    {
        MyClass result;
        // Perform addition logic
        return result;
    }
};

int main()
{
    MyClass obj;
    obj.process(10); // Invokes process(int)
    obj.process(3.14); // Invokes process(double)

    MyClass obj1, obj2, obj3;
    obj3 = obj1 + obj2; // Invokes operator+ overload

    return 0;
}
```

In this example, we have a class MyClass with two overloaded member functions: process(int) and process(double). These functions have different parameter lists, allowing them to be called based on the argument type.

Additionally, the operator+ is overloaded to perform custom addition logic for two objects of MyClass. It allows the use of the + operator between MyClass objects.

Function overloading and operator overloading provide flexibility and convenience in designing and using classes in C++. Function overloading allows you to

----

## **Is it possible for a C++ program to be compiled without the main() function?**

Yes, it is possible. However, as the main() function is essential for the execution of the program, the program will stop after compiling and will not execute.

No, it is not possible for a C++ program to be compiled without the main() function. According to the C++ language standard, every C++ program must contain a definition for the main() function, which serves as the entry point of the program.

----

## **What is a destructor?**

A destructor is the member function of the class. It has the same name as the class name and is also prefixed with a tilde symbol. It can be executed automatically whenever an object loses its scope. A destructor cannot be overloaded, and it has the only form without the parameters.

```c++
#include <iostream>

class MyClass
{
public:
    MyClass()
    {
        std::cout << "Constructor called." << std::endl;
    }

    ~MyClass()
    {
        std::cout << "Destructor called." << std::endl;
    }
};

int main()
{
    MyClass obj;  // Constructor called

    // Other code...

    return 0;  // Destructor called
}
```

In this example, we have a class MyClass with a constructor and a destructor. The constructor is called when an object of MyClass is created, and the destructor is automatically called when the object goes out of scope or is explicitly destroyed.

In the main() function, we create an object obj of type MyClass. When the main() function ends, the obj object goes out of scope, and the destructor of MyClass is automatically called to perform any necessary cleanup tasks. In this case, it will print "Destructor called" to the console.

Destructors are particularly useful for releasing dynamically allocated memory, closing file handles, releasing system resources, or performing any other necessary cleanup operations. They ensure that resources are properly released and prevent memory leaks or resource leaks.

It's important to note that if a class manages any dynamically allocated memory or resources, it is often a good practice to define a destructor to handle the cleanup of those resources. The compiler automatically generates a default destructor if one is not provided, but it may not be sufficient for cases where explicit resource management is needed.

Also, if a class inherits from other classes, the destructors of the base classes are called before the derived class destructor is executed, ensuring proper cleanup of the complete object hierarchy.

----

## **What is the default constructor?**

The compiler provides a constructor to every class in case the provider does not offer the same. This is when the programmer provides the constructor with no specific parameters - this is called a default constructor. The code for default constructor can be displayed in the following example.

```c++
// Cpp program to illustrate the
// concept of Constructors
#include <iostream>
using namespace std;
class construct
{
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
```

----

## **Can we provide one default constructor for our class?**

No, we cannot provide one default constructor for our class. When a variable in the class type is set to null, it means that it was never initialized and the outcomes will be zero.

----

## **What is the main difference between the keyword struct and class?**

The keyword struct is used for resembling public members by default, while the keyword class is used for resembling private members by default.

```c++
// struct example
#include <iostream>

struct Person
{
    std::string name;
    int age;
};

int main()
{
    Person person;

    person.name = "John Doe";
    person.age = 25;

    std::cout << "Name: " << person.name << std::endl;
    std::cout << "Age: " << person.age << std::endl;

    return 0;
}
```

```c++
// class example
#include <iostream>

class Rectangle
{
private:
    double length;
    double width;

public:
    // Constructor
    Rectangle(double len, double wid) : length(len), width(wid)
    {
    }

    // Member function to calculate area
    double calculateArea()
    {
        return length * width;
    }

    // Member function to print dimensions
    void printDimensions()
    {
        std::cout << "Length: " << length << ", Width: " << width << std::endl;
    }
};

int main()
{
    // Create an object of class Rectangle
    Rectangle rect(5.0, 3.0);

    // Access member functions
    rect.printDimensions();
    std::cout << "Area: " << rect.calculateArea() << std::endl;

    return 0;
}
```

----

## **What is the output of the following program?**

```c++
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

// The program will ask the user to enter 5 numbers and then present with their sum.For instance,
// Enter 5 numbers: 22
// 25
// 32
// 46
// 66
// Sum = 191
```

----

## **Explain Virtual Functions and Runtime Polymorphism in C++ with an example.**

Any function when accompanying the virtual keyword exhibits the behavior of a virtual function. Unlike normal functions that are called in accordance with the type of pointer or reference used, virtual functions are called as per the type of the object pointed or referred.

In simple terms, virtual functions resolve at runtime, not anytime sooner. Use of virtual functions could also be understood as writing a C++ program leveraging the concept of runtime polymorphism. Things essential to writing a virtual function in C++ are:
- A base class
- A derived class
- A function with the same name in both the classes i.e. the base class and the derived class
- A pointer or reference of base class type that points or refers, respectively to an object of the derived class
- An example demonstrating the use of virtual functions (or runtime polymorphism at play) is:

```c++
#include <iostream>

using namespace std;

class Base
{
public:
	virtual void show()
    {
        cout << " In Base \n";
    }
};

class Derived : public Base
{
public:
	void show()
    {
        cout << "In Derived \n";
    }
};

int main(void)
{
	Base* bp = new Derived;
	bp->show(); // <- Runtime Polymorphism in Action
	return 0;
}
```

In the aforementioned program bp is a pointer of type Base. A call to bp->show() calls show() function of the Derived class. This is because bp points to an object of the Derived class.

----

## **What differences separate structure from a class in C++?**

There are two important distinctions between a class and a structure in C++. These are:

When deriving a structure from a class or some other structure, the default access specifier for the base class or structure is public. On the contrary, the default access specifier is private when deriving a class.
While the members of a structure are public by default, the members of a class are private by default

----

## **What is a static member?**

Denoted by the static keyword, a static member is allocated storage, in the static storage area, only once during the program lifetime. Some important facts pertaining to the static members are:

Any static member function can’t be virtual
Static member functions don’t have ‘this’ pointer
The const, const volatile, and volatile declaration aren’t available for static member functions

----

## **What is the Reference variable?**

The reference variable in C++ is the name given to the existing variables. The variable name and reference variable point share the same memory location in C++, which helps in updating the original variable using the reference variable. The code can be displayed in the following example.

```c++
#include <iostream>

using namespace std;

int main()
{
	int x = 10;
	// ref is a reference to x.
	int& ref = x;
	// Value of x is now changed to 20
	ref = 20;
	cout << "x = " << x << endl;
	// Value of x is now changed to 30
	x = 30;
	cout << "ref = " << ref << endl;
	return 0;
}
```

----

## **Explain the Copy Constructor?**

A member function that initializes an object using another object of the same class is known as a copy constructor in C++. They can also be made private. A call to the copy constructor can happen in any of the following 4 scenarios when:

The compiler generates a temporary object
An object is constructed or based on some another object of the same class
An object of the class is returned by value
An object of the class is passed (i.e., to a function) by value as an argument
The general function prototype for the Copy Constructor is:

```c++
ClassName (const ClassName &old_obj);

Point(int x1, int y1)
{
    x=x1;
    y=y1;
}

Point(const Point &p2)
{
    x=p2.x;
    y=p2.y;
}
```

----

## **Take a look at the following two code examples for printing a vector. Is there any advantage of using one over the other?**

```c++
vector vec;
/* ... .. ... */
for (auto itr = vec.begin(); itr != vec.end(); itr++)
{
    itr->print();
}
```

```c++
// Sample Code 2:
vector vec;
/* ... .. ... */
for (auto itr = vec.begin(); itr != vec.end(); ++itr)
{
    itr->print();
}
```

Though both codes will generate the same output, sample code 2 is a more performant option. This is due to the fact that the post-increment ‘itr++’ operator is more expensive than the pre-increment ‘++itr’ operator.

The post-increment operator generates a copy of the element before proceeding with incrementing the element and returning the copy. Moreover, most compilers will automatically optimize sample code 1 by converting it implicitly into sample code 2.

----

## **Write a program that stores and displays the GPA (Grade Point Average) of a certain number of students, and you need to store and display it using C++.**

```c++
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
	for (int i = 0; i < num; ++i)
    {
		cout << "Student" << i + 1 << " :" << *(ptr + i) << endl;
	}
	delete[] ptr;
	return 0;
}
```

----

## **What is a mutable storage class specifier? How can they be used?**

A mutable storage class specifier is applied only to the class's non-static and non-constant member variable. It is used for altering the constant class object's member by declaring it. This can be done by using a storage class specifier.

----

## **What are the differences between a shallow copy and a deep copy?**

The differences between a shallow copy and a deep copy are:

Shallow Copy
Deep Copy

Allows memory dumping on a bit-by-bit basis from one object to another
Allows the copy field, which is done by field from one object to another.

Reflects changes made to the new/copied object in the original object. 
Doesn't reflect changes made to the new/copied object in the original object.

----

## **What is an Abstract class?**

An abstract class in C++ is referred to as the base class, which has at least one pure virtual function. In such a function, a person cannot instantiate an abstract class. This way, a pure virtual function is defined by using a pure specifier which is equal to zero during the declaration of the virtual member function in the class declaration. The code sample can be displayed as follows in example.

```c++
// An abstract class
class Test
{
// Data members of class
public:
    // Pure Virtual Function
    virtual void show() = 0;
    /* Other members */
};
```

----

## **What are the functions of the scope resolution operator?**

The functions of the scope resolution operator include the following.

It helps resolve the scope of various global variables.
It helps associate the function with the class when it is defined outside the class.
The code of the scope resolution operator can be displayed as follows.

```c++
#include <iostream>

using namespace std;

int my_var = 0;

int main(void)
{
	int my_var = 0;
	::my_var = 1; // set global my_var to 1
	my_var = 2; // setlocal my_var to 2
	cout << ::my_var << ", " << my_var;
	return 0;
}
```

----

## **What is the 'diamond problem' that occurs with multiple inheritance in C++?**

The "diamond problem" is a term used to describe a particular issue that can occur in multiple inheritance scenarios in C++ (and other languages that support multiple inheritance). It arises when a class inherits from two or more classes that share a common base class.

Consider the following inheritance hierarchy:

```cmd
       A
      / \
     B   C
      \ /
       D
```

In this example, classes B and C both inherit from class A, and class D inherits from both classes B and C. This creates a situation where class D has two copies of class A within its hierarchy.

The diamond problem occurs when there are conflicting or ambiguous definitions of members (variables or functions) from the common base class A. If both B and C define a member with the same name, and class D does not override it, the compiler is uncertain which version of the member to use when accessed through an object of class D. This ambiguity leads to a compilation error.

To resolve the diamond problem, C++ provides the concept of "virtual inheritance." By using the virtual keyword during inheritance, you can ensure that only one instance of the common base class is shared among the derived classes. The virtual inheritance mechanism helps to eliminate the ambiguity in member access.

To address the diamond problem in the above example, the inheritance declaration for classes B and C would be modified as follows:

```c++
class B : virtual public A
{
    // B class definition
};
```

```c++
class C : virtual public A
{
    // C class definition
};
```

By using virtual inheritance, class D will have a single instance of class A, avoiding conflicts and resolving the diamond problem.

```c++
class D : public B, public C
{
    // D class definition
};
```

In summary, the diamond problem occurs in C++ when multiple inheritance is used, and a class inherits from two or more classes that share a common base class. It leads to ambiguity in member access and can be resolved using virtual inheritance to ensure a single instance of the common base class.

# https://hackr.io/blog/cpp-interview-questions

# https://www.tutorialspoint.com/cplusplus/cpp_interview_questions.htm

## **What is the full form of OOPS?**

Object Oriented Programming System.

----

## **What is a class?**

Class is a blue print which reflects the entities attributes and actions. Technically defining a class is designing an user defined data type.

----

## **What is an object?**

An instance of the class is called as object.

----

## **List the types of inheritance supported in C++.**

Single, Multilevel, Multiple, Hierarchical and Hybrid.

----

## **What is the role of protected access specifier?**

If a class member is protected then it is accessible in the inherited class. However, outside the both the private and protected members are not accessible.

----

## **What is encapsulation?**

The process of binding the data and the functions acting on the data together in an entity (class) called as encapsulation.

----

## **What is abstraction?**

Abstraction refers to hiding the internal implementation and exhibiting only the necessary details.

----

## **What is inheritance?**

Inheritance is the process of acquiring the properties of the exiting class into the new class. The existing class is called as base/parent class and the inherited class is called as derived/child class.

----

## **Explain the purpose of the keyword volatile.**

Declaring a variable volatile directs the compiler that the variable can be changed externally. Hence avoiding compiler optimization on the variable reference.

----

## **What is an inline function?**

A function prefixed with the keyword inline before the function definition is called as inline function. The inline functions are faster in execution when compared to normal functions as the compiler treats inline functions as macros.

----

## **What is a storage class?**

In C++, a storage class is used to define the scope, lifetime, and initialization of variables or functions within a program. C++ provides several storage classes that determine where and how variables or functions are stored in memory. The storage classes in C++ are:

auto: This is the default storage class for local variables. It is automatically assigned to variables declared within a block or function. The auto variables are stored in the stack memory, and their lifetime is limited to the scope in which they are defined.

register: This storage class suggests the compiler to store the variable in a CPU register for faster access. However, the actual usage of register storage class is often ignored by modern compilers, as they perform optimization automatically.

static: Variables declared as static have a lifetime throughout the execution of the program, retaining their values between multiple function calls. Static variables are stored in the data segment of memory. When declared inside a function, they are initialized only once, and their value persists across function calls.

extern: This storage class is used to declare a variable that is defined in another file or module. The extern variables are typically used when multiple files need to access a shared variable.

mutable: This storage class is used only for non-static class members. It allows a member variable to be modified even within a const member function.

thread_local: This storage class is used to declare variables that have a separate instance for each thread. Each thread has its own copy of the variable.

Additionally, C++ has a storage class specifier called const which is used to define constants that cannot be modified after initialization.

It's important to note that the C++ programming language has evolved over time, and new features and enhancements may have been introduced since my knowledge cutoff in September 2021.

1. Example of auto storage class:

```c++
void exampleFunction()
{
    auto x = 10; // 'x' is automatically assigned the 'auto' storage class
    // ...
}
```

2. Example of static storage class:

```c++
void exampleFunction()
{
    static int counter = 0; // 'counter' is a static variable
    counter++;
    cout << "Counter: " << counter << endl;
}
```

3. Example of extern storage class:

In a header file (shared.h):

```c++
extern int sharedVariable; // Declaration of the shared variable
```

In one source file (source1.cpp):

```c++
#include "shared.h"

int sharedVariable = 5; // Definition of the shared variable
```

In another source file (source2.cpp):

```c++
#include "shared.h"

void exampleFunction()
{
    cout << "Shared Variable: " << sharedVariable << endl;
}
```

4. Example of mutable storage class:

```c++
class ExampleClass
{
public:
    void setValue(int value) const
    {
        mutableValue = value; // 'mutableValue' can be modified within a const member function
    }

    int getValue() const
    {
        return mutableValue;
    }

private:
    mutable int mutableValue;
};
```

5. Example of thread_local storage class:

```c++
thread_local int globalCounter = 0; // Each thread has its own copy of 'globalCounter'

void exampleFunction()
{
    globalCounter++;
    cout << "Counter: " << globalCounter << endl;
}
```

----

## **Mention the storage classes names in C++.**

The following are storage classes supported in C++
- auto,
- static,
- extern,
- register and
- mutable

----

## **What is the role of mutable storage class specifier?**

A constant class object’s member variable can be altered by declaring it using mutable storage class specifier. Applicable only for non-static and non-constant member variable of the class.

----

## **Distinguish between shallow copy and deep copy.**

Shallow copy does memory dumping bit-by-bit from one object to another.

```c++
#include <iostream>

class ShallowCopyExample
{
private:
    int* data;

public:
    // Constructor
    ShallowCopyExample(int value)
    {
        data = new int(value);
    }

    // Destructor
    ~ShallowCopyExample()
    {
        delete data;
    }

    // Shallow copy constructor
    ShallowCopyExample(const ShallowCopyExample& other)
    {
        data = other.data;
    }

    // Getter function
    int getData() const
    {
        return *data;
    }
};

int main()
{
    // Create an object with value 10
    ShallowCopyExample obj1(10);

    // Create a shallow copy of obj1
    ShallowCopyExample obj2 = obj1;

    // Print the data of both objects
    std::cout << "obj1 data: " << obj1.getData() << std::endl;
    std::cout << "obj2 data: " << obj2.getData() << std::endl;

    // Modify the data of obj1
    *obj1.data = 20;

    // Print the data of both objects again
    std::cout << "obj1 data: " << obj1.getData() << std::endl;
    std::cout << "obj2 data: " << obj2.getData() << std::endl;

    return 0;
}
```

Deep copy is copy field by field from object to another. Deep copy is achieved using copy constructor and or overloading assignment operator.

```c++
#include <iostream>

class DeepCopyExample
{
private:
    int* data;

public:
    // Constructor
    DeepCopyExample(int value)
    {
        data = new int(value);
    }

    // Destructor
    ~DeepCopyExample()
    {
        delete data;
    }

    // Deep copy constructor
    DeepCopyExample(const DeepCopyExample& other)
    {
        data = new int(*other.data);
    }

    // Getter function
    int getData() const
    {
        return *data;
    }
};

int main()
{
    // Create an object with value 10
    DeepCopyExample obj1(10);

    // Create a deep copy of obj1
    DeepCopyExample obj2 = obj1;

    // Print the data of both objects
    std::cout << "obj1 data: " << obj1.getData() << std::endl;
    std::cout << "obj2 data: " << obj2.getData() << std::endl;

    // Modify the data of obj1
    *obj1.data = 20;

    // Print the data of both objects again
    std::cout << "obj1 data: " << obj1.getData() << std::endl;
    std::cout << "obj2 data: " << obj2.getData() << std::endl;

    return 0;
}
```

----

## **What is a pure virtual function?**

A virtual function with no function body and assigned with a value zero is called as pure virtual function.

```c++
#include <iostream>

class Shape
{
public:
    // Pure virtual function
    virtual double calculateArea() const = 0;

    // Non-pure virtual function
    void printArea() const
    {
        std::cout << "Area: " << calculateArea() << std::endl;
    }
};

class Rectangle : public Shape
{
private:
    double length;
    double width;

public:
    Rectangle(double l, double w) : length(l), width(w)
    {
    }

    // Implementing the pure virtual function
    double calculateArea() const override
    {
        return length * width;
    }
};

class Circle : public Shape
{
private:
    double radius;

public:
    Circle(double r) : radius(r)
    {
    }

    // Implementing the pure virtual function
    double calculateArea() const override
    {
        return 3.14159 * radius * radius;
    }
};

int main()
{
    Rectangle rectangle(5.0, 3.0);
    Circle circle(2.5);

    rectangle.printArea(); // Output: Area: 15
    circle.printArea();    // Output: Area: 19.6349

    return 0;
}
```

----

## **What is an abstract class in C++?**

A class with at least one pure virtual function is called as abstract class. We cannot instantiate an abstract class.

```c++
#include <iostream>

class Shape
{
public:
    // Pure virtual function
    virtual double calculateArea() const = 0;

    // Non-pure virtual function
    void printArea() const
    {
        std::cout << "Area: " << calculateArea() << std::endl;
    }
};

class Rectangle : public Shape
{
private:
    double length;
    double width;

public:
    Rectangle(double l, double w) : length(l), width(w) {}

    // Implementing the pure virtual function
    double calculateArea() const override
    {
        return length * width;
    }
};

class Circle : public Shape {
private:
    double radius;

public:
    Circle(double r) : radius(r)
    {
    }

    // Implementing the pure virtual function
    double calculateArea() const override
    {
        return 3.14159 * radius * radius;
    }
};

int main()
{
    Rectangle rectangle(5.0, 3.0);
    Circle circle(2.5);

    rectangle.printArea(); // Output: Area: 15
    circle.printArea(); // Output: Area: 19.6349

    return 0;
}
```

----

## **What is a reference variable in C++?**

A reference variable is an alias name for the existing variable. Which mean both the variable name and reference variable point to the same memory location. Therefore updation on the original variable can be achieved using reference variable too.

```c++
#include <iostream>

int main()
{
    int num = 42;
    int& ref = num;  // Reference variable "ref" bound to "num"

    std::cout << "num: " << num << std::endl;   // Output: num: 42
    std::cout << "ref: " << ref << std::endl;   // Output: ref: 42

    ref = 99;  // Modifying "ref" also modifies "num"

    std::cout << "num: " << num << std::endl;   // Output: num: 99
    std::cout << "ref: " << ref << std::endl;   // Output: ref: 99

    return 0;
}
```

----

## **What is role of static keyword on class member variable?**

A static variable does exit though the objects for the respective class are not created. Static member variable share a common memory across all the objects created for the respective class. A static member variable can be referred using the class name itself.

## **Explain the static member function?**

A static member function can be invoked using the class name as it exits before class objects comes into existence. It can access only static members of the class.

```c++
#include <iostream>

class MyClass
{
private:
    static int count; // Static member variable

public:
    static void incrementCount() // Static member function
    { 
        count++;
    }

    static int getCount()
    {
        return count;
    }
};

int MyClass::count = 0; // Initialize static member variable

int main()
{
    std::cout << "Initial count: " << MyClass::getCount() << std::endl; // Output: Initial count: 0

    MyClass::incrementCount(); // Calling static member function
    MyClass::incrementCount();

    std::cout << "Updated count: " << MyClass::getCount() << std::endl; // Output: Updated count: 2

    return 0;
}
```

## **Name the data type which can be used to store wide characters in C++?**

wchar_t

----

## **What are/is the operator/operators used to access the class members?**

Dot (.) and Arrow ( -> )

----

## **Can we initialize a class/structure member variable as soon as the same is defined?**

No, Defining a class/structure is just a type definition and will not allocated memory for the same.

----

## **What is the data type to store the Boolean value?**

bool, is the new primitive data type introduced in C++ language.

----

## **What is function overloading?**

Defining several functions with the same name with unique list of parameters is called as function overloading.

```c++
#include <iostream>

// Function with two integer parameters
void add(int a, int b)
{
    int result = a + b;
    std::cout << "Sum of integers: " << result << std::endl;
}

// Function with two double parameters
void add(double a, double b)
{
    double result = a + b;
    std::cout << "Sum of doubles: " << result << std::endl;
}

// Function with a string parameter
void add(const std::string& a, const std::string& b)
{
    std::string result = a + b;
    std::cout << "Concatenated strings: " << result << std::endl;
}

int main()
{
    add(3, 4);                  // Calls the function with two integer parameters
    add(2.5, 3.7);              // Calls the function with two double parameters
    add("Hello, ", "world!");   // Calls the function with two string parameters

    return 0;
}
```

----

## **What is operator overloading?**

Defining a new job for the existing operator w.r.t the class objects is called as operator overloading.

```c++
#include <iostream>

class Complex
{
private:
    double real;
    double imag;

public:
    Complex(double r = 0.0, double i = 0.0) : real(r), imag(i)
    {
    }

    // Overloading the + operator
    Complex operator+(const Complex& other) const
    {
        return Complex(real + other.real, imag + other.imag);
    }

    // Overloading the - operator
    Complex operator-(const Complex& other) const
    {
        return Complex(real - other.real, imag - other.imag);
    }

    // Overloading the * operator
    Complex operator*(const Complex& other) const
    {
        return Complex(real * other.real - imag * other.imag, real * other.imag + imag * other.real);
    }

    // Overloading the << operator for output
    friend std::ostream& operator<<(std::ostream& os, const Complex& c)
    {
        os << "(" << c.real << " + " << c.imag << "i)";
        return os;
    }
};

int main()
{
    Complex a(2.0, 3.0);
    Complex b(1.0, 4.0);

    Complex sum = a + b;
    Complex diff = a - b;
    Complex product = a * b;

    std::cout << "Sum: " << sum << std::endl;             // Output: Sum: (3 + 7i)
    std::cout << "Difference: " << diff << std::endl;     // Output: Difference: (1 - 1i)
    std::cout << "Product: " << product << std::endl;     // Output: Product: (-10 + 11i)

    return 0;
}
```

----

## **Do we have a String primitive data type in C++?**

No, it’s a class from STL (Standard template library).

----

## **Name the default standard streams in C++?**

cin, cout, cerr and clog.

----

## **Which access specifier/s can help to achive data hiding in C++?**

Private & Protected.

----

## **When a class member is defined outside the class, which operator can be used to associate the function definition to a particular class?**

Scope resolution operator (::)

----

## **What is a destructor? Can it be overloaded?**

A destructor is the member function of the class which is having the same name as the class name and prefixed with tilde (~) symbol. It gets executed automatically w.r.t the object as soon as the object loses its scope. It cannot be overloaded and the only form is without the parameters.

```c++
#include <iostream>

class MyClass
{
private:
    int* data;

public:
    MyClass()
    {
        data = new int[10]; // Allocate memory
        std::cout << "Constructor called" << std::endl;
    }

    ~MyClass()
    {
        delete[] data; // Deallocate memory
        std::cout << "Destructor called" << std::endl;
    }
};

int main()
{
    {
        MyClass obj; // Create an object of MyClass

        // Perform operations with obj
        // ...

    } // Object goes out of scope here

    std::cout << "Object destroyed" << std::endl;

    return 0;
}
```

----

## **What is a constructor?**

A constructor is the member function of the class which is having the same as the class name and gets executed automatically as soon as the object for the respective class is created.

```c++
#include <iostream>

class MyClass
{
private:
    int value;

public:
    // Constructor with a parameter
    MyClass(int v)
    {
        value = v;
        std::cout << "Constructor called with value: " << value << std::endl;
    }

    // Default constructor (constructor with no parameters)
    MyClass()
    {
        value = 0;
        std::cout << "Default constructor called" << std::endl;
    }

    int getValue()
    {
        return value;
    }
};

int main() {
    MyClass obj1(42); // Create an object using the constructor with a parameter
    MyClass obj2; // Create an object using the default constructor

    std::cout << "Value of obj1: " << obj1.getValue() << std::endl;
    std::cout << "Value of obj2: " << obj2.getValue() << std::endl;

    return 0;
}
```

----

## **What is a default constructor? Can we provide one for our class?**

Every class does have a constructor provided by the compiler if the programmer doesn’t provides one and known as default constructor. A programmer provided constructor with no parameters is called as default constructor. In such case compiler doesn’t provides the constructor.

```c++
#include <iostream>

class MyClass
{
private:
    int value;

public:
    // Constructor with a parameter
    MyClass(int v)
    {
        value = v;
        std::cout << "Constructor called with value: " << value << std::endl;
    }

    // Default constructor (constructor with no parameters)
    MyClass()
    {
        value = 0;
        std::cout << "Default constructor called" << std::endl;
    }

    int getValue()
    {
        return value;
    }
};

int main()
{
    MyClass obj1(42); // Create an object using the constructor with a parameter
    MyClass obj2; // Create an object using the default constructor

    std::cout << "Value of obj1: " << obj1.getValue() << std::endl;
    std::cout << "Value of obj2: " << obj2.getValue() << std::endl;

    return 0;
}
```

----

## **Which operator can be used in C++ to allocate dynamic memory?**

'new' is the operator can be used for the same.

1. Allocating a single object:

```c++
int* ptr = new int; // Allocate memory for a single integer
*ptr = 42; // Assign a value to the allocated integer
delete ptr; // Deallocate the memory when no longer needed
```

2. Allocating an array of objects:

```c++
int* ptr = new int; // Allocate memory for a single integer
*ptr = 42; // Assign a value to the allocated integer
delete ptr; // Deallocate the memory when no longer needed
```

3. Allocating an object using a custom constructor:

```c++
class MyClass {
public:
    MyClass(int value)
    {
        // Constructor implementation
    }
};

MyClass* obj = new MyClass(42);  // Allocate memory for an object of MyClass
delete obj;                     // Deallocate the memory for the object
```

In all of these examples, the new operator is used to allocate memory on the heap. After allocating the memory, you can access and manipulate the allocated objects or arrays using the pointer returned by new. Once you're done using the dynamically allocated memory, it is important to deallocate it using the delete operator (or delete[] for arrays) to free the memory and avoid memory leaks.

Note that when using new, you are responsible for managing the allocated memory by ensuring proper deallocation. Failure to deallocate dynamically allocated memory can lead to memory leaks and potential resource issues.

----

## **What is the purpose of 'delete' operator?**

'delete' operator is used to release the dynamic memory which was created using 'new' operator.

```c++
#include <iostream>

int main()
{
    int* ptr = new int(42);  // Allocate memory for an integer and assign a value
    std::cout << "Value: " << *ptr << std::endl;
    delete ptr;  // Deallocate the memory

    return 0;
}
```

----

## **Can I use malloc() function of C language to allocate dynamic memory in C++?**

Yes, as C is the subset of C++, we can all the functions of C in C++ too.

```c++
#include <iostream>
#include <cstdlib>

int main()
{
    int* ptr = static_cast<int*>(malloc(sizeof(int)));  // Allocate memory using malloc

    if (ptr != nullptr)
    {
        *ptr = 42;  // Assign a value to the allocated memory
        std::cout << "Value: " << *ptr << std::endl;
        free(ptr);  // Deallocate the memory using free
    }

    return 0;
}
```

----

## **Can I use 'delete' operator to release the memory which was allocated using malloc() function of C language?**

No, we need to use free() of C language for the same.

```c
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int* ptr = (int*)malloc(sizeof(int));  // Allocate memory using malloc

    if (ptr != NULL)
    {
        *ptr = 42;  // Assign a value to the allocated memory
        printf("Value: %d\n", *ptr);

        free(ptr);  // Deallocate the memory using free
    }

    return 0;
}
```

----

## **What is a friend function?**

A function which is not a member of the class but still can access all the member of the class is called so. To make it happen we need to declare within the required class following the keyword 'friend'.

```c++
#include <iostream>

class MyClass
{
private:
    int value;

public:
    MyClass(int v) : value(v)
    {
    }

    friend void printValue(const MyClass& obj); // Declaration of friend function
};

void printValue(const MyClass& obj)
{
    std::cout << "Value: " << obj.value << std::endl;  // Accessing private member
}

int main()
{
    MyClass obj(42);
    printValue(obj);  // Calling the friend function

    return 0;
}
```

----

## **What is a copy constructor?**

A copy constructor is the constructor which take same class object reference as the parameter. It gets automatically invoked as soon as the object is initialized with another object of the same class at the time of its creation.

```c++
#include <iostream>

class MyClass
{
private:
    int value;

public:
    MyClass(int v) : value(v)
    {
        std::cout << "Constructor called: " << value << std::endl;
    }

    // Copy constructor
    MyClass(const MyClass& other) : value(other.value)
    {
        std::cout << "Copy constructor called: " << value << std::endl;
    }

    int getValue()
    {
        return value;
    }
};

int main()
{
    MyClass obj1(42); // Create an object using the constructor
    MyClass obj2 = obj1; // Create a new object using the copy constructor

    std::cout << "Value of obj1: " << obj1.getValue() << std::endl;
    std::cout << "Value of obj2: " << obj2.getValue() << std::endl;

    return 0;
}
```

----

## **Does C++ supports exception handling? If so what are the keywords involved in achieving the same?**

C++ does supports exception handling. Try, catch & throw are keyword used for the same.

```c++
#include <iostream>

int divideNumbers(int numerator, int denominator)
{
    if (denominator == 0)
    {
        throw std::runtime_error("Division by zero is not allowed.");
    }

    return numerator / denominator;
}

int main()
{
    int result;
    int num = 10;
    int den = 0;

    try
    {
        result = divideNumbers(num, den);
        std::cout << "Result: " << result << std::endl;
    }
    catch (const std::exception& e)
    {
        std::cout << "Exception occurred: " << e.what() << std::endl;
    }

    return 0;
}
```

----

## **Explain the pointer – this?**

This, is the pointer variable of the compiler which always holds the current active object’s address.

```c++
#include <iostream>

class MyClass
{
private:
    int value;

public:
    void setValue(int newValue)
    {
        this->value = newValue;  // Accessing member variable using 'this' pointer
    }

    int getValue()
    {
        return this->value;  // Accessing member variable using 'this' pointer
    }
};

int main()
{
    MyClass obj;
    obj.setValue(42);

    std::cout << "Value: " << obj.getValue() << std::endl;

    return 0;
}
```

## **What is the difference between the keywords struct and class in C++?**

By default the members of struct are public and by default the members of the class are private.

----

## **Can we implement all the concepts of OOPS using the keyword struct?**

Yes.

----

## **What is the block scope variable in C++?**

A variable whose scope is applicable only within a block is said so. Also a variable in C++ can be declared anywhere within the block.

----

## **What is the role of the file opening mode ios::trunk?**

If the file already exists, its content will be truncated before opening the file.

```c++
#include <iostream>

int main()
{
    int x = 5;  // Block scope variable

    {
        int y = 10;  // Nested block scope variable

        std::cout << "Inside nested block:" << std::endl;
        std::cout << "x = " << x << std::endl;  // Accessing outer block variable
        std::cout << "y = " << y << std::endl;
    }

    // y is not accessible here, as it is outside its scope

    std::cout << "Outside nested block:" << std::endl;
    std::cout << "x = " << x << std::endl;

    return 0;
}
```

----

## **What is the scope resolution operator?**

The scope resolution operator is used to
- Resolve the scope of global variables.
- To associate function definition to a class if the function is defined outside the class.

```c++
#include <iostream>

namespace MyNamespace
{
    int x = 5;

    void myFunction()
    {
        std::cout << "Inside MyNamespace::myFunction()" << std::endl;
    }
}

int main()
{
    int x = 10;

    std::cout << "Local x = " << x << std::endl;                   // Accessing local x
    std::cout << "Global x = " << ::x << std::endl;                // Accessing global x using the scope resolution operator

    MyNamespace::myFunction();                                     // Accessing function inside a namespace using the scope resolution operator
    std::cout << "Value of x in MyNamespace = " << MyNamespace::x << std::endl;  // Accessing variable inside a namespace using the scope resolution operator

    return 0;
}
```

----

## **What is a namespace?**

A namespace is the logical division of the code which can be used to resolve the name conflict of the identifiers by placing them under different name space.

----

## **What are command line arguments?**

The arguments/parameters which are sent to the main() function while executing from the command line/console are called so. All the arguments sent are the strings only.

```c++
#include <iostream>

int main(int argc, char* argv[])
{
    std::cout << "Number of command-line arguments: " << argc << std::endl;

    // Print each command-line argument
    for (int i = 0; i < argc; ++i)
    {
        std::cout << "Argument " << i << ": " << argv[i] << std::endl;
    }

    return 0;
}
```

----

## **What is a class template?**

A template class is a generic class. The keyword template can be used to define a class template.

```c++
#include <iostream>

// Class template for a generic Pair
template <typename T1, typename T2>
class Pair
{
private:
    T1 first;
    T2 second;

public:
    Pair(const T1& a, const T2& b) : first(a), second(b)
    {
    }

    T1 getFirst() const
    {
        return first;
    }

    T2 getSecond() const
    {
        return second;
    }
};

int main()
{
    // Creating objects of Pair with different types
    Pair<int, double> pair1(10, 3.14);
    Pair<std::string, bool> pair2("Hello", true);

    // Accessing and printing the values
    std::cout << "Pair 1: " << pair1.getFirst() << ", " << pair1.getSecond() << std::endl;
    std::cout << "Pair 2: " << pair2.getFirst() << ", " << pair2.getSecond() << std::endl;

    return 0;
}
```

----

## **How can we catch all kind of exceptions in a single catch block?**

The catch block with ellipses as follows

```c++
catch() 
{
    // code example to do here
}
```

----

## **What is keyword 'auto' for?**

By default every local variable of the function is automatic (auto). In the below function both the variables ‘i’ and ‘j’ are automatic variables.

```c++
void f() 
{
   int i;
   auto int j;
}
```

NOTE − A global variable can’t be an automatic variable.

----

## **What is a static variable?**

A static local variables retains its value between the function call and the default value is 0. The following function will print 1 2 3 if called thrice.

```c++
void f() 
{ 
   static int i; 
   ++i; 
   printf(“%d “,i); 
}
```

If a global variable is static then its visibility is limited to the same source code.

----

## **What is the purpose of extern storage specifier?**

Used to resolve the scope of global symbol

```c++
#include <iostream>

using namespace std;	
main()
{
   extern int i;
      
   cout<<i<<endl;
}
int i = 20;
```

----

## **What is the meaning of base address of the array?**

The starting address of the array is called as the base address of the array.

----

## **When should we use the register storage specifier?**

If a variable is used most frequently then it should be declared using register storage specifier, then possibly the compiler gives CPU register for its storage to speed up the look up of the variable.

----

## **Can a program be compiled without main() function?**

Yes, it can be but cannot be executed, as the execution requires `main()` function definition.

----

## **Where an automatic variable is stored?**

Every local variable by default being an auto variable is stored in stack memory

----

## **What is a container class?**

A class containing at least one member variable of another class type in it is called so.

----

## **What is a token?**

A C++ program consists of various tokens and a token is either a keyword, an identifier, a constant, a string literal, or a symbol.

----

## **What is a preprocessor?**

Preprocessor is a directive to the compiler to perform certain things before the actual compilation process begins.

----

## **What are command line arguments?**

The arguments which we pass to the main() function while executing the program are called as command line arguments. The parameters are always strings held in the second argument (below in args) of the function which is array of character pointers. First argument represents the count of arguments (below in count) and updated automatically by operating system.

----

## **What are the different ways of passing parameters to the functions? Which to use when?**

__Call by value__ − We send only values to the function as parameters. We choose this if we do not want the actual parameters to be modified with formal parameters but just used.

```c++
#include <iostream>

// Function to increment a value by 1
void increment(int num)
{
    num++;
    std::cout << "Inside increment function: " << num << std::endl;
}

int main()
{
    int value = 5;

    std::cout << "Before calling increment: " << value << std::endl;
    increment(value);
    std::cout << "After calling increment: " << value << std::endl;

    return 0;
}
```

__Call by address__ − We send address of the actual parameters instead of values. We choose this if we do want the actual parameters to be modified with formal parameters.

```c++
#include <iostream>

// Function to increment a value by 1 using call-by-address
void incrementByAddress(int* numPtr)
{
    (*numPtr)++;
    std::cout << "Inside incrementByAddress function: " << *numPtr << std::endl;
}

int main()
{
    int value = 5;

    std::cout << "Before calling incrementByAddress: " << value << std::endl;
    incrementByAddress(&value);
    std::cout << "After calling incrementByAddress: " << value << std::endl;

    return 0;
}
```

__Call by reference__ − The actual parameters are received with the C++ new reference variables as formal parameters. We choose this if we do want the actual parameters to be modified with formal parameters.

```c++
#include <iostream>

// Function to increment a value by 1 using call-by-address
void incrementByAddress(int* numPtr)
{
    (*numPtr)++;
    std::cout << "Inside incrementByAddress function: " << *numPtr << std::endl;
}

int main()
{
    int value = 5;

    std::cout << "Before calling incrementByAddress: " << value << std::endl;
    incrementByAddress(&value);
    std::cout << "After calling incrementByAddress: " << value << std::endl;

    return 0;
}
```

----

## **What is reminder for 5.0 % 2?**

Error, It is invalid that either of the operands for the modulus operator (%) is a real number.

```c++
// TestApplication.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <string>
#include <stdio.h>

using namespace std;

int main()
{
    // float result = 5.0 % 2; // expression must have integral or unscoped enum type
    float result = 5 % 2;
    cout << "The result is : " << result << endl;

    return 0;
}
```

----

## **Which compiler switch to be used for compiling the programs using math library with g++ compiler?**

Option `–lm` to be used as `g++ –lm <file.cpp>`.

----

## **Can we resize the allocated memory which was allocated using ‘new’ operator?**

No, there is no such provision available.

----

## **Which operator can be used to determine the size of a data type/class or variable/object?**

sizeof

```c++
#include <iostream>

int main()
{
    int num = 10;
    std::cout << "Size of int: " << sizeof(int) << " bytes" << std::endl;
    std::cout << "Size of num: " << sizeof(num) << " bytes" << std::endl;

    double pi = 3.14159;
    std::cout << "Size of double: " << sizeof(double) << " bytes" << std::endl;
    std::cout << "Size of pi: " << sizeof(pi) << " bytes" << std::endl;

    char ch = 'A';
    std::cout << "Size of char: " << sizeof(char) << " byte" << std::endl;
    std::cout << "Size of ch: " << sizeof(ch) << " byte" << std::endl;

    return 0;
}
```

In this example, we use the sizeof operator to determine the size of different data types. We first declare an int variable num and use sizeof(int) and sizeof(num) to get the size of int and num.

Similarly, we do the same for a double variable pi and a char variable ch. The output will vary depending on the platform and the size of the data types on your system.

This example demonstrates how the sizeof operator can be used to determine the size of data types in C++. Note that the size may vary depending on the system architecture and the compiler being used.

----

## **How can we refer to the global variable if the local and the global variable names are same?**

We can apply scope resolution operator (::) to the for the scope of global variable.

In C++, if you have a local variable with the same name as a global variable, you can use the scope resolution operator :: to explicitly refer to the global variable.

Here's an example to illustrate how to refer to a global variable when there is a local variable with the same name:

```c++
#include <iostream>

int num = 10; // Global variable

int main()
{
    int num = 20; // Local variable with the same name

    std::cout << "Local num: " << num << std::endl;      // Output: Local num: 20
    std::cout << "Global num: " << ::num << std::endl;   // Output: Global num: 10

    return 0;
}
```

In this example, we have a global variable num declared outside the main() function with a value of 10. Inside the main() function, we declare a local variable num with a value of 20.

When we use the variable num without any qualification, it refers to the local variable because local variables take precedence over global variables within the same scope. So, num outputs the value of the local variable, which is 20.

To refer to the global variable explicitly, we use the scope resolution operator :: followed by the variable name. In this case, ::num refers to the global variable num outside the main() function, and it outputs the value 10.

By using the scope resolution operator, we can differentiate between local and global variables with the same name and access the desired variable based on the scope we specify.

----

## **What are valid operations on pointers?**

The only two permitted operations on pointers are
1. Comparision
2. Addition/Substraction (excluding void pointers)

----

## **What is recursion?**

Function calling itself is called as recursion.

```c++
#include <iostream>

unsigned long long factorial(int n)
{
    if (n == 0 || n == 1)
    {
        return 1;
    }
    else
    {
        return n * factorial(n - 1);
    }
}

int main()
{
    int number = 5;
    unsigned long long result = factorial(number);
    std::cout << "Factorial of " << number << " is: " << result << std::endl;

    return 0;
}
```

----

## **What is the first string in the argument vector w.r.t command line arguments?**

Program name.

----

## **What is the maximum length of an identifier?**

Ideally it is 32 characters and also implementation dependent.

----

## **What is the default function call method?**

By default the functions are `called by value`.

----

## **What are available mode of inheritance to inherit one class from another?**

Public, private & protected

----

## **What is the difference between delete and delete[]?**

Delete[] is used to release the array allocated memory which was allocated using new[] and delete is used to release one chunk of memory which was allocated using new.

----

## **Does an abstract class in C++ need to hold all pure virtual functions?**

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

----

## **Are class functions taken into consideration as part of the object size?**

No, only the class member variables determines the size of the respective class object.

----

## **Can we create and empty class? If so what would be the size of such object.**

We can create an empty class and the object size will be 1.

----

## **What is 'std'?**

Default namespace defined by C++.

----

## **What is the full form of STL?**

Standard template library

----

## **What is 'cout'?**

cout is the object of ostream class. The stream ‘cout’ is by default connected to console output device.

----

## **What is 'cin'?**

cin is the object of istream class. The stream ‘cin’ is by default connected to console input device.

----

## **What is the use of the keyword ‘using’?**

It is used to specify the namespace being used in.

----

## **If a pointer declared for a class, which operator can be used to access its class members?**

Arrow `->` operator can be used for the same.

----

## **What is difference between including the header file with-in angular braces and double quotes?**

If a header file is included with in < > then the compiler searches for the particular header file only with in the built in include path. If a header file is included with in “ “, then the compiler searches for the particular header file first in the current working directory, if not found then in the built in include path

----

## **S++ or S = S+1, which can be recommended to increment the value by 1 and why?**

S++, as it is single machine instruction (INC) internally.

----

## **What is the difference between actual and formal parameters?**

The parameters sent to the function at calling end are called as actual parameters while at the receiving of the function definition called as formal parameters.

----

## **What is the difference between variable declaration and variable definition?**

Declaration associates type to the variable whereas definition gives the value to the variable.

----

## **Which key word is used to perform unconditional branching?**

goto.

----

## **Is 068 a valid octal number?**

No, it contains invalid octal digits.

---

## **What is the purpose of #undef preprocessor?**

It will be used to undefine an existing macro definition.

----

## **Can we nest multi line comments in a C++ code?**

No, we cannot.

----

## **What is a virtual destructor?**

A virtual destructor ensures that the objects resources are released in the reverse order of the object being constructed w.r.t inherited object.

----

## **What is the order of objects destroyed in the memory?**

The objects are destroyed in the reverse order of their creation.

----

## **What is a friend class?**

A class members can gain accessibility over other class member by placing the class declaration prefixed with the keyword ‘friend’ in the destination class.

# https://www.tutorialspoint.com/cplusplus/cpp_interview_questions.htm

# https://www.interviewkickstart.com/interview-questions/cpp-interview-questions-for-experienced-developers
 
*## *Why would you choose C++ over other programming languages?**

The following prominent advantages of C++ make it software developers' choice:
- It is a portable language and can allow developers to run it on any platform and operating system.
- - It has abundant function libraries.
- C++ supports inheritance, polymorphism, and friend functions.
- Data hiding in C++ language provides additional data security.
- Learn how C++ is different from the C programming language. 

----

## **What do you understand about scopes in C++?**

This is one of the most commonly asked C++ interview questions and answers. The area wherein the variable is active is referred to as scope. Thus, you can declare, define, and use the variable in scope. C++ has the following two types of scopes:

__Local scope:__ When a variable is declared inside the block of code and remains active only inside that block, it is said to be in a local scope and is accessible outside the block.
__Global scope:__ When a variable is declared at the top of the program, it is in a global scope and is accessible throughout the program.

---

## **What tokens does the C++ language support?**

C++ supports the following types of tokens:
- Keyword
- Constant
- Identifier
- Literal
- Symbol

----

## **How is the assignment operator ( = ) different from the equal to operator ( == )?**

The assignment operator ( = ) assigns the value to the variable and is sometimes used in complex equations.
The 'equal to' operator ( == ) is an equality operator used to compare two values. It returns true if they are equal; else, it returns false.

----

## **Explain comments in context with C++?**

Comments are the source code that the compiler ignores, and they are not a part of programs. The purpose of comments is to inform the programmer about additional information. It provides details about the source code. There are two types of comments in C++:

__Single line comment:__ It uses "//"for commenting, and the compiler ignores everything after "//"in the line.

__Multiline comment or block comment:__ It uses “ /* ” “ */ “ for commenting and the compiler ignores everything between “ /* “ “ */ “.

----

## **What is containership?**

It is one of the most important C++ interview questions and answers concepts. You can contain an object of one class into another, and that object will be a member of the other class. This relationship between classes wherein one class contains the object of another class is referred to as containership. 

----

## **What is data hiding?**

The process of hiding elements of a program's code from object members is called data hiding. It ensures controlled data access and objects integrity. It also prevents unintentional or intended changes to the program.

----

## **What is the use of getline in C++?**

The C++ getline() is a standard library in-built function and it is defined in the <string.h> header file. It allows accepting and reading single and multiple lines. 

----

## **What is a singleton design pattern?**

Design patterns are reusable solutions that you can apply to recurring Object-Oriented Design problems. Singleton design patterns fall under the category of Creational Design Patterns. This pattern helps design a class with a maximum of a single instance at any time. It cannot be instantiated further. 

The concept of a singleton design pattern can be applied to creating a logger or hardware interface class. 

----

## **What operators cannot be overloaded?**

The following operators cannot be overloaded:

`?:` – conditional operator

`.*` – dereferencing operator

`sizeof` – sizeof operator

`::` – scope resolution operator

`.` – Dot operator

`->` – member dereferencing operator

----

## **What do you understand about RTTI?**

RTTI stands for Run-time type information. This mechanism gives information about an object's data type at runtime. It is available only for classes that have at least one virtual function. You can determine the type of an object during program runtime execution.

----

## **What is the sparse matrix?**

An array of elements wherein many elements have a value of zero is called a sparse matrix. For instance, if you are given a matrix with several elements and the number of zeroes is more than half the elements of the matrix, then it is a sparse matrix.

----

## **What do you understand about smart pointers in C++?**

Smart pointers are employed in garbage collection to ensure no memory leaks. If you use smart pointers, you need not call delete for any memory allocated dynamically as it is automatically deallocated. You can implement smart pointers in C++11 and higher versions. C++11 has the following four kinds of smart pointers:
- auto_ptr
- unique_ptr
- shared_ptr 
- weak_ptr.

----

## **What is the role of this pointer and void pointer?**

__This pointer:__ The 'this pointer' is present in the member functions of every object. It points to the object itself and can be used to access the object's data. 

__Void pointer:__ A pointer that has no data type associated with it is called a void pointer. You can assign any type of pointer to a void pointer, but the reverse isn't true unless you use it as follows 

```c++
str=(char*) ptr;.
```

----

## **What do you understand about pure virtual functions?**

A virtual function is a member function in the base class that can be redefined in a derived class. It can be declared using the virtual keyword. On the contrary, a pure virtual function has no implementation. It has no body and is declared by assigning 0. 

----

## **Is it possible to call a virtual function from a constructor?**

Yes, you can call a virtual function from a constructor. However, the behavior differs in that case. When you call a virtual function, the virtual call is resolved at runtime. The virtual machine does not work within the constructor.

## **What is a copy constructor in C++?**

```c++
#include <iostream>

class MyClass
{
private:
    int data;

public:
    // Default constructor
    MyClass()
    {
        data = 0;
        std::cout << "Default constructor called" << std::endl;
    }

    // Parameterized constructor
    MyClass(int value)
    {
        data = value;
        std::cout << "Parameterized constructor called" << std::endl;
    }

    // Copy constructor
    MyClass(const MyClass& other)
    {
        data = other.data;
        std::cout << "Copy constructor called" << std::endl;
    }

    int getData() const
    {
        return data;
    }
};

int main()
{
    // Create an object using the parameterized constructor
    MyClass obj1(10);

    // Create a new object and copy the contents of obj1 using the copy constructor
    MyClass obj2 = obj1;

    // Print the data of obj2
    std::cout << "Data in obj2: " << obj2.getData() << std::endl;

    return 0;
}
```

----

## **How is modularity introduced in C++?**

```c++
// Module1.cpp
#include <iostream>

void function1()
{
    std::cout << "Function 1 from Module 1" << std::endl;
}

void function2()
{
    std::cout << "Function 2 from Module 1" << std::endl;
}
```

```c++
// Module2.cpp
#include <iostream>

void function3()
{
    std::cout << "Function 3 from Module 2" << std::endl;
}

void function4()
{
    std::cout << "Function 4 from Module 2" << std::endl;
}
```

```c++
// Main.cpp
#include <iostream>

// Function declarations
void function1();
void function2();
void function3();
void function4();

int main()
{
    function1();
    function2();
    function3();
    function4();

    return 0;
}
```

----

## **What is the difference between method overloading and method overriding?**

*Method Overloading:*

Method overloading in C++ allows multiple methods with the same name but different parameters to exist within the same class. The overloaded methods can have the same or different return types. Overloading is determined at compile-time based on the number, order, or type of parameters.

Key points about method overloading in C++:
- Occurs within the same class.
- The methods must have the same name but different parameter lists.
- Overloaded methods can have different return types.
- The methods can have different access specifiers (e.g., public, private, protected).
- Overloading is determined at compile-time based on the method signature.
- Method overloading is used to provide multiple ways of invoking a method with different parameter options.
- The compiler selects the appropriate method to invoke based on the method signature and the arguments provided.

*Method Overriding:*

Method overriding in C++ is a feature of inheritance that allows a derived class to provide its own implementation of a method that is already defined in the base class. The base class method must be declared as virtual (or pure virtual) to enable overriding.

Key points about method overriding in C++:
- Occurs between a base class and its derived class.
- The derived class provides its own implementation of a method defined in the base class.
- The method in the base class must be declared as virtual (or pure virtual) to enable overriding.
- The method signature (name and parameters) in the derived class must match that of the base class method.
- Method overriding is determined at runtime based on the actual object type.
- Method overriding is used to achieve runtime polymorphism.

The base class pointer or reference can be used to invoke the overridden method, and the appropriate derived class implementation is executed.

## **What is the size of an empty class in C++?**

```c++
#include <iostream>

class EmptyClass
{
};

int main()
{
    std::cout << "Size of an empty class: " << sizeof(EmptyClass) << " bytes" << std::endl;
    return 0;
}
```

----

## **Explain the following concepts in C++?**

__Inheritance__

```c++
#include <iostream>

// Base class
class Shape
{
protected:
    int width;
    int height;

public:
    Shape(int w, int h) : width(w), height(h) {}

    void display() {
        std::cout << "Width: " << width << ", Height: " << height << std::endl;
    }
};

// Derived class
class Rectangle : public Shape
{
public:
    Rectangle(int w, int h) : Shape(w, h) {}

    int getArea() {
        return width * height;
    }
};

int main()
{
    Rectangle rect(5, 3);

    rect.display();         // Output: Width: 5, Height: 3
    int area = rect.getArea();
    std::cout << "Area: " << area << std::endl;   // Output: Area: 15

    return 0;
}

```

__Abstraction__

```c++
#include <iostream>

// Abstract base class
class Shape
{
public:
    virtual void draw() = 0;  // Pure virtual function

    virtual ~Shape()
    { 
    }  // Virtual destructor
};

// Concrete derived class
class Circle : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a circle." << std::endl;
    }
};

// Concrete derived class
class Square : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a square." << std::endl;
    }
};

int main()
{
    Shape* shape1 = new Circle();
    Shape* shape2 = new Square();

    shape1->draw();  // Output: Drawing a circle.
    shape2->draw();  // Output: Drawing a square.

    delete shape1;
    delete shape2;

    return 0;
}
```

__Encapsulation__

```c++
#include <iostream>

class Person
{
private:
    std::string name;
    int age;

public:
    // Getter functions
    std::string getName() const
    {
        return name;
    }

    int getAge() const
    {
        return age;
    }

    // Setter functions
    void setName(const std::string& newName)
    {
        name = newName;
    }

    void setAge(int newAge)
    {
        if (newAge >= 0)
        {
            age = newAge;
        }
    }
};

int main()
{
    Person person;

    // Accessing private data through public member functions
    person.setName("John Doe");
    person.setAge(25);

    std::cout << "Name: " << person.getName() << std::endl;
    std::cout << "Age: " << person.getAge() << std::endl;

    return 0;
}
```

__Polymorphism__

```c++
#include <iostream>

// Base class
class Shape {
public:
    virtual void draw() {
        std::cout << "Drawing a shape." << std::endl;
    }
};

// Derived class
class Circle : public Shape {
public:
    void draw() override {
        std::cout << "Drawing a circle." << std::endl;
    }
};

// Derived class
class Square : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a square." << std::endl;
    }
};

int main()
{
    Shape* shape1 = new Circle();
    Shape* shape2 = new Square();

    shape1->draw();  // Output: Drawing a circle.
    shape2->draw();  // Output: Drawing a square.

    delete shape1;
    delete shape2;

    return 0;
}
```

__Friend Function__

```c++
#include <iostream>

class MyClass {
private:
    int data;

public:
    MyClass(int d) : data(d)
    {
    }

    friend void displayData(const MyClass& obj);
};

void displayData(const MyClass& obj)
{
    std::cout << "Data: " << obj.data << std::endl;
}

int main()
{
    MyClass obj(42);
    displayData(obj);  // Output: Data: 42

    return 0;
}
```

__Data Binding__

In C++, data binding is not a language feature like in some other programming languages. However, you can achieve data binding-like behavior through various techniques and libraries.

One popular approach is to use the Model-View-Controller (MVC) or Model-View-ViewModel (MVVM) architectural patterns, along with frameworks such as Qt or libraries like Boost.Property.

Here's a simple example using the Boost.Property library to demonstrate data binding-like behavior:

```c++
#include <iostream>
#include <boost/property/property_map.hpp>

// Model class
class Person {
private:
    boost::property<std::string> name;
    boost::property<int> age;

public:
    // Getter and setter for the name property
    std::string getName() const {
        return name;
    }

    void setName(const std::string& newName) {
        name = newName;
    }

    // Getter and setter for the age property
    int getAge() const {
        return age;
    }

    void setAge(int newAge) {
        age = newAge;
    }
};

// View class
class PersonView {
public:
    void display(const Person& person) {
        std::cout << "Name: " << person.getName() << std::endl;
        std::cout << "Age: " << person.getAge() << std::endl;
    }
};

int main() {
    Person person;
    PersonView view;

    // Binding the view to the model
    boost::property_map<Person> properties(person);
    properties["name"].bind(view, &PersonView::display);
    properties["age"].bind(view, &PersonView::display);

    // Modifying the model
    person.setName("John Doe");
    person.setAge(25);

    // The view is automatically updated
    // due to the binding with the model

    return 0;
}
```

In this example, we have a Person class representing the model. It has two properties, name and age, which are implemented using the boost::property class from the Boost.Property library. The properties provide automatic notification when their values change.

The PersonView class represents the view and has a display() function to display the person's name and age.

In the main() function, we create an instance of Person and PersonView. We then use the boost::property_map to bind the properties of the Person object to the display() function of the PersonView. This establishes a data binding-like relationship between the model and the view.

When we modify the properties of the Person object, such as setting the name and age, the view is automatically updated due to the binding. This allows for synchronization of the model and view without explicitly calling display functions.

Note that this example uses the Boost.Property library for demonstration purposes, but in real-world scenarios, you might use more comprehensive frameworks or libraries that provide extensive support for data binding and automatic view updates, such as Qt or other UI frameworks.

Remember that data binding is not a built-in feature of C++, so achieving data binding-like behavior typically involves using external libraries or implementing custom mechanisms based on the desired architectural pattern or framework.

__Virtual Function__

```c++
#include <iostream>

// Base class
class Animal
{
public:
    virtual void makeSound() 
    {
        std::cout << "The animal makes a sound." << std::endl;
    }
};

// Derived class
class Dog : public Animal
{
public:
    void makeSound() override
    {
        std::cout << "The dog barks." << std::endl;
    }
};

// Derived class
class Cat : public Animal
{
public:
    void makeSound() override
    {
        std::cout << "The cat meows." << std::endl;
    }
};

int main()
{
    Animal* animal1 = new Dog();
    Animal* animal2 = new Cat();

    animal1->makeSound();  // Output: The dog barks.
    animal2->makeSound();  // Output: The cat meows.

    delete animal1;
    delete animal2;

    return 0;
}
```

In this example, we have a base class called Animal that defines a virtual function makeSound(). The makeSound() function is marked as virtual, indicating that it can be overridden by derived classes.

We then have two derived classes, Dog and Cat, which inherit from the Animal base class. Both derived classes override the makeSound() function with their specific implementation.

In the main() function, we create two pointers of type Animal* that point to objects of the Dog and Cat classes. Since the pointers are of the base class type, they can hold objects of both the base class and derived classes.

When we call the makeSound() function through the base class pointers, the appropriate implementation based on the actual object being referred to is invoked dynamically at runtime. This is known as dynamic binding or runtime polymorphism.

In this case, when animal1->makeSound() is called, the makeSound() function of the Dog class is invoked, and "The dog barks." is printed. Similarly, when animal2->makeSound() is called, the makeSound() function of the Cat class is invoked, and "The cat meows." is printed.

This example demonstrates how virtual functions allow us to treat objects of derived classes as objects of the base class, enabling the selection of the appropriate function implementation at runtime based on the actual object being referred to.

__Access Specifiers__

```c++
#include <iostream>

class MyClass
{
public:
    int publicVar; // Public variable

    void publicFunc()  // Public function
    {
        std::cout << "Public function called." << std::endl;
    }

private:
    int privateVar; // Private variable

    void privateFunc() // Private function
    {
        std::cout << "Private function called." << std::endl;
    }

protected:
    int protectedVar; // Protected variable

    void protectedFunc() // Protected function
    {
        std::cout << "Protected function called." << std::endl;
    }
};

int main()
{
    MyClass obj;
    
    obj.publicVar = 42;     // Accessible
    obj.publicFunc();       // Accessible

    // obj.privateVar = 42;  // Not accessible - private
    // obj.privateFunc();    // Not accessible - private

    // obj.protectedVar = 42;  // Not accessible - protected
    // obj.protectedFunc();    // Not accessible - protected

    return 0;
}
```

In this example, we have a class named MyClass that contains various class members with different access specifiers.

publicVar and publicFunc() are declared as public. They can be accessed from anywhere in the program, including the main() function. In the main() function, we can directly access and modify publicVar and call publicFunc().

privateVar and privateFunc() are declared as private. They are only accessible from within the class itself. Attempting to access them from outside the class or from the main() function will result in a compilation error.

protectedVar and protectedFunc() are declared as protected. They are accessible within the class itself and by derived classes. In this example, since there are no derived classes, attempting to access them from the main() function will result in a compilation error.

By using access specifiers, you can control the visibility and accessibility of class members, ensuring proper encapsulation and preventing unwanted modifications or access from outside the class.

__Overloading__

```c++
#include <iostream>

// Function with int parameter
void printNumber(int num)
{
    std::cout << "Integer number: " << num << std::endl;
}

// Function with double parameter
void printNumber(double num)
{
    std::cout << "Double number: " << num << std::endl;
}

// Function with string parameter
void printNumber(const std::string& str)
{
    std::cout << "String: " << str << std::endl;
}

int main()
{
    int intValue = 42;
    double doubleValue = 3.14;
    std::string stringValue = "Hello, world!";

    printNumber(intValue);        // Output: Integer number: 42
    printNumber(doubleValue);     // Output: Double number: 3.14
    printNumber(stringValue);     // Output: String: Hello, world!

    return 0;
}
```

In this example, we have three functions named printNumber that are overloaded based on the type of the parameter.

The first printNumber function takes an int parameter.
The second printNumber function takes a double parameter.
The third printNumber function takes a const std::string& parameter.
Inside the main() function, we have variables of different types: intValue (int), doubleValue (double), and stringValue (std::string).

When we call the printNumber function with these variables as arguments, the appropriate overloaded function is selected based on the parameter type. The matching function is then executed, and the corresponding output is printed.

----

__Destructor__

```c++
#include <iostream>

class MyClass
{
public:
    // Constructor
    MyClass()
    {
        std::cout << "Constructor called." << std::endl;
    }

    // Destructor
    ~MyClass()
    {
        std::cout << "Destructor called." << std::endl;
    }
};

int main()
{
    MyClass obj;  // Object creation

    // Other statements...

    return 0;
}

```

In this example, we have a class called MyClass that contains a constructor and a destructor.

The constructor is invoked when an object of the class is created. In the main() function, we create an object named obj of type MyClass. This triggers the constructor, and "Constructor called." is printed.

The destructor is a special member function that is automatically called when an object of the class goes out of scope or is explicitly destroyed. In this example, when the main() function ends, the obj object goes out of scope, and the destructor is called automatically. The destructor prints "Destructor called." before the object is destroyed.

When you run this program, the output will be:

```cmd
Constructor called.
Destructor called.
```

The destructor is useful for performing cleanup tasks, releasing resources, or finalizing operations before an object is destroyed. It is automatically called and cannot be explicitly invoked like a regular member function. The destructor name is the same as the class name, preceded by a tilde (~).

It's important to note that if you allocate an object dynamically using the new operator, you must manually deallocate it using the delete operator to ensure that the destructor is called before the object is destroyed.

----

## **Write a program in C++ to print the first non-repeated character in the given string.**

```c++
#include <iostream>
#include <unordered_map>

char findFirstNonRepeatedChar(const std::string& str)
{
    std::unordered_map<char, int> charCount;

    // Count the occurrences of each character
    for (char c : str)
    {
        charCount[c]++;
    }

    // Find the first non-repeated character
    for (char c : str)
    {
        if (charCount[c] == 1)
        {
            return c;
        }
    }

    // Return '\0' if no non-repeated character found
    return '\0';
}

int main()
{
    std::string str;
    std::cout << "Enter a string: ";
    std::getline(std::cin, str);

    char result = findFirstNonRepeatedChar(str);

    if (result != '\0')
    {
        std::cout << "First non-repeated character: " << result << std::endl;
    }
    else
    {
        std::cout << "No non-repeated character found." << std::endl;
    }

    return 0;
}
```

----

## **Write a program in C++ to print the first non-repeated character in the given string.**

```c++
#include <iostream>
#include <unordered_map>

char findFirstNonRepeatedChar(const std::string& str)
{
    std::unordered_map<char, int> charCount;

    // Count the occurrences of each character
    for (char c : str)
    {
        charCount[c]++;
    }

    // Find the first non-repeated character
    for (char c : str)
    {
        if (charCount[c] == 1)
        {
            return c;
        }
    }

    // Return '\0' if no non-repeated character found
    return '\0';
}

int main()
{
    std::string str;
    std::cout << "Enter a string: ";
    std::cin >> str;

    char result = findFirstNonRepeatedChar(str);

    if (result != '\0')
    {
        std::cout << "First non-repeated character: " << result << std::endl;
    }
    else
    {
        std::cout << "No non-repeated character found." << std::endl;
    }

    return 0;
}
```

---

## **Write a program in C++ to find duplicate numbers in a given array that contains multiple duplicates.**

```c++
#include <iostream>
#include <unordered_map>
#include <vector>

void findDuplicateNumbers(const std::vector<int>& arr)
{
    std::unordered_map<int, int> numCount;

    // Count the occurrences of each number
    for (int num : arr)
    {
        numCount[num]++;
    }

    // Find and print the duplicate numbers
    bool duplicatesFound = false;
    std::cout << "Duplicate numbers: ";
    for (const auto& pair : numCount)
    {
        if (pair.second > 1)
        {
            std::cout << pair.first << " ";
            duplicatesFound = true;
        }
    }

    if (!duplicatesFound)
    {
        std::cout << "None";
    }
    std::cout << std::endl;
}

int main()
{
    std::vector<int> arr = {1, 2, 3, 4, 5, 2, 4, 6, 4, 3};

    findDuplicateNumbers(arr);

    return 0;
}
```

----

## **Write a program to print the date in dd/mm/yy format.**

```c++
#include <iostream>
#include <ctime>

int main()
{
    // Get the current time
    std::time_t currentTime = std::time(nullptr);

    // Convert the time to a string representation
    std::tm* localTime = std::localtime(&currentTime);
    int day = localTime->tm_mday;
    int month = localTime->tm_mon + 1;
    int year = localTime->tm_year + 1900;

    // Print the date in the desired format
    std::cout << "Current date: ";
    if (day < 10)
    {
        std::cout << "0";
    }
    std::cout << day << "/";
    if (month < 10)
    {
        std::cout << "0";
    }
    std::cout << month << "/";
    std::cout << year % 100 << std::endl;

    return 0;
}
```

In this program, we use the <ctime> library to work with dates and times. The std::time_t data type represents the current time.

We get the current time using std::time(nullptr), which returns the number of seconds since the Unix epoch. We then convert this time to a std::tm structure using std::localtime(&currentTime).

The std::tm structure contains various members such as tm_mday (day of the month), tm_mon (month), and tm_year (years since 1900).

We extract the day, month, and year components from the std::tm structure and print them in the desired format: "dd/mm/yy".

When you run this program, it will print the current date in the "dd/mm/yy" format.

Note that the program assumes the local time zone. If you need to work with a different time zone or customize the date format further, you may need to use additional libraries or modify the code accordingly.

----

## **How would you check if a given linked list contains a cycle? Also, find the initial node of the cycle.**

```c++
struct ListNode
{
    int val;
    ListNode* next;
    ListNode(int x) : val(x), next(nullptr)
    {   
    }
};

ListNode* detectCycle(ListNode* head)
{
    ListNode* slow = head;
    ListNode* fast = head;

    // Step 1: Check if there's a cycle
    while (fast != nullptr && fast->next != nullptr)
    {
        slow = slow->next;
        fast = fast->next->next;
        if (slow == fast)
        {
            break; // Cycle detected
        }
    }

    // Step 2: Find the initial node of the cycle
    if (fast == nullptr || fast->next == nullptr)
    {
        return nullptr; // No cycle found
    }

    slow = head;
    while (slow != fast)
    {
        slow = slow->next;
        fast = fast->next;
    }

    return slow; // Return the initial node of the cycle
}
```

----

## **Write a program to reverse a singly linked list without recursion.**

```c++
#include <iostream>

struct ListNode
{
    int val;
    ListNode* next;
    
    ListNode(int x) : val(x), next(nullptr)
    {
    }
};

ListNode* reverseLinkedList(ListNode* head)
{
    ListNode* prev = nullptr;
    ListNode* current = head;
    ListNode* next = nullptr;

    while (current != nullptr)
    {
        next = current->next;   // Save the next node
        current->next = prev;   // Reverse the link
        prev = current;         // Move prev to the current node
        current = next;         // Move current to the next node
    }

    return prev;  // Return the new head of the reversed list
}

void printLinkedList(ListNode* head)
{
    ListNode* current = head;
    while (current != nullptr)
    {
        std::cout << current->val << " ";
        current = current->next;
    }
    std::cout << std::endl;
}

int main()
{
    // Create a sample linked list: 1 -> 2 -> 3 -> 4 -> 5
    ListNode* head = new ListNode(1);
    ListNode* second = new ListNode(2);
    ListNode* third = new ListNode(3);
    ListNode* fourth = new ListNode(4);
    ListNode* fifth = new ListNode(5);

    head->next = second;
    second->next = third;
    third->next = fourth;
    fourth->next = fifth;

    std::cout << "Original Linked List: ";
    printLinkedList(head);

    // Reverse the linked list
    ListNode* reversedHead = reverseLinkedList(head);

    std::cout << "Reversed Linked List: ";
    printLinkedList(reversedHead);

    return 0;
}
```

----

## **How would you implement a binary search tree?**

```c++
#include <iostream>

struct ListNode
{
    int val;
    ListNode* next;

    ListNode(int x) : val(x), next(nullptr)
    {
    }
};

ListNode* reverseLinkedList(ListNode* head)
{
    ListNode* prev = nullptr;
    ListNode* current = head;
    ListNode* next = nullptr;

    while (current != nullptr)
    {
        next = current->next;   // Save the next node
        current->next = prev;   // Reverse the link
        prev = current;         // Move prev to the current node
        current = next;         // Move current to the next node
    }

    return prev;  // Return the new head of the reversed list
}

void printLinkedList(ListNode* head)
{
    ListNode* current = head;
    while (current != nullptr)
    {
        std::cout << current->val << " ";
        current = current->next;
    }
    std::cout << std::endl;
}

int main()
{
    // Create a sample linked list: 1 -> 2 -> 3 -> 4 -> 5
    ListNode* head = new ListNode(1);
    ListNode* second = new ListNode(2);
    ListNode* third = new ListNode(3);
    ListNode* fourth = new ListNode(4);
    ListNode* fifth = new ListNode(5);

    head->next = second;
    second->next = third;
    third->next = fourth;
    fourth->next = fifth;

    std::cout << "Original Linked List: ";
    printLinkedList(head);

    // Reverse the linked list
    ListNode* reversedHead = reverseLinkedList(head);

    std::cout << "Reversed Linked List: ";
    printLinkedList(reversedHead);

    return 0;
}
```

----

## **Write a program to traverse a given binary tree in preorder without recursion.**

```c++
#include <iostream>
#include <stack>

struct TreeNode
{
    int val;
    TreeNode* left;
    TreeNode* right;

    TreeNode(int x) : val(x), left(nullptr), right(nullptr) {}
};

void preorderTraversal(TreeNode* root)
{
    if (root == nullptr)
    {
        return;
    }

    std::stack<TreeNode*> stack;
    stack.push(root);

    while (!stack.empty())
    {
        TreeNode* node = stack.top();
        stack.pop();
        std::cout << node->val << " ";

        if (node->right != nullptr)
        {
            stack.push(node->right);
        }

        if (node->left != nullptr)
        {
            stack.push(node->left);
        }
    }
}

int main()
{
    // Create a sample binary tree
    TreeNode* root = new TreeNode(1);
    root->left = new TreeNode(2);
    root->right = new TreeNode(3);
    root->left->left = new TreeNode(4);
    root->left->right = new TreeNode(5);
    root->right->left = new TreeNode(6);
    root->right->right = new TreeNode(7);

    // Perform preorder traversal
    std::cout << "Preorder Traversal: ";
    preorderTraversal(root);
    std::cout << std::endl;

    return 0;
}
```

----

## **How would you implement a merge sort algorithm?**

```c++
#include <iostream>
#include <vector>

// Merge two sorted subarrays into one sorted array
void merge(std::vector<int>& arr, int left, int mid, int right)
{
    int n1 = mid - left + 1; // Size of the left subarray
    int n2 = right - mid; // Size of the right subarray

    // Create temporary arrays to hold the subarrays
    std::vector<int> leftArray(n1);
    std::vector<int> rightArray(n2);

    // Copy data from the original array to the temporary arrays
    for (int i = 0; i < n1; ++i)
    {
        leftArray[i] = arr[left + i];
    }
    for (int j = 0; j < n2; ++j)
    {
        rightArray[j] = arr[mid + 1 + j];
    }

    // Merge the two sorted subarrays back into the original array
    int i = 0;      // Index of the left subarray
    int j = 0;      // Index of the right subarray
    int k = left;   // Index of the merged array

    while (i < n1 && j < n2)
    {
        if (leftArray[i] <= rightArray[j])
        {
            arr[k] = leftArray[i];
            ++i;
        }
        else
        {
            arr[k] = rightArray[j];
            ++j;
        }
        ++k;
    }

    // Copy any remaining elements from the left subarray
    while (i < n1)
    {
        arr[k] = leftArray[i];
        ++i;
        ++k;
    }

    // Copy any remaining elements from the right subarray
    while (j < n2)
    {
        arr[k] = rightArray[j];
        ++j;
        ++k;
    }
}

// Recursive function to perform merge sort
void mergeSort(std::vector<int>& arr, int left, int right)
{
    if (left < right)
    {
        int mid = left + (right - left) / 2;

        // Sort the left and right halves recursively
        mergeSort(arr, left, mid);
        mergeSort(arr, mid + 1, right);

        // Merge the sorted halves
        merge(arr, left, mid, right);
    }
}

// Helper function to print the elements of an array
void printArray(const std::vector<int>& arr)
{
    for (int i = 0; i < arr.size(); ++i)
    {
        std::cout << arr[i] << " ";
    }
    std::cout << std::endl;
}

int main()
{
    std::vector<int> arr = {5, 2, 8, 12, 3, 9, 1, 7};
    std::cout << "Original Array: ";
    printArray(arr);

    mergeSort(arr, 0, arr.size() - 1);

    std::cout << "Sorted Array: ";
    printArray(arr);

    return 0;
}
```

----

## **How do I prepare for C++ interview questions and answers?**

You should begin your preparation by brushing up on core programming concepts and move on to practicing programming problems. You can also enroll in mock interviews and practice mocks with hiring managers who are closely acquainted with the FAANG companies' interview process. Learn important tips on how to prepare for C++ interviews here.

----

## **What topics are important for C++ interview questions and answers?**

You should be prepared for questions on crucial C++ concepts, including methods, events in C++, lists, inheritance, polymorphism, abstraction, data binding, and commands to crack the most challenging C++ interview questions and answers.

----

## **Can I use C++ for the FAANG company's coding interviews?**

Yes, you can use C++ in coding interview rounds. Top tech companies, including Microsoft, LinkedIn, PayPal, and Amazon, list C++ as one of their main programming languages for coding interviews. C++ has become one of the most sought-after skills in modern developers at FAANG+ companies. 

----

## **What positions am I eligible for with C++ programming skills?**

You can make a career in the following roles with C++ programming skills: Junior/Senior Programmer, Software Developer, Quality Analyst, Game Programmer, Software Developer Engineer, C++ Analyst, and Programming Architect.

----

## **What is the average salary of C++ developers in the US?**

The average base salary of a C++ developer is $116,987 per annum in the United States. You can expect a higher salary in US cities like Orlando, New York, and San Francisco (Source: Indeed.com). The salary increases according to your experience and based on your performance. The higher the experience, the higher the salary will be.

‍# https://www.interviewkickstart.com/interview-questions/cpp-interview-questions-for-experienced-developers/

# https://www.softwaretestinghelp.com/cpp-interview-questions/

## **What is the basic structure of a C++ program?**

The basic structure of a C++ program is shown below:

```c++
#include<iostream.h>

int main()
{
    cout<<”Hello,World!”;
    return 0;
}
```

The first line that begins with “#” is a preprocessor directive. In this case, we are using include as a directive which tells the compiler to include a header while “iostream.h” will be used for basic input/output later in the program.

The next line is the “main” function that returns an integer. The main function is the starting point of execution for any C++ program. Irrespective of its position in the source code file, the contents of the main function are always executed first by the C++ compiler.

In the next line, we can see open curly braces that indicate the start of a block of code. After this, we see the programming instruction or the line of code that uses the count which is the standard output stream (its definition is present in iostream.h).

This output stream takes a string of characters and prints it to a standard output device. In this case, it is, “Hello, World!”. Please note that each C++ instruction ends with a semicolon (;), which is very much necessary, and omitting it will result in compilation errors.

Before closing the curly braces, we see another line “return 0;”. This is the returning point to the main function.

Every C++ program will have a basic structure as shown above with a preprocessor directive, the main function declaration followed by a block of code, and then a returning point to the main function which indicates successful execution of the program.

----

## **What are the Comments in C++?**

Comments in C++ are simply a piece of source code ignored by the compiler. They are only helpful for a programmer to add a description or additional information about their source code.

In C++ there are two ways to add comments:

```c++
//single-line comment
```

```c++
/* block comment */
```

The first type will discard everything after the compiler encounters “//”. In the second type, the compiler discards everything between “/*” and “*/”.

----

## **Difference between Declaration and Definition of a variable?**

The declaration of a variable is merely specifying the data type of a variable and the variable name. As a result of the declaration, we tell the compiler to reserve the space for a variable in the memory according to the data type specified.

Example:

```c++
int result;
char c;
int a,b,c;
```

All the above are valid declarations. Also, note that as a result of the declaration, the value of the variable is undetermined.

Whereas, a definition is an implementation/instantiation of the declared variable where we tie up appropriate value to the declared variable so that the linker will be able to link references to the appropriate entities.

From the above Example,

```c++
result = 10;
C = 'A';
```

These are valid definitions.

----

## **Comment on the Local and Global scope of a variable?**

Answer: The scope of a variable is defined as the extent of the program code within which the variable remains active i.e. it can be declared, defined, or worked with.

There are two types of scope in C++:

*Local Scope:* A variable is said to have a local scope or is local when it is declared inside a code block. The variable remains active only inside the block and is not accessible outside the code block.

*Global Scope:* A variable has a global scope when it is accessible throughout the program. A global variable is declared on top of the program before all the function definitions.

Example:

```c++
#include <iostream.h>

int globalResult = 0; //global variable

int main()
{
    int localVar = 10; //local variable. 
}
```

----

## **What is the precedence when there are a Global variable and a Local variable in the program with the same name?**

Whenever there is a local variable with the same name as that of a global variable, the compiler gives precedence to the local variable.

```c++
#include <iostream.h>

int globalVar = 2;

int main()
{
    int globalVar = 5;
    cout << globalVar << endl;
}
```

The output of the above code is 5. This is because, although both the variables have the same name, the compiler has given preference to the local scope.

----

## **When there are a Global variable and a Local variable with the same name, how will you access the global variable?**

When there are two variables with the same name but different scopes, i.e. one is a local variable and the other is a global variable, the compiler will give preference to a local variable.

In order to access the global variable, we make use of a “scope resolution operator (::)”. Using this operator, we can access the value of the global variable.

Example:

```c++
#include<iostream.h>

int x= 10;

int main()
{
    int x = 2;
    cout << "Global Variable x = " << ::x;
    cout << "\nlocal Variable x = " << x;
}

// Output:
// Global Variable x = 10
// local Variable x = 2
```

----

## **How many ways are there to initialize an int with a Constant?**

There are two ways:

The first format uses traditional C notation.

```c++
int result = 10;
```

The second format uses the constructor notation.

```c++
int result (10);
```

----

## **What is a Constant? Explain with an example?**

A constant is an expression that has a fixed value. They can be divided into integer, decimal, floating-point, character, or string constants depending on their data type.

Apart from the decimal, C++ also supports two more constants i.e. octal (to the base 8) and hexadecimal (to the base 16) constants.

Examples of Constants:

```c++
75 // integer (decimal)
0113 // octal
0x4b // hexadecimal
3.142 // floating point
'c' // character constant
"Hello, World" // string constant
```

Note: When we have to represent a single character, we use single quotes and when we want to define a constant with more than one character, we use double quotes.

----

## **How do you define/declare constants in C++?**

In C++, we can define our own constants using the #define preprocessor directive.

```c++
#define Identifier value

#include<iostream.h>
#define PI 3.142

int main ()
{
    float radius =5, area;
    area = PI * r * r;
    cout<<”Area of a Circle = “<<area;
}

// Output: Area of a Circle = 78.55
```

As shown in the above example, once we define a constant using #define directive, we can use it throughout the program and substitute its value.

We can declare constants in C++ using the “const” keyword. This way is similar to that of declaring a variable, but with a const prefix.

Examples of declaring a constant

```c++
const int pi = 3.142;
const char c = “sth”;
const zipcode = 411014;
```

In the above examples, whenever the type of a constant is not specified, the C++ compiler defaults it to an integer type.

----

## **Comment on Assignment Operator in C++?**

The assignment operator in C++ is used to assign a value to another variable.

```c++
a = 5;
```

This line of code assigns the integer value 5 to variable a.

The part at the left of the =operator is known as an lvalue (left value) and the right as rvalue (right value). Lvalue must always be a variable whereas the right side can be a constant, a variable, the result of an operation, or any combination of them.

The assignment operation always takes place from the right to left and never at the inverse.

One property which C++ has over the other programming languages is that the assignment operator can be used as the rvalue (or part of an rvalue) for another assignment.

```c++
int a, b;
a = 2 + (b = 5);
```

is equivalent to:

```c++
b = 5;
a = 2 + b;
```

This means, first assign 5 to variable b and then assign to a, the value 2 plus the result of the previous expression of b(that is 5), leaving a with a final value of 7.

Thus, the following expression is also valid in C++:

```c++
a = b = c = 5;
```

assign 5 to variables a, b and c.

----

## **What is the difference between equal to (==) and Assignment Operator (=)?**

In C++, equal to (==) and assignment operator (=) are two completely different operators.

Equal to (==) is an equality relational operator that evaluates two expressions to see if they are equal and returns true if they are equal and false if they are not.

The assignment operator (=) 

is used to assign a value to a variable. Hence, we can have a complex assignment operation inside the equality relational operator for evaluation.

----

## **What are the various Arithmetic Operators in C++?**

C++ supports the following arithmetic operators:

+ addition
– subtraction
* multiplication
/ division
% module

Let’s demonstrate the various arithmetic operators with the following piece of code:

```c++
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

// Output:
// a + b = 8
// a – b =2
// a * b =15
// a / b =2
// a % b=1
```

As shown above, all the other operations are straightforward and the same as actual arithmetic operations, except the modulo operator which is quite different. Modulo operator divides a and b and the result of the operation is the remainder of the division.

----

## **What are the various Compound Assignment Operators in C++?**

Following are the Compound assignation operators in C++:

+=, -=, *=, /=, %=, >>=, <<=, &=, ^=,|=

The compound assignation operator is one of the most  important features of C++ language which allow us to change the value of a variable with one of the basic operators:

```c++
value += increase; // is equivalent to ...
value = value + increase;
```

if base_salary is a variable of type int.

```c++
int base_salary = 1000;
base_salary += 1000; #base_salary = base_salary + 1000
base_salary *= 5; #base_salary = base_salary * 5;
```

----

## **State the difference between Pre and Post Increment/Decrement Operations?**

C++ allows two operators i.e ++ (increment) and –(decrement), that allow you to add 1 to the existing value of a variable and subtract 1 from the variable respectively. These operators are in turn, called increment (++) and decrement (–).

Example:

```c++
a = 5;
a++;
```

The second statement, a++, will cause 1 to be added to the value of a. Thus a++ is equivalent to

```c++
a = a+1; or
a += 1;
```

A unique feature of these operators is that we can prefix or suffix these operators with the variable. Hence, if a is a variable and we prefix the increment operator it will be

```c++
++a;
```

This is called Pre-increment. Similarly, we have pre-decrement as well.

If we prefix the variable a with an increment operator, we will have,

```c++
a++;
```

This is the post-increment. Likewise, we have post-decrement too.

The difference between the meaning of pre and post depends upon how the expression is evaluated and the result is stored.

In the case of the pre-increment/decrement operator, the increment/decrement operation is carried out first, and then the result is passed to an lvalue. Whereas for post-increment/decrement operations, the lvalue is evaluated first and then increment/decrement is performed accordingly.

Example:

```c++
a = 5; b=6;
++a; // a=6
b–; // b=6
–a; // #a=5
b++; // #6
```

----

## **What are the Extraction and Insertion operators in C++? Explain with examples?**

In the iostream.h library of C++, cin, and cout is the two data streams that are used for input and output respectively. Cout is normally directed to the screen and cin is assigned to the keyboard.

*“cin”* (extraction operator): By using overloaded operator >> with cin stream, C++ handles the standard input.

```c++
int age;
cin >> age;
```

As shown in the above example, an integer variable ‘age’ is declared and then it waits for cin (keyboard) to enter the data. “cin” processes the input only when the RETURN key is pressed.

*“cout”* (insertion operator): This is used in conjunction with the overloaded << operator. It directs the data that followed it into the cout stream.

Example:

```c++
cout << ”Hello, World!”;
cout << 123;
// Control Structures And Functions
// Control Structures And Loops
```

----

## **What is the difference between a while and a do while loop? Explain with examples?**

The format of the while loop in C++ is:

```c++
While (expression)
{
    statements;
}

```

The statement block under while is executed as long as the condition in the given expression is true.

Example:

```c++
#include <iostream.h>
int main()
{
    int n;
    cout << "Enter the number : ";
    cin>>n;
    while(n>0)
    {
        cout << " " << n;
        --n;
    }
    cout << "While loop complete";
}
```

In the above code, the loop will directly exit if n is 0. Thus in the while loop, the terminating condition is at the beginning of the loop and if it’s fulfilled, no iterations of the loop are executed.

Next, we consider the do-while loop.

The general format of do-while is:

do {statement;} while(condition);

Example:

```c++
#include <iostream.h>

int main()
{
    int n;
    cout << "Enter the number : " << endl;
    cin >> n;
    
    do
    {
        cout << n << "," << endl;
        --n;
    }
    while (n > 0);
    
    cout << "do - while complete";
}
```

In the above code, we can see that the statement inside the loop is executed at least once as the loop condition is at the end. These are the main differences between the while and the do-while.

In the case of the while loop, we can directly exit the loop at the beginning, if the condition is not met whereas in the do-while loop we execute the loop statements at least once.

----

## **What do you mean by 'void' return type?**

All functions should return a value as per the general syntax.

However, in case, if we don’t want a function to return any value, we use “void” to indicate that. This means that we use “void” to indicate that the function has no return value or it returns “void”.

Example:

```c++
void myfunc()
{
    cout << "Hello, This is my function!!" << endl;
}

int main()
{
    myfunc();
    return 0;
}
```

----

## **Explain Pass by Value and Pass by Reference?**

While passing parameters to the function using “Pass by Value”, we pass a copy of the parameters to the function.

Hence, whatever modifications are made to the parameters in the called function are not passed back to the calling function. Thus the variables in the calling function remain unchanged.

Example:

```c++
void printFunc(int a, int b, int c)
{
    a *= 2;
    b *= 2;
    c *= 2;
}

int main()
{
    int x = 1, y = 3, z = 4;
    printFunc(x, y, z);
    cout << "x = " << x << "\ny = " << y << "\nz = " << z;
}

// Output:
// x=1
// y=3
// z=4
```

As seen above, although the parameters were changed in the called function, their values were not reflected in the calling function as they were passed by value.

However, if we want to get the changed values from the function back to the calling function, then we use the “Pass by Reference” technique.

To demonstrate this we modify the above program as follows:

```c++
void printFunc(int& a, int& b, int& c)
{
    a *= 2;
    b *= 2;
    c *= 2;
}

int main()
{
    int x = 1, y = 3, z = 4;
    printFunc(x, y, z);
    cout << "x = " << x << "\ny = " << y << "\nz = " << z;
}

// Output:
// x=2
// y=6
// z=8
```

As shown above, the modifications done to the parameters in the called functions are passed to the calling function when we use the “Pass by reference” technique. This is because using this technique we do not pass a copy of the parameters but we actually pass the variable’s reference itself.

----

## **What are Default Parameters? How are they evaluated in the C++ function?**

A default Parameter is a value that is assigned to each parameter while declaring a function.

This value is used if that parameter is left blank while calling the function. To specify a default value for a particular parameter, we simply assign a value to the parameter in the function declaration.

If the value is not passed for this parameter during the function call, then the compiler uses the default value provided. If a value is specified, then this default value is stepped on and the passed value is used.

Example:

```c++
int multiply(int a, int b = 2)
{
    int r;
    r = a * b;
    return r;
}

int main()
{
    cout << multiply(6) << endl;
    cout << "\n" << endl;
    cout << multiply(2, 3) << endl;
}

// Output:
// 12
// 6
```

As shown in the above code, there are two calls to the multiply function. In the first call, only one parameter is passed with a value. In this case, the second parameter is the default value provided. But in the second call, as both the parameter values are passed, the default value is overridden and the passed value is used.

----

## **What is an Inline function in C++?**

Inline function is a function that is compiled by the compiler as the point of calling the function and the code is substituted at that point. This makes compiling faster. This function is defined by prefixing the function prototype with the keyword “inline”.

Such functions are advantageous only when the code of the inline function is small and simple. Although a function is defined as Inline, it is completely compiler dependent to evaluate it as inline or not.

Advanced-Data Structure
Arrays

----

## **Why are arrays usually processed with for loop?**

Array uses the index to traverse each of its elements.

If A is an array then each of its elements is accessed as A[i]. Programmatically, all that is required for this to work is an iterative block with a loop variable i that serves as an index (counter) incrementing from 0 to A.length-1.

This is exactly what a loop does and this is the reason why we process arrays using for loops.

----

## **State the difference between delete and delete[]?**

“delete[]” is used to release the memory allocated to an array that was allocated using new[]. “delete” is used to release one chunk of memory which was allocated using new.

----

## **What is wrong with this code?**

```c++
T *p = new T[10];
delete p;
```

The above code is syntactically correct and will compile fine.

The only problem is that it will just delete the first element of the array. Though the entire array is deleted, only the destructor of the first element will be called and the memory for the first element is released.

----

## **What's the order in which the objects in an array are destructed?**

Objects in an array are destructed in the reverse order of construction: First constructed, last destructed.

In the following Example, the order for destructors will be a[9], a[8], …, a[1], a[0]:

```c++
voiduserCode()
{
    Car a[10];
    ...
}
```

----

## **What is wrong with this code?**

```c++
T *p = 0;
delete p;
```

In the above code, the pointer is a null pointer. Per the C++ 03 standard, it’s perfectly valid to call delete on a NULL pointer. The delete operator would take care of the NULL check internally.

----

## **What is a Reference Variable in C++?**

A reference variable is an alias name for the existing variable. This means that both the variable name and the reference variable point to the same memory location. Hence, whenever the variable is updated, the reference is updated too.

Example:

```c++
int a=10;
int& b = a;
```

Here, b is the reference of a.

Suggested reading =>> Most Common Data Structure Interview Questions

----

## **What is a Storage Class? Mention the Storage Classes in C++?**

Storage class determines the life or scope of symbols such as variables or functions.

C++ supports the following storage classes:
- Auto
- Static
- Extern
- Register
- Mutable

----

## **Explain the Mutable Storage class specifier?**

The variable of a constant class object’s member cannot be changed. However, by declaring the variables as “mutable”, we can change the values of these variables.

----

## **What is the keyword auto for?**

By default, every local variable of the function is automatic i.e. auto. In the below function both the variables ‘i’ and ‘j’ are automatic variables.

```c++
void f()
{
    int i; 
    auto int j;
}
 ```
 
NOTE: A global variable is not an automatic variable.

----

## **What is a Static Variable?**

A static variable is a local variable that retains its value across the function calls. Static variables are declared using the keyword “static”. Numeric variables which are static have the default value as zero.

The following function will print 1 2 3 if called thrice.

```c++
void f()
{
    static int i;
    ++i;
    printf(" % d ", i);
}

int main()
{
    f();
}
```

If a global variable is static, then its visibility is limited to the same source code.

----

## **What is the purpose of the Extern Storage Specifier?**

"Extern" specifier is used to resolve the scope of a global symbol.

```c++
#include <iostream>

using namespace std;

main()
{
    extern int i;
    cout << i << endl;
}
int i = 20;
```
 
In the above code, "i" can be visible outside the file where it is defined.

----

## **Explain Register Storage Specifier?**

"Register" variable should be used whenever the variable is used. When a variable is declared with a “register” specifier, then the compiler gives a CPU register for its storage to speed up the lookup of the variable.

----

## **When to use "const" reference arguments in a function?**

Using "const" reference arguments in a function is beneficial in several ways:

"const" protects from programming errors that could alter data.
As a result of using “const”, the function is able to process both const and non-const actual arguments, which is not possible when “const” is not used.
Using a const reference will allow the function to generate and use a temporary variable in an appropriate manner.
Structure & User-Defined Data Types

```c++
#include <iostream>

void printValue(const int& value)
{
    std::cout << "Value: " << value << std::endl;
}

void modifyValue(int& value)
{
    value = 10;  // Modifying the passed object
}

int main()
{
    int x = 5;

    printValue(x);       // Passing a non-const reference
    printValue(10);      // Passing a temporary (rvalue)

    modifyValue(x);      // Modifying the object

    const int y = 3;
    printValue(y);       // Passing a const reference

    return 0;
}
```

----

## **What is a Class?**

Class is a user-defined data type in C++. It can be created to solve a particular kind of problem. After creation, the user is not required to know the details of the working of a class.

In general, class acts as a blueprint of a project and can include various parameters and functions or actions operating on these parameters. These are called the members of the class.

```c++
#include <iostream>

class Person
{
private:
    std::string name;
    int age;

public:
    Person(const std::string& personName, int personAge) : name(personName), age(personAge)
    {
    }

    void setName(const std::string& newName)
    {
        name = newName;
    }

    void setAge(int newAge)
    {
        age = newAge;
    }

    std::string getName() const
    {
        return name;
    }

    int getAge() const
    {
        return age;
    }

    void displayInfo() const
    {
        std::cout << "Name: " << name << ", Age: " << age << std::endl;
    }
};

int main()
{
    Person person("John Doe", 25);
    person.displayInfo(); // Output: Name: John Doe, Age: 25

    person.setName("Jane Smith");
    person.setAge(30);
    person.displayInfo(); // Output: Name: Jane Smith, Age: 30

    std::string name = person.getName();
    int age = person.getAge();
    std::cout << "Retrieved Info - Name: " << name << ", Age: " << age << std::endl;

    return 0;
}
```

----

## **Difference between Class and Structure?**

__Structure:__ In C language, the structure is used to bundle different types of data types together. The variables inside a structure are called the members of the structure. These members are by default public and can be accessed by using the structure name followed by a dot operator and then the member name.

```c++
#include <iostream>

struct Person
{
    std::string name;
    int age;
    std::string address;
};

int main()
{
    Person person1;
    person1.name = "John Doe";
    person1.age = 25;
    person1.address = "123 Main Street";

    std::cout << "Person 1 - Name: " << person1.name << ", Age: " << person1.age << ", Address: " << person1.address << std::endl;

    Person person2 = { "Jane Smith", 30, "456 Elm Street" };
    std::cout << "Person 2 - Name: " << person2.name << ", Age: " << person2.age << ", Address: " << person2.address << std::endl;

    return 0;
}
```

__Class:__ Class is a successor of the Structure. C++ extends the structure definition to include the functions that operate on its members. By default all the members of the class are private.

Object-Oriented Programming With C++
Classes, Constructors, Destructors

```c++
class Person
{
private:
    std::string name;
    int age;

public:
    Person(const std::string& personName, int personAge) : name(personName), age(personAge)
    {
    }

    void setName(const std::string& newName)
    {
        name = newName;
    }

    void setAge(int newAge)
    {
        age = newAge;
    }

    std::string getName() const
    {
        return name;
    }

    int getAge() const
    {
        return age;
    }

    void displayInfo() const
    {
        std::cout << "Name: " << name << ", Age: " << age << std::endl;
    }
};
```

----

## **What is Namespace?**

Namespace allows us to group a set of global classes, objects, and/or functions under a specific name.

The general form to use namespaces is:

namespace identifier { namespace-body }

Where identifier is any valid identifier and the namespace-body is the set of classes, objects, and functions that are included within the namespace. Namespaces are especially useful in cases where there is a possibility for more than one object to have the same name, resulting in name clashes.

```c++
#include <iostream>

namespace MyNamespace
{
    void sayHello()
    {
        std::cout << "Hello from MyNamespace!" << std::endl;
    }
}

using namespace MyNamespace;

int main()
{
    sayHello(); // Output: Hello from MyNamespace!

    return 0;
}
```

----

## **What is the use of a 'using' declaration?**

Answer: Using Declaration is used to refer to a name from the namespace without the scope resolution operator.

----

## **What is Name Mangling?**

C++ compiler encodes the parameter types with function/method into a unique name. This process is called name mangling. The inverse process is called demangling.

A::b(int, long) const is mangled as ‘b__C3Ail’.

For a constructor, the method name is left out.

That is A:: A(int, long) const is mangled as ‘C3Ail’.

----

## **What is the difference between an Object and a Class?**

Class is a blueprint of a project or problem to be solved and consists of variables and methods. These are called the members of the class. We cannot access methods or variables of the class on its own unless they are declared static.

In order to access the class members and put them to use, we should create an instance of a class which is called an Object. The class has an unlimited lifetime whereas an object has a limited lifespan only.

Example:

```c++
#include <iostream>

void foo(int x)
{
    std::cout << "Called foo(int) with value: " << x << std::endl;
}

void foo(double x)
{
    std::cout << "Called foo(double) with value: " << x << std::endl;
}

int main()
{
    foo(10);       // Calls foo(int)
    foo(3.14);     // Calls foo(double)

    return 0;
}
```

----

## **What are the various Access Specifiers in C++?**

++ supports the following access specifiers:

*Public:* Data members and functions are accessible outside the class.
*Private:* Data members and functions are not accessible outside the class. The exception is the usage of a friend class.
*Protected:* Data members and functions are accessible only to the derived classes.

Example:

Describe PRIVATE, PROTECTED, and PUBLIC along with their differences and give examples.

```c++
class A
{
    int x; int y;
    public int a;
    protected bool flag;
    public A() : x(0) , y(0) {} // default (no argument) constructor
};

main()
{
    A MyObj;
    MyObj.x = 5; // Compiler will issue a ERROR as x is private
    int x = MyObj.x; // Compiler will issue a compile ERROR MyObj.x is private
    MyObj.a = 10; // no problem; a is public member
    int col = MyObj.a; // no problem
    MyObj.flag = true; // Compiler will issue a ERROR; protected values are read only
    bool isFlag = MyObj.flag; // no problem
}
```

----

## **What is a Constructor and what is it called?**

Constructor is a member function of the class having the same name as the class. It is mainly used for initializing the members of the class. By default constructors are public.

There are two ways in which the constructors are called:

*Implicitly:* Constructors are implicitly called by the compiler when an object of the class is created. This creates an object on a Stack.
*Explicit Calling:* When the object of a class is created using new, constructors are called explicitly. This usually creates an object on a Heap.

Example:

```c++
class 
{
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
```

----

## **What is a COPY CONSTRUCTOR and when is it called?**

A copy constructor is a constructor that accepts an object of the same class as its parameter and copies its data members to the object on the left part of the assignment. It is useful when we need to construct a new object of the same class.

Example:

```c++
class A
{
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
```

----

## **What is a Default Constructor?**

A default constructor is a constructor that either has no arguments or if there are any, then all of them are default arguments.

Example:

```c++
// TestApplication.cpp : Example of function overriding.
//

using namespace std;

class B
{
    public: B(int m = 0) : n(m) {} int n;
};

int main(int argc, char* argv[])
{
    B b; return 0;
}
```

----
 
*## *What is a Conversion Constructor?**

It is a constructor that accepts one argument of a different type. Conversion constructors are mainly used for converting from one type to another.

```c++
#include <iostream>

class Distance {
private:
    double meters;

public:
    Distance(double m) : meters(m)
    {
    }

    double getMeters() const
    {
        return meters;
    }
};

class Speed {
private:
    double metersPerSecond;

public:
    Speed(const Distance& distance, double time)
    {
        metersPerSecond = distance.getMeters() / time;
    }

    double getMetersPerSecond() const
    {
        return metersPerSecond;
    }
};

int main() {
    Distance dist(1000.0); // Distance object
    Speed speed = dist; // Implicit conversion using conversion constructor

    std::cout << "Speed: " << speed.getMetersPerSecond() << " m/s" << std::endl;

    return 0;
}
```

----

## **What is an Explicit Constructor?**

A conversion constructor is declared with the explicit keyword. The compiler does not use an explicit constructor to implement an implied conversion of types. Its purpose is reserved explicitly for construction.

```c++
#include <iostream>

class MyNumber
{
private:
    int value;

public:
    explicit MyNumber(int val) : value(val)
    {
    }

    int getValue() const
    {
        return value;
    }
};

void printNumber(const MyNumber& num)
{
    std::cout << "Number: " << num.getValue() << std::endl;
}

int main()
{
    int intValue = 42;
    MyNumber myNum(intValue);  // Explicit construction
    printNumber(myNum);

    // Implicit conversion prevented by the 'explicit' keyword
    // MyNumber myNum2 = intValue;  // Compilation error

    return 0;
}
```

----

## **What is the role of the Static keyword for a class member variable?**

The static member variable shares a common memory across all the objects created for the respective class. We need not refer to the static member variable using an object. However, it can be accessed using the class name itself.

----

## **Explain the Static Member Function?**

A static member function can access only the static member variable of the class. Same as the static member variables, a static member function can also be accessed using the class name.

```c++
#include <iostream>

class MathUtils
{
public:
    // static member function
    static int add(int a, int b)
    {
        return a + b;
    }
};

int main()
{
    int sum = MathUtils::add(3, 4); // access via the scope resolution operator
    std::cout << "Sum: " << sum << std::endl; 
    return 0;
}

// Output:
// Sum: 7

```

----

## **What’s the order in which the local objects are destructed?**

Consider following a piece of code:

```c++
Class A
{
    // Do something 
};

int main()
{
    A a; // Destructor secondly
    A b; // Destructor will be called first
}
```

In the main function, we have two objects created one after the other. They are created in order, first a then b.

But when these objects are deleted or if they go out of scope, the destructor for each will be called in the reverse order in which they were constructed.

Hence, the destructor of b will be called first followed by a. Even if we have an array of objects, they will be destructed in the same way in the reverse order of their creation.

----

## **Explain Function Overloading and Operator Overloading?**

C++ supports OOPs concept Polymorphism which means “many forms”.

In C++ we have two types of polymorphism, i.e. Compile-time polymorphism, and Run-time polymorphism. Compile-time polymorphism is achieved by using an Overloading technique. Overloading simply means giving additional meaning to an entity by keeping its base meaning intact.

C++ supports two types of overloading:

__Function Overloading:__

Function overloading is a technique that allows the programmer to have more than one function with the same name but a different parameter list. In other words, we overload the function with different arguments i.e. be it the type of arguments, number of arguments, or the order of arguments.

Function overloading is never achieved on its return type.

__Operator Overloading:__

This is yet another type of compile-time polymorphism that is supported by C++. In operator overloading, an operator is overloaded, so that it can operate on the user-defined types as well as the operands of the standard data type. But while doing this, the standard definition of that operator is kept intact.

For Example, an Addition operator (+) that operates on numerical data types can be overloaded to operate on two objects just like an object of a complex number class.

----

## **What is the difference between Method Overloading and Method Overriding in C++?**

*Method overloading* is having functions with the same name but different argument lists. This is a form of compile-time polymorphism.

```c++
#include <iostream>

class Calculator
{
public:
    int add(int a, int b)
    {
        return a + b;
    }

    double add(double a, double b)
    {
        return a + b;
    }

    int add(int a, int b, int c)
    {
        return a + b + c;
    }
};

int main()
{
    Calculator calc;

    int sum1 = calc.add(3, 4);
    std::cout << "Sum1: " << sum1 << std::endl;  // Output: Sum1: 7

    double sum2 = calc.add(2.5, 3.7);
    std::cout << "Sum2: " << sum2 << std::endl;  // Output: Sum2: 6.2

    int sum3 = calc.add(1, 2, 3);
    std::cout << "Sum3: " << sum3 << std::endl;  // Output: Sum3: 6

    return 0;
}
```

*Method overriding* comes into the picture when we rewrite the method that is derived from a base class. Method overriding is used while dealing with run-time polymorphism or virtual functions.

```c++
#include <iostream>

class Calculator
{
public:
    int add(int a, int b)
    {
        return a + b;
    }

    double add(double a, double b)
    {
        return a + b;
    }

    int add(int a, int b, int c)
    {
        return a + b + c;
    }
};

int main()
{
    Calculator calc;

    int sum1 = calc.add(3, 4);
    std::cout << "Sum1: " << sum1 << std::endl;  // Output: Sum1: 7

    double sum2 = calc.add(2.5, 3.7);
    std::cout << "Sum2: " << sum2 << std::endl;  // Output: Sum2: 6.2

    int sum3 = calc.add(1, 2, 3);
    std::cout << "Sum3: " << sum3 << std::endl;  // Output: Sum3: 6

    return 0;
}
```

----

## **What is the difference between a Copy Constructor and an Overloaded Assignment Operator?**

A copy constructor and an overloaded assignment operator basically serve the same purpose i.e. assigning the content of one object to another. But still, there is a difference between the two.

Example:

```c++
complex c1, c2;
c1=c2; // this is assignment
complex c3=c2; // copy constructor
```

In the above example, the second statement c1 = c2 is an overloaded assignment statement.

Here, both c1 and c2 are already existing objects and the contents of c2 are assigned to the object c1. Hence, for an overloaded assignment statement both the objects need to be created already.

Next statement, complex c3 = c2 is an example of the copy constructor. Here, the contents of c2 are assigned to a new object c3, which means the copy constructor creates a new object every time when it executes.

----

## **Name the Operators that cannot be Overloaded?**

```c++
sizeof – sizeof operator
. – Dot operator
.* – dereferencing operator
-> – member dereferencing operator
:: – scope resolution operator
?: – conditional operator
```

----

## **Function can be overloaded based on the parameter which is a value or a reference. Explain if the statement is true?**

False. Both, Passing by value and Passing by reference look identical to the caller.

----

## **What are the benefits of Operator Overloading?**

By overloading standard operators on a class, we can extend the meaning of these operators, so that they can also operate on the other user-defined objects.

Function overloading allows us to reduce the complexity of the code and make it more clear and readable as we can have the same function names with different argument lists.

----

## **What is Inheritance?**

Inheritance is a process by which we can acquire the characteristics of an existing entity and form a new entity by adding more features to it.

In terms of C++, inheritance is creating a new class by deriving it from an existing class so that this new class has the properties of its parent class as well as its own.

----

## **What are the advantages of Inheritance?**

Inheritance allows code re-usability, thereby saving time on code development.

By inheriting, we make use of bug-free high-quality software that reduces future problems.

----

## **Does C++ support Multilevel and Multiple Inheritances?**

Yes.

----

## **What are Multiple Inheritances (virtual inheritance)? What are its advantages and disadvantages?**

In multiple inheritances, we have more than one base classes from which a derived class can inherit. Hence, a derived class takes the features and properties of more than one base class.

For Example, a class driver will have two base classes namely, employee and a person because a driver is an employee as well as a person. This is advantageous because the driver class can inherit the properties of the employee as well as the person class.

But in the case of an employee and a person, the class will have some properties in common. However, an ambiguous situation will arise as the driver class will not know the classes from which the common properties should be inherited. This is the major disadvantage of multiple inheritances.

----

## **Explain the ISA and HASA class relationships. How would you implement each?**

"ISA" relationship usually exhibits inheritance as it implies that a class “ISA” specialized version of another class. For Example, An employee ISA person. That means an Employee class is inherited from the Person class.

Contrary to “"ISA", "HASA" relationship depicts that an entity may have another entity as its member or a class has another object embedded inside it.

So taking the same example of an Employee class, the way in which we associate the Salary class with the employee is not by inheriting it but by including or containing the Salary object inside the Employee class. “HASA” relationship is best exhibited by containment or aggregation.

----

## **Does a derived class inherit or doesn’t inherit?**

When a derived class is constructed from a particular base class, it basically inherits all the features and ordinary members of the base class. But there are some exceptions to this rule. For instance, a derived class does not inherit the base class’s constructors and destructors.

Each class has its own constructors and destructors. The derived class also does not inherit the assignment operator of the base class and friends of the class. The reason is that these entities are specific to a particular class and if another class is derived or if it is the friend of that class, then they cannot be passed on to them.

----

## **What is Polymorphism?**

The basic idea behind polymorphism is in many forms. In C++, we have two types of Polymorphism:

1. Compile-time Polymorphism:

In compile-time polymorphism, we achieve many forms by overloading. Hence, we have an Operator overloading and function overloading. (We have already covered this above)

2. Run-time Polymorphism:

This is the polymorphism for classes and objects. General idea is that a base class can be inherited by several classes. A base class pointer can point to its child class and a base class array can store different child class objects.

This means, that an object reacts differently to the same function call. This type of polymorphism can use a virtual function mechanism.

----

## **What are Virtual Functions?**

A virtual function allows the derived classes to replace the implementation provided by the base class.

Whenever we have functions with the same name in the base as well as the derived class, there arises an ambiguity when we try to access the child class object using a base class pointer. As we are using a base class pointer, the function that is called is the base class function with the same name.

To correct this ambiguity we use the keyword “virtual” before the function prototype in the base class. In other words, we make this polymorphic function Virtual. By using a Virtual function, we can remove the ambiguity and we can access all the child class functions correctly using a base class pointer.

```c++
#include <iostream>

// Base class
class Shape
{
public:
    virtual void draw()
    {
        std::cout << "Drawing a shape." << std::endl;
    }
};

// Derived class
class Circle : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a circle." << std::endl;
    }
};

// Derived class
class Square : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a square." << std::endl;
    }
};

int main()
{
    Shape* shapePtr1 = new Circle();
    shapePtr1->draw();  // Output: "Drawing a circle."

    Shape* shapePtr2 = new Square();
    shapePtr2->draw();  // Output: "Drawing a square."

    delete shapePtr1;
    delete shapePtr2;
    return 0;
}
```

----

## **Give an example of Run-time Polymorphism/Virtual Functions?**

Answer:

```c++
class SHAPE {
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
    cout << shape1->Draw(0,0,2) << endl;
    cout << shape2->Draw(0,0,10,10) << endl;
}
```

In the above code, the SHAPE class has a pure virtual function and is an abstract class (which cannot be instantiated). Each class is derived from SHAPE implementing the Draw () function in its own way.

Further, each Draw function is virtual so that when we use a base class (SHAPE) pointer each time with the object of the derived classes (Circle and SQUARE), then appropriate Draw functions are called.

----

## **What do you mean by Pure Virtual Functions?**

A Pure Virtual Member Function is a member function in which the base class forces the derived classes to override. Normally this member function has no implementation. Pure virtual functions are equated to zero.

Example:

```c++
class Shape { public: virtual void draw() = 0; };
```

A base class that has a pure virtual function as its member can be termed an “Abstract class”. This class cannot be instantiated and it usually acts as a blueprint that has several sub-classes with further implementation.

----

## **What are Virtual Constructors/Destructors?**

*Virtual Destructors:* When we use a base class pointer pointing to a derived class object and use it to destroy it, then instead of calling the derived class destructor, the base class destructor is called.

Example:

```c++
Class A
{
    ~A();
};

Class B : public A
{
    ~B();
};

// Output
// B b;
// A a = &b;
// delete a;
```

As shown in the above example, when we say delete a the destructor is called but it’s actually the base class destructor. This gives rise to the ambiguity that all the memory held by b will not be cleared properly.

This problem can be solved by using the “Virtual Destructor” concept.

What we do is, we make the base class constructor “Virtual” so that all the child class destructors also become virtual and when we delete the object of the base class pointing to the object of the derived class, the appropriate destructor is called and all the objects are properly deleted.

This is shown as follows:

```c++
Class A
{
    virtual ~A();
};

Class B : public A
{
    ~B();
};

// Output:
// B b;
// A a = &b;
// delete a;
```

Virtual constructor: Constructors cannot be virtual. Declaring a constructor as a virtual function is a syntax error.

----

## **What is a friend function?**

C++ class does not allow its private and protected members to be accessed outside the class. But this rule can be violated by making use of the *"friend"* function.

As the name itself suggests, the friend function is an external function that is a friend of the class. For the friend function to access the private and protected methods of the class, we should have a prototype of the friend function with the keyword “friend” included inside the class.

```c++
#include <iostream>

class MyClass
{
private:
    int data;

public:
    MyClass(int value) : data(value)
    {
    }

    friend void displayData(const MyClass& obj);
};

void displayData(const MyClass& obj)
{
    std::cout << "Data in MyClass: " << obj.data << std::endl;
}

int main()
{
    MyClass obj(42);
    displayData(obj);  // Output: Data in MyClass: 42

    return 0;
}
```

----

## **What is a friend class?**

Friend classes are used when we need to override the rule for private and protected access specifiers so that two classes can work closely with each other.

Hence, we can have a friend class to be a friend of another class. This way, friend classes can keep private, inaccessible things the way they are.

When we have a requirement to access the internal implementation of a class (private member) without exposing the details by making the public, we go for friend functions.

```c++
#include <iostream>

class B;  // Forward declaration of class B

class A
{
private:
    int dataA;

public:
    A() : dataA(0)
    {
    }

    void display()
    {
        std::cout << "Data in class A: " << dataA << std::endl;
    }

    friend class B;  // Declaration of class B as a friend
};

class B {
private:
    int dataB;

public:
    B() : dataB(0)
    {
    }

    void modifyA(A& obj)
    {
        obj.dataA += 10;  // Accessing private member of class A
    }

    void display()
    {
        std::cout << "Data in class B: " << dataB << std::endl;
    }
};

int main()
{
    A objA;
    B objB;

    objA.display();  // Output: Data in class A: 0
    objB.modifyA(objA);
    objA.display();  // Output: Data in class A: 10

    return 0;
}
```

----

## **What is a template?**

Templates allow creating functions that are independent of data type (generic) and can take any data type as parameters and return value without having to overload the function with all the possible data types. Templates nearly fulfill the functionality of a macro.

Its prototype is any of the following ones:

template (ankle bracktes)class identifier(ankle bracktes) function_declaration;

template (ankle bracktes)typename identifier(ankle bracktes) function_declaration;

The only difference between both prototypes is the use of keyword class or typename. Their basic functionality of being generic remains the same.

```c++
#include <iostream>

// Generic function using templates
template<typename T>
T add(T a, T b)
{
    return a + b;
}

// Generic class using templates
template<typename T>
class Pair
{
private:
    T first;
    T second;

public:
    Pair(T first, T second) : first(first), second(second)
    {
    }

    void display()
    {
        std::cout << "First: " << first << ", Second: " << second << std::endl;
    }
};

int main()
{
    // Using the generic add() function
    int sum1 = add(5, 7);
    std::cout << "Sum1: " << sum1 << std::endl;

    double sum2 = add(3.14, 2.5);
    std::cout << "Sum2: " << sum2 << std::endl;

    // Using the generic Pair class
    Pair<int> intPair(10, 20);
    intPair.display();

    Pair<std::string> stringPair("Hello", "World");
    stringPair.display();

    return 0;
}
```

----
    
**Wh## at is Exception Handling? Does C++ support Exception Handling?**

Yes C++ supports exception handling.

We cannot ensure that code will execute normally at all times. There can be certain situations that might force the code written by us to malfunction, even though it’s error-free. This malfunctioning of code is called an Exception.

When an exception has occurred, the compiler has to throw it so that we know an exception has occurred. When an exception has been thrown, the compiler has to ensure that it is handled properly, so that the program flow continues or terminates properly. This is called the handling of an exception.

Thus in C++, we have three keywords i.e. try, throw, and catch which are in exception handling.

The general syntax for exception block is:

```c++
try{ 
    // Code that is potentially about to throw exception goes here
    throw exception;
}

catch(exception type)
{
    // code to handle exception goes here
}
```
    
As shown above, the code that might potentially malfunction is put under the try block. When code malfunctions, an exception is thrown. This exception is then caught under the catch block and is handled i.e. appropriate action is taken.

----
    
## **Comment on C++ standard exceptions?**

C++ supports some standard exceptions that can be caught if we put the code inside the try block. These exceptions are a part of the base class “std:: exception”. This class is defined in the C++ header file exception.

A few Examples of Exceptions supported by this class include:

*bad_alloc* – thrown by 'new'

*runtime_error* – thrown for runtime errors

*bad_typeid* – thrown by type id

Introduction to Standard Template Library

----

## **What is a Standard Template Library (STL)? What are the various types of STL Containers?**

A Standard Template Library (STL) is a library of container templates approved by the ANSI committee for inclusion in the standard C++ specification. We have various types of STL containers depending on how they store the elements:

- Queue, Stack – These are the same as traditional queue and stack and are called adaptive containers.
- Set, Map – These are basically containers that have key/value pairs and are associative in nature.
- Vector, deque – These are sequential in nature and have similarities to arrays.

----

## **What is an Iterator class?**

In C++ a container class is a collection of different objects.

If we need to traverse through this collection of objects, we cannot do it using simple index variables. Hence, we have a special class in STL called an Iterator class which can be used to step through the contents of the container class.

The various categories of iterators include input iterators, output iterators, forward iterators, bidirectional iterators, random access, etc.

```c++
#include <iostream>
#include <vector>

class Iterator
{
private:
    std::vector<int>& collection;
    int currentPosition;

public:
    Iterator(std::vector<int>& coll) : collection(coll), currentPosition(0)
    {
    }

    bool hasNext() const
    {
        return currentPosition < collection.size();
    }

    int next()
    {
        return collection[currentPosition++];
    }
};

int main()
{
    std::vector<int> numbers = {1, 2, 3, 4, 5};

    Iterator iterator(numbers);
    while (iterator.hasNext())
    {
        std::cout << iterator.next() << " ";
    }
    std::cout << std::endl;

    return 0;
}
```

----

## **What is the difference between an External Iterator and an Internal Iterator? Describe an advantage of the External Iterator?**

An *internal iterator* is implemented with member functions of the class that has items to step through.

An *external iterator* is implemented as a separate class that can be bound to the object that has items to step through. The basic advantage of an External iterator is that it’s easy to implement as it is implemented as a separate class.

Secondly, as it’s a different class, many iterator objects can be active simultaneously.

# https://www.softwaretestinghelp.com/cpp-interview-questions

# https://interviewsansar.com/category/cplusplus-advanced-interview-questions-and-answers

## **Write a complete class stating function overriding feature in C++**

```c++
#include <iostream>

// Base class
class Shape
{
public:
    virtual void draw()
    {
        std::cout << "Drawing a shape." << std::endl;
    }
};

// Derived class
class Circle : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a circle." << std::endl;
    }
};

// Derived class
class Square : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a square." << std::endl;
    }
};

int main()
{
    Shape* shapePtr1 = new Circle();
    shapePtr1->draw();  // Output: "Drawing a circle."

    Shape* shapePtr2 = new Square();
    shapePtr2->draw();  // Output: "Drawing a square."

    delete shapePtr1;
    delete shapePtr2;
    return 0;
}
```

----

## **Show the function call in main program.**

```c++
#include <iostream>

// Base class
class Shape
{
public:
    virtual void draw()
    {
        std::cout << "Drawing a shape." << std::endl;
    }
};

// Derived class
class Circle : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a circle." << std::endl;
    }
};

int main()
{
    Shape* shapePtr = new Circle();
    shapePtr->draw();  // Function call

    delete shapePtr;
    return 0;
}
```

----

## **Explain the concept of function overriding.**

```c++
#include <iostream>

// Base class
class Shape
{
public:
    virtual void draw()
    {
        std::cout << "Drawing a shape." << std::endl;
    }
};

// Derived class
class Circle : public Shape
{
public:
    void draw() override
    {
        std::cout << "Drawing a circle." << std::endl;
    }
};

int main()
{
    Shape* shapePtr = new Circle();
    shapePtr->draw();  // Output: "Drawing a circle."

    delete shapePtr;
    return 0;
}
```

----

## **Take example of drawing multiple shapes e.g. circle and rectangle etc.**

If you follow best coding practice and the things you care when write the code.

NOTE: As per question criteria, we will write code using interface, but, to describe the concept a basic example will be covered first.

Answer:

Function overriding concept is run time polymorphism in oops, in which functions get resolved on run time using VTABLE (Virtual table) by compiler.

If we have definition /declaration of a function in base class and want to have a definition of same function name in derive class and want to call derived function using base class pointer, then we need to override function. It’s simple, just we must make base class function virtual. for example,
Example if base class has a function definition:

```c++
class A{
public:
	virtual void foo()
    {
		cout<<" Base::A";
	}
};

class B: public A
{
public:
	void foo()
    {
		cout<<" Derived::B";
    }
};

int main()
{ 
    A *p = new B(); p->foo();
	delete p;
	return 0;
}
```

Example if base class has a function declaration(Interface):

Recommended to read C++ Interface and Pure virtual function.

```c++
//Interface
class IShape
{
public:
	virtual void draw()=0;
};

//Derived class
class Circle: public IShape
{
public:
	void draw();
};

//define the function
void Circle::draw()
{
	cout<<"Circle"<<endl;
}

int main()
{
    IShape *s = new Circle();
    s->draw();
	delete s;
	
    return 0;
}
```

As a best practice, what we have taken care of in above program so for? Here are the points

We have used interface not a class to maintain loose coupling.
We have deallocated the dynamically allocated memory.
But, still we have missed one important point i.e. we should have written virtual destructor in the above base class to maintain the hierarchy of destructor call.

You can read here constructor and destructor call order in inheritance in C++. ( In short, constructor gets called from the base to derived class, and destructor call order is vice versa).

In the current program, derived class that is “Circle” class destructor will not be called, as we have not written virtual destructor in base class. Here is the example and output in which derived class destructor is not called.

In the above program lets write destructors in base class and derived class

```c++
//Interface
class IShape
{
public:
	virtual void draw()=0;
	
    //destructor
	~IShape()
    {
		cout<<"Base destructor"<<endl;
	}
};

//Derived class
class Circle : public IShape
{
public:
	void draw();

	//destructor
	~Circle()
    {
		cout<<"Circle destructor"<<endl;
	}
};

//define the function
void Circle::draw()
{
	cout<<"Circle"<<endl;
}

// Output:
// Circle
// Base destructor
```

But, if we make base class destructor virtaul as virtual ~IShape()then derived class destructor will also be called and output will be as below in reverse order(derived to base)
- Circle
- Circle destructor
- Base destructor

There is no harm if we have not written virtual destructor, but, a pain comes at later point in a large project, if some other programmer comes and deallocate memory consuming resources in the destructor of derived class. A memory leak will happen and it may take huge time identifying that at run time. so, as a best practice we should write virtual destructor in base class too.

You can read virtual destructor in C++ with example in detail.

How to delete array of objects in C++? Proof by C++ code for proper deletion
Posted in C++ AdvancedBy rsinghPosted on April 26, 2017Tagged delete array of pointers in C++
Answer includes how to delete array of objects in C++ created dynamically with C++ code example with proof. In other words, delete array of pointers to objects in c++.

----

## **Write C++ code to create an array of objects using new keyword and delete these objects. Also, proof that all the objects are deleted properly.**

We know that when we create an object of a class dynamically from heap memory using new keyword, then we must delete it explicitly to avoid memory leaks in C++ programs after we are done with its operations.

Let’s take below class Pen as an example.

```c++
class Pen
{
public:
    Pen()
    { 
        cout << "Constructor..." <<endl; 
    }
		
    ~Pen()
    { 
        cout << "Destructor...!" <<endl; 
    }
	
    void write()
    {
	    cout << "Writing...!" <<endl; 
	}
};

Below is an example, how we create an object of the class Pen dynamically and delete it after we are done with operations.

int main()
{
    // create an object dynamically
    Pen* pen = new Pen();
    pen->write(); // operations
   
    delete pen; // de-allocate the memory
   
    return 0;
}
```

How to create array of objects of a class in C?
Let’s see how we create an array of objects in below C++ program example. In this example, we will create array of 3 objects, perform operation and delete dynamic array of pointers properly.

```c++
int main()
{
    //create an array of objects
    Pen* pen = new Pen[3];

    pen[0].write();
    pen[1].write();
    pen[2].write();
   
    delete[] pen; // de-allocate array of objects

    return 0;
}

// Output:
// Constructor…
// Constructor…
// Constructor…
// Writing…!
// Writing…!
// Writing…!
// Destructor…!
// Destructor…!
// Destructor…!
```

Proof of proper deletion of array of objects in C++
First, note that if we create an object of a class and delete the object then class constructor and destructor will be called respectively.

In above example, we have created an array of 3 objects and delete it using statement delete [] pen; if we look at the output the class constructor and destructor were called 3 times each. means, we have deleted objects properly.

Now, If we delete the object using the statement “delete pen” ( This is general mistake a programmer make) then the destructor will be called only once and for rest 2 objects destructor will not be called and program will crash. and this will proof that objects are not deleted properly.

Lets see the output if we use statement “delete pen”

```c++
int main()
{
    // create an array of objects
    Pen* pen = new Pen[3];

    pen[0].write();
    pen[1].write();
    pen[2].write();
   
    // this is not a prper way to delete
    // array of objects
    delete pen;

    return 0;
}

// Output:
// Constructor…
// Constructor…
// Constructor…
// Writing…!
// Writing…!
// Writing…!
// Destructor…!
```

and then program will crash at run time.

Conclusion:
In C++, single object of a class created dynamically is deleted using statement “delete pointer” and array of objects are deleted using statement “delete [ ] pointer”.

How to stop class inheritance in C++ with condition that object creation should be allowed
Posted in C++ AdvancedBy rsinghPosted on April 11, 2017Tagged C# inheritance, C++ stop inheritance
Answer includes multiple solutions to stop or prevent class inheritance in C++ with condition that object creation of the class should be allowed with C++ program example and explanation.

----

## **I want to stop a class to be inherited and allow to create an object of the class. Design a solution for this problem statement. Give as many solutions as you can.**

We can apply 3 solutions to prevent a class to be inherited in C++ where object creations will be allowed.

*Solution-1:* Use the final keyword (from C++11)
In the below example, we’ve made the Unique class final. So, it’ll not be inherited by any class.

If you try to inherit it, the compiler will flash an error that “a final class cannot be used as a base class“.


Note that you can create an object of the final class as show in the main() method here.

```c++
#include <iostream>

using namespace std;

class Unique final
{
public:
    void display()
    {
		cout << "My unique class" << endl;
	}
};

// class Derived : Unique {
// YOUR GET ERROR HERE if you inherit the Unique class
// class Unique - a final class cannot be used as
// a base class.
// };

int main()
{
	// you can create an object of the final class 
	Unique ob;
	ob.display(); 
	
	return 0;
}
```

*Solution-2:*

Make the constructor of the class private and write a static function in the class that create object and return it to users.
Here is the C++ program example, in which constructor of the class named Unique is private and have written one static function, that is GetInstance() that create object and returns to user i.e. main() function.

So, the below program will fulfil the criteria mentioned in the question.

Note that if a class has its constructor private then neither an object of it can be created nor it can be inherited by any class.

So, if we try to derive a new class from it then compiler will throw an error stating that private constructor of the class is inaccessible at the compile time itself.

Since, we’ve prevented a class to be inherited by making the class constructor private. So, an object will also not be created of this class.

But, we want to allow an object of the class to be created. To solve this problem,

we can have a static function in the class that is called by class name without creating an object. And this function will create the class object, and return to users or main program.

Here is the complete working program that’ll satisfy the above criteria.

C++ Code Example:

```c++
// TestApplication.cpp : "Unique" class cannot be inherited but object of it can be created.
//

#include<iostream>

using namespace std;

class Unique
{
private:
	//Make constructor private
	Unique()
    {
    }

public:
	//Create a static fuction that
	//returns object of the class
	static Unique*  GetInstance()
    {
		return new Unique();
	}	
	
    void Display()
    {
		cout<<" My Unique Class"<<endl;
    }
};

int main()
{ 
    Unique *u = Unique::GetInstance();
    u->Display();
	return 0;
}
```

If we try to derive a class from Unique class (example below) compiler will throw an error stating that private constructor of Unique class is inaccessible at compile time itself.

```c++
class Derived:public Unique{
public:
	Derived(){
		cout << "Derived constructor" << endl;
	}

public:
	void Display(){
		cout << " My Derived Class" << endl;
	}
};
```

*Solution-3:*

Create a dummy class having a private constructor and make the class friend of dummy class and extend the class virtually from dummy class.
Below is the C++ program example that will not allow Unique class to be inherited. But, allow object creation of the Unique class.

When we create the object of the Unique class, it will access and call the private constructor of the dummy class StopInheritance, Because the Unique class is friend of the dummy class.

Note that if a class is friend of another class then it can access private data of that class.

Recommend to read the order of constructor and destructor call in C++ inheritance relationship if you are not familiar with calling orders.

So, we can create an object of the Unique class. But, if we derive a class from the Unique class and create an object of derived class, then it will directly try to access the constructor of dummy class because the Unique class has inherited it virtually.

And since the derived class is not a friend of the dummy class, it cannot access the private constructor resulting in a compiler error.

```c++
#include <iostream>

using namespace std;

//dummy class
class StopInheritance
{
private:
	//make constructor private
	StopInheritance()
    {
    }

	//make Unique class a friend of it
	friend class Unique;
};

class Unique:virtual StopInheritance
{
public:	
	Unique()
    {
		cout<<"Class";
	}
	
    void Display()
    {
		cout<<" My Unique Class"<<endl;
	}
};

class Derived : public Unique{
public:
	void Display()
    {
		cout << " My derived Class" << endl;
	}
};

int main()
{	
	Derived obj;
	obj.Display();

	return 0;
}
```

----

## **What is Advantage and Use of THIS pointer in C++ – Scenarios?**

Answer includes uses and advantage of the this pointer in C++ programming with multiple scenarios where the this pointer is used.

__Sceranio-1:__

Internal use of this pointer as an argument to a function.
Wherever an object calls a class member function, then the compiler internally passes a “this” pointer to the member function internally.

For example,

In the below class Car, we have a “SetModel” member function that receives one argument i.e. car model.

In fact, besides the model parameter, one more argument is passed to the set model function internally, and that is the “this” pointer.

```c++
class Car
{
	int model;
public:
	void SetModel(int model)
    {		
		this->model = model;
	}
};

int main()
{
	int modelNumber = 1024;
	Car obj;
	// On calling function using class obj
	// THIS pointer is also passed internally besides
	// model number paramer.
	obj.SetModel(modelNumber);

	return 0;
}
```

You can Read in detail: “this” pointer internal working in C++.

__Scenario-2:__

Use “this” pointer to assign value of the function’s parameter to a class member variable correctly
In the below code example,

the class member variable “ modle”, and the parameter “modle” in the function SetModel(int model) are of the same name.

```c++
class Car
{
	int model;
public:
	void SetModel(int model)
    {		
		this->model = model;
	}
};
```

Even though if we write model=model in the SetModel function instead of this->model = model; the compiler will throw no error and everything would seems fine at the compile time, but when you run the program, you’ll get garbage value.

Scenario-3: In a large code base of a function, identifying the class member variable is easy
Assume a function of a class or multiple functions uses the class fields and they have very large and complex code base, then

it’s easy for a programmer to identify the class fields. Specially when a maintenance or modification is done within it.

```c++
class Car
{
	int model;

public:
	void SetModel(int m)
    {
		// do something;
		this->model = m;
	}
};
```

----

## **Can we use THIS Pointer in static function – Reason in C++?**

We cannot use THIS pointer in static function of a class in C++ program.

Reason: Whenever we call a class non-static member function using class object, then THIS pointer is also passed to the function as a parameter internally and this is why a non-static member function of a class know that on which class object it is being called in case of multiple objects creation of the class.

Recommended: How does "this" pointer in C++ work internally?

But, static function of a class is not associated with class object. So, THIS pointer is not passed to a static function as an internal parameter. So, a static function does not understand THIS pointer inside its body.

If we compile below class, compiler with throw an error i.e. static functions do not have this pointer.

```c++
class Printer
{
	static int a;

public:
	static void print()
    {
		//Error static funtions do not have 
		//this pointer.
		this->a; 
	}
};
```

This is why static member function cannot have this pointer in C++ language.

----

## **C++ Public access specifier instead of Private – What is bad?**

A class is having private data members and that is by design and expected. Question is, if we write C++ public access specifier instead of private for that data members, then what issue we can face in a C++ program?

Wrongly placed specifiers may create a huge pain in maintenance or finding bugs for changed behavior of a large C++ project.

In a simple program it may not be noticeable. But, in a large program where tons of classes and tons of functions are there, it may be difficult to find issues. So, we need to keep focus when using access specifiers in C++ software projects.

Let’s take a simple C++ code example . If we use public access specifier instead of private for data members in a class,  compiler is not going to complain and programs work fine.  However, it may lead to an issue unknowingly.

In below C++ program, there is a class called Insurance and it contains a data member "float sum" and the value of "sum" has been initialize to 5.0. There is another class TaxCalculator which is using the value of sum variable to calculate the tax with formula float tax = obj.getSum()*10/100;. Expected answer for this program is 0.5.

But assume, by mistake, if some programmer changed its value in TaxCalculator class that is sum=100, may be to solve other problems. Then value of tax will become 10 that was not expected. So, we have to be careful  with choosing access specifiers for members and functions.

```c++
class Insurance
{
public:	
	int year;
	float sum;

public:
	Insurance()
    {
		this->sum =5.0;
	}
	float getSum()
    {
		return sum;
	}
};

class TaxCalculator
{
	Insurance obj;
public:
	TaxCalculator()
    {
		obj.sum = 100;
	}

	float getTax()
    {
		float tax = obj.getSum()*10/100;		
		return tax;
	}
};

int main()
{
	// Access to public functions 
	TaxCalculator tc;
	cout << "Tax=" << tc.getTax();
	
	return 0;
}
```

----

## **Use of Public Private and Protected access specifiers in C++?**

Use of public, private and protected access specifiers in C++ is to control the access/visibility of member data and functions out of a class. It all depends upon requirement when a class is designed, what access level to fields and member functions, we want to provide in a class with the use of public private and protected specifiers.

Use of public private and protected access specifiers.

__Use of private access specifier in C++:__

Use private specifier for data and functions of a class that are not supposed to be exposed outside of a class.

As a good class design, a class should have all data members private in a class and it's functions should use these member data.

If we have to provide access to data members of a class to another class or program e.g. main(), we should not make it public or protected, but we should provide it using an interface i.e. public methods to access from outside of a class.

In below C++ class, all member fields are private. Let’s say, we want to allow another class to set or get the value of sum, then we should have public method getSum() and setSum() etc.

```c++
class Insurance
{
private:
	float sum;
	int year;
	
public:
	float getSum()
    {
		return sum;
	}
	void setSum(float sum)
    {
		this->sum = sum;
	}	
};

int main()
{
	Insurance obj;
	
	obj.setSum(5.0);
	cout << obj.getSum();	

	return 0;
}
```

All the internal functions of a class that is used in class itself and public exposer of internal functions not required, then make them private. Only make function public which is supposed to be accessed from outside of a class.

__Use of Public access specifier in C++:__

Expose only required member functions to out of a class. So, it can be accessed from anywhere from another class or program.

```c++
class Insurance
{
private:
	int year;
	float sum;
	
public:
	float getSum()
    {
		return sum;
	}
	void setSum(float sum)
    {
		this->sum = sum;
	}	
};

int main()
{
	// Access to public functions 
	Insurance iobj;	
	vobj.getSum();
	return 0;
}
```

__Use of Protected access specifier in C++:__

Use protected specifier if you want to allow access of data and member functions to child class only in inheritance.

In below program, data member “sum” and displaySum() function are protected and only available to child class. If we call them in main() program, compiler will flash an error i.e. protected member can’t be accessed.

```c++
class Insurance
{
private:	
	int year;

protected:
	float sum;
	void displaySum()
    {
		cout<<"sum="<<sum;
    }
    
    public: float getSum()
    {
        return sum;
    }
    
    void setSum(float sum)
    { 
        this->sum = sum;
	}	
};

class VehicleInsurance : public Insurance
{
public:
	VehicleInsurance()
    {
		sum = 100.00; // can access protected member
		displaySum(); // access protected function
	}
};

int main()
{
	VehicleInsurance vobj;
	// vobj.sum = 12; // Error can't access protected member
	// vobj.displaySum(); // Error can't access protected function
	vobj.getSum(); // public fucntin OK
	return 0;
}
```

Also, use of public private and protected access specifiers in C++ is in inheritance hierarchy that is how we want to inherit the base class. For example

```c++
class VehicleInsurance:public Insurance{}
class VehicleInsurance:private Insurance{}
class VehicleInsurance:protected Insurance{}
```

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

```c++
class Insurance
{
private:
	float sum;
	int year;

public:
	float getSum()
    {
		return sum;
	}
	
    void setSum(float sum)
    {
		this->sum = sum;
	}	
};

int main()
{
	Insurance obj;
	
	obj.setSum(5.0);
	cout<<obj.getSum();	

	return 0;
}
```

All the internal functions of a class that is used in class itself and public exposer of internal functions not required, then make them private. Only make function public which is supposed to be accessed from outside of a class.

__Use of Public access specifier in C++:__

Expose only required member functions to out of a class. So, it can be accessed from anywhere from another class or program.

```c++
class Insurance
{
private:	
	int year;
	float sum;
	
public:
	float getSum()
    {
		return sum;
	}

	void setSum(float sum)
    {
		this->sum = sum;
	}	
};

int main()
{
	// Access to public functions 
	Insurance iobj;	
	vobj.getSum();
	
    return 0;
}
```

__Use of Protected access specifier in C++:__

Use protected specifier if you want to allow access of data and member functions to child class only in inheritance.

In below program, data member “sum” and displaySum() function are protected and only available to child class. If we call them in main() program, compiler will flash an error i.e. protected member can’t be accessed.

```c++
// TestApplication.cpp : Use of Protected access specifier.
//

#include <iostream>
#include <string>
#include <stdio.h>
#include <math.h>
#include <stdbool.h>
#include <cstdlib>
#include <cstring>

using namespace std;

class Insurance
{
private:
	int year;

protected:
	float sum;
	void displaySum()
    {
		cout << "sum=" << sum;
	}
    public: float getSum()
    {
        return sum;
    }
    
    void setSum(float sum)
    {
		this->sum = sum;
	}
};

class VehicleInsurance : public Insurance
{
public:
	VehicleInsurance() {
		sum = 100.00;//can access protected member
		displaySum();//access protected function
	}
};

int main()
{
	VehicleInsurance vobj;
	//vobj.sum = 12;//Error can't access protected member
	//vobj.displaySum();//Error can't access protected function
	vobj.getSum();// public fucntin OK

	return 0;
}
```

Also, use of public private and protected access specifiers in C++ is in inheritance hierarchy that is how we want to
inherit the base class. For example:

```c++
class VehicleInsurance:public Insurance{}
class VehicleInsurance:private Insurance{}
class VehicleInsurance:protected Insurance{}
```

----

## **Use of public instead of private may lead you in great pain. How?**

Using the "public" access modifier instead of "private" in software development can lead to various issues and potential pain points. Here are some reasons why this can be problematic:

1. Encapsulation: One of the fundamental principles of object-oriented programming is encapsulation, which involves hiding internal implementation details of a class and providing controlled access through methods. By declaring members as public, you expose the internal state and implementation of a class, breaking encapsulation. This can lead to unintended dependencies and make it difficult to maintain or modify the code in the future.

2. Dependency management: Public members are accessible to all other classes, leading to increased coupling between different parts of the codebase. When changes are made to a public member, it can impact other classes that rely on it, potentially causing a ripple effect of changes throughout the codebase. This can make the code more fragile and harder to maintain.

3. Inconsistent or invalid state: With public members, other parts of the code can directly modify the state of an object without any checks or validation. This can result in the object being in an inconsistent or invalid state, leading to bugs and unexpected behavior that may be difficult to trace and debug.

4. Security vulnerabilities: Public members are accessible to all code, including external code or untrusted sources. This can introduce security risks, as sensitive data or critical operations may be exposed and manipulated by unauthorized entities. By keeping members private, you can control access and enforce security measures more effectively.

5. Limited control and evolution: By exposing implementation details through public members, you limit your ability to modify or improve the internal workings of a class in the future. Making changes to a public member may have unintended consequences for the existing codebase, requiring extensive modifications and potentially breaking other parts of the system.

To mitigate these potential issues, it is generally recommended to follow the principle of information hiding and use the "private" access modifier by default. This allows you to control access to class members, enforce encapsulation, minimize dependencies, ensure data integrity, and maintain the flexibility to evolve the codebase in a controlled manner.

----

## **What if memory allocation using new fails in C++ how to handle**

In another words, when you allocate memory on heap using new operator, how do you handle memory allocation using new in C++ failure? What is the issue when you don’t handle it?

Answer: If C++ new fails to allocate memory will include 2 techniques to handle dynamic memory allocation using new failure in C++.

When we allocate memory from heap dynamically in a C++ program using new operator, the program crashes when memory is not available, or the system is not able to allocate memory to a program, as it throws an exception. So, to prevent program crash, we need to handle the exception when memory allocation fails.

Techniques to handle bad allocation exception in C++ program:

*Using Try Catch Block with std::bad_alloc exception:*

We need to put the memory allocation code using new operator in try catch block. Below C++ program catches exception when it is thrown on memory allocation failure.

```c++
#include <iostream>

using namespace std;

int main()
{
    // Try to allocate very huge amount of memory
	// so memory allocation fails.
	long CHUNK_SIZE = 0x7fffffff;

	// Allocate memory dynamically using "new" 
	// using try catch block
	try
    {
		char *ptr = new char[CHUNK_SIZE];
		// on exception below line will not be printed.
		// and control will go in catch block.
		cout<<"Memory allocation Successful"<<endl;
	}
	catch (const bad_alloc& e)
    {
		cout << "Allocation failed: " << e.what() << '\n';
		// handle error
	}		

	return 0;
}
```

Using no_throw version of “new” i.e. new(std::nothrow)
Rather than simply using new operator for memory allocation in C++, we need to use no throw version of “new” as it handle the exception and there is no program crash.

```c++
#include <iostream>

using namespace std;

int main()
{
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
	else
    {
		cout << "Memory allocation fails" << endl;
	}      

	return 0;
}
```

----

## **When to use RTTI – Dynamic_cast in C++**

Scenarios – Use of Dynamic_cast in C++ program:

__Situation 1__ - When we need to call a specialized member function of child class that’s not available to the base class in inheritance hierarchy. Polymorphism breaks down here but sometimes we get this situation. Below, class B contains specialized funcB() function: 

```c++
class A
{
public:	
	virtual void func()
    {
    }
};

class B : public A
{
public:
	void func()
    {
    }
	
    // Specialized function to B class
	void funcB()
    {
    }
};
```

What if we need to call specialized funcB() using base class pointer like in theprogram below? Dynamic cast operator, Part of RTTI in C++ comes into picture to type cast from base to child class.

```c++
// A* arg: base class pointer that can have
// any child classes object.
void f(A* arg)
{

// down cast from base pointer to derive pointer
// as, base class pointer does not understand 
// specialized function of derived class.
B* bp = dynamic_cast<B*>(arg);
    if (bp)
    {   	
        bp->func();
        bp->func2();// ok
    }  
    else
    {
        // Call respective class function
        arg->func();
    }
};
```

__Situation 2__ – We want to override a function from base class that is not virtual and we can’t make it virtual as base class is sitting in a library and it can’t be modified.

So, overriding is not possible. If we use statements for below program, A* ptr = new B(), ptr->func2(); always base call method will be called as its not virtual in base class. But we want to call child class func2() method.

Then we need to use dynamic_cast operator to type cast base pointer to child pointer to call child’s class method.

```c++
// We cannot touch base class A but can be inherited. 
class A
{
public:	
	virtual void func()
    {
        printf("Class A :func()\n")
    }

	void func2()
    {
        printf("Class A :func2()\n");
    } // not virtual 
};

class B : public A
{
public:
	void func()
    {
        printf("Class B :func()\n");
    }

	// Want to override func2 but can't func2 is not virtual in base class.
	// If we use base class pointer with B object, base class func2 function will be called.
	// Can't make class A:func2 virtual as it is in a library- binary form.
	// Only option is RTTI to access it via base class pointer in client code.
	void func2()
    {
        printf("Class B :func2()\n");
    }
};
```

Complete Example: Situation-1: Call specialized member function of a child class using dynamic_cast RTTI in C++.

```c++
using namespace std;

class A {
public:	
	virtual void func() { printf("Class A :func()\n"); }
};

class B : public A
{
public:
	void func()
    {
        printf("Class B :func()\n");
    }

	//Specialized function to B class
	void funcB()
    {
        printf("Class B :funcB()\n");
        }
};

int main()
{
	A* ap = new B();
 	//Call funcB() function of class B using base pointer A
    // ap->funcB();//Compiler error as funcB() is not a member of Animal	

	//Now use dymaic cast to convert base pointer to derived pointer i.e. A to B.
	B* bp = dynamic_cast<B*>(ap);
	
	if (bp)
	{
		bp->funcB();
	}
	
    return 0;
}
```

Complete Example: Situation-2: Call child class method if it is not virtual in base class in C++

```c++
using namespace std;

class A
{
public:	
	virtual void func() { printf("Class A :func()\n");
    }
    
    void func2()
    {
        printf("Class A :func2()\n");
    } // not virtual 
};


class B : public A
{
public:
	void func()
    {
        printf("Class B :func()\n");
    }

	void func2()
    {
        printf("Class B :func2()\n");
    }
};

class C : public A
{
public:
	void func()
    {
        printf("Class C :func()\n");
    }	
};

//-----Client code------
void f(A* arg)
{
    //call 
    B* bp = dynamic_cast<B*>(arg);	

    //Call Specific class B function.
    if (bp)
    {   	
        bp->func();
        bp->func2();
    }  
    els
    {
        //Call respective class function
        arg->func();
    }
};

int main()
{
	A* ap1 = new B(); 
	f(ap1);

	// operate C object
	A* ap2 = new C();
	f(ap2);

    return 0;
}
```

----
    
## **Writing Smart Pointer in C++ for a Specific Class**

__What is smart pointer and implementation of Smart pointer in C++?__

Smart pointers are a pointers that get de-allocated by itself, when it goes out of scope and we don’t need to to delete it manually. Generally , in C++ programming we use new and delete to allocate and deallocate memory dynamically / at run time.

When we use “new” to allocate memory, the programmer is responsible to free the memory using delete keyword. Where as this is not the case of smart pointers. In fact, smart pointers are objects which store pointers to dynamically allocated objects.

Lets see a simple example to create a smart pointer class.

Consider a class called “Car” having a method Run () as shown below. We will create a smart pointer for this class named CarSP. This smart pointer in C++ program will handle automatic deallocation of memory i.e. for Car object allocated dynamically.

Car Class :

```c++
// Car class for which we have to implement
// a Smart pointer.
class Car
{
public:
	void Run()
    {
		cout<<"Car Running..."<<"\n";
	}
};
```
    
__Implementation of Smart pointer in C++__

In CarSP smart pointer class, we’ll have a field Car *sp, that hold the pointer of Car object. In the destructor of CarSP, we will write code to delete object of Car class.

To call the function of car class we have to overload arrow operator -> operator, that returns pointer of object Car. Note that After overloading -> only we would be able to use -> on class CarSP that act as a pointer.

Smart pointer class and testing code

```c++
// Smart pointer for class Car
class CarSP
{
	Car *sp; //  

public:
	// Initialize Car pointer when Car 
	// object is createdy dynamically
	CarSP(Car * cptr):sp(cptr)
    {
    }

	// Smart pointer destructor that will de-allocate
	// The memory allocated by Car class.
	~CarSP()
    {		
		printf("Deleting dynamically allocated car object\n");
		delete sp;
	}

	// Overload: operator that will be used to 
	// call functions of class car
	Car* operator-> ()
	{    
		return sp;
	}
};

//Test
int main()
{
	//Create car object and initialize to smart pointer
	CarSP ptr(new Car());
	ptr->Run();

	//Memory allocated for car will be deleted
	//Once it goes out of scope.
	return 0;
}
```

# https://interviewsansar.com/category/cplusplus-advanced-interview-questions-and-answers/

## **What is Qt?**

Qt is a popular cross-platform framework for C++ development. It provides a comprehensive set of libraries and tools for building graphical user interfaces (GUIs), networked applications, and other software projects. Qt was initially developed by the Norwegian company Trolltech and is now maintained and developed by The Qt Company.

Key features of Qt include:

Cross-Platform Development: Qt enables developers to write applications that can run on multiple operating systems, including Windows, macOS, Linux, and embedded platforms. Qt achieves this through its abstraction layer, which allows developers to write code once and deploy it on various platforms without extensive modifications.

GUI Development: Qt offers a powerful set of tools and libraries for creating rich and interactive graphical user interfaces. It provides a widget toolkit with a wide range of pre-built UI components, support for layouts, styling options, and theming capabilities.

Signal and Slot Mechanism: Qt introduces a signal and slot mechanism, which facilitates communication between different components of an application. This mechanism allows objects to emit signals and other objects to respond to those signals by connecting them to slots, enabling flexible and decoupled communication.

Object-Oriented Programming: Qt follows an object-oriented programming paradigm, allowing developers to create reusable and modular code. Qt's classes and APIs are designed to facilitate object-oriented development and encapsulation.

Networking and Web Integration: Qt provides modules for networking and web integration, allowing developers to build networked applications, communicate with web services, handle HTTP requests, and more. It supports various network protocols, making it suitable for applications that require network connectivity.

Multimedia Support: Qt offers multimedia modules that enable developers to incorporate audio, video, and multimedia capabilities into their applications. It provides APIs for playing audio and video files, capturing media from devices, and processing multimedia data.

Database Integration: Qt provides support for database integration, allowing developers to connect to and interact with various database systems. It offers high-level APIs and SQL-based classes for database operations, making it easier to work with databases in Qt applications.

Internationalization and Localization: Qt includes features for internationalization and localization, allowing developers to create applications that can be easily translated into multiple languages. It provides tools for managing and translating strings, handling different date and time formats, and supporting locale-specific requirements.

Qt has a large and active community, with extensive documentation, tutorials, and sample code available. It is widely used in industries such as automotive, industrial automation, consumer electronics, and software development companies. Qt is available under both commercial and open source licenses, offering flexibility in terms of licensing options for developers and organizations.

----

## **Can you provide a minimum example of Qt?*

Certainly! Here's a minimum example of a Qt application in C++:

```cpp
#include <QApplication>
#include <QLabel>

int main(int argc, char *argv[]) {
    QApplication app(argc, argv);

    QLabel label("Hello, Qt!");
    label.show();

    return app.exec();
}
```

In this example, we include the necessary Qt headers, `QApplication` and `QLabel`, for our application. We create an instance of `QApplication` and pass the command line arguments (`argc` and `argv`) to it.

Next, we create a `QLabel` widget and set its text to "Hello, Qt!". We call `label.show()` to make the label visible on the screen.

Finally, we enter the event loop by calling `app.exec()`. The event loop handles user interactions and other events within the application until the application is closed.

This simple example creates a window with a label displaying the text "Hello, Qt!".

To compile and run this code, you'll need to have Qt installed and properly configured in your development environment. You can use the Qt command-line tools or an integrated development environment (IDE) like Qt Creator to build and run the application.

Note that this is a minimal example just to demonstrate the basic structure of a Qt application. In real-world applications, you would typically create more complex UI layouts, handle user interactions, connect signals and slots, and utilize various Qt modules for additional functionality.

----

## **How to create a linux binary out of C++ code?**

To create a Linux binary from C++ code, you can follow these general steps:

1. Write your C++ code: Create a C++ source file (e.g., `my_program.cpp`) that contains your code.

2. Open a terminal: Open a terminal on your Linux system.

3. Install the required build tools: Ensure that you have the necessary build tools installed on your system, such as the GNU Compiler Collection (GCC) and the build-essential package. If they are not already installed, you can typically install them using your distribution's package manager. For example, on Ubuntu or Debian-based systems, you can use the following command:
```bash
sudo apt-get install build-essential
```

4. Navigate to the directory containing your C++ code: Use the `cd` command to navigate to the directory where your C++ source file (`my_program.cpp`) is located.

5. Compile the C++ code: Compile your C++ code using the `g++` command, which is part of the GCC toolchain. The basic syntax is:
```bash
g++ -o output_file_name input_file_name.cpp
```
For example, to compile `my_program.cpp` and generate an output file named `my_program`, you can use the following command:
```bash
g++ -o my_program my_program.cpp
```

6. Run the binary: Once the compilation process completes successfully, you can run the generated binary by specifying its filename:
```bash
./my_program
```

By running the `./my_program` command, the Linux operating system will execute the binary file and run your C++ program.

Note: Ensure that your C++ code is free of any errors or issues before compiling. Additionally, depending on the complexity of your code and any external libraries used, you may need to provide additional compiler flags or link against specific libraries during the compilation process.

----

## **How is an MSI file created out of an EXE file?**

To create an MSI (Microsoft Installer) file out of an EXE (executable) file, you can use a packaging and deployment tool such as WiX (Windows Installer XML) or a commercial installer creation software like InstallShield or Advanced Installer. Here is a general overview of the process using WiX:

1. Install the necessary tools: Download and install the WiX Toolset, which includes the required tools for creating MSI packages. You can get the WiX Toolset from the WiX website (https://wixtoolset.org/).

2. Define the installer project: Create an XML file (e.g., `Product.wxs`) that defines the structure and components of your installer project using the WiX markup language. This file specifies the files, directories, registry entries, shortcuts, and other settings that should be included in the MSI package.

3. Define the user interface (optional): If you want to create a custom user interface for your installer, you can create additional XML files to define the UI using the WiX User Interface (UI) extension.

4. Build the MSI package: Use the `candle` tool from the WiX Toolset to compile your WiX source files into object files:
```bash
candle Product.wxs
```
This will generate object files (.wixobj) that represent the components of your installer.

Next, use the `light` tool to link the object files and create the MSI package:
```bash
light Product.wixobj
```
This will generate the MSI file (e.g., `Product.msi`).

5. Test and sign the MSI package: It is recommended to test the generated MSI package to ensure that it installs and functions correctly. Additionally, you may consider digitally signing the MSI file using a code signing certificate to provide an additional level of trust and security.

Note that creating an MSI file requires knowledge of the Windows Installer technology and the WiX markup language. It may take some time and effort to learn and become proficient in using these tools effectively.

Alternatively, if you prefer a commercial solution, tools like InstallShield or Advanced Installer provide graphical interfaces and wizards to simplify the process of creating MSI packages from EXE files. These tools typically offer additional features and flexibility for customizing the installation process.

----

## **How to cross compile on Windows??**

Cross-compiling on Windows typically involves setting up a cross-compilation toolchain that can generate binaries for a different target platform. Here's a general overview of the process:

1. Choose a cross-compilation toolchain: Identify and download a cross-compilation toolchain that is compatible with your target platform. For example, if you want to cross-compile for Linux, you can use tools like MinGW-w64, MXE (M cross environment), or Cygwin. These toolchains provide compilers, libraries, and other necessary components to build binaries for the target platform.

2. Install the cross-compilation toolchain: Follow the installation instructions provided by the chosen cross-compilation toolchain. This typically involves downloading and running an installer or extracting the toolchain files to a specific directory.

3. Set up the environment variables: Configure the necessary environment variables to point to the cross-compilation toolchain. This ensures that your build system uses the cross-compiler and related tools from the toolchain instead of the default ones. The exact environment variables and their values depend on the specific cross-compilation toolchain you are using.

4. Write the build scripts: Create or modify your build scripts (e.g., Makefile, CMakeLists.txt) to use the cross-compiler and appropriate build settings. Update the build configurations to specify the target platform, architecture, and other relevant options required for cross-compilation.

5. Build the project: Execute your build scripts to trigger the cross-compilation process. The build system will use the cross-compilation toolchain to compile the code, link the libraries, and generate the binary executable for the target platform.

6. Test and deploy the binary: After successful cross-compilation, test the generated binary on the target platform to ensure it functions as expected. Transfer the binary to the target platform (e.g., Linux machine) and execute it to verify its compatibility and behavior.

Note that the specific steps and tools involved in cross-compilation may vary depending on the target platform and the cross-compilation toolchain you choose. It's recommended to consult the documentation and resources provided by the toolchain to get detailed instructions and best practices for cross-compiling on Windows.

Here's a basic example of cross-compiling a simple "Hello, World!" program for Linux using the MinGW-w64 cross-compilation toolchain on Windows:

1. Install MinGW-w64:
   - Download the MinGW-w64 installer from the official website: https://mingw-w64.org/doku.php/download
   - Run the installer and choose the appropriate architecture (e.g., x86_64 for 64-bit Linux).
   - Select the desired installation directory and complete the installation process.

2. Set up environment variables:
   - Add the MinGW-w64 binaries directory to the `PATH` environment variable. For example, if you installed MinGW-w64 in `C:\mingw-w64`, add `C:\mingw-w64\bin` to the `PATH` variable.

3. Write the C code:
   - Create a file named `hello.c` and place the following code inside:
   ```c
   #include <stdio.h>
   
   int main() {
       printf("Hello, World!\n");
       return 0;
   }
   ```

4. Cross-compile the code:
   - Open a command prompt or terminal.
   - Navigate to the directory containing `hello.c`.
   - Run the following command to compile the code using the MinGW-w64 cross-compiler:
     ```
     x86_64-w64-mingw32-gcc -o hello hello.c
     ```

5. Verify the generated binary:
   - The cross-compiled Linux binary named `hello` should be generated in the current directory.
   - Transfer the `hello` binary to a Linux machine or a Linux virtual machine.
   - Execute the binary on the Linux platform to verify the output:
     ```
     ./hello
     ```
     It should display:
     ```
     Hello, World!
     ```

This example demonstrates the basic steps involved in cross-compiling a simple program for Linux using the MinGW-w64 toolchain on Windows. You can adapt these steps and use other cross-compilation toolchains for different target platforms and project configurations.

----

## **How to cross-compile on linux?**

Cross-compiling on Linux involves setting up a cross-compilation toolchain that can generate binaries for a different target platform. Here's a general overview of the process:

1. Choose a cross-compilation toolchain: Identify and download a cross-compilation toolchain that is compatible with your target platform. Toolchains like Linaro, crosstool-ng, or Buildroot provide compilers, libraries, and other necessary components to build binaries for the target platform.

2. Install the cross-compilation toolchain: Follow the installation instructions provided by the chosen cross-compilation toolchain. This typically involves downloading and extracting the toolchain files to a specific directory.

3. Set up the environment variables: Configure the necessary environment variables to point to the cross-compilation toolchain. This ensures that your build system uses the cross-compiler and related tools from the toolchain instead of the default ones. The exact environment variables and their values depend on the specific cross-compilation toolchain you are using.

4. Write the build scripts: Create or modify your build scripts (e.g., Makefile, CMakeLists.txt) to use the cross-compiler and appropriate build settings. Update the build configurations to specify the target platform, architecture, and other relevant options required for cross-compilation.

5. Build the project: Execute your build scripts to trigger the cross-compilation process. The build system will use the cross-compilation toolchain to compile the code, link the libraries, and generate the binary executable for the target platform.

6. Test and deploy the binary: After successful cross-compilation, test the generated binary on the target platform to ensure it functions as expected. Transfer the binary to the target platform and execute it to verify its compatibility and behavior.

Note that the specific steps and tools involved in cross-compilation may vary depending on the target platform and the cross-compilation toolchain you choose. It's recommended to consult the documentation and resources provided by the toolchain to get detailed instructions and best practices for cross-compiling on Linux.

Additionally, some build systems like CMake or autotools have built-in support for cross-compilation. They provide mechanisms to specify the cross-compilation toolchain, target platform, and other configuration options directly in the build scripts, simplifying the cross-compilation process.

----

## **How to translate strings in a Qt application?**

In Qt, you can translate strings in a Qt application using the Qt Linguist tool and the Qt translation system. Here are the general steps to translate strings:

1. Mark strings for translation: In your application's source code, mark the strings that need to be translated using the `tr()` function or its variants. For example:
   ```cpp
   QLabel* label = new QLabel(tr("Hello, World!"));
   ```

2. Extract translatable strings: Use the `lupdate` tool provided by Qt to extract the translatable strings from your source code into a translation template (.ts) file. Open a terminal and navigate to your project directory, then run:
   ```bash
   lupdate myproject.pro
   ```
   This command will generate a .ts file (e.g., `myproject_en.ts`) that contains the extracted strings.

3. Create translations: Open the .ts file with Qt Linguist, a graphical translation editor that comes with Qt. You can open it by running `linguist` in the terminal or launching it from the Qt Creator IDE. In Linguist, you can provide translations for each string by entering the corresponding translated text in the target language.

4. Compile translations: After providing translations in Linguist, save the .ts file. Then, use the `lrelease` tool to compile the .ts file into a binary .qm file that can be loaded by your application at runtime. Run the following command in the terminal:
   ```bash
   lrelease myproject_en.ts
   ```
   This will generate a .qm file (e.g., `myproject_en.qm`).

5. Load translations in your application: In your application's code, load the translations at runtime using the `QTranslator` class. Load the .qm file for the target language using the `load()` method, and install the translator using `installTranslator()`. For example:
   ```cpp
   QTranslator translator;
   translator.load("myproject_en.qm");
   qApp->installTranslator(&translator);
   ```

6. Update UI elements: After loading the translator, the translated strings will be automatically used by Qt's internationalization system. UI elements like labels, buttons, and menus that are marked for translation will display the translated text based on the loaded translation.

Remember to repeat steps 2 to 6 for each language you want to support in your application, creating separate .ts and .qm files for each language.

By following these steps, you can enable string translation in your Qt application and provide translations for different languages.

----

## **UserHow to execute a python script in C++?**

To execute a Python script within a C++ program, you can use the `system()` function or the `popen()` function from the C standard library. Here's an example of how you can achieve this:

```cpp
#include <cstdlib>
#include <cstdio>

int main() {
    // Replace "python_script.py" with the path to your Python script
    const char* pythonScript = "python_script.py";

    // Using system() function
    const int exitCode = system("python " + std::string(pythonScript));
    if (exitCode == -1) {
        // Handle the error
    }

    // Using popen() function
    FILE* pipe = popen(("python " + std::string(pythonScript)).c_str(), "r");
    if (!pipe) {
        // Handle the error
    }

    char buffer[128];
    std::string result;
    while (fgets(buffer, sizeof(buffer), pipe) != nullptr) {
        result += buffer;
    }

    pclose(pipe);

    // Process the result if needed

    return 0;
}
```

In this example, the C++ program uses either the `system()` function or the `popen()` function to execute the Python script. The `system()` function runs the Python script as a separate process, while the `popen()` function allows you to capture the output of the Python script.

You should replace `"python_script.py"` with the actual path to your Python script. If Python is not in the system's `PATH`, you may need to provide the full path to the Python interpreter as well.

After executing the Python script, you can handle the result as needed. In the `popen()` example, the script's output is read line by line and stored in the `result` string.

Please note that using these functions may introduce security risks if the command or script being executed is based on user input. Ensure that you sanitize and validate any user-supplied input to prevent potential security vulnerabilities like code injection.

----

## **What are large C++ Open Source Projects to learn?**

1. **Boost** (https://www.boost.org/): Boost is a widely used collection of peer-reviewed libraries that extend the functionality of C++. It covers various domains like algorithms, containers, concurrency, and more.

2. **Qt** (https://www.qt.io/): Qt is a cross-platform application framework for developing user interfaces and applications. It provides a comprehensive set of libraries and tools for building desktop, mobile, and embedded applications.

3. **LLVM** (https://llvm.org/): LLVM is a compiler infrastructure project that provides a collection of modular and reusable compiler and toolchain components. It is used by various programming languages and offers a rich set of libraries and tools.

4. **OpenCV** (https://opencv.org/): OpenCV is an open-source computer vision library that provides a wide range of algorithms and tools for image and video processing. It is widely used in fields like robotics, augmented reality, and machine learning.

5. **Blender** (https://www.blender.org/): Blender is a popular open-source 3D creation suite that supports modeling, animation, rendering, and more. It is extensively used in the field of computer graphics and animation.

6. **CMake** (https://cmake.org/): CMake is a cross-platform build system that generates build files for various platforms and compilers. It is widely used in large C++ projects to manage the build process.

7. **FFmpeg** (https://www.ffmpeg.org/): FFmpeg is a powerful multimedia framework that provides libraries and tools for handling audio, video, and other multimedia formats. It is widely used in media-related applications and projects.

8. **PCL** (Point Cloud Library) (https://pointclouds.org/): PCL is an open-source library for 2D and 3D point cloud processing. It offers a wide range of algorithms and tools for point cloud manipulation, registration, filtering, and more.

9. **Mozilla Firefox** (https://www.mozilla.org/en-US/firefox/): The Firefox web browser is an open-source project with a large codebase written in C++. It covers various aspects of web browsing, including rendering, networking, security, and user interface. Exploring the Firefox codebase can provide insights into building complex applications and working with a large team.

10 **Bitcoin Core** (https://github.com/bitcoin/bitcoin): Bitcoin Core is the reference implementation of the Bitcoin cryptocurrency. It is written in C++ and covers the core functionalities of the Bitcoin protocol. Studying the Bitcoin Core codebase can deepen your understanding of networking, cryptography, and distributed systems.

----

## **Show that you are an c++ expert?**

To showcase your C++ knowledge and skills, you can work on various types of projects that demonstrate different aspects of the language and its applications. Here are some project ideas that can help you exhibit your C++ expertise:

1. **Game Development:** Develop a game using a C++ game engine like Unreal Engine or create your own game engine using C++. This project will involve graphics programming, physics simulations, AI algorithms, and real-time performance optimizations.

2. **Compiler or Interpreter:** Build a small-scale compiler or interpreter for a simple programming language using C++. This project will demonstrate your understanding of language parsing, syntax analysis, code generation, and optimization techniques.

3. **Networking Application:** Develop a networking application using C++ to implement protocols like HTTP, TCP/IP, or WebSocket. This project will showcase your understanding of socket programming, network protocols, and concurrent programming.

4. **Algorithmic Implementations:** Implement various algorithms and data structures in C++, such as sorting algorithms, graph algorithms, or machine learning algorithms. This project will highlight your understanding of algorithm design, complexity analysis, and efficient coding practices.

5. **Image Processing Application:** Create an image processing application using C++ and libraries like OpenCV. This project will demonstrate your skills in computer vision, image manipulation, and algorithm implementation.

6. **Embedded Systems Project:** Develop an embedded systems project using C++ to control hardware devices or sensors. This could involve robotics, home automation, or IoT applications. This project will exhibit your knowledge of low-level programming, device interfacing, and real-time constraints.

7. **Parallel Processing Project:** Implement a project that utilizes parallel processing techniques, such as multi-threading or GPU programming, to achieve improved performance. This project will demonstrate your understanding of concurrency, synchronization, and parallel algorithms.

8. **Library/Framework Development:** Build a reusable library or framework in C++ that solves a specific problem or provides functionality for other developers. This project will showcase your software design skills, API development, and code organization.

9. **High-Performance Computing:** Develop a project that utilizes C++ for high-performance computing, such as numerical simulations, scientific computing, or simulations of physical systems. This project will demonstrate your ability to optimize code for performance, utilize hardware resources efficiently, and handle large datasets.

Remember that the complexity and scope of the project should align with your skills and expertise. Start with smaller projects and gradually work your way up to more challenging ones as you gain confidence and experience in C++.

----

## **Work with C++ on Arduino?**

To use C++ on Arduino, you can follow these steps:

1. **Set up the Arduino IDE**: Download and install the Arduino Integrated Development Environment (IDE) from the official Arduino website (https://www.arduino.cc/en/software). The Arduino IDE provides a convenient environment for writing, compiling, and uploading code to Arduino boards.

2. **Create a new Arduino project**: Launch the Arduino IDE and create a new sketch by selecting "File" > "New". This will open a new blank sketch window.

3. **Write C++ code**: In the Arduino IDE, you can write C++ code within the `setup()` and `loop()` functions. The `setup()` function runs once at the beginning, and the `loop()` function runs repeatedly.

   ```cpp
   void setup() {
     // Initialization code
   }
   
   void loop() {
     // Code to be repeated
   }
   ```

   You can define variables, use control structures (if, for, while, etc.), and call functions within these functions.

4. **Upload code to Arduino**: Connect your Arduino board to your computer using a USB cable. Select the correct board and port under the "Tools" menu in the Arduino IDE. Then, click on the "Upload" button (or press Ctrl+U) to compile and upload your code to the Arduino board.

5. **Interact with Arduino hardware**: You can use various Arduino libraries and functions to interact with the hardware components connected to the Arduino board. These libraries provide functions to control digital and analog inputs/outputs, communicate with sensors and actuators, and more. You can include Arduino libraries at the beginning of your sketch.

   ```cpp
   #include <Arduino.h>
   #include <Wire.h>  // Example library
   
   void setup() {
     // Initialization code
     Wire.begin();  // Example library function
   }
   
   void loop() {
     // Code to be repeated
     int value = analogRead(A0);  // Example analog input
     // Perform actions based on the value
   }
   ```

6. **Compile and upload code**: After writing your C++ code, verify it by clicking on the "Verify" button (or press Ctrl+R) to compile the code without uploading it. Fix any errors if they occur. Once your code is error-free, click on the "Upload" button (or press Ctrl+U) to compile and upload your code to the Arduino board.

The Arduino IDE simplifies the process of using C++ on Arduino boards by providing a simplified programming environment and libraries specifically designed for Arduino. It takes care of the underlying build system, allowing you to focus on writing C++ code to interact with the hardware.

----

## **Work with C++ on the Raspberry Pi?**

Yes, you can program the Raspberry Pi with C++. The Raspberry Pi supports various programming languages, including C++, and provides the necessary tools and libraries to develop C++ applications. Here's an overview of how to program the Raspberry Pi with C++:

1. **Set up the Raspberry Pi**: Start by setting up your Raspberry Pi. Install the operating system (such as Raspbian) on an SD card and configure the Raspberry Pi to connect to the network.

2. **Install C++ Compiler**: By default, the Raspberry Pi comes with the GNU C++ compiler (`g++`) installed. However, you may need to update it to the latest version. Open a terminal on the Raspberry Pi and run the following command to install or update the `g++` compiler:

   ```bash
   sudo apt-get update
   sudo apt-get install g++
   ```

3. **Write C++ Code**: Use a text editor or an Integrated Development Environment (IDE) of your choice to write your C++ code. Create a new source code file with a `.cpp` extension and start writing your C++ program.

   ```cpp
   #include <iostream>
   
   int main()
   {
       std::cout << "Hello, Raspberry Pi!" << std::endl;
       return 0;
   }
   ```

4. **Compile and Run**: Open a terminal on the Raspberry Pi, navigate to the directory where your C++ code is saved, and use the `g++` compiler to compile the code into an executable. Run the following command to compile the code:

   ```bash
   g++ your_code.cpp -o your_program
   ```

   This will generate an executable file named `your_program`. Run the compiled program using the following command:

   ```bash
   ./your_program
   ```

5. **Interact with Raspberry Pi Hardware**: To interact with the Raspberry Pi's hardware, such as GPIO pins or peripheral devices, you can utilize libraries like WiringPi (http://wiringpi.com/) or pigpio (http://abyz.me.uk/rpi/pigpio/). These libraries provide C++ APIs to control various aspects of the Raspberry Pi's hardware.

   Before using these libraries, you may need to install them on your Raspberry Pi. Refer to their respective documentation for installation instructions and usage examples.

6. **Further Exploration**: As you gain familiarity with programming the Raspberry Pi using C++, you can explore more advanced topics and libraries. This includes using libraries like Boost, Poco, or OpenCV for specific functionalities, or accessing lower-level interfaces through system APIs or kernel modules.

Remember to refer to the documentation and resources available for the specific hardware or libraries you are using, as they may provide additional guidance and examples tailored to the Raspberry Pi platform.

----

## **Where do I find C++ exception handling and more?**

C++ exception handling features are defined and documented in the ISO/IEC Standard 14882, which is the international standard for the C++ programming language. The standard specifies the syntax, semantics, and behavior of the C++ language, including exception handling.

You can access the C++ standard documents from various sources, including:

1. Official ISO/IEC Standard: The official [ISO/IEC Standard documents can be purchased from the International Organization for Standardization (ISO)](https://www.iso.org/standard/74528.html) or the International Electrotechnical Commission (IEC) websites. The C++ standard is typically referred to as "ISO/IEC 14882" or "C++ Standard."

2. Online C++ Standard Reference: Several online references provide the C++ standard for free, such as [cppreference.com](https://en.cppreference.com/w/). These references offer a convenient way to access the standard documentation without purchasing the official documents. The exception handling features, including try-catch blocks, throw statements, and exception specifications, are documented in the C++ Standard Library section.

3. C++ Compiler Documentation: Compiler vendors often provide their own documentation, which includes information about the language features, including exception handling. You can refer to the documentation of the specific C++ compiler you are using, such as GCC, Clang, or Visual C++, to find details about exception handling and its implementation-specific aspects.

4. C++ Programming Books: Various C++ programming books cover exception handling extensively. These books often provide explanations, examples, and best practices related to exception handling. Some popular books on C++ programming that cover exception handling include ["The C++ Programming Language" by Bjarne Stroustrup](http://chenweixiang.github.io/docs/The_C++_Programming_Language_4th_Edition_Bjarne_Stroustrup.pdf) and ["Effective C++" by Scott Meyers](https://www.dsi.fceia.unr.edu.ar/downloads/informatica/info_II/c++/Effective%20C++%20+%20More%20Effective%20C++.pdf).

When referring to the C++ standard or any documentation source, it's important to consider the version of the standard you are targeting, as the C++ language evolves over time. The most recent version of the C++ standard at the time of writing this response is C++17, with C++20 and C++23 being the upcoming versions.

----

## **Best practices for security programming in C++?**

When it comes to security programming in C++, there are several best practices you should follow to enhance the security of your code. Here are some important considerations:

1. Input validation: Always validate and sanitize input from external sources (e.g., user input, network input) to prevent potential vulnerabilities such as buffer overflows, format string attacks, or SQL injection. Use secure input handling functions and validate data against expected ranges and formats.

2. Memory management: Properly manage memory to avoid vulnerabilities such as buffer overflows, use-after-free, or memory leaks. Use safe alternatives for memory manipulation functions (e.g., `strncpy_s`, `snprintf`) and follow best practices for dynamic memory allocation and deallocation (e.g., using smart pointers, RAII).

3. Secure coding practices: Follow secure coding practices such as avoiding the use of deprecated or unsafe functions (e.g., `gets`, `strcpy`), using secure string handling functions (`strncat_s`, `memcpy_s`), and avoiding insecure coding patterns (e.g., using hardcoded passwords, insecure cryptographic algorithms).

4. Input/output validation: Validate and sanitize data used for input/output operations (e.g., file I/O, network communication). Be cautious about the data read from files or received over the network to prevent attacks like directory traversal, file inclusion, or command injection.

5. Encryption and hashing: Use secure cryptographic algorithms and libraries for sensitive data encryption and hashing. Avoid implementing custom cryptographic algorithms, as they are prone to vulnerabilities. Follow recommended practices for key management, random number generation, and secure storage of sensitive information.

6. Error handling: Implement proper error handling and logging mechanisms to detect and respond to security-related issues. Avoid exposing detailed error messages or system information that could be exploited by attackers.

7. Secure communication: When transmitting data over the network, use secure communication protocols (e.g., HTTPS, SSL/TLS) to protect sensitive information from interception or tampering.

8. Secure coding reviews and testing: Conduct regular code reviews and security assessments to identify and fix vulnerabilities in your code. Perform thorough testing, including functional, integration, and security testing, to ensure the robustness and security of your software.

9. Stay updated: Keep track of security advisories, vulnerability reports, and updates for the libraries and frameworks you use. Stay informed about new security threats and apply patches or updates promptly.

Remember that security is a multi-layered approach, and no single practice can guarantee complete security. It's essential to adopt a proactive mindset, follow security best practices, and continuously enhance your knowledge about secure programming techniques and emerging threats.

----
