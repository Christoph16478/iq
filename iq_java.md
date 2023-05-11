# https://quescol.com/interview-preparation/core-java-interview-questions

**What do you understand by Class in Java?**

A class is a blueprint from which objects are created. We can also define it as it is a group of objects which
have common properties. This properties is set by class for all method and properties of class.

Class declaration have components mentioned below:

__Class name__

```java
class Person { // class name
    // Body of the class
}
```

[__Modifiers__](https://www.w3schools.com/java/java_modifiers.asp)

```java
public class Main
```

__Interface__

```java
// interface
interface Animal {
    public void animalSound(); // interface method (does not have a body)
    public void run(); // interface method (does not have a body)
}
```

__Super Class__

```java
class Vehicle { // Vehicle is the super class
    protected String brand = "Ford"; // Vehicle attribute
    public void honk() { // Vehicle method
        System.out.println("Tuut, tuut!");
    }
}

class Car extends Vehicle { // Car is the subclass
    private String modelName = "Mustang"; // Car attribute
    public static void main(String[] args) {

        // Create a myCar object
        Car myCar = new Car();

        // Call the honk() method (from the Vehicle class) on the myCar object
        myCar.honk();

        // Display the value of the brand attribute (from the Vehicle class) and the value of the modelName from the Car class
        System.out.println(myCar.brand + " " + myCar.modelName);
  }
}
```

__Methods__

```java
public class Main {
    static void myMethod() { //myMethod is the method name
        System.out.println("Hello World!");
    }
}
```

__Members__

```java
import java.io.*;
public class Employee {

    // this instance (member) variable is visible for any child class.
    public String name;

    // salary variable is visible in Employee class only.
    private double salary;

    // The name variable is assigned in the constructor.
    public Employee (String empName) {
        name = empName;
    }

    // The salary variable is assigned a value.
    public void setSalary(double empSal) {
        salary = empSal;
    }

    // This method prints the employee details.
    public void printEmp() {
        System.out.println("name  : " + name );
        System.out.println("salary :" + salary);
    }

    public static void main(String args[]) {
        Employee empOne = new Employee("Ransika");
        empOne.setSalary(1000);
        empOne.printEmp();
    }
}
```

__Constructor__

```java
// Create a Main class
public class Main {
    int x;  // Create a class attribute

    // Create a class constructor for the Main class
    public Main() {
        x = 5;  // Set the initial value for the class attribute x
    }

    public static void main(String[] args) {
        Main myObj = new Main(); // Create an object of class Main (This will call the constructor)
        System.out.println(myObj.x); // Print the value of x
    }
}
```

__Blocks__

```java
// Create a Main class
public class Main {
    int x;

    public Main() { // code block between curly brackets 
        x = 5; 
    }

    public static void main(String[] args) {
        Main myObj = new Main(); // Create an object of class Main (This will call the constructor)
        System.out.println(myObj.x); // Print the value of x
    }
}
```

__Nested Class__

```java
// Java program to demonstrate accessing
// a static nested class

// outer class
class OuterClass {
	// static member
	static int outer_x = 10;

	// instance(non-static) member
	int outer_y = 20;

	// private member
	private static int outer_private = 30;

	// static nested class
	static class StaticNestedClass {
		void display()
		{
			// can access static member of outer class
			System.out.println("outer_x = " + outer_x);

			// can access private static member of
			// outer class
			System.out.println("outer_private = "
							+ outer_private);

			// The following statement will give compilation
			// error as static nested class cannot directly
			// access non-static members
			// System.out.println("outer_y = " + outer_y);
		
			// Therefore create object of the outer class
			// to access the non-static member
			OuterClass out = new OuterClass();
			System.out.println("outer_y = " + out.outer_y);
		
		
		}
	}
}

// Driver class
public class StaticNestedClassDemo {
	public static void main(String[] args)
	{
		// accessing a static nested class
		OuterClass.StaticNestedClass nestedObject
			= new OuterClass.StaticNestedClass();

		nestedObject.display();
	}
}
```

__Nested Interface__

```java
// Java program to demonstrate working of
// interface inside a class.
import java.util.*;
class Test
{
	interface Yes
	{
		void show();
	}
}

class Testing implements Test.Yes
{
	public void show()
	{
		System.out.println("show method of interface");
	}
}

class A
{
	public static void main(String[] args)
	{
		Test.Yes obj;
		Testing t = new Testing();
		obj=t;
		obj.show();
	}
}
```

__Declaration of Class__ 

```java
// declaration of the class
class
{
    // body of the class
	field;
	method;
}
```

----

**What do you understand by Object?**

Object is a basic unit of OOPs. It is also an instance of a class. Everything in OOPs is
represented using Objects. In General we can define Object as it is a real world entity
that has its own some states and behaviour.

For Example: Cat is a suitable example of an objects. Cat has its own states and
behaviour and its is also a real world entity. Cat can walk, eat is its behaviour
and Cat can be white, black is its states.

Objects have some characteristics :

1). State : State Reflects the properties of Objects. Just like Cat can be white,
black or may be combination of both is its properties. State can be denoted by
attributes.

2). Behaviour : Behaviours shows that how object is responding to other objects.
Behaviour can be denoted by Methods.

3). Identity: Every objects should have unique identity. Like if we say cat
then it may be a group of cat but If we talk about a particular cat then we
need a identity for that particular cat.

---

**Explain JDK, JVM and JRE?**

JDK: JDK stands for Java Development Kit which contains JRE. It gives a
development environment for Java applications where developer can code and
run java programs.

JRE: JRE Stands for Java Runtime Environment that contains class libraries, loader class
and JVM. Its main function is to run Java Program. If you don’t want to develop program
then you don’t need JDK But, for only the purpose of execution of java program you only need
JRE. JRE comes with JDK bundle you don’t need to download it separately.

JVM: JVM stands for Java Virtual Machine that provide the runtime environment to java code
where Java code is executed. JVM is a part of JRE that converts java byte code into
machine code. In java, compiler produces code for JVM.

----

**Explain Public Static void Main(String args[]) in Java?**

It is an entry point of any Java program from where Execution starts.

Public: Public is a access modifier that define the accessibility of method. If any method have Public access modifier it means that it can access by any other class.

Static: static is a keyword in java that define class level member. It means that without
creating any instance it can be accessible using class name.

void: void is also a keyword that define the return type of any methods. If method have void
keyword it means that method will not return any value.

Main: It is a method from where execution starts. It is searched by JVM to start the execution.

String args[]: it is a main method argument.

---

What is the different between Final, finally and finilize?

Final:
final is a modifier which is used with classes, methods and variables. If the class is declared as final then that class is not extended by other class. If the method is declared as final then we cannot override that method in the child class. i.e. final method is not overridden by child class. If the variable is declared as final then it behave as a constant and we cannot re-assingment for that variable.

finally:
finally is a block which is always associated with try-catch block.finally block is always executed whether exception is handled or not.finally block is used to execute important code such as closing connection, stream when any exception arise.

finalize();
finalize() method is used to perform cleanup operation just before destroying any object. This finalize() method is always invoked by garbage collector. 

----

What is the difference between “==” and “equals()” method.

"==" is used for address/reference comparison.

Example:
String str1=new String("prakash");
String str2=new String("prakash");
System.out.println(str1==str2);
output: false

equals() is used for content comparision.

Example:

String str1=new String("prakash");
String Str2=new String("prakash");
System.out.println(str1.equals(str2));
output: true

----

Why Java is called as platform independent?

After the compilation of Java code, code is converted into byte code. This byte code
can be executed in any other system and environment. Because of that it is known as
platform independent.

---

What is meant by Local variable and Instance variable?

Local variables are defined in the method and scope of the variables that have existed
inside the method itself.

An instance variable is defined inside the class and outside the method and scope of the
variables exist throughout the class.

Oops Concept Interview Questions
Q1). Define Constructor.
Ans: We can define as constructor is a method or block which is use to initialise the objects. Constructor should have same name as a name of class which have no return type. It is automatically called by java at the time of object creation.

There are 3 types of constructor
1). Default constructor: It is automatically inserted by Java when we not declared any constructor. It is not visible in your source code.
2). Parameterised constructor : Constructor with arguments are known as Parameterised constructor.
3). No-arg Constructor : it is very similar to default constructor. We declare it when we want to perform some operation at a time of object creation then we write that code in no-args constructor. For example some initialization of value.

----

Explain access modifiers in Java?

Access modifiers is a keywords in Java that define the accessibility of any class, methods and member variables.

There are 4 types of access modifiers in Java:-

Public
Private
Protected
Default
Modifier	Default	Private	Protected	Public
Same class	YES	YES	YES	YES
Same Package subclass	YES	NO	YES	YES
Same Package non-subclass	YES	NO	YES	YES
Different package subclass	NO	NO	YES	YES
Different package non-subclass	NO	NO	NO	YES

----

Explain some features of oops?

Inheritance: Inheritance is process in which child objects of child class acquires the all properties and behaviour of its parent class. It improves the code reusability.

Abstraction: Abstraction means hide the complexity and show the functionality. For examples in education portal
you just sign up and then login by giving credential and then access your dashboard but you won’t aware of
how its happening in backend. It is known as abstraction.

Encapsulation: Encapsulation is a process of binding the data and methods together in a single entity
known as class for data safety.

Polymorphism: Polymorphism defines to perform single actions in multiple form. It is derived from two
word Poly + morphs that means many forms.

It is of two types:
Method overloading
Method Overriding

----

What is this and super keyword in Java?

this : this is a keyword is use to access the member of present class.
super : super keyword is used to access the member of parent class.

----

What is the different between static and non-static method of java?

Static method: static method is a class level method. We need not required any instance to access them we can access it directly using class. A static method can only access static variable.

non-static method: non-static method belongs to objects of the class. It can be accessible inside the static method with the help of class instance.

----

What do you mean by Polymorphism?

Polymorphism is derived from two greek word “poly” and “morphs” means many form. It allows to perform single task in multiple form. In Java term we can say that there can be multiple methods with same name but different functionality.

It is of two types:
1). Compile time polymorphism
2). Runtime Polymorphism

Compile time polymorphism is also known as method overloading and Runtime polymorphism is known as overriding.

----

Explain Method overloading and method overriding?

Method overloading: In method overloading a class have different methods with same name but different number of arguments. In Overloading case methods should have different signature. It is also known as compile time polymorphism.

Method Overriding: In Method Overriding sub class have similar method as parent class. Similar mean name, return type, parameter of methods for both parent and sub class method.

----

How many ways you can overload method?

1) By number of passing parameters the valid case for overloading the method is
add(int,int)
add(int,int,int)

2) By changing the data type of parameter
add(int,int)
add(float,int)

3) By changing the sequence of data type
add(int, float)
add(float,int)

----

What is the some invalid cases of method overloading in Java?

In java if two methods having the same name, same parameters but different return type,
then this is not a valid method overloading. Also if two methods having the same name,
same parameters and different return type, then this is also not a valid method
overloading. This will throw compilation error.

Example:
int sum(int,int)
float sum(int,int)

----

What do you mean by abstract class?

Abstract class is declared with the help of Abstract Keyword. It can have both abstract and non-abstract method. We cannot instantiate abstract method. It is extended by another class which can implement its methods to use. It can have static and final methods.

----

What do you mean by Interface?

Interface is a blueprint of class that have abstract and public methods without body. Class that implements interface should implement all methods of interface.

public interface Man
{
	public void eat();
	public void sleep();
	public void walk();
}

Java String Interview Questions

Difference between String and StringBuffer.

String: String object is immutable but the StringBuffer objects are mutable.
Immutable means once we create a String object we cannot perform any changes
on object.

Example of String:

String str=new String("prakash");
str.concat("kumar");
System.out.println(str);
output:- prakash

Example of StringBuffer:

StringBuffer strbfr=new StringBuffer("prakash");
strbfr.append("kumar");
System.out.println(strbfr);
output:- prakash kumar

----

Difference between StringBuffer and StringBuilder?

Ans: Both StringBuffer and StringBuilder are mutable.

StringBuffer:
All method of StringBuffer is synchronized. As it is synchronized, it is also thread-safe.

Thread-Safe means two threads can’t call the StringBuffer method simultaneously. Its performance is low because every task is dependent on the other.

Example:

StringBuffer strbuffer = new StringBuffer("java"); 
strbuffer.append("developer"); 
System.out.println(strbuffer); 

StringBuilder:
Methods are not synchronized so it is not thread-safe. It means two threads can call the string builder method simultaneously. Its performance is high because more than one thread can be allowed.

Example:

StringBuilder strBuilder=new StringBuilder("java"); 
strBuilder.append("developer"); 
System.out.println(strBuilder);

----

Difference between String, StringBuilder, and StringBuffer.

Factor

String

StringBuilder

StringBuffer

Storage Area

Constant String Pool

Heap Area

Heap Area

Mutability

Immutable

Mutable

Mutable

Thread Safety

Yes

No

Yes

Performance

Fast

More efficient

Less efficient

----

Difference between Array and ArrayList?

Arrays:
Array is fixed in size which is decided at a time of array declaration.
Array can contain both primitives data and objects.
Example:
int arr[] = new int[3];
arr[0]=10; 
arr[1]=20; 
arr[2]=70;
Arrays.stream(arr).forEach(e->System.out.print(e + " "));

ArrayList:
Size of ArrayList is dynamic.
It is a part of the collection framework of java.
ArrayList can contain the only object. After Java 5 It converts primitive data into object itself.
ArrayList<Integer> arrList = new ArrayList<Integer>(3);
for (int i = 1; i <= 3; i++)
  arrList.add(i);
arrList.stream().forEach(e->System.out.print(e + " ")); 

----

What do you mean by Collections in Java?

Collection is a Java framework that have some predefined class and interfaces to store and manipulate the group of objects.

Interfaces comes with Collection framework:
Set
List
Queue
Dequeue
Classes comes with Collection framework:

ArrayList
LinkedList
HashSet
TreeSet
LinkedHashSet etc.

Explain the lists that are present in Java Collection?
Types of Lists are:

1). ArrayList
Fast iteration and fast Random Access
It is an ordered collection.
It is not sorted collection.
Example:
Output:
[Dog, Cat, Donkey, Cow]

2). Linked List
Performance is slow than ArrayList.
Maintain the Insertion Order.
It can have duplicate values
Output:
[Dog, Cat, Donkey, Cow]

3). Vector
Similar as ArrayList.
Maintain the Insertion Order.
It can have duplicate values.
Its Methods are Synchronized.
Output:
[Dog, Cat, Donkey, Cow]

----

Explain the Set and their types in a Java Collection?

Set cares of uniqueness, It means that it does not allow duplicate value.


Types of Set in Java Collection are:

1). Hash Set

HashSet is unordered and unsorted.
It uses the hash code of the object to insert the values.
We can use Hash Set when order is not concerned and we want no duplicate value.
Example:

Output:

[Dog, Cat, Donkey, Cow]

2). Linked Hash set

It maintains the insertion order.
Does not allows duplicate value.
It can be used when iteration order is required.
Output:

[Dog, Cat, Donkey, Cow]

3). Tree Set

It sorts the elements in ascending order.
It does not allow duplicate values.
Output:

[Dog, Cat, Donkey, Cow]

Q5). Difference between HashMap and HashTable
Ans:

HashMap	HashTable
1. HashMap is non synchronized	1. HashTable is synchronized
2. HashMap allows NULL Key and Value.	2. HashTable does not allows any NULL Key and Value.
3. Performance of HashMap is fast.	3. HashTable is slow.
4. HashMap inherits class AbstractMap.	4. HashTable inherits class Dictionary.
5. We can traverse HashMap using Iterator.	5. We can traverse HashTable using Iterator and Enumerator.
Q6). Difference between HashSet and TreeSet.
Ans:

HashSet	TreeSet
1. HashSet is faster and gives better performace.	1. TreeSet is little bit slower than HashSet.
2. HashSet performs operation in constant time	2. TreeSet performs operation in Log(n) time.
3. HashSet does not follow any order	3. TreeSet elements are arranged in ascending order.
4. HashSet does not hold duplicate value.	4. TreeSet also does not hold duplicate value.
Q7). Difference between Collection and Collections in Java.
Ans:


Collection:

The collection is an interface in Java. It represents a group of individual objects as a single unit. 

After java8, Collection can contain a static method. and abstract and default method.

Collections:

The collections is a utility class in Java. It defines several utility methods that are used to operate on collection.

Collections includes only static methods. 

</https://quescol.com/interview-preparation/core-java-interview-questions>

<https://www.simplilearn.com/tutorials/java-tutorial/java-interview-questions>

----

What are the differences between C++ and Java?

Concept.
C++ is not platform-independent; the principle behind C++ programming is “write once, compile anywhere.”
In contrast, because the byte code generated by the Java compiler is platform-independent, it can run on any
machine, Java programs are written once and run everywhere.

Languages Compatibility.
C++ is a programming language that is based on the C programming language. Most other high-level languages are
compatible with C++. Most of the languages of Java are incompatible. Java is comparable to those of C and C++.

Interaction with the library.
It can access the native system libraries directly in C++. As a result, it’s better for programming at the system level.
Java’s native libraries do not provide direct call support. You can use Java Native Interface or access the libraries.

Characteristics.
C++ distinguishes itself by having features that are similar to procedural and object-oriented languages.
The characteristic that sets Java apart is automatic garbage collection. Java doesn’t support destructors
at the moment.

The semantics of the type.
Primitive and object types in C++ have the same kind of semantics. The primitive and object and classes of Java, on the other hand, are not consistent.

In the context of Compiler and Interpreter.
Java refers to a compiled and interpreted language. In contrast, C++ is only a compiled language.

In Java, the source code is the compiled output is a platform-independent byte code.
In C++, the source program is compiled into an object code that is further executed to produce an output.

----

List the features of the Java Programming language?

A few of the significant features of Java Programming Language are:
Easy: Java is a language that is considered easy to learn. One fundamental concept of OOP Java has a
catch to understand.
Secured Feature: Java has a secured feature that helps develop a virus-free and tamper-free system for the users.
OOP: OOP stands for Object-Oriented Programming language. OOP signifies that, in Java, everything is considered
an object.
Independent Platform: Java is not compiled into a platform-specific machine; instead, it is compiled into
platform-independent bytecode. This code is interpreted by the Virtual Machine on which the platform runs.

----

What do you get in the Java download file? How do they differ from one another?

We get two major things along with the Java Download file. 

JDK - Java Development Kit
JRE - Java Runtime Environment

JDK
JRE

Abbreviation for JavaDevelopment Kit
Abbreviation for Java Runtime Environment

JDK is a dedicated kit for solely software development
JRE is a set of software and library designed for executing Java Programs

Unlike JVM, JDK is Platform Dependent
Unlike JVM, JRE is also Platform Dependent

JDK package is a set of tools for debugging and Developing
JRE Package is one that only supports files and libraries for a runtime environment 

JDK package will be provided with an installer file
JRE Package does not get an installer but has only a runtime environment

----

What is a ClassLoader?

A classloader in Java is a subsystem of Java Virtual Machine, dedicated to loading class files when a program is executed; ClassLoader is the first to load the executable file.

Java has Bootstrap, Extension, and Application classloaders.

Also Read: What is Bootstrap and How to Embed Bootstrap into Angular?

----

What are the Memory Allocations available in Java?

Java has five significant types of memory allocations.

Class Memory
Heap Memory
Stack Memory
Program Counter-Memory
Native Method Stack Memory

----

What are the differences between Heap and Stack Memory in Java?

Stack memory in data structures is the amount of memory allocated to each individual programme. It is a
fixed memory space. Heap memory, in contrast, is the portion that was not assigned to the Java code but
will be available for use by the Java code when it is required, which is generally during the program's runtime.

----

Will the program run if we write static public void main?

Yes, the program will successfully execute if written so. Because, in Java, there is no specific rule
for the order of specifiers

----

What is the default value stored in Local Variables?

Neither the Local Variables nor any primitives and Object references have any default
value stored in them. 

----

Explain the expected output of the following code segment?

public class Simplilearn   
{  
    public static void main (String args[])   
{

System.out.println(100 + 100 +“Simplilearn");   
System.out.println(“E-Learning Company" + 100 + 100);  

The answers for the two print statements are as follows.

200Simplilearn
E-Learning Company100100

Why? Missing instantiation of the class. 

----

What is an Association?

An Association can be defined as a relationship that has no ownership over another.
For example, a person can be associated with multiple banks, and a bank can be related
to various people, but no one can own the other.

----

What do you mean by aggregation?

The term aggregation refers to the relationship between two classes best described as a “whole/part” and “has-a” relationship. This kind is the most specialized version of an association relationship. It contains the reference to another class and is said to have ownership of that class.

----

Define Copy Constructor in Java?

A Copy Constructor in Java is a constructor that initializes an object through another object of the same class.

----

What is a Marker Interface?

An empty interface in Java is referred to as a Marker interface. Serializable and Cloneable are
some famous examples of Marker Interface. 

----

What is Object Cloning?

An ability to recreate an object entirely similar to an existing object is known as Object
Cloning in Java. Java provides a clone() method to clone a current object offering the same
functionality as the original object.

----

Can Java be said to be the complete object-oriented programming language?

No, Java cannot be treated as a complete object-oriented programming language.

----

What is an object-oriented paradigm?

A Paradigm that is based on the concepts of “Objects.” It contains data and code. Data that is
in the form of fields, and regulation, that is in the form of procedures. The exciting feature
of this paradigm is that the object’s procedures can access and often modify the data
fields themselves.

----

Define Wrapper Classes in Java?

In Java, when you declare primitive datatypes, then Wrapper classes are responsible for converting
them into objects(Reference types). 

----

What is a singleton class in Java? And How to implement a singleton class?

A class that can possess only one object at a time is called a singleton class. To implement a singleton
class given steps are to be followed:

* Make sure that the class has only one object
* Give global access to that object

----

Define package in Java?

The package is a collective bundle of classes and interfaces and the necessary libraries and JAR files.
The use of packages helps in code reusability.

---

Can you implement pointers in a Java Program?

Java Virtual Machine takes care of memory management implicitly. Java's primary motto was to keep
programming simple. So, accessing memory directly through pointers is not a recommended action.
Hence, pointers are eliminated in Java. 

----

Differentiate between instance and local variables?

For instance, variables are declared inside a class, and the scope of variables in javascript is
limited to only a specific object.

A local variable can be anywhere inside a method or a specific block of code. Also, the scope
is limited to the code segment where the variable is declared. 

----

Explain Java String Pool

A collection of strings in Java's Heap memory is referred to as Java String Pool. In case you try
to create a new string object, JVM first checks for the presence of the object in the pool. If
available, the same object reference is shared with the variable, else a new object is created.

----

What is an Exception?

An Exception handling in Java is considered an unexpected event that can disrupt the program's
normal flow. These events can be fixed through the process of Exception Handling.

----

What is the final keyword in Java?

The term final is a predefined word in Java that is used while declaring values to variables.
When a value is declared using the final keyword, then the variable's value remains constant
throughout the program's execution.

----

What happens when the main() isn't declared as static?

When the main method is not declared as static, then the program may be compiled correctly but ends
up with a severe ambiguity and throws a run time error that reads "NoSuchMethodError."

----

Why is Java a platform independent language?

One of the most well-known and widely used programming languages is Java. It is a programming
language that is independent of platforms. Java doesn't demand that the complete programme be
rewritten for every possible platform. The Java Virtual Machine and Java Bytecode are used to
support platform independence. Any JVM operating system can run this platform-neutral byte code.
The application is run after JVM translates the byte code into machine code. Because Java
programmes can operate on numerous systems without having to be individually rewritten for
each platform, the language is referred to as "Write Once, Run Anywhere" (WORA).

----

Why is the main method static in Java?

Java's main() function is static by default, allowing the compiler to call it either before or after creating a class object. The main () function is where the compiler begins programme execution in every Java programme. Thus, the main () method needs to be called by the compiler. If the main () method is permitted to be non-static, the JVM must instantiate its class when calling the function. 

----

What part of memory - Stack or Heap - is cleaned in the garbage collection process?

On Heap memory, garbage collection is employed to release the memory used by objects with no references. Every object created in the Heap space has access to the entire application and may be referred to from anywhere.

----

What is the difference between the program and the process?

A programme is a non-active entity that includes the collection of codes necessary to carry out a specific operation. When a programme is run, an active instance of the programme called a process is launched. A process is begun by a programme once it has been run. The process carries out the program's specified instructions.

----

What are the differences between constructor and method of a class in Java?

Initializing the state of the object is done by constructors. A function Object () { [native code] }, like methods, contains a group of statements (or instructions) that are carried out when an object is created. A method is a group of statements that work together to complete a certain task and return the outcome to the caller. A method has the option of working without returning anything.

----

Which among String or String Buffer should be preferred when there are a lot of updates required to be done in the data?

Because StringBuilder is quicker than StringBuffer, it is advised to utilize it wherever possible. However, StringBuffer objects are the best choice if thread safety is required.

----

What happens if the static modifier is not included in the main method signature in Java?

The main function is called by the JVM even before the objects are created, thus even if the code correctly compiles, there will still be an error at runtime.

----

Can we make the main() thread a daemon thread?

This technique designates whether the active thread is a user thread or a daemon thread. For instance, tU.setDaemon(true) would convert a user thread named tU into a daemon thread. On the other side, executing tD.setDaemon(false) would convert a Daemon thread, tD, into a user thread.

----

What happens if there are multiple main methods inside one class in Java?

There is no limit to the number of major approaches you can use. Overloading is the ability to have main methods with different signatures than main (String []), and the JVM will disregard those main methods.

----

How does an exception propagate in the code?

In the event that an exception is not caught, it is initially thrown from the top of the stack and then moves down the call stack to the preceding method. The runtime system looks for a way to handle an exception that a method throws. The ordered list of methods that were called to get to the method where the error occurred is the collection of potential "somethings" that can be used to manage the exception. The call stack is the list of methods, and exception propagation is the search technique.

----

How do exceptions affect the program if it doesn't handle them?

If you don't deal with an exception once it occurs, the programme will end abruptly and the code after the line where the exception occurred won't run.

----

Is it mandatory for a catch block to be followed after a try block?

Each attempt block does not necessarily have to be followed by a catch block. Either a catch block or a final block ought to come after it. Additionally, any exceptions that are expected to be thrown should be mentioned in the method's throws clause.

----

Can you call a constructor of a class inside another constructor?

Yes, a class may include any number of constructors, and each function Object () {[native code] } may call the others using the this() function Object() { [native code] } call function [please do not mix the this() function Object() { [native code] } call function with this keyword]. The constructor's first line should be either this () or this(args). Overloading of constructors is what this is called.

----

Contiguous memory locations are usually used for storing actual values in an array but not in ArrayList. Explain?

Primitive data types like int, float, and others are typically present in an array. In such circumstances, the array immediately saves these elements at contiguous memory regions. While an ArrayList does not contain primitive data types. Instead of the actual object, an ArrayList includes the references to the objects' many locations in memory. The objects are not kept in consecutive memory regions because of this.

----

Why does the java array index start with 0?

The distance from the array's beginning is just an offset. There is no distance because the first element is at the beginning of the array. Consequently, the offset is 0.

----

Why is the remove method faster in the linked list than in an array?

Because there is no background scaling of an array, insertion, addition, and removal operations are quicker with a LinkedList. Only references in adjacent items need to update when a new item is added in the middle of the list.

----

How many overloaded add() and addAll() methods are available in the List interface? Describe the need and uses.

List is an interface in the Java Collections Framework. The add() and addAll() methods      are the main methods at the List interface. The add() method is used to add an element to the list, while the addAll() method is used to add a collection of elements to the list.

The List interface contains two overloaded versions of the add() method:

The first add() method accepts a single argument of type E, the element to be added to the list.

The second add() method accepts a variable number of arguments of type E, which are the elements to be added to the list.

The List interface also contains two overloaded versions of the addAll() method:

The first addAll() method accepts a single argument of type Collection<? Extends E>, which is the collection of elements to be added to the list.

The second addAll() method accepts a variable number of arguments of type E, which are the elements to be added to the list.

----

How does the size of ArrayList grow dynamically? And also state how it is implemented internally?

A resizable array implementation in Java is called ArrayList. Dynamically expanding array lists make it
possible to add new elements at any time. The underlying data structure of the ArrayList is an array of
the Object class. The ArrayList class in Java has three constructors. There are available readObject
and writeObject methods specific to it. The Object Array in an ArrayList is temporary. There are
implemented and Serialization-capable versions of RandomAccess, Cloneable, and java.io (that are Marker Interface in Java).

----

Although inheritance is a popular OOPs concept, it is less advantageous than composition. Explain.

A class's testability is improved through composition over inheritance. If a class is comprised of another class,
it is simple to create a mock object to simulate the combined class for testing purposes. This privilege is not
given by inheritance. Even while Composition and Inheritance both let you reuse code, Inheritance has the
drawback of breaking encapsulation. If the function of the subclass depends on the superclass's action,
it suddenly becomes vulnerable. Sub-class functionality may be broken without any alteration on the part
of the super-class when its behaviour changes.

----

45. What are Composition and Aggregation? State the difference.
Aggregation (HAS-A) and composition are its two forms (Belongs-to). In contrast to composition, which has a significant correlation, the aggregation has a very modest association. Aggregation can be thought of as a more confined version of the composition. Since all compositions are aggregates but not all aggregates are compositions, aggregate can be thought of as the superset of composition.

----

46. How is the creation of a String using new() different from that of a literal?
The new () operator always produces a new object in heap memory when creating a String object. The String pool may return an existing object if we build an object using the String literal syntax, such as "Baeldung," on the other hand.

----

47. How is the ‘new' operator different from the ‘newInstance()' operator in java?
Both the new operator and the newInstance() method are used to create objects in Java. If we already know the kind of object to create, we can use the new operator; however, if the type of object to create is supplied to us at runtime, we must use the newInstance() function.

----

48. Is exceeding the memory limit possible in a program despite having a garbage collector?
Yes, even with a garbage collector in place, the programme could still run out of memory. Garbage collection aids in identifying and removing programme objects that are no longer needed in order to release the resources they use. When an object in a programme cannot be reached, trash collection is executed with respect to that object. If there is not enough memory available to create new objects, a garbage collector is used to free up memory for things that have been removed from the scope. When the amount of memory released is insufficient for the creation of new objects, the program's memory limit is exceeded.

----

49. Why is synchronization necessary? Explain with the help of a relevant example.
Multiple threads trying to access the same resources in a multi-threaded software may frequently result in unexpected and incorrect outcomes. Therefore, it must be ensured through some form of synchronization that only one thread can access the resource at any given time. Java offers a method for setting up threads and synchronizing their operations with the aid of synchronized blocks. The synchronized keyword in Java is used to identify synchronized blocks. In Java, a synchronized block is one that is tied to an object. Only one thread can be running at a time inside synchronized blocks since they are all synchronized on the same object. Until the thread inside the synchronized block exits the block, all other threads trying to enter the block are blocked. 

----

50. Define System.out.println().
System.out.println() in Java outputs the argument that was supplied to it. On the monitor, the println() method displays the findings. An objectname is typically used to call a method.

FREE Java Certification Training
Learn A-Z of Java like never beforeENROLL NOWFREE Java Certification Training

----

51. Can you explain the Java thread lifecycle?
A thread can be in any of the following states in Java. These are the states:

New: A new thread is always in the new state when it is first formed. The function hasn't been run yet, thus it hasn't started to execute for a thread in the new state.
Active: A thread switches from the new state to the active state when it calls the start() method. The runnable state and the running state are both contained within the active state.
Blocked or Waiting: A thread is either in the blocked state or the waiting state when it is inactive for a while (but not indefinitely).
Timed waiting: When we use the sleep () method on a particular thread, we are actually engaging in timed waiting. The thread enters the timed wait state using the sleep () function. The thread awakens when the allotted time has passed and resumes execution where it left off.
Termination: A thread that has been terminated means it is no longer active in the system. In other words, the thread is inactive and cannot be revived (made active again after being killed).
52. What could be the tradeoff between the usage of an unordered array versus the usage of an ordered array?
When opposed to an unordered array, which has a time complexity of O, an ordered array's search times have a time complexity of O(log n) (n). Due to the need to shift the elements with higher values to create room for the new member, an ordered array has a temporal complexity of O(n) during the insertion process. Instead, an unordered array's insertion operation requires a constant O amount of time (1).

----

53. Is it possible to import the same class or package twice in Java and what happens to it during runtime?
The same package or class may be imported more than once. Neither the JVM nor the compiler raise an objection. Even if you import the same class several times, the JVM will only internally load it once.

----

54. In case a package has sub packages, will it suffice to import only the main package? e.g. Does importing of com.myMainPackage.* also import com.myMainPackage.mySubPackage.*?
Sub-packages won't be imported when a package is imported. When you import a package, all of its classes and interfaces—with the exception of those from its sub-packages—are imported.

----

55. Will the final block be executed if the code System.exit(0) is written at the end of the try block?
The system is established as the last line to be run, after which nothing will happen, therefore both the catch and finally blocks are essentially ignored.

----

56. Explain the term “Double Brace Initialisation” in Java?
The outer braces of the double-brace initialization construct an anonymous class that is descended from the provided class and gives an initializer block for that class (the inner braces).

----

57. Why is it said that the length() method of String class doesn't return accurate results?
Since this char [] array is used by the Java String class internally, the length variable cannot be made public.

----

58. What are the possible ways of making objects eligible for garbage collection (GC) in Java?
If a reference variable for an object is removed from the programme while it is running, the object may be trash collected. They are also referred to as inaccessible objects occasionally.  The new operator returns a reference to an object after dynamically allocating memory for it.

----

59. In the below Java Program, how many objects are eligible for garbage collection?
I don't know about the program, but generally, three objects are eligible for garbage collection. 

The first object is created when the program is started and is no longer needed when the program ends. 

The second object is created when the user inputs their name and is no longer required when the program ends. 

The third object is created when the user inputs their address and is no longer needed when the program ends.

60. What is the best way to inject dependency? Also, state the reason.
Constructor injection. A class requesting its dependencies through its function Object() { [native code] } is the most typical instance of dependency injection. Since the client cannot be constructed without the required dependencies, this guarantees that it is always in a correct state.

----

61. How we can set the spring bean scope. And what supported scopes does it have?
There are four ways to set the scope of a Spring bean: singleton, prototype, request, and session.

The singleton scope creates a single instance of a bean, which is shared by all objects that request it. 

The prototype scope creates a new instance of a bean for each object that requests it.

The request and session scopes are only available in a web-based context. The request scope creates a new bean instance for each HTTP request, and the session scope creates a single instance of a bean shared by all objects in a single HTTP session.

----

62. What are the different categories of Java Design patterns?
The three categories of Java design patterns are creational, structural, and behavioural design patterns.

----

63. What is a Memory Leak? Discuss some common causes of it.
A memory leak is the slow degradation of system performance over time brought on by the fragmentation of a computer's RAM as a result of shoddy application design or programming that fails to release memory chunks when they are no longer required. These memory leaks frequently result from session items in excess, insertion into Collection objects without deletion, infinite caches, excessive page switching on the operating system, listener methods that are not called, and bespoke data structures that are poorly written.

----

64. Assume a thread has a lock on it, calling the sleep() method on that thread will release the lock?
No, the thread might release the locks using notify, notifyAll(), and wait() methods.

----

65. Write a Java Program to print Fibonacci Series using Recursion.
class FibonacciExample2{  

 static int n1=0,n2=1,n3=0;    

 static void printFibonacci(int count){    

    if(count>0){    

         n3 = n1 + n2;    

         n1 = n2;    

         n2 = n3;    

         System.out.print(" "+n3);   

         printFibonacci(count-1);    

     }    

 }    

 public static void main(String args[]){    

  int count=10;    

  System.out.print(n1+" "+n2);//printing 0 and 1    

  printFibonacci(count-2);//n-2 because 2 numbers are already printed   

 }  

 }  

----

66. Write a Java program to check if the two strings are anagrams.
import java.util.Arrays;     

public class AnagramString {  

    static void isAnagram(String str1, String str2) {  

        String s1 = str1.replaceAll("\\s", "");  

        String s2 = str2.replaceAll("\\s", "");  

        boolean status = true;  

        if (s1.length() != s2.length()) {  

            status = false;  

        } else {  

            char[] ArrayS1 = s1.toLowerCase().toCharArray();  

            char[] ArrayS2 = s2.toLowerCase().toCharArray();  

            Arrays.sort(ArrayS1);  

            Arrays.sort(ArrayS2);  

            status = Arrays.equals(ArrayS1, ArrayS2);  

        }  

        if (status) {  

            System.out.println(s1 + " and " + s2 + " are anagrams");  

        } else {  

            System.out.println(s1 + " and " + s2 + " are not anagrams");  

        }  

    }  

    public static void main(String[] args) {  

        isAnagram("Keep", "Peek");  

        isAnagram("Mother In Law", "Hitler Woman");  

    }  

}  

Output

Keep and Peek are anagrams

MotherInLaw and HitlerWoman are anagrams

----

67. Write a Java Program to find the factorial of a given number.
4! = 4*3*2*1 = 24  

5! = 5*4*3*2*1 = 120  

----

68. Given an array of non-duplicating numbers from 1 to n where one number is missing, write an efficient java program to find that missing number.
Input: arr[] = {1, 2, 4, 6, 3, 7, 8}, N = 8

             Output: 5

            Explanation: The missing number between 1 to 8 is 5

----

69. Write a Java Program to check if any number is a magic number or not. A number is said to be a magic number if after doing the sum of digits in each step and in turn doing the sum of digits of that sum, the ultimate result (when there is only one digit left) is 1.
  // Java program to check if

// a number is Magic number.

class GFG

{

public static boolean isMagic(int n)

{

            int sum = 0;        

            // Note that the loop continues

            // if n is 0 and sum is non-zero.

            // It stops when n becomes 0 and

            // sum becomes single digit.

            while (n > 0 || sum > 9)

            {

                           if (n == 0)

                           {

                                          n = sum;

                                          sum = 0;

                           }

                           sum += n % 10;

                           n /= 10;

            }

           

            // Return true if sum becomes 1.

            return (sum == 1);

}

// Driver code

public static void main(String args[])

            {

            int n = 1234;

            if (isMagic(n))

                           System.out.println("Magic Number");

                          

            else

                           System.out.println("Not a magic Number");

            }

}

class InvalidAgeException  extends Exception  

{  

    public InvalidAgeException (String str)  

    {  

// calling the constructor of parent Exception  

        super(str);  

    }  

}  

----

70. Write a Java program to create and throw custom exceptions.
// class that uses custom exception InvalidAgeException  

public class TestCustomException1  

{  

    // method to check the age  

    static void validate (int age) throws InvalidAgeException{    

       if(age < 18){  

        // throw an object of user defined exception  

        throw new InvalidAgeException("age is not valid to vote");    

    }  

       else {   

        System.out.println("welcome to vote");   

        }   

     }    

    // main method  

    public static void main(String args[])  

    {  

        try  

        {  

            // calling the method   

            validate(13);  

        }  

        catch (InvalidAgeException ex)  

        {  

            System.out.println("Caught the exception");  

    

            // printing the message from InvalidAgeException object  

            System.out.println("Exception occured: " + ex);  

        }  

        System.out.println("rest of the code...");    

    }  

}  

----

71. Write a Java program to rotate arrays 90 degree clockwise by taking matrices from user input.
public class RotateMatrixClockwise  

{  

public static void main(String args[])  

{  

//matrix to rotate   

int a[][]= {{1,2,3},{4,5,6},{7,8,9}};    

System.out.println("Original Matrix: \n");  

//loop for rows  

for(int i=0;i<3;i++)  

{  

//loop for columns  

for(int j=0;j<3;j++)  

{  

//prints the elements of the original matrix  

System.out.print(" "+a[i][j]+"\t");  

}  

System.out.println("\n");  

}  

System.out.println("Rotate Matrix by 90 Degrees Clockwise: \n");  

for(int i=0;i<3;i++)  

{  

for(int j=2;j>=0;j--)  

{  

//prints the elements of the rotated matrix  

System.out.print(""+a[j][i]+"\t");  

}  

System.out.println("\n");  

}  

}  

}   

----

72. Write a java program to check if any number given as input is the sum of 2 prime numbers.        
// C program to check if a prime number

// can be expressed as sum of

// two Prime Numbers

#include <stdio.h>

#include <math.h>

#include <stdbool.h>

// Function to check whether a number

// is prime or not

bool isPrime(int n)

{

            if (n <= 1)

                           return false;

            for (int i = 2; i <= sqrt(n); i++)

            {

                           if (n % i == 0)

                                          return false;

            }

            return true;

}

// Function to check if a prime number

// can be expressed as sum of

// two Prime Numbers

bool isPossible(int N)

{

            // if the number is prime,

            // and number-2 is also prime

            if (isPrime(N) && isPrime(N - 2))

                           return true;

            else

                           return false;

}

// Driver code

int main()

{

            int n = 13;

 

            if (isPossible(n))

                           printf("%s", "Yes");

            else

                           printf("%s", "No");

 

            return 0;

}

----

73. Write a Java program for solving the Tower of Hanoi Problem.
 // Java recursive program to solve tower of hanoi puzzle

class GFG

{

            // Java recursive function to solve tower of hanoi puzzle

            static void towerOfHanoi(int n, char from_rod, char to_rod, char aux_rod)

            {

                           if (n == 1)

                           {

                                          System.out.println("Move disk 1 from rod " + from_rod + " to rod " +to_rod);

                                          return;

                           }

                           towerOfHanoi(n-1, from_rod, aux_rod, to_rod);

                           System.out.println("Move disk " + n + " from rod " + from_rod + " to rod " +to_rod);

                           towerOfHanoi(n-1, aux_rod, to_rod, from_rod);

            }     

            // Driver method

            public static void main(String args[])

            {

                           int n = 4; // Number of disks

                           towerOfHanoi(n, \'A\', \'C\', \'B\'); // A, B and C are names of rods

            }

}

----

74. Implement Binary Search in Java using recursion.
// Java Program to Illustrate Recursive Binary Search

// Importing required classes

import java.util.*;

// Main class

class GFG {

            // Method 1

            // Recursive binary search

            // Returns index of x if it is present

            // in arr[l..r], else return -1

            int binarySearch(int arr[], int l, int r, int x)

            {

                           // Restrict the boundary of right index

                           // and the left index to prevent

                           // overflow of indices

                           if (r >= l && l <= arr.length - 1) {

                                          int mid = l + (r - l) / 2;

                                          // If the element is present

                                          // at the middle itself

                                          if (arr[mid] == x)

                                                         return mid;

                                          // If element is smaller than mid, then it can

                                          // only be present in left subarray

                                          if (arr[mid] > x)

                                                         return binarySearch(arr, l, mid - 1, x);

 

                                          // Else the element can only be present

                                          // in right subarray

                                          return binarySearch(arr, mid + 1, r, x);

                           }

                           // We reach here when element is not present in

                           // array

                           return -1;

            }

            // Method 2

            // Main driver method

            public static void main(String args[])

            {

                           // Creating object of above class

                           GFG ob = new GFG();

                           // Custom input array

                           int arr[] = { 2, 3, 4, 10, 40 };

 

                           // Length of array

                           int n = arr.length;

                           // Custom element to be checked

                           // whether present or not

                           int x = 10;

                           // Calling above method

                           int result = ob.binarySearch(arr, 0, n - 1, x);

                           // Element present

                           if (result == -1)

                                          // Print statement

                                          System.out.println("Element not present");

 

                           // Element not present

                           else

                                        // Print statement

                                          System.out.println("Element found at index "

                                                                                                      + result);

            }

}

----

75. Is delete, next, main, exit or null keyword in java?
No, these keywords do not exist in Java. Delete, Next, Exit are the operations performed in the Java program, Main is the predefined method, and Null is the default String type.

With this we are done with the first section that is Basic Java Interview Question, Now, lets move on to our next section of Intermediate Java Interview Questions.

Java Interview Coding Questions For Intermediate
Now, let's have a look at some of the most asked Java technical interview questions for intermediate experienced professionals.

----

76. What is JDK? Mention the variants of JDK?
JDK is an abbreviation for Java Development Kit. It is a combined Package of JRE and Developer tools used for designing Java Applications and Applets. Oracle has the following variants.

JDK Standard Edition
JDK Enterprise Edition
JDK Micro Edition

----

77. What is the difference between JDK, JRE, and JVM?
JVM has a Just in Time (JIT) compiler tool that converts all the Java source code into the low-level compatible machine language. Therefore, it runs faster than the regular application.

JRE has class libraries and other JVM supporting files. But it doesn’t have any tool for java development such as compiler or debugger.

JDK has tools that are required to write Java Programs and uses JRE to execute them. It has a compiler, Java application launcher, and an applet viewer.

----

78. What is a JIT compiler?
JIT compiler refers to Just in Time compiler. It is the simplest way of executing the computer code that takes in compilation during the execution of a program rather than before performance. It commonly uses bytecode translation to machine code. It is then executed directly.

----

79. What are Brief Access Specifiers and Types of Access Specifiers?
Access Specifiers are predefined keywords used to help JVM understand the scope of a variable, method, and class. We have four access specifiers.

Public Access Specifier 
Private Access Specifier 
Protected Access Specifier 
Default Access Specifier
80. How many types of constructors are used in Java?
There are two types of constructors in Java.

Parameterized Constructors: Parameterized constructor accepts the parameters with which users can initialize the instance variables. Users can initialize the class variables dynamically at the time of instantiating the class.

Default constructors: This type doesn’t accept any parameters; rather, it instantiates the class variables with their default values. It is used mainly for object creation.

----

81. Can a constructor return a value?
Yes, A constructor can return a value. It replaces the class's current instance implicitly; you cannot make a constructor return a value explicitly.

----

82. Explain ‘this’ keyword in Java.
The term "this" is a particular keyword designated as a reference keyword. The "this" keyword is used to refer to the current class properties like method, instance, variable, and constructors.

----

83. Explain ‘super’ keyword in Java.
The term "super" is a particular keyword designated as a reference keyword. The "super" keyword refers to the immediate parent class object.

----

84. Explain Method Overloading in Java.
The process of creating multiple method signatures using one method name is called Method Overloading in Java. Two ways to achieve method overloading are:

Varying the number of arguments
Changing the return type of the Method

----

85. Can we overload a static method?
No, Java does not support the Overloading of a static method. The process would throw an error reading "static method cannot be referenced."

----

86. Define Late Binding.
Binding is a process of unifying the method call with the method's code segment. Late binding happens when the method's code segment is unknown until it is called during the runtime. 

New Course: Full Stack Development for Beginners
Learn Git Command, Angular, NodeJS, Maven & MoreENROLL NOWNew Course: Full Stack Development for Beginners

----

87. Define Dynamic Method Dispatch.
The Dynamic method dispatch is a process where the method call is executed during the runtime. A reference variable is used to call the super-class. This process is also known as Run-Time Polymorphism.     

----

88. Why is the delete function faster in the linked list than an array?
Delete Function is faster in linked lists in Java as the user needs to make a minor update to the pointer value so that the node can point to the next successor in the list

----

89. Give a briefing on the life cycle of a thread.
The life cycle of a thread includes five stages, as mentioned below.

New Born State
Runnable State
Running State
Blocked State
Dead State

----

90. Explain the difference between >> and >>> operators.
Although they look similar, there is a massive difference between both.

>> operator does the job of right shifting the sign bits
>>> operator is used in shifting out the zero-filled bits

----

91. Brief the life cycle of an applet.
The life cycle of an applet involves the following.

Initialization
Start
Stop
Destroy
Paint
92. Why are generics used in Java Programming?
Compile-time type safety is provided by using generics. Compile-time type safety allows users to catch unnecessary invalid types at compile time. Generic methods and classes help programmers specify a single method declaration, a set of related methods, or related types with an available class declaration. 

----

93. Explain the Externalizable interface.
The Externalizable interface helps with control over the process of serialization. An "externalisable" interface incorporates readExternal and writeExternal methods.

----

94. What is the Daemon Thread?
The Daemon thread can be defined as a thread with the least priority. This Daemon thread is designed to run in the background during the Garbage Collection in Java.

The setDaemon() method creates a Daemon thread in Java.

----

95. Explain the term enumeration in Java.
Enumeration or enum is an interface in Java. Enum allows the sequential access of the elements stored in a collection in Java.

----

96. Why is Java is Dynamic?
Java is designed to adapt to an evolving environment. Java programs include a large amount of runtime information that is used to resolve access to objects in real-time. 

----

97. Can you run a code before executing the main method?
Yes, we can execute any code, even before the main method. We will be using a static block of code when creating the objects at the class's load time. Any statements within this static block of code will get executed at once while loading the class, even before creating objects in the main method.

----

98. How many times is the finalize method called?
The finalize method is called the Garbage collector. For every object, the Garbage Collector calls the finalize() method just for one time.

Java Interview Questions for Experienced
Now, lets move on to our last section of Advanced Core Java Interview Questions which is primarly useful for experienced and working professionals.

----

99. Can "this" and "super" keywords be used together?
No, "this" and "super" keywords should be used in the first statement in the class constructor. The following code gives you a brief idea.

public class baseClass {  

     baseClass() {  

         super();   

         this();  

         System.out.println(" baseClass object is created");  

     }  

     public static void main(String []args){  

         baseClass bclass = new baseClass();  

     }  

}

----

100. What is a JSP page?
JSP is an abbreviation for Java Servlet Page. The JSP page consists of two types of text.

Static Data 
JSP elements
Find Our Java Training in Top Cities

India	United States	Other Countries
Java Training in Bangalore	Java Training New York	Java Course London
Java Training in Chennai	Java Training San Diego	Java Course Singapore
Java Training in Hyderabad	Java Training Dallas	Java Course Melbourne
101. What is JDBC?
JDBC is an abbreviation for Java Database Connector.

JDBC is an abstraction layer used to establish connectivity between an existing database and a Java application

----

102. Explain the various directives in JSP.
Directives are instructions processed by JSP Engine. After the JSP page is compiled into a Servlet, Directives set page-level instructions, insert external files, and define customized tag libraries. Directives are defined using the symbols below:

start with "< %@" and then end with "% >" 

The various types of directives are shown below:

Include directive
It includes a file and combines the content of the whole file with the currently active pages.

Page directive
Page Directive defines specific attributes in the JSP page, like the buffer and error page.

Taglib
Taglib declares a custom tag library, which is used on the page.

----

103. What are the observer and observable classes?
Objects that inherit the "Observable class" take care of a list of "observers." 

When an Observable object gets upgraded, it calls the update() method of each of its observers. 

After that, it notifies all the observers that there is a change of state. 

The Observer interface gets implemented by objects that observe Observable objects.

Free Course: JavaScript for Beginners
Learn the Basics of JavaScriptENROLL NOWFree Course: JavaScript for Beginners

----

104. What is Session Management in Java?
A session is essentially defined as the random conversation's dynamic state between the client and the server. The virtual communication channel includes a string of responses and requests from both sides. The popular way of implementing session management is establishing a session ID in the client's communicative discourse and the server.

----

105. Briefly explain the term Spring Framework.
Spring is essentially defined as an application framework in Java and inversion of control containers for Java. The spring framework creates enterprise applications in Java. Especially useful to keep in mind that the spring framework's central features are essentially conducive to any Java application.

----

106. How to handle exceptions in Spring MVC Framework?
Spring MVC has two approaches for handling the exceptions:

Exception handler method: In this kind of exception handling, the user will get the @ExceptionHandler annotation type used to annotate a method to handle exceptions.
XML Configuration: The user can use the SimpleMappingExceptionResolver bean in Spring’s application file and map the exception.

----

107. What is JCA in Java?
Java Cryptography Architecture gives a platform and provides architecture and application programming interfaces that enable decryption and encryption. 

Developers use Java Cryptography Architecture to combine the application with the security applications. Java Cryptography Architecture helps in implementing third party security rules and regulations. 

Java Cryptography Architecture uses the hash table, encryption message digest, etc. to implement the security.

----

108. Explain JPA in Java.
The Java Persistence API enables us to create the persistence layer for desktop and web applications. Java Persistence deals in the following:

Java Persistence API
Query Language
Java Persistence Criteria API
Object Mapping Metadata

----

109. Explain the different authentications in Java Servlets.
Authentication options are available in Servlets: There are four different options for authentication in servlet:

Basic Authentication: 
Usernames and passwords are given by the client to authenticate the user.

Form-based authentication: 
In this, the login form is made by the programmer by using HTML.

Digest Authentication: 
It is similar to basic authentication, but the passwords are encrypted using the Hash formula. Hash Formula makes digest more secure.

Client certificate Authentication:
It requires that each client accessing the resource has a certificate that it sends to authenticate itself. Client Authentication requires the SSL protocol.

----

110. Explain FailFast iterator and FailSafe iterator along with examples for each.
FailFast iterators and FailSafe iterators are used in Java Collections. 

FailFast iterators do not allow changes or modifications to the Java Collections, which means they fail when the latest element is added to the collection or an existing element gets removed from the collection. The FailFast iterators tend to fail and throw an exception called ConcurrentModificationException.

Ex: ArrayList, HashMap

Whereas, on the other hand, FailSafe iterators allow changes or modifications to be done on the Java Collections. It is possible, as the FailSafe iterators usually operate on the cloned copy of the collection. Hence, they do not throw any specific exception.

Ex: CopyOnWriteArrayList

----

111. How do we reverse a string?
The string can be reversed by using the following program.

package simplilearnJava;

public class StringReverse {

public static void main(String args[]) {

String str = "Simplilearn";

String reverse = new StringBuffer(str).reverse().toString();

System.out.printf("Actual Word: %s, Word after reversing %s", str, reverse);

}

public static String reverse(String source) {

if (source == null || source.isEmpty()) {

return source;

}

String reverse = "";

for (int i = source.length() - 1; i >= 0; i--) {

reverse = reverse + source.charAt(i);

}

return reverse;

}

}

Expected Output:

Actual Word: Simplilearn, Word after reversing nraelilpmiS

----

112. Write a program to find the square root of a number.
The Square root of a number can be found by using the following program.

package simplilearnJava;

import java.util.Scanner;

public class SRoot {

public static void main(String args[]) {

try (Scanner sc = new Scanner(System.in)) {

System.out.println("Input a number to find square root: ");

double square = sc.nextDouble();

double squareRoot = Math.sqrt(square);

System.out.printf("The square root is: %f ", squareRoot);

}

}

}

Expected Output:

Input a number to find square root: 

25

The square root is: 5

Free Course: Java Hibernate Fundamentals
Learn Java Hibernate Basic Skills for FreeENROLL NOWFree Course: Java Hibernate Fundamentals
113. Write a program that detects the duplicate characters in a string.
The program that finds the duplicate elements in a string is written below:

package simplilearnJava;

import java.util.HashMap;

import java.util.Map;

import java.util.Set;

public class FindDuplicate {

public static void main(String args[]) {

printDuplicateCharacters("Simplilearn");

}

public static void printDuplicateCharacters(String word) {

char[] characters = word.toCharArray();

Map<Character, Integer> charMap = new HashMap<Character, Integer>();

for (Character ch : characters) {

if (charMap.containsKey(ch)) {

charMap.put(ch, charMap.get(ch) + 1);

} else {

charMap.put(ch, 1);

}

}

Set<Map.Entry<Character, Integer>> entrySet = charMap.entrySet();

System.out.printf("List of duplicate characters in String '%s' %n", word);

for (Map.Entry<Character, Integer> entry : entrySet) {

if (entry.getValue() > 1) {

System.out.printf("%s: %d %n", entry.getKey(), entry.getValue());

}

}

}

}

Expected output:

List of duplicate characters in String 'Simplilearn.' 

i: 2 

l: 2 

----

114. Write a Program to remove duplicates in an ArrayList.
The following program can be implemented to remove duplicate elements in an ArrayList

package simplilearnJava;

import java.util.ArrayList;

import java.util.LinkedHashSet;

import java.util.List;

import java.util.Set;

public class ArrayDuplicate {

public static void main(String args[]) {

List<Integer> num = new ArrayList<Integer>();

num.add(1);

num.add(2);

num.add(3);

num.add(4);

num.add(5);

num.add(6);

num.add(3);

num.add(4);

num.add(5);

num.add(6);

System.out.println("Your list of elements in ArrayList : " + num);

Set<Integer> primesWithoutDuplicates = new LinkedHashSet<Integer>(num);

num.clear();

num.addAll(primesWithoutDuplicates);

System.out.println("list of original numbers without duplication: " + num);

}

}

Expected Output:

Your list of elements in ArrayList : [1, 2, 3, 4, 5, 6, 3, 4, 5, 6]

list of original numbers without duplication: [1, 2, 3, 4, 5, 6]

----

115. Find the word count in a string using HashMap Collection.
The following program can be used for word count.

package simplilearnJava;

import java.util.HashMap;

public class WordCount {

public static void main(String[] args) {

String str = "Hello World, Welcome to Simplilearn";

String[] split = str.split(" ");

HashMap<String, Integer> map = new HashMap<String, Integer>();

for (int i = 0; i < split.length; i++) {

if (map.containsKey(split[i])) {

int count = map.get(split[i]);

map.put(split[i], count + 1);

} else {

map.put(split[i], 1);

}

}

System.out.println(map);

}

}

Expected Output:

{Hello=1, Simplilearn=1, Welcome=1, to=1, World,=1}

----

116. Write a program to find the Second Highest number in an ArrayList
The following program can be used to find the second biggest number in an array list.

package simplilearnJava;

public class NextHighest {

public static void main(String[] args)

    {

        int array[] = { 1, 2, 3, 4, 11, 12, 13, 14, 21, 22, 23, 24, 31, 32};

        int high = 0;

        int nextHigh = 0;

        System.out.println("The given array is:");

        for (int i = 0; i < array.length; i++)

        {

            System.out.print(array[i] + "\t");

        }

        for (int i = 0; i < array.length; i++)

        {

            if (array[i] > high)

            {

                nextHigh = high;

                high = array[i];

            }

            else if (array[i] > nextHigh)

            {

                nextHigh = array[i];

            }

        }

        System.out.println("Second Highest is:" + nextHigh);

        System.out.println("Highest Number is: "  +high);

    }

}

Expected Output:

The given array is:

1 2 3 4 11 12 13 14 21 22 23 24 31 32

Second Highest is:31

The highest number is: 32

----

117. What is the difference between System.out, System.err, and System.in?
System.out and System.err represent the monitor by default and thus can be used to send data or results to the monitor. System.out is used to display normal messages and results. System.eerr is used to display error messages. System.in represents InputStream object which by default represents standard input device, i.e., keyboard.

----

118. Could you provide some implementation of a Dictionary having a large number of words?
The simplest implementation that can be given is that of a List wherein one can place ordered words and perform a Binary search. The other implementation with a better search performance is HashMap where the key is used as the first character of the word and the value as a LinkedList.

Up another level, there are HashMaps like:

hashmap {

a (key) -> hashmap (key-aa , value (hashmap(key-aaa,value)

b (key) -> hashmap (key-ba , value (hashmap(key-baa,value)

z (key) -> hashmap (key-za , value (hashmap(key-zaa,value)

}

Up to n levels where n is the average size of the word in the dictionary.

----

119. How would you tackle it if you might have to encounter pattern programs in Java?
Solution - Top 25 Most Frequently asked Pattern Programs in Java

With this, we have come to the end of this Java Interview Questions article. Moving ahead, we will look into the next crucial steps that you could pursue, to master Java.

----

120. What do you understand by an instance variable and a local variable?
Generally, instance variables are declared in a class but outside methods whereas a local variable is declared within the blocks of code.

//Local Variable

import Java.io.*;

class Main {

public static void main(String[] args)

{

int var = 145;

System.out.println("Local Variable: " + var);

}

}

//Instance variable

import Java.io.*;

class Main {

public int value = 12;

public static void main(String[] args)

{

Main va = new Main();

System.out.println("My value is: " + va.value);

}

}

----

121. Can the main method be overloaded?
Yes, the main method can be overloaded as many times as we want. Nevertheless, JVM prefers to call the main method with the help of its predefined calling method. 

Example:

class Main {

    public static void main(String args[]) {

        System.out.println(" Main Method");

    }

    public static void main(int[] args){

        System.out.println("Overloaded Integer array Main Method");

    }

    public static void main(char[] args){

        System.out.println("Overloaded Character array Main Method");

    }

    public static int main(double[] args){

        System.out.println("Overloaded Double array Main Method");

    }

    public static void main(float args){

        System.out.println("Overloaded float Main Method");

    }

}

----

122. Comment on method overloading and overriding by citing relevant examples.
Method overloading occurs during the compile time, whereas method overriding occurs during the run time. Static binding is used during overloading, whereas dynamic binding is used during methods overriding.

//Function overloading

#function1

void addPodium(int a, int b)

{

System.out.println(a + b);

}

#function2

float addPodium(float a, float b, float c)

{

System.out.println(a + b + c);

}

//Function overriding

class Parent {

    void show()

    {

        System.out.println("I am Parent");

    }

}

class Child extends Parent {

    void show()

    {

        System.out.println("I am Child");

    }

}

class Main {

    public static void main(String[] args)

    {

        Parent obja = new Parent();

        obja.show();

        Parent objb = new Child();

        objb.show();

    }

}

----

123. A single try block and multiple catch blocks can co-exist in a Java Program. Explain.
One or more catch blocks can follow a try block. Each catch block must have a unique exception handler. So, if you want to perform multiple tasks in response to various exceptions, use the Java multi-catch block.

----

124. Do final, finally and finalize keywords have the same function?
No, final, finally and finalize keywords have different functionalities.

Final is used to restrict classes, variables, or methods, the final keyword.

Finally is used to execute the code written inside the block without handling any exceptions.

Finalize is used to call the function of the implementation of cleaning the garbage collection of an object. 

----

125. When can you use the "super" keyword?
Basically, the super keyword is used to refer to the parent class. When there are the same fields in both parent and child classes, then one can use a super keyword to access data members of the parent class.

----

126. What are shallow copy and deep copy in Java?
In the case of a shallow copy, primitive data types are copied, whereas in the case of a deep copy along with primitive data types the object references are also copied.

----

127. Using relevant properties highlight the differences between interfaces and abstract classes.
An abstract class can have a combination of both abstract and non-abstract methods, whereas an interface has only abstract methods in it.

----

128. What are the different ways of thread usage? 
There are two ways to define and implement a thread in Java. They are by implementing the runnable interface and extending the thread class.

Extending the Thread class

class InterviewBitThreadExample extends Thread{  

   public void run(){  

       System.out.println("Thread runs...");  

   }  

   public static void main(String args[]){  

       InterviewBitThreadExample ib = new InterviewBitThreadExample();  

       ib.start();  

   }  

}

Implementing the Runnable interface

class InterviewBitThreadExample implements Runnable{  

   public void run(){  

       System.out.println("Thread runs...");  

   }  

   public static void main(String args[]){  

       Thread ib = new Thread(new InterviewBitThreadExample()); 

       ib.start();  

   }  

}

Implementing a thread using the method of Runnable interface is more preferred and advantageous as Java does not have support for multiple inheritances of classes.

start() method is used for creating a separate call stack for the thread execution. Once the call stack is created, JVM calls the run() method for executing the thread in that call stack.

----

129. What is the difference between the ‘throw' and ‘throws' keyword in Java?
The throw keyword is often used to explicitly throw an exception. It can only throw one exception at a time whereas throws can be used to declare multiple exceptions.

----

130. Identify the output of the below Java program and Justify your answer.
class Main {

    public static void main(String args[]) {

        Scaler s = new Scaler(5);

    }

}

class InterviewBit{

    InterviewBit(){

        System.out.println(" Welcome to InterviewBit ");

    }

}

class Scaler extends InterviewBit{

    Scaler(){

        System.out.println(" Welcome to Scaler Academy ");

    }

    Scaler(int x){

        this();

        super();

        System.out.println(" Welcome to Scaler Academy 2");

    }

}

The above code will throw the compilation error. It is because the super() is used to call the parent class constructor. But there is the condition that super() must be the first statement in the block. Now in this case, if we replace this() with super() then also it will throw the compilation error. Because this() also has to be the first statement in the block. So in conclusion, we can say that we cannot use this() and super() keywords in the same block.

----

131. Java works as a “pass by value” or “pass by reference” phenomenon?
Java works as a “pass by value” phenomenon, because “pass by reference” needs the help of pointers. But there are no pointers in Java.

----

132. How to not allow serialization of attributes of a class in Java?
One approach to not allow serialization of attributes of a class in Java is by using writeObject() and readObject() methods in the subclass and throwing a not Serializable exception.

----

133. What are the default values assigned to variables and instances in Java?
By default, for a numerical value it is 0, for the boolean value it is false and for objects it is NULL.

----

134. What do you mean by data encapsulation?
Data encapsulation is one of the properties of OOPS concepts, where all the data such as variables and methods are enclosed together as a single unit.

----

135. Can you tell the difference between equals() method and equality operator (==) in Java?
Equality operator (==) is used to check the equality condition between two variables. But the equals() method is used to check the equality condition between two objects.

----

136. How is an infinite loop declared in Java?
An infinite loop can be declared in Java by breaking the logic in the instruction block.  For example,

for(int i = 1; i > 0; i++)

{

//statements

}

The above code forms an infinite loop in Java.

----

137. Briefly explain the concept of constructor overloading
The concept of constructor overloading refers to having multiple methods in a class with their name being the same as the class name. The difference lies in the set of parameters passed to the functions.

----

138. Explain the use of the final keyword in variable, method and class.
In Java, one can apply the final keyword to a variable, methods, and class. With the help of the final keyword, the variable turns out to be a constant, the method cannot be inherited and the class cannot be overridden.

----

139. Is it possible that the ‘finally' block will not be executed? If yes then list the case.
Yes, there is a possibility that the ‘finally’ block cannot get executed. Here are some of the cases where the above situation occurs.

During the time of fatal errors such as memory exhaustion, memory access error, etc.
During the time of using System.exit()

----

140. Difference between static methods, static variables, and static classes in Java.
A variable, method, or class can be made static by using the static keyword. A static class cannot be instantiated. When both objects or instances of a class share the same variables, this is referred to as static variables. Static methods are simply methods that refer to the class in which they are written.

----

141. What is the main objective of garbage collection?
The main goal of using garbage collection is to free the heap memory by eliminating unnecessary objects.

----

142. Apart from the security aspect, what are the reasons behind making strings immutable in Java?
Because of security, synchronization, concurrency, caching, and class loading, the String is immutable in Java. The reason for making string final would be to destroy its immutability and help stop others from trying to extend it. String objects are cached in the String pool, making them immutable.

143. Which of the below generates a compile-time error? State the reason.
int[] n1 = new int[0];

boolean[] n2 = new boolean[-200];

double[] n3 = new double[2241423798];

char[] ch = new char[20];

We get a compile-time error in line 3. The error we will get in Line 3 is - the integer number too large. It is because the array requires size as an integer.  And Integer takes 4 Bytes in the memory. And the number (2241423798) is beyond the capacity of the integer. The maximum array size we can declare is - (2147483647).

Because the array requires the size in integer, none of the lines (1, 2, and 4) will give a compile-time error. The program will compile fine. But we get the runtime exception in line 2. The exception is - NegativeArraySizeException. 

Here what will happen is - At the time when JVM will allocate the required memory during runtime then it will find that the size is negative. And the array size can’t be negative. So the JVM will throw the exception.

----

144. How would you differentiate between a String, StringBuffer, and a StringBuilder?
The string class is immutable but the other two are mutable in nature. StringBuffer is synchronous whereas the StringBuilder is asynchronous. String uses string pool as memory storage whereas the other two use heap memory for storage purposes.

----

145. What is a Comparator in Java?
A comparator is an interface, which is used to sort the objects. 

----

146. In Java, static as well as private method overriding is possible. Comment on the statement.
In Java, you could indeed override a private or static method. If you create a similar method in a child class with the same return type and method arguments, it will hide the super class method; this is known as method hiding. Similarly, you cannot override a private method in a subclass because it is not accessible from that.

----

147. What makes a HashSet different from a TreeSet?
In a HashSet, the elements are unsorted and work faster than a Tree set.  It is implemented using a hash table.

----

148. Why is the character array preferred over string for storing confidential information?
Because Strings are immutable, any change will result in the creation of a new String, whereas char[] allows you to set all of the elements to blank or zero. So storing a password in a character array clearly reduces the security risk of password theft.

----

149. What are the differences between HashMap and HashTable in Java?
HashMap

HashTable

1. Asynchronous in nature

1. Synchronous in nature

2. Not thread-safe

2. Thread safe

3. It allows one null key and null values

3. It doesn’t allow null keys and values.

----

150. What is the importance of reflection in Java?
Reflection is a property of Java, enabling the Java code to inspect itself. A Java class, for example, can get the names of all its members and showcase them.

----

151. What are the different types of Thread Priorities in Java? And what is the default priority of a thread assigned by JVM?
There are different types of thread properties in Java. They are MIN_PRIORITY, MAX_PRIORITY, and NORM_PRIORITY. By default, the thread is assigned NORM_PRIORITY.

----

152. What is the ‘IS-A ‘ relationship in OOPs Java?
‘IS-A’ relationship is related to the Inheritance property of OOPs Java. It is a kind of parent-child relationship that is established between two classes.

We offer complete Job Guarantee and money-back if you don't secure a job within 6 months of graduation. Get interview ready with intense and comprehensive career mentoring sessions in our Full Stack Java Developer Program. Enroll TODAY!

</https://www.simplilearn.com/tutorials/java-tutorial/java-interview-questions>

<https://www.edureka.co/blog/interview-questions/java-interview-questions/>

----

Q1. Explain JDK, JRE and JVM?
JDK vs JRE vs JVM
JDK	JRE	JVM
It stands for Java Development Kit.	It stands for Java Runtime Environment.	It stands for Java Virtual Machine.
It is the tool necessary to compile, document and package Java programs.	JRE refers to a runtime environment in which Java bytecode can be executed.	It is an abstract machine. It is a specification that provides a run-time environment in which Java bytecode can be executed.
It contains JRE + development tools.	It’s an implementation of the JVM which physically exists.	JVM follows three notations: Specification, Implementation, and Runtime Instance.

----

Q2. Explain public static void main(String args[]) in Java.
main() in Java is the entry point for any Java program. It is always written as public static void main(String[] args).

public: Public is an access modifier, which is used to specify who can access this method. Public means that this Method will be accessible by any Class.
static: It is a keyword in java which identifies it is class-based. main() is made static in Java so that it can be accessed without creating the instance of a Class. In case, main is not made static then the compiler will throw an error as main() is called by the JVM before any objects are made and only static methods can be directly invoked via the class. 
void: It is the return type of the method. Void defines the method which will not return any value.
main: It is the name of the method which is searched by JVM as a starting point for an application with a particular signature only. It is the method where the main execution occurs.
String args[]: It is the parameter passed to the main method.

----

Q3. Why Java is platform independent?
Java is called platform independent because of its byte codes which can run on any system irrespective of its underlying operating system.


----

Q4. Why Java is not 100% Object-oriented?

Java is not 100% Object-oriented because it makes use of eight primitive data types such as boolean, byte, char, int, float, double, long, short which are not objects.

----

Q5. What are wrapper classes in Java?

Wrapper classes convert the Java primitives into the reference types (objects). Every primitive data type has a class dedicated to it. These are known as wrapper classes because they “wrap” the primitive data type into an object of that class. Refer to the below image which displays different primitive type, wrapper class and constructor argument.


----

Q6. What are constructors in Java?
In Java, constructor refers to a block of code which is used to initialize an object. It must have the same name as that of the class. Also, it has no return type and it is automatically called when an object is created.

There are two types of constructors:

Default Constructor: In Java, a default constructor is the one which does not take any inputs. In other words, default constructors are the no argument constructors which will be created by default in case you no other constructor is defined by the user. Its main purpose is to initialize the instance variables with the default values. Also, it is majorly used for object creation. 
Parameterized Constructor: The parameterized constructor in Java, is the constructor which is capable of initializing the instance variables with the provided values. In other words, the constructors which take the arguments are called parameterized constructors.

----

Q7. What is singleton class in Java and how can we make a class singleton?
Singleton class is a class whose only one instance can be created at any given time, in one JVM. A class can be made singleton by making its constructor private.

----

Q8. What is the difference between Array list and vector in Java?
ArrayList	Vector
Array List is not synchronized.	 Vector is synchronized.
Array List is fast as it’s non-synchronized.	Vector is slow as it is thread safe.
If an element is inserted into the Array List, it increases its Array size by 50%.	Vector defaults to doubling size of its array.
Array List does not define the increment size.	Vector defines the increment size.
Array List can only use Iterator for traversing an Array List.	Vector can use both Enumeration and Iterator for traversing.

----

Q9. What is the difference between equals() and == in Java?
Equals() method is defined in Object class in Java and used for checking equality of two objects defined by business logic.

“==” or equality operator in Java is a binary operator provided by Java programming language and used to compare primitives and objects. public boolean equals(Object o) is the method provided by the Object class. The default implementation uses == operator to compare two objects. For example: method can be overridden like String class. equals() method is used to compare the values of two objects.

Course Curriculum
Java Certification Training Course
Instructor-led SessionsReal-life Case StudiesAssignmentsLifetime Access
Q10. When can you use the super keyword?
In Java, the super keyword is a reference variable that refers to an immediate parent class object.

When you create a subclass instance, you’re also creating an instance of the parent class, which is referenced to by the super reference variable.

The uses of the Java super Keyword are- 

To refer to an immediate parent class instance variable, use super.
The keyword super can be used to call the method of an immediate parent class.
Super() can be used to call the constructor of the immediate parent class.
 

----

Q11. What makes a HashSet different from a TreeSet?
HashSet	TreeSet
It is implemented through a hash table.	TreeSet implements SortedSet Interface that uses trees for storing data.
It permits the null object.	It does not allow the null object.
It is faster than TreeSet especially for search, insert, and delete operations.	It is slower than HashSet for these operations.
It does not maintain elements in an ordered way.	The elements are maintained in a sorted order.
It uses equals() method to compare two objects.	It uses compareTo() method for comparing two objects.
It does not permit a heterogenous object.	It permits a heterogenous object.
 

----

Q12. What are the differences between HashMap and HashTable in Java?

 

HashMap	Hashtable
It is non synchronized. It cannot be shared between many threads without proper synchronization code.	It is synchronized. It is thread-safe and can be shared with many threads.
It permits one null key and multiple null values.	It does not permit any null key or value.
is a new class introduced in JDK 1.2.	It was present in earlier versions of java as well.
It is faster.	It is slower.
It is traversed through the iterator.	It is traversed through Enumerator and Iterator.
It uses fail fast iterator.	It uses an enumerator which is not fail fast.
It inherits AbstractMap class.	It inherits Dictionary class.
 

----

Q13. What is the importance of reflection in Java?

Reflection is a runtime API for inspecting and changing the behavior of methods, classes, and interfaces. Java Reflection is a powerful tool that can be really beneficial. Java Reflection allows you to analyze classes, interfaces, fields, and methods during runtime without knowing what they are called at compile time. Reflection can also be used to create new objects, call methods, and get/set field values. External, user-defined classes can be used by creating instances of extensibility objects with their fully-qualified names. Debuggers can also use reflection to examine private members of classes.

----

Q14. How to not allow serialization of attributes of a class in Java?

The Non-Serialized attribute can be used to prevent member variables from being serialized.
You should also make an object that potentially contains security-sensitive data non-serializable if possible. Apply the Non-Serialized attribute to certain fields that store sensitive data if the object must be serialized. If you don’t exclude these fields from serialization, the data they store will be visible to any programs with serialization permission.

----

Q15. Can you call a constructor of a class inside another constructor?

Yes, we can call a constructor of a class inside another constructor. This is also called as constructor chaining. Constructor chaining can be done in 2 ways-

Within the same class: For constructors in the same class, the this() keyword can be used.
From the base class: The super() keyword is used to call the constructor from the base class.
The constructor chaining follows the process of inheritance. The constructor of the sub class first calls the constructor of the super class. Due to this, the creation of sub class’s object starts with the initialization of the data members of the super class. The constructor chaining works similarly with any number of classes. Every constructor keeps calling the chain till the top of the chain.
 

----

Q16. Contiguous memory locations are usually used for storing actual values in an array but not in ArrayList. Explain.

An array generally contains elements of the primitive data types such as int, float, etc. In such cases, the array directly stores these elements at contiguous memory locations. While an ArrayList does not contain primitive data types. An arrayList contains the reference of the objects at different memory locations instead of the object itself. That is why the objects are not stored at contiguous memory locations.

 

----

Q17. How is the creation of a String using new() different from that of a literal?
When we create a string using new(), a new object is created. Whereas, if we create a string using the string literal syntax, it may return an already existing object with the same name.

 

----

Q18. Why is synchronization necessary? Explain with the help of a relevant example.

Java allows multiple threads to execute. They may be accessing the same variable or object. Synchronization helps to execute threads one after another.
It is important as it helps to execute all concurrent threads while being in sync. It prevents memory consistency errors due to access to shared memory. An example of synchronization code is-

Programming & Frameworks Training
1
2
3
4
public synchronized void increment()
{
a++;
}
As we have synchronized this function, this thread can only use the object after the previous thread has used it.

----

Q19. Explain the term “Double Brace Initialization” in Java?

Double Brace Initialization is a Java term that refers to the combination of two independent processes. There are two braces used in this. The first brace creates an anonymous inner class. The second brace is an initialization block. When these both are used together, it is known as Double Brace Initialization. The inner class has a reference to the enclosing outer class, generally using the ‘this’ pointer. It is used to do both creation and initialization in a single statement. It is generally used to initialize collections. It reduces the code and also makes it more readable.

 
----


Q20. Why is it said that the length() method of String class doesn’t return accurate results?

The length() method of String class doesn’t return accurate results because
it simply takes into account the number of characters within in the String. In other words, code points outside of the BMP (Basic Multilingual Plane), that is, code points having a value of U+10000 or above, will be ignored.

The reason for this is historical. One of Java’s original goals was to consider all text as Unicode; yet, Unicode did not define code points outside of the BMP at the time. It was too late to modify char by the time Unicode specified such code points.

 

----

Q21. What are the differences between Heap and Stack Memory in Java?

The major difference between Heap and Stack memory are:

Features	Stack	Heap
Memory	Stack memory is used only by one thread of execution.	Heap memory is used by all the parts of the application.
Access	Stack memory can’t be accessed by other threads.	Objects stored in the heap are globally accessible.
Memory Management	Follows LIFO manner to free memory.	Memory management is based on the generation associated with each object.
Lifetime	Exists until the end of execution of the thread.	Heap memory lives from the start till the end of application execution.
Usage	Stack memory only contains local primitive and reference variables to objects in heap space.	Whenever an object is created, it’s always stored in the Heap space.

----

Q22. What is a package in Java? List down various advantages of packages.
Packages in Java, are the collection of related classes and interfaces which are bundled together. By using packages, developers can easily modularize the code and optimize its reuse. Also, the code within the packages can be imported by other classes and reused. Below I have listed down a few of its advantages:

Packages help in avoiding name clashes
They provide easier access control on the code
Packages can also contain hidden classes which are not visible to the outer classes and only used within the package
Creates a proper hierarchical structure which makes it easier to locate the related classes

----

Q23. Why pointers are not used in Java?
Java doesn’t use pointers because they are unsafe and increases the complexity of the program. Since, Java is known for its simplicity of code, adding the concept of pointers will be contradicting. Moreover, since JVM is responsible for implicit memory allocation, thus in order to avoid direct access to memory by the user,  pointers are discouraged in Java.

----

Q24. What is JIT compiler in Java?
JIT stands for Just-In-Time compiler in Java. It is a program that helps in converting the Java bytecode into instructions that are sent directly to the processor. By default, the JIT compiler is enabled in Java and is activated whenever a Java method is invoked. The JIT compiler then compiles the bytecode of the invoked method into native machine code, compiling it “just in time” to execute. Once the method has been compiled, the JVM summons the compiled code of that method directly rather than interpreting it. This is why it is often responsible for the performance optimization of Java applications at the run time.

----

Q25. What are access modifiers in Java?
In Java, access modifiers are special keywords which are used to restrict the access of a class, constructor, data member and method in another class. Java supports four types of access modifiers:

Default
Private
Protected
Public
Modifier	Default	Private	Protected	Public
Same class	YES	YES	YES	YES
Same Package subclass	YES	NO	YES	YES
Same Package non-subclass	YES	NO	YES	YES
Different package subclass	NO	NO	YES	YES
Different package non-subclass	NO	NO	NO	YES
Q26. Define a Java Class.
A class in Java is a blueprint which includes all your data.  A class contains fields (variables) and methods to describe the behavior of an object. Let’s have a look at the syntax of a class.

1
2
3
class Abc {
member variables // class body
methods}

----

Q27. What is an object in Java and how is it created?
An object is a real-world entity that has a state and behavior. An object has three characteristics:

State
Behavior
Identity
An object is created using the ‘new’ keyword. For example:

ClassName obj = new ClassName();

----

Q28. What is Object Oriented Programming?
Object-oriented programming or popularly known as OOPs is a programming model or approach where the programs are organized around objects rather than logic and functions. In other words, OOP mainly focuses on the objects that are required to be manipulated instead of logic. This approach is ideal for the programs large and complex codes and needs to be actively updated or maintained.

----

Q29. What are the main concepts of OOPs in Java?
Object-Oriented Programming or OOPs is a programming style that is associated with concepts like:

Inheritance: Inheritance is a process where one class acquires the properties of another.
Encapsulation: Encapsulation in Java is a mechanism of wrapping up the data and code together as a single unit.
Abstraction: Abstraction is the methodology of hiding the implementation details from the user and only providing the functionality to the users. 
Polymorphism: Polymorphism is the ability of a variable, function or object to take multiple forms.

----

Q30. What is the difference between a local variable and an instance variable?
In Java, a local variable is typically used inside a method, constructor, or a block and has only local scope. Thus, this variable can be used only within the scope of a block. The best benefit of having a local variable is that other methods in the class won’t be even aware of that variable.

Example
1
2
3
4
if(x > 100)
{
String test = "Edureka";
}
Whereas, an instance variable in Java, is a variable which is bounded to its object itself. These variables are declared within a class, but outside a method. Every object of that class will create it’s own copy of the variable while using it. Thus, any changes made to the variable won’t reflect in any other instances of that class and will be bound to that particular instance only.

1
2
3
4
class Test{
public String EmpName;
public int empAge;
}

----

Q31. Differentiate between the constructors and methods in Java?
Methods	Constructors
1. Used to represent the behavior of an object	1. Used to initialize the state of an object
2. Must have a return type	2. Do not have any return type
3. Needs to be invoked explicitly	3. Is invoked implicitly
4. No default method is provided by the compiler	4. A default constructor is provided by the compiler if the class has none
5. Method name may or may not be same as class name	5. Constructor name must always be the same as the class name
In case you are facing any challenges with these Core Java interview questions, please comment on your problems in the section below.

----

Q32. What is final keyword in Java?
final is a special keyword in Java that is used as a non-access modifier. A final variable can be used in different contexts such as:

final variable
When the final keyword is used with a variable then its value can’t be changed once assigned. In case the no value has been assigned to the final variable then using only the class constructor a value can be assigned to it.

Course Curriculum
Java Certification Training Course
Weekday / Weekend Batches
final method
When a method is declared final then it can’t be overridden by the inheriting class.

final class
When a class is declared as final in Java, it can’t be extended by any subclass class but it can extend other class.

----

Q33. What is the difference between break and continue statements?
break	continue
1. Can be used in switch and loop (for, while, do while) statements	1. Can be only used with loop statements
2. It causes the switch or loop statements to terminate the moment it is executed	2. It doesn’t terminate the loop but causes the loop to jump to the next iteration
3. It terminates the innermost enclosing loop or switch immediately	3. A continue within a loop nested with a switch will cause the next loop iteration to execute
Example break:
1
2
3
4
5
6
7
8
for (int i = 0; i < 5; i++)
{
if (i == 3)
{
break;
}
System.out.println(i);
}
Example continue:
1
2
3
4
5
6
7
8
for (int i = 0; i < 5; i++)
{
if(i == 2)
{
continue;
}
System.out.println(i);
}

----

Q34. What is an infinite loop in Java? Explain with an example.
An infinite loop is an instruction sequence in Java that loops endlessly when a functional exit isn’t met. This type of loop can be the result of a programming error or may also be a deliberate action based on the application behavior. An infinite loop will terminate automatically once the application exits.

For example:

1
2
3
4
5
6
7
8
public class InfiniteForLoopDemo
{
public static void main(String[] arg) {
for(;;)
System.out.println("Welcome to Edureka!");
// To terminate this program press ctrl + c in the console.
}
}
 

----

Q35. What is the difference between this() and super() in Java?
In Java, super() and this(), both are special keywords that are used to call the constructor. 

this()	super()
1. this() represents the current instance of a class	1. super() represents the current instance of a parent/base class
2. Used to call the default constructor of the same class	2. Used to call the default constructor of the parent/base class
3. Used to access methods of the current class	3. Used to access methods of the base class
4.  Used for pointing the current class instance	4. Used for pointing the superclass instance
5. Must be the first line of a block	5. Must be the first line of a block

----

Q36. What is Java String Pool?
Java String pool refers to a collection of Strings which are stored in heap memory. In this, whenever a new object is created, String pool first checks whether the object is already present in the pool or not. If it is present, then the same reference is returned to the variable else new object will be created in the String pool and the respective reference will be returned.

String pool - Java Interview Questions - Edureka

----

Q37. Differentiate between static and non-static methods in Java.
Static Method	Non-Static Method
1. The static keyword must be used before the method name	1. No need to use the static keyword before the method name
2. It is called using the class (className.methodName) 	2. It is can be called like any general method
3. They can’t access any non-static instance variables or methods	3. It can access any static method and any static variable without creating an instance of the class
Q38. Explain the term “Double Brace Initialisation” in Java?
Double Brace Initialization is a Java term that refers to the combination of two independent processes. There are two braces used in this. The first brace creates an anonymous inner class. The second brace is an initialization block. When these both are used together, it is known as Double Brace Initialisation. The inner class has a reference to the enclosing outer class, genertally using the ‘this’ pointer. It is used to do both creation and initialization in a single statement. It is generally used to initialize collections. It reduces the code and also makes it more readable.

----

Q39. What is constructor chaining in Java?
In Java, constructor chaining is the process of calling one constructor from another with respect to the current object. Constructor chaining is possible only through legacy where a subclass constructor is responsible for invoking the superclass’ constructor first. There could be any number of classes in the constructor chain. Constructor chaining can be achieved in two ways:

Within the same class using this()
From base class using super()

----

Q40. Difference between String, StringBuilder, and StringBuffer.

Factor	String	StringBuilder	StringBuffer
Storage Area	Constant String Pool	Heap Area	Heap Area
Mutability	Immutable	Mutable	Mutable
Thread Safety	Yes	No	Yes
Performance	Fast	More efficient	Less efficient
If you think this article on Java Interview Questions is helpful, you can check out Edureka’s Java Training in Chennai as well.

----

Q41. What is a classloader in Java?
The Java ClassLoader is a subset of JVM (Java Virtual Machine) that is responsible for loading the class files. Whenever a Java program is executed it is first loaded by the classloader. Java provides three built-in classloaders:

Bootstrap ClassLoader
Extension ClassLoader
System/Application ClassLoader

----

Q42. Why Java Strings are immutable in nature?
In Java, string objects are immutable in nature which simply means once the String object is created its state cannot be modified. Whenever you try to update the value of that object instead of updating the values of that particular object, Java creates a new string object. Java String objects are immutable as String objects are generally cached in the String pool. Since String literals are usually shared between multiple clients, action from one client might affect the rest. It enhances security, caching, synchronization, and performance of the application. 

----

Q43. What is the difference between an array and an array list?
Array	ArrayList
Cannot contain values of different data types	Can contain values of different data types.
Size must be defined at the time of declaration	Size can be dynamically changed
Need to specify the index in order to add data	No need to specify the index
Arrays are not type parameterized	Arraylists are type 
Arrays can contain primitive data types as well as objects	Arraylists can contain only objects, no primitive data types are allowed

----

Q44. What is a Map in Java?
In Java, Map is an interface of Util package which maps unique keys to values. The Map interface is not a subset of the main Collection interface and thus it behaves little different from the other collection types. Below are a few of the characteristics of Map interface: 

Map doesn’t contain duplicate keys.
Each key can map at max one value.

----

Q45. What is collection class in Java? List down its methods and interfaces.
In Java, the collection is a framework that acts as an architecture for storing and manipulating a group of objects. Using Collections you can perform various tasks like searching, sorting, insertion, manipulation, deletion, etc. Java collection framework includes the following:

Interfaces
Classes
Methods
The below image shows the complete hierarchy of the Java Collection.

FrameworkHierarchy - Java Collections - Edureka

 

Want to upskill yourself to get ahead in Career? Check out this video
Core Java Interview Quesions And Answers for Freshers and Experienced

This 120+ core java interview question and answer will help freshers and experience to crack the interview in 1st attempt.


OOPS Java Interview Questions

----

Q1. What is Polymorphism?
Polymorphism is briefly described as “one interface, many implementations”. Polymorphism is a characteristic of being able to assign a different meaning or usage to something in different contexts – specifically, to allow an entity such as a variable, a function, or an object to have more than one form. There are two types of polymorphism:

Compile time polymorphism
Run time polymorphism
Compile time polymorphism is method overloading whereas Runtime time polymorphism is done using inheritance and interface.

----

Q2. What is runtime polymorphism or dynamic method dispatch?
In Java, runtime polymorphism or dynamic method dispatch is a process in which a call to an overridden method is resolved at runtime rather than at compile-time. In this process, an overridden method is called through the reference variable of a superclass. Let’s take a look at the example below to understand it better.

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
class Car {
void run()
{
System.out.println(&ldquo;car is running&rdquo;); 
}
}
class Audi extends Car {
void run()
{
System.out.prinltn(&ldquo;Audi is running safely with 100km&rdquo;);
}
public static void main(String args[])
{
Car b= new Audi();    //upcasting
b.run();
}
}

----

Q3. What is abstraction in Java?
Abstraction refers to the quality of dealing with ideas rather than events. It basically deals with hiding the details and showing the essential things to the user. Thus you can say that abstraction in Java is the process of hiding the implementation details from the user and revealing only the functionality to them. Abstraction can be achieved in two ways:

Abstract Classes (0-100% of abstraction can be achieved)
Interfaces (100% of abstraction can be achieved)

----

Q4. What do you mean by an interface in Java?
An interface in Java is a blueprint of a class or you can say it is a collection of abstract methods and static constants. In an interface, each method is public and abstract but it does not contain any constructor. Thus, interface basically is a group of related methods with empty bodies. Example:

public interface Animal {
  public void eat();
  public void sleep();
  public void run();
}

----

Q5. What is the difference between abstract classes and interfaces?
Abstract Class	Interfaces
An abstract class can provide complete, default code and/or just the details that have to be overridden	An interface cannot provide any code at all, just the signature
In the case of an abstract class, a class may extend only one abstract class	A Class may implement several interfaces
An abstract class can have non-abstract methods	All methods of an Interface are abstract
An abstract class can have instance variables	An Interface cannot have instance variables
An abstract class can have any visibility: public, private, protected	An Interface visibility must be public (or) none
If we add a new method to an abstract class then we have the option of providing default implementation and therefore all the existing code might work properly	If we add a new method to an Interface then we have to track down all the implementations of the interface and define implementation for the new method
An abstract class can contain constructors	An Interface cannot contain constructors
Abstract classes are fast	Interfaces are slow as it requires extra indirection to find the corresponding method in the actual class

----

Q6. What is inheritance in Java?

Inheritance in Java is the concept where the properties of one class can be inherited by the other. It helps to reuse the code and establish a relationship between different classes. Inheritance is performed between two types of classes:

Parent class (Super or Base class)
Child class (Subclass or Derived class)

A class which inherits the properties is known as Child Class whereas a class whose properties are inherited is known as Parent class.

----

Q7. What are the different types of inheritance in Java?
Java supports four types of inheritance which are:

Single Inheritance: In single inheritance, one class inherits the properties of another i.e there will be only one parent as well as one child class.
Multilevel Inheritance: When a class is derived from a class which is also derived from another class, i.e. a class having more than one parent class but at different levels, such type of inheritance is called Multilevel Inheritance.
Hierarchical Inheritance: When a class has more than one child classes (subclasses) or in other words, more than one child classes have the same parent class, then such kind of inheritance is known as hierarchical.
Hybrid Inheritance: Hybrid inheritance is a combination of two or more types of inheritance.

----

Q8. What is method overloading and method overriding?
Method Overloading :
In Method Overloading, Methods of the same class shares the same name but each method must have a different number of parameters or parameters having different types and order.
Method Overloading is to “add” or “extend” more to the method’s behavior.
It is a compile-time polymorphism.
The methods must have a different signature.
It may or may not need inheritance in Method Overloading.
Let’s take a look at the example below to understand it better.

1
2
3
4
5
6
7
8
9
10
11
12
13
14
class Adder {
Static int add(int a, int b)
{
return a+b;
}
Static double add( double a, double b)
{
return a+b;
}
public static void main(String args[])
{
System.out.println(Adder.add(11,11));
System.out.println(Adder.add(12.3,12.6));
}}
Method Overriding:  
In Method Overriding, the subclass has the same method with the same name and exactly the same number and type of parameters and same return type as a superclass.
Method Overriding is to “Change” existing behavior of the method.
It is a run time polymorphism.
The methods must have the same signature.
It always requires inheritance in Method Overriding.
Let’s take a look at the example below to understand it better.

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
class Car {
void run(){
System.out.println(&ldquo;car is running&rdquo;); 
}
Class Audi extends Car{
void run()
{
System.out.prinltn("Audi is running safely with 100km");
}
public static void main( String args[])
{
Car b=new Audi();
b.run();
}
}

----

Q9. Can you override a private or static method in Java?
You cannot override a private or static method in Java. If you create a similar method with the same return type and same method arguments in child class then it will hide the superclass method; this is known as method hiding. Similarly, you cannot override a private method in subclass because it’s not accessible there. What you can do is create another private method with the same name in the child class. Let’s take a look at the example below to understand it better.

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
class Base {
private static void display() {
System.out.println("Static or class method from Base");
}
public void print() {
System.out.println("Non-static or instance method from Base");
}
class Derived extends Base {
private static void display() {
System.out.println("Static or class method from Derived");
}
public void print() {
System.out.println("Non-static or instance method from Derived");
}
public class test {
public static void main(String args[])
{
Base obj= new Derived();
obj1.display();
obj1.print();
}
}

----

Q10. What is multiple inheritance? Is it supported by Java?
MultipleInheritance - Java Interview Questions - EdurekaIf a child class inherits the property from multiple classes is known as multiple inheritance. Java does not allow to extend multiple classes.

The problem with multiple inheritance is that if multiple parent classes have the same method name, then at runtime it becomes difficult for the compiler to decide which method to execute from the child class.

Therefore, Java doesn’t support multiple inheritance. The problem is commonly referred to as Diamond Problem.

In case you are facing any challenges with these java interview questions, please comment on your problems in the section below.

----

Q11. What is encapsulation in Java?
Encapsulation is a mechanism where you bind your data(variables) and code(methods) together as a single unit. Here, the data is hidden from the outer world and can be accessed only via current class methods. This helps in protecting the data from any unnecessary modification. We can achieve encapsulation in Java by:

Declaring the variables of a class as private.
Providing public setter and getter methods to modify and view the values of the variables.

----

Q12. What is an association?
Association is a relationship where all object have their own lifecycle and there is no owner. Let’s take the example of Teacher and Student. Multiple students can associate with a single teacher and a single student can associate with multiple teachers but there is no ownership between the objects and both have their own lifecycle. These relationships can be one to one, one to many, many to one and many to many.

----

Q13. What do you mean by aggregation?
An aggregation is a specialized form of Association where all object has their own lifecycle but there is ownership and child object can not belong to another parent object. Let’s take an example of Department and teacher. A single teacher can not belong to multiple departments, but if we delete the department teacher object will not destroy. 

----


Q14. What is composition in Java?
Composition is again a specialized form of Aggregation and we can call this as a “death” relationship. It is a strong type of Aggregation. Child object does not have their lifecycle and if parent object deletes all child object will also be deleted. Let’s take again an example of a relationship between House and rooms. House can contain multiple rooms there is no independent life of room and any room can not belongs to two different houses if we delete the house room will automatically delete.

----


Q15. What is a marker interface?

A Marker interface can be defined as the interface having no data member and member functions. In simpler terms, an empty interface is called the Marker interface. The most common examples of Marker interface in Java are Serializable, Cloneable etc. The marker interface can be declared as follows.

1
2
public interface Serializable{
}

----

Q16. What is object cloning in Java?

Object cloning in Java is the process of creating an exact copy of an object. It basically means the ability to create an object with a similar state as the original object. To achieve this, Java provides a method clone() to make use of this functionality. This method creates a new instance of the class of the current object and then initializes all its fields with the exact same contents of corresponding fields. To object clone(), the marker interface java.lang.Cloneable must be implemented to avoid any runtime exceptions. One thing you must note is Object clone() is a protected method, thus you need to override it.

----

Q17. What is a copy constructor in Java?
Copy constructor is a member function that is used to initialize an object using another object of the same class. Though there is no need for copy constructor in Java since all objects are passed by reference. Moreover, Java does not even support automatic pass-by-value.

----

Q18. What is a constructor overloading in Java?
In Java, constructor overloading is a technique of adding any number of constructors to a class each having a different parameter list. The compiler uses the number of parameters and their types in the list to differentiate the overloaded constructors.

1
2
3
4
5
6
7
8
9
10
11
12
class Demo
{
int i;
public Demo(int a)
{
i=k;
}
public Demo(int a, int b)
{
//body
}
}
In case you are facing any challenges with these java interview questions, please comment on your problems in the section below. Apart from this Java Interview Questions Blog, if you want to get trained from professionals on this technology, you can opt for a structured training from edureka!

Servlets – Java Interview Questions  

----

Q1. What is a servlet?
Java Servlet is server-side technologies to extend the capability of web servers by providing support for dynamic response and data persistence.
The javax.servlet and javax.servlet.http packages provide interfaces and classes for writing our own servlets.
All servlets must implement the javax.servlet.Servlet interface, which defines servlet lifecycle methods. When implementing a generic service, we can extend the GenericServlet class provided with the Java Servlet API. The HttpServlet class provides methods, such as doGet() and doPost(), for handling HTTP-specific services.
Most of the times, web applications are accessed using HTTP protocol and thats why we mostly extend HttpServlet class. Servlet API hierarchy is shown in below image.
Servlet - Java Interview Questions - Edureka

----

Q2. What are the differences between Get and Post methods?
Get	Post
Limited amount of data can be sent because data is sent in header.	Large amount of data can be sent because data is sent in body.
 Not Secured because data is exposed in URL bar.	 Secured because data is not exposed in URL bar.
 Can be bookmarked	 Cannot be bookmarked
 Idempotent	 Non-Idempotent
 It is more efficient and used than Post	 It is less efficient and used

----

Q3. What is Request Dispatcher?
RequestDispatcher interface is used to forward the request to another resource that can be HTML, JSP or another servlet in same application. We can also use this to include the content of another resource to the response.

There are two methods defined in this interface:

1.void forward()

2.void include()

ForwardMethod - Java Interview Questions - Edureka
IncludeMethod - Java Interview Questions - Edureka

----

Q4. What are the differences between forward() method and sendRedirect() methods?

forward() method	SendRedirect() method
forward() sends the same request to another resource.	sendRedirect() method sends new request always because it uses the URL bar of the browser.
 forward() method works at server side.	 sendRedirect() method works at client side.
 forward() method works within the server only.	sendRedirect() method works within and outside the server.

----

Q5. What is the life-cycle of a servlet?
There are 5 stages in the lifecycle of a servlet:LifeCycleServlet - Java Interview Questions - Edureka

Servlet is loaded
Servlet is instantiated
Servlet is initialized
Service the request
Servlet is destroyed

----

Q6. How does cookies work in Servlets?
Cookies are text data sent by server to the client and it gets saved at the client local machine.
Servlet API provides cookies support through javax.servlet.http.Cookie class that implements Serializable and Cloneable interfaces.
HttpServletRequest getCookies() method is provided to get the array of Cookies from request, since there is no point of adding Cookie to request, there are no methods to set or add cookie to request.
Similarly HttpServletResponse addCookie(Cookie c) method is provided to attach cookie in response header, there are no getter methods for cookie.

----

Q7. What are the differences between ServletContext vs ServletConfig?
The difference between ServletContext and ServletConfig in Servlets JSP is in below tabular format.

ServletConfig	ServletContext
Servlet config object represent single servlet	It represent whole web application running on particular JVM and common for all the servlet
Its like local parameter associated with particular servlet	Its like global parameter associated with whole application
It’s a name value pair defined inside the servlet section of web.xml file so it has servlet wide scope	ServletContext has application wide scope so define outside of servlet tag in web.xml file.
getServletConfig() method is used to get the config object	getServletContext() method is  used to get the context object.
for example shopping cart of a user is a specific to particular user so here we can use servlet config	To get the MIME type of a file or application session related information is stored using servlet context object.

----

Q8. What are the different methods of session management in servlets?
Session is a conversational state between client and server and it can consists of multiple request and response between client and server. Since HTTP and Web Server both are stateless, the only way to maintain a session is when some unique information about the session (session id) is passed between server and client in every request and response.

Some of the common ways of session management in servlets are:

User Authentication
HTML Hidden Field
Cookies
URL Rewriting
Session Management API

SessionManagement - Java Interview Questions - Edureka
Apart from this blog, if you want to get trained by professionals on this technology, you can opt for structured training from edureka! Click below to know more.

JDBC – Java Interview Questions 
1. What is JDBC Driver?
JDBC Driver is a software component that enables java application to interact with the database. There are 4 types of JDBC drivers:

JDBC-ODBC bridge driver
Native-API driver (partially java driver)
Network Protocol driver (fully java driver)
Thin driver (fully java driver)
2. What are the steps to connect to a database in java?
Registering the driver class
Creating connection
Creating statement
Executing queries
Closing connection
3. What are the JDBC API components?
The java.sql package contains interfaces and classes for JDBC API.

Interfaces:
Connection
Statement
PreparedStatement
ResultSet
ResultSetMetaData
DatabaseMetaData
CallableStatement etc.
Classes:
DriverManager
Blob
Clob
Types
SQLException etc.

----

4. What is the role of JDBC DriverManager class?
The DriverManager class manages the registered drivers. It can be used to register and unregister drivers. It provides factory method that returns the instance of Connection.

----

5. What is JDBC Connection interface?
The Connection interface maintains a session with the database. It can be used for transaction management. It provides factory methods that returns the instance of Statement, PreparedStatement, CallableStatement and DatabaseMetaData.

ConnectionInterface - Java Interview Questions - Edureka
In case you are facing any challenges with these java interview questions, please comment on your problems in the section below.

----

6.  What is the purpose of JDBC ResultSet interface?
The ResultSet object represents a row of a table. It can be used to change the cursor pointer and get the information from the database.

----

7. What is JDBC ResultSetMetaData interface?
The ResultSetMetaData interface returns the information of table such as total number of columns, column name, column type etc.

----

8. What is JDBC DatabaseMetaData interface?
The DatabaseMetaData interface returns the information of the database such as username, driver name, driver version, number of tables, number of views etc.

----

9. What do you mean by batch processing in JDBC?
Batch processing helps you to group related SQL statements into a batch and execute them instead of executing a single query. By using batch processing technique in JDBC, you can execute multiple queries which makes the performance faster.

----

10. What is the difference between execute, executeQuery, executeUpdate?
Statement execute(String query) is used to execute any SQL query and it returns TRUE if the result is an ResultSet such as running Select queries. The output is FALSE when there is no ResultSet object such as running Insert or Update queries. We can use getResultSet() to get the ResultSet and getUpdateCount() method to retrieve the update count.

Statement executeQuery(String query) is used to execute Select queries and returns the ResultSet. ResultSet returned is never null even if there are no records matching the query. When executing select queries we should use executeQuery method so that if someone tries to execute insert/update statement it will throw java.sql.SQLException with message “executeQuery method can not be used for update”.

Statement executeUpdate(String query) is used to execute Insert/Update/Delete (DML) statements or DDL statements that returns nothing. The output is int and equals to the row count for SQL Data Manipulation Language (DML) statements. For DDL statements, the output is 0.

You should use execute() method only when you are not sure about the type of statement else use executeQuery or executeUpdate method.

----

Q11. What do you understand by JDBC Statements?
JDBC statements are basically the statements which are used to send SQL commands to the database and retrieve data back from the database. Various methods like execute(), executeUpdate(), executeQuery, etc. are provided by JDBC to interact with the database.

JDBC supports 3 types of statements:

Statement: Used for general purpose access to the database and executes a static SQL query at runtime.
PreparedStatement: Used to provide input parameters to the query during execution.
CallableStatement: Used to access the database stored procedures and helps in accepting runtime parameters.
In case you are facing any challenges with these java interview questions, please comment your problems in the section below. Apart from this Java Interview Questions Blog, if you want to get trained from professionals on this technology, you can opt for a structured training from edureka!

----

Spring Framework – Java Interview Questions

Q1. What is Spring?
Wikipedia defines the Spring framework as “an application framework and inversion of control container for the Java platform. The framework’s core features can be used by any Java application, but there are extensions for building web applications on top of the Java EE platform.” Spring is essentially a lightweight, integrated framework that can be used for developing enterprise applications in java.

----

Q2. Name the different modules of the Spring framework.
Some of the important Spring Framework modules are:

Spring Context – for dependency injection.
Spring AOP – for aspect oriented programming.
Spring DAO – for database operations using DAO pattern
Spring JDBC – for JDBC and DataSource support.
Spring ORM – for ORM tools support such as Hibernate
Spring Web Module – for creating web applications.
Spring MVC – Model-View-Controller implementation for creating web applications, web services etc.
SpringFramework - Java Interview Questions - EdurekaQ3. List some of the important annotations in annotation-based Spring configuration.
The important annotations are:

@Required
@Autowired
@Qualifier
@Resource
@PostConstruct
@PreDestroy

----

Q4. Explain Bean in Spring and List the different Scopes of Spring bean.
Beans are objects that form the backbone of a Spring application. They are managed by the Spring IoC container. In other words, a bean is an object that is instantiated, assembled, and managed by a Spring IoC container.

There are five Scopes defined in Spring beans.

SpringBean - Java Interview Questions - Edureka

Singleton: Only one instance of the bean will be created for each container. This is the default scope for the spring beans. While using this scope, make sure spring bean doesn’t have shared instance variables otherwise it might lead to data inconsistency issues because it’s not thread-safe.
Prototype: A new instance will be created every time the bean is requested.
Request: This is same as prototype scope, however it’s meant to be used for web applications. A new instance of the bean will be created for each HTTP request.
Session: A new bean will be created for each HTTP session by the container.
Global-session: This is used to create global session beans for Portlet applications.
In case you are facing any challenges with these java interview questions, please comment on your problems in the section below.

----

Q5. Explain the role of DispatcherServlet and ContextLoaderListener.
DispatcherServlet is basically the front controller in the Spring MVC application as it loads the spring bean configuration file and initializes all the beans that have been configured. If annotations are enabled, it also scans the packages to configure any bean annotated with @Component, @Controller, @Repository or @Service annotations.

DispatcherServlet - Java Interview Questions - EdurekaContextLoaderListener, on the other hand, is the listener to start up and shut down the WebApplicationContext in Spring root. Some of its important functions includes tying up the lifecycle of Application Context to the lifecycle of the ServletContext and automating the creation of ApplicationContext.

ContextLoader - Java Interview Questions - Edureka

----

Q6. What are the differences between constructor injection and setter injection?
No.	Constructor Injection	Setter Injection
 1)	 No Partial Injection	 Partial Injection
 2)	 Doesn’t override the setter property	 Overrides the constructor property if both are defined.
 3)	Creates a new instance if any modification occurs	Doesn’t create a new instance if you change the property value
 4) 	 Better for too many properties	 Better for a few properties.

----

Q7. What is autowiring in Spring? What are the autowiring modes?
Autowiring enables the programmer to inject the bean automatically. We don’t need to write explicit injection logic. Let’s see the code to inject bean using dependency injection.

<bean id=“emp” class=“com.javatpoint.Employee” autowire=“byName” />  
The autowiring modes are given below:

No.	Mode	Description
 1)	 no	 this is the default mode, it means autowiring is not enabled.
 2)	 byName	 Injects the bean based on the property name. It uses setter method.
 3)	 byType	 Injects the bean based on the property type. It uses setter method.
 4)	 constructor	 It injects the bean using constructor

----

Q8. How to handle exceptions in Spring MVC Framework?
Spring MVC Framework provides the following ways to help us achieving robust exception handling.

Controller Based:
We can define exception handler methods in our controller classes. All we need is to annotate these methods with @ExceptionHandler annotation.

Global Exception Handler:
Exception Handling is a cross-cutting concern and Spring provides @ControllerAdvice annotation that we can use with any class to define our global exception handler.

HandlerExceptionResolver implementation: 
For generic exceptions, most of the times we serve static pages. Spring Framework provides HandlerExceptionResolver interface that we can implement to create global exception handler. The reason behind this additional way to define global exception handler is that Spring framework also provides default implementation classes that we can define in our spring bean configuration file to get spring framework exception handling benefits.

----


Q9. What are some of the important Spring annotations which you have used?
Some of the Spring annotations that I have used in my project are:

@Controller – for controller classes in Spring MVC project.

@RequestMapping – for configuring URI mapping in controller handler methods. This is a very important annotation, so you should go through Spring MVC RequestMapping Annotation Examples

@ResponseBody – for sending Object as response, usually for sending XML or JSON data as response.

@PathVariable – for mapping dynamic values from the URI to handler method arguments.

@Autowired – for autowiring dependencies in spring beans.

@Qualifier – with @Autowired annotation to avoid confusion when multiple instances of bean type is present.

@Service – for service classes.

@Scope – for configuring the scope of the spring bean.

@Configuration, @ComponentScan and @Bean – for java based configurations.

AspectJ annotations for configuring aspects and advices , @Aspect, @Before, @After, @Around, @Pointcut, etc.

----

Q10. How to integrate Spring and Hibernate Frameworks?
We can use Spring ORM module to integrate Spring and Hibernate frameworks if you are using Hibernate 3+ where SessionFactory provides current session, then you should avoid using HibernateTemplate or HibernateDaoSupport classes and better to use DAO pattern with dependency injection for the integration.

Also, Spring ORM provides support for using Spring declarative transaction management, so you should utilize that rather than going for hibernate boiler-plate code for transaction management. 

----

Q11. Name the types of transaction management that Spring supports.
Two types of transaction management are supported by Spring. They are:

Programmatic transaction management: In this, the transaction is managed with the help of programming. It provides you extreme flexibility, but it is very difficult to maintain.
Declarative transaction management: In this, transaction management is separated from the business code. Only annotations or XML based configurations are used to manage the transactions.
Apart from these Core Java interview questions for experienced professionals, if you want to get trained by professionals on this technology, you can opt for a structured training from edureka!

Hibernate – Java Interview Questions for Experienced Professionals

----

1. What is Hibernate Framework?
Object-relational mapping or ORM is the programming technique to map application domain model objects to the relational database tables. Hibernate is Java-based ORM tool that provides a framework for mapping application domain objects to the relational database tables and vice versa.

Hibernate provides a reference implementation of Java Persistence API, that makes it a great choice as ORM tool with benefits of loose coupling. We can use the Hibernate persistence API for CRUD operations. Hibernate framework provide option to map plain old java objects to traditional database tables with the use of JPA annotations as well as XML based configuration.

Similarly, hibernate configurations are flexible and can be done from XML configuration file as well as programmatically.

----

2. What are the important benefits of using Hibernate Framework?
Some of the important benefits of using hibernate framework are:

Hibernate eliminates all the boiler-plate code that comes with JDBC and takes care of managing resources, so we can focus on business logic.
Hibernate framework provides support for XML as well as JPA annotations, that makes our code implementation independent.
Hibernate provides a powerful query language (HQL) that is similar to SQL. However, HQL is fully object-oriented and understands concepts like inheritance, polymorphism, and association.
Hibernate is an open source project from Red Hat Community and used worldwide. This makes it a better choice than others because learning curve is small and there are tons of online documentation and help is easily available in forums.
Hibernate is easy to integrate with other Java EE frameworks, it’s so popular that Spring Framework provides built-in support for integrating hibernate with Spring applications.
Hibernate supports lazy initialization using proxy objects and perform actual database queries only when it’s required.
Hibernate cache helps us in getting better performance.
For database vendor specific feature, hibernate is suitable because we can also execute native sql queries.
Overall hibernate is the best choice in current market for ORM tool, it contains all the features that you will ever need in an ORM tool.

----

3. Explain Hibernate architecture.
Hibernate has a layered architecture which helps the user to operate without having to know the underlying APIs. Hibernate makes use of the database and configuration data to provide persistence services (and persistent objects) to the application. It includes many objects such as persistent object, session factory, transaction factory, connection factory, session, transaction etc.HibernateArchitecture - Java Interview Questions - Edureka

The Hibernate architecture is categorized in four layers.

Java application layer
Hibernate framework layer
Backhand API layer
Database layer

----

4. What are the differences between get and load methods?
The differences between get() and load() methods are given below.

No.	get()	load()
 1)	 Returns null if object is not found.	Throws ObjectNotFoundException if an object is not found.
 2)	 get() method always hit the database.	 load() method doesn’t hit the database.
 3)	 It returns a real object, not a proxy.	 It returns a proxy object.
 4)	It should be used if you are not sure about the existence of instance.	It should be used if you are sure that the instance exists.

----

5. What are the advantages of Hibernate over JDBC?
Some of the important advantages of Hibernate framework over JDBC are:

Hibernate removes a lot of boiler-plate code that comes with JDBC API, the code looks cleaner and readable.
Hibernate supports inheritance, associations, and collections. These features are not present with JDBC API.
Hibernate implicitly provides transaction management, in fact, most of the queries can’t be executed outside transaction. In JDBC API, we need to write code for transaction management using commit and rollback. 
JDBC API throws SQLException that is a checked exception, so we need to write a lot of try-catch block code. Most of the times it’s redundant in every JDBC call and used for transaction management. Hibernate wraps JDBC exceptions and throw JDBCException or HibernateException un-checked exception, so we don’t need to write code to handle it. Hibernate built-in transaction management removes the usage of try-catch blocks.
Hibernate Query Language (HQL) is more object-oriented and close to Java programming language. For JDBC, we need to write native SQL queries.
Hibernate supports caching that is better for performance, JDBC queries are not cached hence performance is low.
Hibernate provides option through which we can create database tables too, for JDBC tables must exist in the database.
Hibernate configuration helps us in using JDBC like connection as well as JNDI DataSource for the connection pool. This is a very important feature in enterprise application and completely missing in JDBC API.
Hibernate supports JPA annotations, so the code is independent of the implementation and easily replaceable with other ORM tools. JDBC code is very tightly coupled with the application.

In case you are facing any challenges with these Java interview questions, please comment on your problems in the section below. Apart from this Java Interview Questions Blog, if you want to get trained from professionals on this technology, you can opt for structured training from edureka!

JSP – Java Interview Questions

----

1. What are the life-cycle methods for a jsp?
Methods	Description
 public void jspInit()	It is invoked only once, same as init method of servlet.
public void _jspService(ServletRequest request,ServletResponse)throws ServletException,IOException	It is invoked at each request, same as service() method of servlet.
 public void jspDestroy()	It is invoked only once, same as destroy() method of servlet.

----

2. What are the JSP implicit objects?
JSP provides 9 implicit objects by default. They are as follows:

Object	Type
1) out	 JspWriter
2) request	 HttpServletRequest
3) response	 HttpServletResponse
4) config	 ServletConfig
5) session	 HttpSession
6) application	 ServletContext
7) pageContext	 PageContext
8) page	 Object
9) exception	 Throwable
3. What are the differences between include directive and include action?
include directive	include action
The include directive includes the content at page translation time.	The include action includes the content at request time.
The include directive includes the original content of the page so page size increases at runtime.	The include action doesn’t include the original content rather invokes the include() method of Vendor provided class.
 It’s better for static pages.	 It’s better for dynamic pages.

----

4. How to disable caching on back button of the browser?
<%
response.setHeader(“Cache-Control”,”no-store”);
response.setHeader(“Pragma”,”no-cache”);
response.setHeader (“Expires”, “0”);                    //prevents caching at the proxy server
%>   

----

5. What are the different tags provided in JSTL?
There are 5 type of JSTL tags.

core tags
sql tags
xml tags
internationalization tags
functions tags
6. How to disable session in JSP?
<%@ page session=“false” %>   

----

7.  How to delete a Cookie in a JSP?
The following code explains how to delete a Cookie in a JSP :

1
2
3
4
5
6
7
8
9
10
11
Cookie mycook = new Cookie("name1","value1");
 
response.addCookie(mycook1);
 
Cookie killmycook = new Cookie("mycook1","value1");
 
killmycook . set MaxAge ( 0 );
 
killmycook . set Path ("/");
 
killmycook . addCookie ( killmycook 1 );

----

8. Explain the jspDestroy() method.
jspDestry() method is invoked from javax.servlet.jsp.JspPage interface whenever a JSP page is about to be destroyed. Servlets destroy methods can be easily overridden to perform cleanup, like when closing a database connection.

----

9.  How is JSP better than Servlet technology?
JSP is a technology on the server’s side to make content generation simple. They are document-centric, whereas servlets are programs. A Java server page can contain fragments of Java program, which execute and instantiate Java classes. However, they occur inside an HTML template file. It provides the framework for the development of a Web Application.

----

10. Why should we not configure JSP standard tags in web.xml?

We don’t need to configure JSP standard tags in web.xml because when container loads the web application and find TLD files, it automatically configures them to be used directly in the application JSP pages. We just need to include it in the JSP page using taglib directive.

----

11. How will you use JSP EL in order to get the HTTP method name?
Using pageContext JSP EL implicit object you can get the request object reference and make use of the dot operator to retrieve the HTTP method name in the JSP page. The JSP EL code for this purpose will look like ${pageContext.request.method}.

In case you are facing any challenges with these java interview questions, please comment on your problems in the section below. Apart from this Java Interview Questions Blog, if you want to get trained from professionals on this technology, you can opt for structured training from edureka!

Exception and Thread Java Interview Questions

----

Q1. What is the difference between Error and Exception?
An error is an irrecoverable condition occurring at runtime. Such as OutOfMemory error. These JVM errors you cannot repair them at runtime. Though error can be caught in the catch block but the execution of application will come to a halt and is not recoverable.

While exceptions are conditions that occur because of bad input or human error etc. e.g. FileNotFoundException will be thrown if the specified file does not exist. Or a NullPointerException will take place if you try using a null reference. In most of the cases it is possible to recover from an exception (probably by giving the user feedback for entering proper values etc.

----

Q2. How can you handle Java exceptions?
There are five keywords used to handle exceptions in Java: 

try
catch
finally
throw
throws

----

Q3. What are the differences between Checked Exception and Unchecked Exception?
Checked Exception
The classes that extend Throwable class except RuntimeException and Error are known as checked exceptions. 
Checked exceptions are checked at compile-time.
Example: IOException, SQLException etc.
Unchecked Exception
The classes that extend RuntimeException are known as unchecked exceptions. 
Unchecked exceptions are not checked at compile-time.
Example: ArithmeticException, NullPointerException etc.

----

Q4. What are the different ways of thread usage?
There are two ways to create a thread:

Extending Thread class
This creates a thread by creating an instance of a new class that extends the Thread class. The extending class must override the run() function, which is the thread’s entry point.

Implementing Runnable interface
This is the easiest way to create a thread, by creating a class that implements the runnable interface. After implementing the runnable interface, the class must implement the public void run() method ()

The run() method creates a parallel thread in your programme. When run() returns, the thread will come to an end.

The run() method creates a parallel thread in your programme. When run() returns, the thread will come to an end.

Within the run() method, you must specify the thread’s code.

Like any other method, the run() method can call other methods, use other classes, and define variables.

Java works as “pass by value” or “pass by reference” phenomenon?

Java is always pass-by-value. This means that it creates a copy of the contents of the parameter in memory. In Java, object variables always refer to the memory heap’s real object.

----

Q5. Will the finally block get executed when the return statement is written at the end of try block and catch block as shown below?
The finally block always gets executed even hen the return statement is written at the end of the try block and the catch block. It always executes , whether there is an exception or not. There are only a few situations in which the finally block does not execute, such as VM crash, power failure, software crash, etc. If you don’t want to execute the finally block, you need to call the System.exit() method explicitly in the finally block.

----

Q6. How does an exception propagate in the code?
If an exception is not caught, it is thrown from the top of the stack and falls down the call stack to the previous procedure. If the exception isn’t caught there, it falls back to the previous function, and so on, until it’s caught or the call stack reaches the bottom. The term for this is Exception propagation.

----

Q7. Can you explain the Java thread lifecycle?
The java thread lifecycle has the following states-

New-

When a thread is created, and before the program starts the thread, it is in the new state. It is also referred to as a born thread.

 Runnable

When a thread is started, it is in the Runnable state. In this state, the thread is executing its task.

Waiting

Sometimes, a thread goes to the waiting state, where it remains idle because another thread is executing. When the other thread has finished, the waiting thread again comes into the running state.

Timed Waiting

In timed waiting, the thread goes to waiting state. But, it remains in waiting state for only a specified interval of time after which it starts executing.It remains waiting either till the time interval ends or till the other thread has finished.

Terminated

A thread is said to be in this state once it terminates. It may be because the thread has completed its task or due to any other reason.

----

Q8. What purpose do the keywords final, finally, and finalize fulfill? 
Final:
Final is used to apply restrictions on class, method, and variable. A final class can’t be inherited, final method can’t be overridden and final variable value can’t be changed. Let’s take a look at the example below to understand it better.

1
2
3
4
5
6
class FinalVarExample {
public static void main( String args[])
{
final int a=10;   // Final variable
a=50;             //Error as value can't be changed
}
Finally
Finally is used to place important code, it will be executed whether the exception is handled or not. Let’s take a look at the example below to understand it better.

1
2
3
4
5
6
7
8
9
10
11
12
class FinallyExample {
public static void main(String args[]){
try {
int x=100;
}
catch(Exception e) {
System.out.println(e);
}
finally {
System.out.println("finally block is executing");}
}}
}
Finalize
Finalize is used to perform clean up processing just before the object is garbage collected. Let’s take a look at the example below to understand it better.

1
2
3
4
5
6
7
8
9
10
11
12
13
class FinalizeExample {
public void finalize() {
System.out.println("Finalize is called");
}
public static void main(String args[])
{
FinalizeExample f1=new FinalizeExample();
FinalizeExample f2=new FinalizeExample();
f1= NULL;
f2=NULL;
System.gc();
}
}

----

 Q9. What are the differences between throw and throws? 
throw keyword	throws keyword
Throw is used to explicitly throw an exception.	Throws is used to declare an exception.
Checked exceptions can not be propagated with throw only.	Checked exception can be propagated with throws.
Throw is followed by an instance.	Throws is followed by class.
Throw is used within the method.	Throws is used with the method signature.
You cannot throw multiple exception	You can declare multiple exception e.g. public void method()throws IOException,SQLException.
In case you are facing any challenges with these java interview questions, please comment on your problems in the section below.

----

Q10. What is exception hierarchy in java?
The hierarchy is as follows:

Throwable is a parent class of all Exception classes. There are two types of Exceptions: Checked exceptions and UncheckedExceptions or RunTimeExceptions. Both type of exceptions extends Exception class whereas errors are further classified into Virtual Machine error and Assertion error.

ExceptionHierarchy - Java Interview Questions - Edureka

----

Q11. How to create a custom Exception?
To create you own exception extend the Exception class or any of its subclasses.

class New1Exception extends Exception { }               // this will create Checked Exception
class NewException extends IOException { }             // this will create Checked exception
class NewException extends NullPonterExcpetion { }  // this will create UnChecked exception

----

Q12. What are the important methods of Java Exception Class?
Exception and all of it’s subclasses doesn’t provide any specific methods and all of the methods are defined in the base class Throwable.

String getMessage() – This method returns the message String of Throwable and the message can be provided while creating the exception through it’s constructor.
String getLocalizedMessage() – This method is provided so that subclasses can override it to provide locale specific message to the calling program. Throwable class implementation of this method simply use getMessage() method to return the exception message.
Synchronized Throwable getCause() – This method returns the cause of the exception or null id the cause is unknown.
String toString() – This method returns the information about Throwable in String format, the returned String contains the name of Throwable class and localized message.
void printStackTrace() – This method prints the stack trace information to the standard error stream, this method is overloaded and we can pass PrintStream or PrintWriter as an argument to write the stack trace information to the file or stream.

----

Q13. What are the differences between processes and threads?
 	Process	Thread
Definition	An executing instance of a program is called a process.	A thread is a subset of the process.
Communication	Processes must use inter-process communication to communicate with sibling processes.	Threads can directly communicate with other threads of its process.
Control	Processes can only exercise control over child processes.	Threads can exercise considerable control over threads of the same process.
Changes	Any change in the parent process does not affect child processes.	Any change in the main thread may affect the behavior of the other threads of the process.
Memory	Run in separate memory spaces.	Run in shared memory spaces.
Controlled by	Process is controlled by the operating system.	Threads are controlled by programmer in a program.
Dependence	Processes are independent.	Threads are dependent.

----

Q14. What is a finally block? Is there a case when finally will not execute?
Finally block is a block which always executes a set of statements. It is always associated with a try block regardless of any exception that occurs or not. 
Yes, finally will not be executed if the program exits either by calling System.exit() or by causing a fatal error that causes the process to abort.

----

Q15. What is synchronization?
Synchronization refers to multi-threading. A synchronized block of code can be executed by only one thread at a time. As Java supports execution of multiple threads, two or more threads may access the same fields or objects. Synchronization is a process which keeps all concurrent threads in execution to be in sync. Synchronization avoids memory consistency errors caused due to inconsistent view of shared memory. When a method is declared as synchronized the thread holds the monitor for that method’s object. If another thread is executing the synchronized method the thread is blocked until that thread releases the monitor. 

Synchronization - Java Interview Questions - Edureka

----

 Q16. Can we write multiple catch blocks under single try block? 
Yes we can have multiple catch blocks under single try block but the approach should be from specific to general. Let’s understand this with a programmatic example.

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
public class Example {
public static void main(String args[]) {
try {
int a[]= new int[10];
a[10]= 10/0;
}
catch(ArithmeticException e)
{
System.out.println("Arithmetic exception in first catch block");
}
catch(ArrayIndexOutOfBoundsException e)
{
System.out.println("Array index out of bounds in second catch block");
}
catch(Exception e)
{
System.out.println("Any exception in third catch block");
}
}

----

Q17. What are the important methods of Java Exception Class?
Methods are defined in the base class Throwable. Some of the important methods of Java exception class are stated below. 

String getMessage() – This method returns the message String about the exception. The message can be provided through its constructor.
public StackTraceElement[] getStackTrace() – This method returns an array containing each element on the stack trace. The element at index 0 represents the top of the call stack whereas the last element in the array represents the method at the bottom of the call stack.
Synchronized Throwable getCause() – This method returns the cause of the exception or null id as represented by a Throwable object.

String toString() – This method returns the information in String format. The returned String contains the name of Throwable class and localized message.
void printStackTrace() – This method prints the stack trace information to the standard error stream. 

----

Q18. What is OutOfMemoryError in Java?
OutOfMemoryError is the subclass of java.lang.Error which generally occurs when our JVM runs out of memory.

----

Q19. What is a Thread?
A thread is the smallest piece of programmed instructions which can be executed independently by a scheduler. In Java, all the programs will have at least one thread which is known as the main thread. This main thread is created by the JVM when the program starts its execution. The main thread is used to invoke the main() of the program.

----

Q20. What are the two ways to create a thread?
In Java, threads can be created in the following two ways:- 

By implementing the Runnable interface.
By extending the Thread

----

Q21. What are the different types of garbage collectors in Java?
Garbage collection in Java a program which helps in implicit memory management. Since in Java, using the new keyword you can create objects dynamically, which once created will consume some memory. Once the job is done and there are no more references left to the object, Java using garbage collection destroys the object and relieves the memory occupied by it. Java provides four types of garbage collectors:

Serial Garbage Collector
Parallel Garbage Collector
CMS Garbage Collector
G1 Garbage Collector

</https://www.edureka.co/blog/interview-questions/java-interview-questions/>

<https://www.interviewbit.com/java-interview-questions/>

Java Interview Questions for Freshers

----

1. Why is Java a platform independent language?
Java language was developed in such a way that it does not depend on any hardware or software due to the fact that the compiler compiles the code and then converts it to platform-independent byte code which can be run on multiple systems.

The only condition to run that byte code is for the machine to have a runtime environment (JRE) installed in it

----

2. Why is Java not a pure object oriented language?
Java supports primitive data types - byte, boolean, char, short, int, float, long, and double and hence it is not a pure object oriented language.

----

3. Difference between Heap and Stack Memory in java. And how java utilizes this.
Stack memory is the portion of memory that was assigned to every individual program. And it was fixed. On the other hand, Heap memory is the portion that was not allocated to the java program but it will be available for use by the java program when it is required, mostly during the runtime of the program.

Java Utilizes this memory as - 

When we write a java program then all the variables, methods, etc are stored in the stack memory.
And when we create any object in the java program then that object was created in the heap memory. And it was referenced from the stack memory.
Example- Consider the below java program:

class Main {
   public void printArray(int[] array){
       for(int i : array)
           System.out.println(i);
   }
   public static void main(String args[]) {
       int[] array = new int[10];
       printArray(array);
   }
}
For this java program. The stack and heap memory occupied by java is -


Main and PrintArray is the method that will be available in the stack area and as well as the variables declared that will also be in the stack area. 

And the Object (Integer Array of size 10) we have created, will be available in the Heap area because that space will be allocated to the program during runtime. 

You can download a PDF version of Java Interview Questions.

Download PDF

----

4. Can java be said to be the complete object-oriented programming language?
It is not wrong if we claim that java is the complete object-oriented programming language. Because Everything in Java is under the classes. And we can access that by creating the objects.

But also if we say that java is not a completely object-oriented programming language because it has the support of primitive data types like int, float, char, boolean, double, etc.

Now for the question: Is java a completely object-oriented programming language? We can say that - Java is not a pure object-oriented programming language, because it has direct access to primitive data types. And these primitive data types don't directly belong to the Integer classes.

----

5. How is Java different from C++?
C++ is only a  compiled language, whereas Java is compiled as well as an interpreted language.
Java programs are machine-independent whereas a c++ program can run only in the machine in which it is compiled. 
C++ allows users to use pointers in the program. Whereas java doesn’t allow it. Java internally uses pointers. 
C++ supports the concept of Multiple inheritances whereas Java doesn't support this. And it is due to avoiding the complexity of name ambiguity that causes the diamond problem.

----

6. Pointers are used in C/ C++. Why does Java not make use of pointers?
Pointers are quite complicated and unsafe to use by beginner programmers. Java focuses on code simplicity, and the usage of pointers can make it challenging. Pointer utilization can also cause potential errors. Moreover, security is also compromised if pointers are used because the users can directly access memory with the help of pointers.

Thus, a certain level of abstraction is furnished by not including pointers in Java. Moreover, the usage of pointers can make the procedure of garbage collection quite slow and erroneous. Java makes use of references as these cannot be manipulated, unlike pointers.

----

7. What do you understand by an instance variable and a local variable?
Instance variables are those variables that are accessible by all the methods in the class. They are declared outside the methods and inside the class. These variables describe the properties of an object and remain bound to it at any cost.

All the objects of the class will have their copy of the variables for utilization. If any modification is done on these variables, then only that instance will be impacted by it, and all other class instances continue to remain unaffected.

Example:

class Athlete {
public String athleteName;
public double athleteSpeed;
public int athleteAge;
}
Local variables are those variables present within a block, function, or constructor and can be accessed only inside them. The utilization of the variable is restricted to the block scope. Whenever a local variable is declared inside a method, the other class methods don’t have any knowledge about the local variable.

Example:

public void athlete() {
String athleteName;
double athleteSpeed;
int athleteAge;
}

----

8. What are the default values assigned to variables and instances in java?
There are no default values assigned to the variables in java. We need to initialize the value before using it. Otherwise, it will throw a compilation error of (Variable might not be initialized). 
But for instance, if we create the object, then the default value will be initialized by the default constructor depending on the data type. 
If it is a reference, then it will be assigned to null. 
If it is numeric, then it will assign to 0.
If it is a boolean, then it will be assigned to false. Etc.

----

9. What do you mean by data encapsulation?
Data Encapsulation is an Object-Oriented Programming concept of hiding the data attributes and their behaviours in a single unit.
It helps developers to follow modularity while developing software by ensuring that each object is independent of other objects by having its own methods, attributes, and functionalities.
It is used for the security of the private properties of an object and hence serves the purpose of data hiding.

----

10. Tell us something about JIT compiler.
JIT stands for Just-In-Time and it is used for improving the performance during run time. It does the task of compiling parts of byte code having similar functionality at the same time thereby reducing the amount of compilation time for the code to run.
The compiler is nothing but a translator of source code to machine-executable code. But what is special about the JIT compiler? Let us see how it works:
First, the Java source code (.java) conversion to byte code (.class) occurs with the help of the javac compiler.
Then, the .class files are loaded at run time by JVM and with the help of an interpreter, these are converted to machine understandable code.
JIT compiler is a part of JVM. When the JIT compiler is enabled, the JVM analyzes the method calls in the .class files and compiles them to get more efficient and native code. It also ensures that the prioritized method calls are optimized.
Once the above step is done, the JVM executes the optimized code directly instead of interpreting the code again. This increases the performance and speed of the execution.

----

11. Can you tell the difference between equals() method and equality operator (==) in Java?
We are already aware of the (==) equals operator. That we have used this to compare the equality of the values. But when we talk about the terms of object-oriented programming, we deal with the values in the form of objects. And this object may contain multiple types of data. So using the (==) operator does not work in this case. So we need to go with the .equals() method.

Both [(==) and .equals()] primary functionalities are to compare the values, but the secondary functionality is different. 

So in order to understand this better, let’s consider this with the example -

String str1 = "InterviewBit";
String str2 = "InterviewBit";
 
System.out.println(str1 == str2);
This code will print true. We know that both strings are equals so it will print true. But here (==) Operators don’t compare each character in this case. It compares the memory location. And because the string uses the constant pool for storing the values in the memory, both str1 and str2 are stored at the same memory location. See the detailed Explanation in Question no 73: Link.


Now, if we modify the program a little bit with -

String str1 = new String("InterviewBit");
String str2 = "InterviewBit";
 
System.out.println(str1 == str2);

Then in this case, it will print false. Because here no longer the constant pool concepts are used. Here, new memory is allocated. So here the memory address is different, therefore ( == ) Operator returns false. But the twist is that the values are the same in both strings. So how to compare the values? Here the .equals() method is used.

.equals() method compares the values and returns the result accordingly.  If we modify the above code with - 

System.out.println(str1.equals(str2));
Then it returns true.

equals() 	==
This is a method defined in the Object class. 	It is a binary operator in Java.
The .equals() Method is present in the Object class, so we can override our custom .equals() method in the custom class, for objects comparison.	It cannot be modified. They always compare the HashCode.
This method is used for checking the equality of contents between two objects as per the specified business logic.	This operator is used for comparing addresses (or references), i.e checks if both the objects are pointing to the same memory location.
Note:

In the cases where the equals method is not overridden in a class, then the class uses the default implementation of the equals method that is closest to the parent class.
Object class is considered as the parent class of all the java classes. The implementation of the equals method in the Object class uses the == operator to compare two objects. This default implementation can be overridden as per the business logic.

----

12. How is an infinite loop declared in Java?
Infinite loops are those loops that run infinitely without any breaking conditions. Some examples of consciously declaring infinite loop is:

Using For Loop:
for (;;)
{
   // Business logic
   // Any break logic
}
Using while loop:
while(true){
   // Business logic
   // Any break logic
}
Using do-while loop:
do{
   // Business logic
   // Any break logic
}while(true);

----

13. Briefly explain the concept of constructor overloading
Constructor overloading is the process of creating multiple constructors in the class consisting of the same name with a difference in the constructor parameters. Depending upon the number of parameters and their corresponding types, distinguishing of the different types of constructors is done by the compiler.

class Hospital {
int variable1, variable2;
double variable3;
public Hospital(int doctors, int nurses) {
 variable1 = doctors;
 variable2 = nurses;
}
public Hospital(int doctors) {
 variable1 = doctors;
}
public Hospital(double salaries) {
 variable3 = salaries
}
}

Three constructors are defined here but they differ on the basis of parameter type and their numbers.

----

14. Define Copy constructor in java.
Copy Constructor is the constructor used when we want to initialize the value to the new object from the old object of the same class. 

class InterviewBit{
   String department;
   String service;
   InterviewBit(InterviewBit ib){
       this.departments = ib.departments;
       this.services = ib.services;
   }
}
Here we are initializing the new object value from the old object value in the constructor. Although, this can also be achieved with the help of object cloning.

----

15. Can the main method be Overloaded?
Yes, It is possible to overload the main method. We can create as many overloaded main methods we want. However, JVM has a predefined calling method that JVM will only call the main method with the definition of - 

public static void main(string[] args)
Consider the below code snippets: 

class Main {
    public static void main(String args[]) {
        System.out.println(" Main Method");
    }
    public static void main(int[] args){
        System.out.println("Overloaded Integer array Main Method");
    }
    public static void main(char[] args){
        System.out.println("Overloaded Character array Main Method");
    }
    public static void main(double[] args){
        System.out.println("Overloaded Double array Main Method");
    }
    public static void main(float args){
        System.out.println("Overloaded float Main Method");
    }
}

----

16. Comment on method overloading and overriding by citing relevant examples.
In Java, method overloading is made possible by introducing different methods in the same class consisting of the same name. Still, all the functions differ in the number or type of parameters. It takes place inside a class and enhances program readability.

The only difference in the return type of the method does not promote method overloading. The following example will furnish you with a clear picture of it.

class OverloadingHelp {
   public int findarea (int l, int b) {
           int var1;
           var1 = l * b;
           return var1;
   }
   public int findarea (int l, int b, int h) {
           int var2;
           var2 = l * b * h;
           return var2;
   }
}

Both the functions have the same name but differ in the number of arguments. The first method calculates the area of the rectangle, whereas the second method calculates the area of a cuboid.

Method overriding is the concept in which two methods having the same method signature are present in two different classes in which an inheritance relationship is present. A particular method implementation (already present in the base class) is possible for the derived class by using method overriding.
Let’s give a look at this example:

class HumanBeing {
       public int walk (int distance, int time) {
               int speed = distance / time;
               return speed;
       }
}
class Athlete extends HumanBeing {
       public int walk(int distance, int time) {
               int speed = distance / time;
               speed = speed * 2;
               return speed;
       }
}

Both class methods have the name walk and the same parameters, distance, and time. If the derived class method is called, then the base class method walk gets overridden by that of the derived class.

----

17. A single try block and multiple catch blocks can co-exist in a Java Program. Explain.
Yes, multiple catch blocks can exist but specific approaches should come prior to the general approach because only the first catch block satisfying the catch condition is executed. The given code illustrates the same:

public class MultipleCatch {
public static void main(String args[]) {
 try {
  int n = 1000, x = 0;
  int arr[] = new int[n];
  for (int i = 0; i <= n; i++) {
   arr[i] = i / x;
  }
 }
 catch (ArrayIndexOutOfBoundsException exception) {
  System.out.println("1st block = ArrayIndexOutOfBoundsException");
 }
 catch (ArithmeticException exception) {
  System.out.println("2nd block = ArithmeticException");
 }
 catch (Exception exception) {
  System.out.println("3rd block = Exception");
 }
}
}
Here, the second catch block will be executed because of division by 0 (i / x). In case x was greater than 0 then the first catch block will execute because for loop runs till i = n and array index are till n-1.

----

18. Explain the use of final keyword in variable, method and class.
In Java, the final keyword is used as defining something as constant /final and represents the non-access modifier.

final variable:
When a variable is declared as final in Java, the value can’t be modified once it has been assigned.
If any value has not been assigned to that variable, then it can be assigned only by the constructor of the class.
final method:
A method declared as final cannot be overridden by its children's classes.
A constructor cannot be marked as final because whenever a class is inherited, the constructors are not inherited. Hence, marking it final doesn't make sense. Java throws compilation error saying - modifier final not allowed here
final class:
No classes can be inherited from the class declared as final. But that final class can extend other classes for its usage.

----

19. Do final, finally and finalize keywords have the same function?
All three keywords have their own utility while programming.

Final: If any restriction is required for classes, variables, or methods, the final keyword comes in handy. Inheritance of a final class and overriding of a final method is restricted by the use of the final keyword. The variable value becomes fixed after incorporating the final keyword. Example:

final int a=100;
a = 0;  // error
The second statement will throw an error.

Finally: It is the block present in a program where all the codes written inside it get executed irrespective of handling of exceptions. Example:

try {
int variable = 5;
}
catch (Exception exception) {
System.out.println("Exception occurred");
}
finally {
System.out.println("Execution of finally block");
}
Finalize: Prior to the garbage collection of an object, the finalize method is called so that the clean-up activity is implemented. Example:

public static void main(String[] args) {
String example = new String("InterviewBit");
example = null;
System.gc(); // Garbage collector called
}
public void finalize() {
// Finalize called
}

----

20. Is it possible that the ‘finally’ block will not be executed? If yes then list the case.
 Yes. It is possible that the ‘finally’ block will not be executed. The cases are-

Suppose we use System.exit() in the above statement.
If there are fatal errors like Stack overflow, Memory access error, etc.

----

21. Identify the output of the java program and state the reason.
1. public class InterviewBit
2. {
3.	 public static void main(String[] args) {
4.	 	 final int i;
5.		 i = 20;
6.		 int j = i+20;
7.		 i = j+30;
8.	     System.out.println(i + " " + j);
9.	 }
10. }
The above code will generate a compile-time error at Line 7 saying - [error: variable i might already have been initialized]. It is because variable ‘i’ is the final variable. And final variables are allowed to be initialized only once, and that was already done on line no 5.

----

22. When can you use super keyword?
The super keyword is used to access hidden fields and overridden methods or attributes of the parent class.
Following are the cases when this keyword can be used:
Accessing data members of parent class when the member names of the class and its child subclasses are same.
To call the default and parameterized constructor of the parent class inside the child class.
Accessing the parent class methods when the child classes have overridden them.
The following example demonstrates all 3 cases when a super keyword is used.
class Parent{
       protected int num = 1;
       
       Parent(){
           System.out.println("Parent class default constructor.");
       }
       
       Parent(String x){
           System.out.println("Parent class parameterised constructor.");
       }
       
       public void foo(){
           System.out.println("Parent class foo!");
       }
   }
class Child extends Parent{
       private int num = 2;
       
       Child(){
           //super constructor call should always be in the first line
           // super();              // Either call default super() to call default parent constructor OR
           super("Call Parent");    // call parameterised super to call parameterised parent constructor.
           System.out.println("Child class default Constructor");
       }
       
       void printNum(){
           System.out.println(num);
           System.out.println(super.num); //prints the value of num of parent class
       }
       
       @Override
       public void foo(){
           System.out.println("Child class foo!");
           super.foo();    //Calls foo method of Parent class inside the Overriden foo method of Child class.
       }
   }

public class DemoClass {
    public static void main(String args[]) {
     Child demoObject=new Child();
     demoObject.foo();
     /*
      This would print - 
      Parent class parameterised constructor.
      Child class default Constructor
      Child class foo!
      Parent class foo!
     */
    }
}

----

23. Can the static methods be overloaded?
Yes! There can be two or more static methods in a class with the same name but differing input parameters.

----

24. Why is the main method static in Java?
The main method is always static because static members are those methods that belong to the classes, not to an individual object. So if the main method will not be static then for every object, It is available. And that is not acceptable by JVM. JVM calls the main method based on the class name itself. Not by creating the object.

Because there must be only 1 main method in the java program as the execution starts from the main method. So for this reason the main method is static. 

----

25. Can the static methods be overridden?
No! Declaration of static methods having the same signature can be done in the subclass but run time polymorphism can not take place in such cases.
Overriding or dynamic polymorphism occurs during the runtime, but the static methods are loaded and looked up at the compile time statically. Hence, these methods cant be overridden.

----

26. Difference between static methods, static variables, and static classes in java.
Static Methods and Static variables are those methods and variables that belong to the class of the java program, not to the object of the class. This gets memory where the class is loaded. And these can directly be called with the help of class names.
For example - We have used mathematical functions in the java program like - max(), min(), sqrt(), pow(), etc. And if we notice that, then we will find that we call it directly with the class name. Like - Math.max(), Math.min(), etc. So that is a static method.  And Similarly static variables we have used like (length) for the array to get the length. So that is the static method.
Static classes - A class in the java program cannot be static except if it is the inner class. If it is an inner static class, then it exactly works like other static members of the class.

----

27. What is the main objective of garbage collection?
The main objective of this process is to free up the memory space occupied by the unnecessary and unreachable objects during the Java program execution by deleting those unreachable objects.

This ensures that the memory resource is used efficiently, but it provides no guarantee that there would be sufficient memory for the program execution.

----

28. What is a ClassLoader?
Java Classloader is the program that belongs to JRE (Java Runtime Environment). The task of ClassLoader is to load the required classes and interfaces to the JVM when required. 
Example- To get input from the console, we require the scanner class. And the Scanner class is loaded by the ClassLoader.

----

29. What part of memory - Stack or Heap - is cleaned in garbage collection process?
Heap.

----

30. What are shallow copy and deep copy in java?
To copy the object's data, we have several methods like deep copy and shallow copy. 

Example - 

class Rectangle{
int length = 5;
     int breadth = 3;
}
Object for this Rectangle class - Rectangle obj1 = new Rectangle();

Shallow copy - The shallow copy only creates a new reference and points to the same object. Example - For Shallow copy, we can do this by -
Rectangle obj2 = obj1;
Now by doing this what will happen is the new reference is created with the name obj2 and that will point to the same memory location.

Deep Copy - In a deep copy, we create a new object and copy the old object value to the new object. Example -
Rectangle obj3 = new Rectangle();
Obj3.length = obj1.length;
Obj3.breadth = obj1.breadth;
Both these objects will point to the memory location as stated below -


Now, if we change the values in shallow copy then they affect the other reference as well. Let's see with the help of an example - 

class Rectangle
{
int length = 5;
   int breadth = 3;
}
public class Main
{
public static void main(String[] args) {
 Rectangle obj1 = new Rectangle();
 //Shallow Copy
           Rectangle obj2 = obj1;
      
           System.out.println(" Before Changing the value of object 1, the object2 will be - ");
           System.out.println(" Object2 Length = "+obj2.length+", Object2 Breadth = "+obj2.breadth);
       
           //Changing the values for object1.
           obj1.length = 10;
           obj1.breadth = 20;
       
           System.out.println("\n After Changing the value of object 1, the object2 will be - ");
           System.out.println(" Object2 Length = "+obj2.length+", Object2 Breadth = "+obj2.breadth);
       
}
}
Output -

Before Changing the value of object 1, the object2 will be - 
Object2 Length = 5, Object2 Breadth = 3

After Changing the value of object 1, the object2 will be - 
Object2 Length = 10, Object2 Breadth = 20
We can see that in the above code, if we change the values of object1, then the object2 values also get changed. It is because of the reference.

Now, if we change the code to deep copy, then there will be no effect on object2 if it is of type deep copy. Consider some snippets to be added in the above code.

class Rectangle
{
   int length = 5;
   int breadth = 3;
}
public class Main
{
public static void main(String[] args) {
 Rectangle obj1 = new Rectangle();
 //Shallow Copy
           Rectangle obj2 = new Rectangle();
           obj2.length = obj1.length;
           obj2.breadth = obj1.breadth;
      
           System.out.println(" Before Changing the value of object 1, the object2 will be - ");
           System.out.println(" Object2 Length = "+obj2.length+", Object2 Breadth = "+obj2.breadth);
       
           //Changing the values for object1.
           obj1.length = 10;
           obj1.breadth = 20;
       
           System.out.println("\n After Changing the value of object 1, the object2 will be - ");
           System.out.println(" Object2 Length = "+obj2.length+", Object2 Breadth = "+obj2.breadth);
       
}
}
The above snippet will not affect the object2 values. It has its separate values. The output will be

Before Changing the value of object 1, the object2 will be - 
Object2 Length = 5, Object2 Breadth = 3

After Changing the value of object 1, the object2 will be - 
Object2 Length = 5, Object2 Breadth = 3
Now we see that we need to write the number of codes for this deep copy. So to reduce this, In java, there is a method called clone(). 

The clone() will do this deep copy internally and return a new object. And to do this we need to write only 1 line of code. That is - Rectangle obj2 = obj1.clone();

Java Intermediate Interview Questions

----

31. Apart from the security aspect, what are the reasons behind making strings immutable in Java?
A String is made immutable due to the following reasons:

String Pool: Designers of Java were aware of the fact that String data type is going to be majorly used by the programmers and developers. Thus, they wanted optimization from the beginning. They came up with the notion of using the String pool (a storage area in Java heap) to store the String literals. They intended to decrease the temporary String object with the help of sharing. An immutable class is needed to facilitate sharing. The sharing of the mutable structures between two unknown parties is not possible. Thus, immutable Java String helps in executing the concept of String Pool.

Multithreading: The safety of threads regarding the String objects is an important aspect in Java. No external synchronization is required if the String objects are immutable. Thus, a cleaner code can be written for sharing the String objects across different threads. The complex process of concurrency is facilitated by this method.
Collections: In the case of Hashtables and HashMaps, keys are String objects. If the String objects are not immutable, then it can get modified during the period when it resides in the HashMaps. Consequently, the retrieval of the desired data is not possible. Such changing states pose a lot of risks. Therefore, it is quite safe to make the string immutable.

----

32. What is a singleton class in Java? And How to implement a singleton class?
Singleton classes are those classes, whose objects are created only once. And with only that object the class members can be accessed. 

Understand this with the help of an example-:

Consider the water jug in the office and if every employee wants that water then they will not create a new water jug for drinking water. They will use the existing one with their own reference as a glass. So programmatically it should be implemented as -

class WaterJug{
   private int waterQuantity = 500;
   private WaterJug(){}
   private WaterJug object = null;
   
   // Method to provide the service of Giving Water.
   public int getWater(int quantity){
       waterQuantity -= quantity;
       return quantity;
   }
   // Method to return the object to the user.
   public static Waterjug getInstance(){
       // Will Create a new object if the object is not already created and return the object.
       if(object == null){
           object = new WaterJug();
       }
       return object;
   }
}
In the above class, the Constructor is private so we cannot create the object of the class. But we can get the object by calling the method getInstance(). And the getInstance is static so it can be called without creating the object. And it returns the object. Now with that object, we can call getWater() to get the water.

Waterjug glass1 = WaterJug.getInstance();
glass1.getWater(1);
We can get the single object using this getInstance(). And it is static, so it is a thread-safe singleton class. Although there are many ways to create a thread-safe singleton class. So thread-safe classes can also be:

When singletons are written with double-checked locking, they can be thread-safe.
We can use static singletons that are initialized during class loading. Like we did in the above example.
But the most straightforward way to create a thread-safe singleton is to use Java enums.

----

33. Which of the below generates a compile-time error? State the reason.
int[] n1 = new int[0];
boolean[] n2 = new boolean[-200];
double[] n3 = new double[2241423798];
char[] ch = new char[20];
We get a compile-time error in line 3. The error we will get in Line 3 is - integer number too large. It is because the array requires size as an integer. And Integer takes 4 Bytes in the memory. And the number (2241423798) is beyond the capacity of the integer. The maximum array size we can declare is - (2147483647).

Because the array requires the size in integer, none of the lines (1, 2, and 4) will give a compile-time error. The program will compile fine. But we get the runtime exception in line 2. The exception is - NegativeArraySizeException. 

Here what will happen is - At the time when JVM will allocate the required memory during runtime then it will find that the size is negative. And the array size can’t be negative. So the JVM will throw the exception.

----

34. How would you differentiate between a String, StringBuffer, and a StringBuilder?
Storage area: In string, the String pool serves as the storage area. For StringBuilder and StringBuffer, heap memory is the storage area.
Mutability: A String is immutable, whereas both the StringBuilder and StringBuffer are mutable.
Efficiency: It is quite slow to work with a String. However, StringBuilder is the fastest in performing operations. The speed of a StringBuffer is more than a String and less than a StringBuilder. (For example appending a character is fastest in StringBuilder and very slow in String because a new memory is required for the new String with appended character.)
Thread-safe: In the case of a threaded environment, StringBuilder and StringBuffer are used whereas a String is not used. However, StringBuilder is suitable for an environment with a single thread, and a StringBuffer is suitable for multiple threads.
Syntax:
// String
String first = "InterviewBit";
String second = new String("InterviewBit");
// StringBuffer
StringBuffer third = new StringBuffer("InterviewBit");
// StringBuilder
StringBuilder fourth = new StringBuilder("InterviewBit");

----

35. Using relevant properties highlight the differences between interfaces and abstract classes.
Availability of methods: Only abstract methods are available in interfaces, whereas non-abstract methods can be present along with abstract methods in abstract classes.
Variable types: Static and final variables can only be declared in the case of interfaces, whereas abstract classes can also have non-static and non-final variables.
Inheritance: Multiple inheritances are facilitated by interfaces, whereas abstract classes do not promote multiple inheritances.
Data member accessibility: By default, the class data members of interfaces are of the public- type. Conversely, the class members for an abstract class can be protected or private also.
Implementation: With the help of an abstract class, the implementation of an interface is easily possible. However, the converse is not true;
Abstract class example:

public abstract class Athlete {
public abstract void walk();
}
Interface example:

public interface Walkable {
void walk();
}

----

36. Is this program giving a compile-time error? If Yes then state the reason and number of errors it will give. If not then state the reason.
abstract final class InterviewBit{
2.    public abstract void printMessage();
3. }
4. class ScalarAcademy extends InterviewBit{
5.    public void printMessage(){
6.        System.out.println("Welcome to Scalar Academy By InterviewBit");
7.    }
8. }
9. class ScalarTopics extends ScalarAcademy{
10.    public void printMessage(){
11.        System.out.println("Welcome to Scalar Topics By Scalar Academy");
12.    }
13. }
public class Main{
	public static void main(String[] args) {
 	    InterviewBit ib = new ScalarTopics();
 	    ib.printMessage();
	}
}
The above program will give a compile-time error. The compiler will throw 2 errors in this.

[Illegal Combination of modifiers: abstract and final] at line 1.
[Cannot inherit from final ‘InterviewBit’] at line 4.
It is because abstract classes are incomplete classes that need to be inherited for making their concrete classes. And on the other hand, the final keywords in class are used for avoiding inheritance. So these combinations are not allowed in java.

----

37. What is a Comparator in java?
Consider the example where we have an ArrayList of employees like( EId, Ename, Salary), etc. Now if we want to sort this list of employees based on the names of employees. Then that is not possible to sort using the Collections.sort() method. We need to provide something to the sort() function depending on what values we have to perform sorting. Then in that case a comparator is used.

Comparator is the interface in java that contains the compare method. And by overloading the compare method, we can define that on what basis we need to compare the values. 

----

38. In Java, static as well as private method overriding is possible. Comment on the statement.
The statement in the context is completely False. The static methods have no relevance with the objects, and these methods are of the class level. In the case of a child class, a static method with a method signature exactly like that of the parent class can exist without even throwing any compilation error.

The phenomenon mentioned here is popularly known as method hiding, and overriding is certainly not possible. Private method overriding is unimaginable because the visibility of the private method is restricted to the parent class only. As a result, only hiding can be facilitated and not overriding.

----

39. What makes a HashSet different from a TreeSet?
Although both HashSet and TreeSet are not synchronized and ensure that duplicates are not present, there are certain properties that distinguish a HashSet from a TreeSet.

Implementation: For a HashSet, the hash table is utilized for storing the elements in an unordered manner. However, TreeSet makes use of the red-black tree to store the elements in a sorted manner.
Complexity/ Performance: For adding, retrieving, and deleting elements, the time amortized complexity is O(1) for a HashSet. The time complexity for performing the same operations is a bit higher for TreeSet and is equal to O(log n). Overall, the performance of HashSet is faster in comparison to TreeSet.
Methods: hashCode() and equals() are the methods utilized by HashSet for making comparisons between the objects. Conversely, compareTo() and compare() methods are utilized by TreeSet to facilitate object comparisons.
Objects type: Heterogeneous and null objects can be stored with the help of HashSet. In the case of a TreeSet, runtime exception occurs while inserting heterogeneous objects or null objects.

----

40. Why is the character array preferred over string for storing confidential information?
In Java, a string is basically immutable i.e. it cannot be modified. After its declaration, it continues to stay in the string pool as long as it is not removed in the form of garbage. In other words, a string resides in the heap section of the memory for an unregulated and unspecified time interval after string value processing is executed.

As a result, vital information can be stolen for pursuing harmful activities by hackers if a memory dump is illegally accessed by them. Such risks can be eliminated by using mutable objects or structures like character arrays for storing any variable. After the work of the character array variable is done, the variable can be configured to blank at the same instant. Consequently, it helps in saving heap memory and also gives no chance to the hackers to extract vital data.

----

41. What do we get in the JDK file?
JDK- For making java programs, we need some tools that are provided by JDK (Java Development Kit). JDK is the package that contains various tools, Compiler, Java Runtime Environment, etc.
JRE -  To execute the java program we need an environment. (Java Runtime Environment) JRE contains a library of Java classes +  JVM. What are JAVA Classes?  It contains some predefined methods that help Java programs to use that feature, build and execute. For example - there is a system class in java that contains the print-stream method, and with the help of this, we can print something on the console.
JVM - (Java Virtual Machine) JVM  is a part of JRE that executes the Java program at the end.  Actually, it is part of JRE, but it is software that converts bytecode into machine-executable code to execute on hardware.

----

42. What are the differences between JVM, JRE and JDK in Java?
Criteria	JDK 	JRE	JVM
Abbreviation	Java Development Kit	Java Runtime Environment	Java Virtual Machine
Definition	JDK is a complete software development kit for developing Java applications. It comprises JRE, JavaDoc, compiler, debuggers, etc.	JRE is a software package providing Java class libraries, JVM and all the required components to run the Java applications.	JVM is a platform-dependent, abstract machine comprising of 3 specifications - document describing the JVM implementation requirements, computer program meeting the JVM requirements and instance object for executing the Java byte code and provide the runtime environment for execution.
Main Purpose	JDK is mainly used for code development and execution.	JRE is mainly used for environment creation to execute the code.	JVM provides specifications for all the implementations to JRE.
Tools provided	JDK provides tools like compiler, debuggers, etc for code development	JRE provides libraries and classes required by JVM to run the program.	JVM does not include any tools, but instead, it provides the specification for implementation.
Summary	JDK = (JRE) + Development tools	JRE = (JVM) + Libraries to execute the application	JVM = Runtime environment to execute Java byte code.

----

43. What are the differences between HashMap and HashTable in Java?
HashMap	HashTable
HashMap is not synchronized thereby making it better for non-threaded applications.	HashTable is synchronized and hence it is suitable for threaded applications.
Allows only one null key but any number of null in the values.	This does not allow null in both keys or values.
Supports order of insertion by making use of its subclass LinkedHashMap.	Order of insertion is not guaranteed in HashTable.

----

44. What is the importance of reflection in Java?
The term reflection is used for describing the inspection capability of a code on other code either of itself or of its system and modify it during runtime.
Consider an example where we have an object of unknown type and we have a method ‘fooBar()’ which we need to call on the object. The static typing system of Java doesn't allow this method invocation unless the type of the object is known beforehand. This can be achieved using reflection which allows the code to scan the object and identify if it has any method called “fooBar()” and only then call the method if needed.
Method methodOfFoo = fooObject.getClass().getMethod("fooBar", null);
methodOfFoo.invoke(fooObject, null);
Using reflection has its own cons:
Speed — Method invocations due to reflection are about three times slower than the direct method calls.
Type safety — When a method is invoked via its reference wrongly using reflection, invocation fails at runtime as it is not detected at compile/load time.
Traceability — Whenever a reflective method fails, it is very difficult to find the root cause of this failure due to a huge stack trace. One has to deep dive into the invoke() and proxy() method logs to identify the root cause.
Hence, it is advisable to follow solutions that don't involve reflection and use this method as a last resort.

----

45. What are the different ways of threads usage?
We can define and implement a thread in java using two ways:
Extending the Thread class
class InterviewBitThreadExample extends Thread{  
   public void run(){  
       System.out.println("Thread runs...");  
   }  
   public static void main(String args[]){  
       InterviewBitThreadExample ib = new InterviewBitThreadExample();  
       ib.start();  
   }  
}
Implementing the Runnable interface
class InterviewBitThreadExample implements Runnable{  
   public void run(){  
       System.out.println("Thread runs...");  
   }  
   public static void main(String args[]){  
       Thread ib = new Thread(new InterviewBitThreadExample()); 
       ib.start();  
   }  
}
Implementing a thread using the method of Runnable interface is more preferred and advantageous as Java does not have support for multiple inheritances of classes.
start() method is used for creating a separate call stack for the thread execution. Once the call stack is created, JVM calls the run() method for executing the thread in that call stack.

----

46. What are the different types of Thread Priorities in Java? And what is the default priority of a thread assigned by JVM?
There are a total of 3 different types of priority available in Java. 

MIN_PRIORITY: It has an integer value assigned with 1.
MAX_PRIORITY: It has an integer value assigned with 10.
NORM_PRIORITY: It has an integer value assigned with 5.

In Java, Thread with MAX_PRIORITY gets the first chance to execute. But the default priority for any thread is NORM_PRIORITY assigned by JVM. 

----

47. What is the difference between the program and the process?
A program can be defined as a line of code written in order to accomplish a particular task. Whereas the process can be defined as the programs which are under execution. 
A program doesn't execute directly by the CPU. First, the resources are allocated to the program and when it is ready for execution then it is a process.

----

48. What is the difference between the ‘throw’ and ‘throws’ keyword in java?
The ‘throw’ keyword is used to manually throw the exception to the calling method.
And the ‘throws’ keyword is used in the function definition to inform the calling method that this method throws the exception. So if you are calling, then you have to handle the exception.
Example - 

class Main {
   public static int testExceptionDivide(int a, int b) throws ArithmeticException{
       if(a == 0 || b == 0)
           throw new ArithmeticException();
       return a/b;
   }
   public static void main(String args[]) {
       try{
           testExceptionDivide(10, 0);
       }
       catch(ArithmeticException e){
           //Handle the exception
       }
   }
}
Here in the above snippet, the method testExceptionDivide throws an exception. So if the main method is calling it then it must have handled the exception. Otherwise, the main method can also throw the exception to JVM.

And the method testExceptionDivide 'throws’ the exception based on the condition.

----

49. What are the differences between constructor and method of a class in Java?
Constructor	Method
Constructor is used for initializing the object state.	Method is used for exposing the object's behavior.
Constructor has no return type.	Method should have a return type. Even if it does not return anything, return type is void.
Constructor gets invoked implicitly.	Method has to be invoked on the object explicitly.
If the constructor is not defined, then a default constructor is provided by the java compiler.	If a method is not defined, then the compiler does not provide it.
The constructor name should be equal to the class name.	The name of the method can have any name or have a class name too.
A constructor cannot be marked as final because whenever a class is inherited, the constructors are not inherited. Hence, marking it final doesn't make sense. Java throws compilation error saying - modifier final not allowed here	A method can be defined as final but it cannot be overridden in its subclasses.
Final variable instantiations are possible inside a constructor and the scope of this applies to the whole class and its objects.	A final variable if initialised inside a method ensures that the variable cant be changed only within the scope of that method.

----

50. Identify the output of the below java program and Justify your answer.
class Main {
    public static void main(String args[]) {
        Scaler s = new Scaler(5);
    }
}
class InterviewBit{
    InterviewBit(){
        System.out.println(" Welcome to InterviewBit ");
    }
}
class Scaler extends InterviewBit{
    Scaler(){
        System.out.println(" Welcome to Scaler Academy ");
    }
    Scaler(int x){
        this();
        super();
        System.out.println(" Welcome to Scaler Academy 2");
    }
}
The above code will throw the compilation error. It is because the super() is used to call the parent class constructor. But there is the condition that super() must be the first statement in the block. Now in this case, if we replace this() with super() then also it will throw the compilation error. Because this() also has to be the first statement in the block. So in conclusion, we can say that we cannot use this() and super() keywords in the same block.

----

51. Java works as “pass by value” or “pass by reference” phenomenon?
Java always works as a “pass by value”. There is nothing called a “pass by reference” in Java. However, when the object is passed in any method, the address of the value is passed due to the nature of object handling in Java. When an object is passed, a copy of the reference is created by Java and that is passed to the method. The objects point to the same memory location. 2 cases might happen inside the method:

Case 1: When the object is pointed to another location: In this case, the changes made to that object do not get reflected the original object before it was passed to the method as the reference points to another location.
For example:

class InterviewBitTest{
   int num;
   InterviewBitTest(int x){ 
       num = x; 
   }
   InterviewBitTest(){ 
       num = 0; 
   }
}
class Driver {
   public static void main(String[] args)
   {
       //create a reference
       InterviewBitTest ibTestObj = new InterviewBitTest(20);
       //Pass the reference to updateObject Method
       updateObject(ibTestObj);
       //After the updateObject is executed, check for the value of num in the object.
       System.out.println(ibTestObj.num);
   }
   public static void updateObject(InterviewBitTest ibObj)
   {
       // Point the object to new reference
       ibObj = new InterviewBitTest();
       // Update the value 
       ibObj.num = 50;
   }
}
Output:
20
Case 2: When object references are not modified: In this case, since we have the copy of reference the main object pointing to the same memory location, any changes in the content of the object get reflected in the original object.
For example:

class InterviewBitTest{
   int num;
   InterviewBitTest(int x){ 
       num = x; 
   }
   InterviewBitTest(){ 
       num = 0; 
   }
}
class Driver{
   public static void main(String[] args)
   {
       //create a reference
       InterviewBitTest ibTestObj = new InterviewBitTest(20);
       //Pass the reference to updateObject Method
       updateObject(ibTestObj);
       //After the updateObject is executed, check for the value of num in the object.
       System.out.println(ibTestObj.num);
   }
   public static void updateObject(InterviewBitTest ibObj)
   {
       // no changes are made to point the ibObj to new location
       // Update the value of num
       ibObj.num = 50;
   }
}
Output:
50

----

52. What is the ‘IS-A ‘ relationship in OOPs java?
‘IS-A’ relationship is another name for inheritance. When we inherit the base class from the derived class, then it forms a relationship between the classes. So that relationship is termed an ‘IS-A’ Relationship.

Example - Consider a Television (Typical CRT TV). Now another Smart TV  that is inherited from television class. So we can say that the Smart iv is also a TV. Because CRT TV things can also be done in the Smart TV.


So here ‘IS-A’ Relationship formed. [ SmartTV ‘IS-A’ TV ].

----

53. Which among String or String Buffer should be preferred when there are lot of updates required to be done in the data?
StringBuffer is mutable and dynamic in nature whereas String is immutable. Every updation / modification of String creates a new String thereby overloading the string pool with unnecessary objects. Hence, in the cases of a lot of updates, it is always preferred to use StringBuffer as it will reduce the overhead of the creation of multiple String objects in the string pool.

----

54. How to not allow serialization of attributes of a class in Java?
In order to achieve this, the attribute can be declared along with the usage of transient keyword as shown below:
public class InterviewBitExample { 

   private transient String someInfo; 
   private String name;
   private int id;
   // :
   // Getters setters
   // :
} 
In the above example, all the fields except someInfo can be serialized.

----

55. What happens if the static modifier is not included in the main method signature in Java?
There wouldn't be any compilation error. But then the program is run, since the JVM cant map the main method signature, the code throws “NoSuchMethodError” error at the runtime.

----

56. Consider the below program, identify the output, and also state the reason for that.
public class Main{
public static void main(String[] args) {
 System.out.println(" Hello. Main Method. ");
}
public static void main(int[] args) {
 System.out.println(" Hello. Main Method2. ");
}
}
The output of the above program will be Hello. Main Method. This is because JVM will always call the main method based on the definition it already has. Doesn't matter how many main methods we overload it will only execute one main method based on its declaration in JVM.

----

57. Can we make the main() thread a daemon thread?
In java multithreading, the main() threads are always non-daemon threads. And there is no way we can change the nature of the non-daemon thread to the daemon thread.

----

58. What happens if there are multiple main methods inside one class in Java?
The program can't compile as the compiler says that the method has been already defined inside the class.

----

59. What do you understand by Object Cloning and how do you achieve it in Java?
It is the process of creating an exact copy of any object. In order to support this, a java class has to implement the Cloneable interface of java.lang package and override the clone() method provided by the Object class the syntax of which is:
protected Object clone() throws CloneNotSupportedException{
 return (Object)super.clone();
}
In case the Cloneable interface is not implemented and just the method is overridden, it results in CloneNotSupportedException in Java.

----

60. How does an exception propagate in the code?
When an exception occurs, first it searches to locate the matching catch block. In case, the matching catch block is located, then that block would be executed. Else, the exception propagates through the method call stack and goes into the caller method where the process of matching the catch block is performed. This propagation happens until the matching catch block is found. If the match is not found, then the program gets terminated in the main method.


logo
Practice Problems
Solve these problems to ace this concept
Exception Handling
Easy
4.57 Mins
Solve

Try Catch Block
Easy
3.35 Mins
Solve

Finally Block
Easy
2.42 Mins
Solve

----

61. How do exceptions affect the program if it doesn't handle them?
Exceptions are runtime errors. Suppose we are making an android application with java. And it all works fine but there is an exceptional case when the application tries to get the file from storage and the file doesn’t exist (This is the case of exception in java). And if this case is not handled properly then the application will crash. This will be a bad experience for users.  This is the type of error that cannot be controlled by the programmer. But programmers can take some steps to avoid this so that the application won’t crash. The proper action can be taken at this step.

----

62. Is it mandatory for a catch block to be followed after a try block?
No, it is not necessary for a catch block to be present after a try block. - A try block should be followed either by a catch block or by a finally block. If the exceptions likelihood is more, then they should be declared using the throws clause of the method.

----

63. Will the finally block get executed when the return statement is written at the end of try block and catch block as shown below?
public int someMethod(int i){
   try{
       //some statement
       return 1;
   }catch(Exception e){
       //some statement
       return 999;
   }finally{
       //finally block statements
   }
}
finally block will be executed irrespective of the exception or not. The only case where finally block is not executed is when it encounters ‘System.exit()’ method anywhere in try/catch block.

----

64. Can you call a constructor of a class inside the another constructor?
Yes, the concept can be termed as constructor chaining and can be achieved using this().

----

65. Contiguous memory locations are usually used for storing actual values in an array but not in ArrayList. Explain.
In the case of ArrayList, data storing in the form of primitive data types (like int, float, etc.) is not possible. The data members/objects present in the ArrayList have references to the objects which are located at various sites in the memory. Thus, storing of actual objects or non-primitive data types (like Integer, Double, etc.) takes place in various memory locations.


However, the same does not apply to the arrays. Object or primitive type values can be stored in arrays in contiguous memory locations, hence every element does not require any reference to the next element.

----

66. Why does the java array index start with 0?
It is because the 0 index array avoids the extra arithmetic operation to calculate the memory address.

Example - Consider the array and assume each element takes 4-byte memory space. Then the address will be like this -


Now if we want to access index 4. Then internally java calculates the address using the formula-

[Base Address + (index * no_of_bytes)]. So according to this. The starting address of the index 4 will be - [100 + (4*4)] = 116. And exactly that's what the address is calculated. 
Now consider the same with 1 index Array -


Now if we apply the same formula here. Then we get - 116 as the starting address of the 4th index. Which is wrong. Then we need to apply formula - [Base Address + ((index-1) * no_of_bytes)].

And for calculating this, an extra arithmetic operation has to be performed. And consider the case where millions of addresses need to be calculated, this causes complexity. So to avoid this, ) the index array is supported by java.

----

67. Why is the remove method faster in the linked list than in an array?
In the linked list, we only need to adjust the references when we want to delete the element from either end or the front of the linked list. But in the array, indexes are used. So to manage proper indexing, we need to adjust the values from the array So this adjustment of value is costlier than the adjustment of references.

Example - To Delete from the front of the linked list, internally the references adjustments happened like this.


The only thing that will change is that the head pointer will point to the head’s next node. And delete the previous node. That is the constant time operation.

Whereas in the ArrayList, internally it should work like this-


For deletion of the first element, all the next element has to move to one place ahead. So this copying value takes time. So that is the reason why removing in ArrayList is slower than LinkedList.

----

68. How many overloaded add() and addAll() methods are available in the List interface? Describe the need and uses.
There are a total of 4 overloaded methods for add() and addAll() methods available in List Interface. The below table states the description of all.

Return Type	Method Description
boolean	add(Element e): This method is used for adding the element at the end of the List. The Datatype of the element is of any type it has been initially assigned with. It returns the boolean indicating successfully inserted or not.
void	add(int index, Element e): This method is the overloaded version of add() method. In this, along with the element, the index is also passed to the method for the specific index the value needs to be inserted. 
boolean	addAll(Collection <extends ? Element > c): This method helps to add all elements at the end of collections from the list received in the parameter. It contains an iterator that helps to iterate the list and add the elements to the collection.
boolean	addAll(int index, Collection <extends ? Element > c): This is the overloaded method for addAll() method. In this along with the list, we can pass the specified index from which the list elements need to be added.
69. How does the size of ArrayList grow dynamically? And also state how it is implemented internally.
ArrayList is implemented in such a way that it can grow dynamically. We don't need to specify the size of ArrayList. For adding the values in it, the methodology it uses is -

1. Consider initially that there are 2 elements in the ArrayList. [2, 3].

2. If we need to add the element into this. Then internally what will happen is-

ArrayList will allocate the new ArrayList of Size (current size + half of the current size). And add the old elements into the new. Old - [2, 3],    New - [2, 3, null].

Then the new value will be inserted into it. [2, 3, 4, null]. And for the next time, the extra space will be available for the value to be inserted.

3. This process continues and the time taken to perform all of these is considered as the amortized constant time. 

This is how the ArrayList grows dynamically. And when we delete any entry from the ArrayList then the following steps are performed -

1. It searches for the element index in the array. Searching takes some time. Typically it’s O(n) because it needs to search for the element in the entire array.


2. After searching the element, it needs to shift the element from the right side to fill the index.


So this is how the elements are deleted from the ArrayList internally. Similarly, the search operations are also implemented internally as defined in removing elements from the list (searching for elements to delete).

Java Interview Questions for Experienced

----

70. Although inheritance is a popular OOPs concept, it is less advantageous than composition. Explain.
Inheritance lags behind composition in the following scenarios:

Multiple-inheritance is not possible in Java. Classes can only extend from one superclass. In cases where multiple functionalities are required, for example - to read and write information into the file, the pattern of composition is preferred. The writer, as well as reader functionalities, can be made use of by considering them as the private members.
Composition assists in attaining high flexibility and prevents breaking of encapsulation.
Unit testing is possible with composition and not inheritance. When a developer wants to test a class composing a different class, then Mock Object can be created for signifying the composed class to facilitate testing. This technique is not possible with the help of inheritance as the derived class cannot be tested without the help of the superclass in inheritance.
The loosely coupled nature of composition is preferable over the tightly coupled nature of inheritance.
Let’s take an example:

package comparison;
public class Top {
public int start() {
  return 0;
}
}
class Bottom extends Top {
 public int stop() {
  return 0;
 }
}
In the above example, inheritance is followed. Now, some modifications are done to the Top class like this:

public class Top {
 public int start() {
  return 0;
 }
 public void stop() {
 }
}
If the new implementation of the Top class is followed, a compile-time error is bound to occur in the Bottom class. Incompatible return type is there for the Top.stop() function. Changes have to be made to either the Top or the Bottom class to ensure compatibility. However, the composition technique can be utilized to solve the given problem:

class Bottom {
 Top par = new Top();
 public int stop() {
  par.start();
  par.stop();
  return 0;
 }
} 

----

71. What is the difference between ‘>>’ and ‘>>>’ operators in java?
These 2 are the bitwise right shift operators. Although both operators look similar. But there is a minimal difference between these two right shift operators.

‘>>’ Bitwise Right Shift Operator- This operator shifts each bit to its right position. And this maintains the signed bit.
‘>>>’ Bitwise Right Shift Operator with trailing zero- This operator also shifts each bit to its right. But this doesn’t maintain the signed bit. This operator makes the Most significant bit to 0.
Example- Num1 = 8, Num2 = -8.

So the binary form of these numbers are - 

Num1 = 00000000 00000000 00000000 00001000 
Num2 = 11111111 11111111 11111111  11111000

‘>>’ Operator : 8 >> 1 (Shift by one bit) : 

Num1 = 00000000 00000000 00000000 00000100
Num2 = 11111111 11111111 11111111  11111100

‘>>>’ Operator : 8 >>> 1 (Shift by one bit) = 

Num1 = 00000000 00000000 00000000 00000100
Num2 = 01111111 11111111 11111111 11111100

----

72. What are Composition and Aggregation? State the difference.
Composition, and Aggregation help to build (Has - A - Relationship) between classes and objects. But both are not the same in the end. Let’s understand with the help of an example. 

Consider the University as a class that has some departments in it. So the university will be the container object. And departments in it will contain objects. Now in this case, if the container object destroys then the contained objects will also get destroyed automatically.  So here we can say that there is a strong association between the objects. So this Strong Association is called Composition.
Now consider one more example. Suppose we have a class department and there are several professors' objects there in the department. Now if the department class is destroyed then the professor's object will become free to bind with other objects. Because container objects (Department) only hold the references of contained objects (Professor’s). So here is the weak association between the objects. And this weak association is called Aggregation.

----

73. How is the creation of a String using new() different from that of a literal?
When a String is formed as a literal with the assistance of an assignment operator, it makes its way into the String constant pool so that String Interning can take place. This same object in the heap will be referenced by a different String if the content is the same for both of them.

public bool checking() {
String first = "InterviewBit";
String second = "InterviewBit";
if (first == second)
 return true;
else
 return false;
}
The checking() function will return true as the same content is referenced by both the variables.


Conversely, when a String formation takes place with the help of a new() operator, interning does not take place. The object gets created in the heap memory even if the same content object is present.

public bool checking() {
String first = new String("InterviewBit");
String second = new String("InterviewBit");
if (first == second)
 return true;
else
 return false;
}
The checking() function will return false as the same content is not referenced by both the variables.


----

74. How is the ‘new’ operator different from the ‘newInstance()’ operator in java?
Both ‘new’ and ‘newInstance()’ operators are used to creating objects. The difference is- that when we already know the class name for which we have to create the object then we use a new operator. But suppose we don’t know the class name for which we need to create the object, Or we get the class name from the command line argument, or the database, or the file. Then in that case we use the ‘newInstance()’ operator.

The ‘newInstance()’ keyword throws an exception that we need to handle. It is because there are chances that the class definition doesn’t exist, and we get the class name from runtime. So it will throw an exception.

----

75. Is exceeding the memory limit possible in a program despite having a garbage collector?
Yes, it is possible for the program to go out of memory in spite of the presence of a garbage collector. Garbage collection assists in recognizing and eliminating those objects which are not required in the program anymore, in order to free up the resources used by them.

In a program, if an object is unreachable, then the execution of garbage collection takes place with respect to that object. If the amount of memory required for creating a new object is not sufficient, then memory is released for those objects which are no longer in the scope with the help of a garbage collector. The memory limit is exceeded for the program when the memory released is not enough for creating new objects.

Moreover, exhaustion of the heap memory takes place if objects are created in such a manner that they remain in the scope and consume memory. The developer should make sure to dereference the object after its work is accomplished. Although the garbage collector endeavors its level best to reclaim memory as much as possible, memory limits can still be exceeded.

Let’s take a look at the following example:

List<String> example = new LinkedList<String>();
while(true){
example.add(new String("Memory Limit Exceeded"));
}

----

76. Why is synchronization necessary? Explain with the help of a relevant example.
Concurrent execution of different processes is made possible by synchronization. When a particular resource is shared between many threads, situations may arise in which multiple threads require the same shared resource.

Synchronization assists in resolving the issue and the resource is shared by a single thread at a time. Let’s take an example to understand it more clearly. For example, you have a URL and you have to find out the number of requests made to it. Two simultaneous requests can make the count erratic.

No synchronization:

package anonymous;
public class Counting {
       private int increase_counter;
       public int increase() {
               increase_counter = increase_counter + 1;
               return increase_counter;
       }
}

If a thread Thread1 views the count as 10, it will be increased by 1 to 11. Simultaneously, if another thread Thread2 views the count as 10, it will be increased by 1 to 11. Thus, inconsistency in count values takes place because the expected final value is 12 but the actual final value we get will be 11.

Now, the function increase() is made synchronized so that simultaneous accessing cannot take place.

With synchronization:

package anonymous;
public class Counting {
       private int increase_counter;
       public synchronized int increase() {
               increase_counter = increase_counter + 1;
               return increase_counter;
       }
}

If a thread Thread1 views the count as 10, it will be increased by 1 to 11, then the thread Thread2 will view the count as 11, it will be increased by 1 to 12. Thus, consistency in count values takes place.

----

77. In the given code below, what is the significance of ... ?
public void fooBarMethod(String... variables){
   // method code
}
Ability to provide ... is a feature called varargs (variable arguments) which was introduced as part of Java 5.
The function having ... in the above example indicates that it can receive multiple arguments of the datatype String.
For example, the fooBarMethod can be called in multiple ways and we can still have one method to process the data as shown below:
fooBarMethod("foo", "bar");
fooBarMethod("foo", "bar", "boo");
fooBarMethod(new String[]{"foo", "var", "boo"});
public void myMethod(String... variables){
   for(String variable : variables){
       // business logic
   }
}

----

78. What will be the output of the below java program and define the steps of Execution of the java program with the help of the below code?
class InterviewBit{
    int i;
    static int j;
    {
        System.out.println(" Instance Block 1. Value of i = "+i);
    }
    static{
        System.out.println(" Static Block 1. Value of j = "+j);
        method_2();
    }
    {
        i = 5;
    }
    static{
        j = 10;
    }
    InterviewBit(){
        System.out.println(" Welcome to InterviewBit ");
    }
    public static void main(String[] args){
        InterviewBit ib = new InterviewBit();
    }
    public void method_1(){
        System.out.println(" Instance method. ");
    }
    static{
        System.out.println(" Static Block 2. Value of j = "+j);
    }
    {
        System.out.println(" Instance Block 2. Value of i = "+i);
        method_1();
    }
    public static void method_2(){
        System.out.println(" Static method. ");
    }
}
The Output we get by executing this program will be

Static Block 1. Value of j = 0
Static method. 
Static Block 2. Value of j = 10
Instance Block 1. Value of i = 0
Instance Block 2. Value of i = 5
Instance method. 
Welcome to InterviewBit

This is a java tricky interview question frequently asked in java interviews for the experienced. The output will be like this because, when the java program is compiled and gets executed, then there are various steps followed for execution. And the steps are - 

Identification of Static Members from top to bottom.
Execution of Static variable assignment and a Static block from top to bottom.
Execution of the main method.
Identification of Instance Members from top to bottom.
Execution of Instance variable assignment and Instance block from top to bottom.
Execution of Constructor.
In above steps from 4 to 6, will be executed for every object creation. If we create multiple objects then for every object these steps will be performed.

Now from the above code, the execution will happen like this - 

1. In the step of identification of static members. It is found that -

static int j.
static block.
main method.
static method_2.
During identification, the JVM will assign the default value in the static int j variable. Then it is currently in the state of reading and indirectly writing. Because the original value is not assigned.

2. In the next step, it will execute the static block and assign the value in static variables.

First static block it will print and because execution from top to bottom and original value in j is not assigned. So it will print the default value of 0.
After executing static block 1. It will execute the static method_1 because it is called from the static block 1.
Then it will assign the original value of 5 in the j variable. And executes the remaining static block.
3. Now it will execute the main method. In which it will create an object for the class InterviewBit. And then the execution of instances will happen.

4. Identify the instance variables and blocks from top to bottom. 

int i.
Instance block 1.
Instance method_1.
Like a static variable, the instance variable also has been initialized with the default value 0 and will be in the state of reading and writing indirectly.

5. It will execute the instance methods and assign the original value to the instance variable.

Prints the Instance block 1. And the current value of i is not assigned till now, so it will print 0.
Assign the original value to i. Then print instance block 2. And after that instance method will be called and printed because it is being called in the instance block.
6. And at the last step, the constructor will be invoked and the lines will be executed in the constructor.

This is how the java program gets executed.

----

79. Define System.out.println().
System.out.println() is used to print the message on the console. System - It is a class present in java.lang package. Out is the static variable of type PrintStream class present in the System class. println() is the method present in the PrintStream class.

So if we justify the statement, then we can say that if we want to print anything on the console then we need to call the println() method that was present in PrintStream class. And we can call this using the output object that is present in the System class.

----

80. Can you explain the Java thread lifecycle?
Java thread life cycle is as follows:

New – When the instance of the thread is created and the start() method has not been invoked, the thread is considered to be alive and hence in the NEW state.
Runnable – Once the start() method is invoked, before the run() method is called by JVM, the thread is said to be in RUNNABLE (ready to run) state. This state can also be entered from the Waiting or Sleeping state of the thread.
Running – When the run() method has been invoked and the thread starts its execution, the thread is said to be in a RUNNING state.
Non-Runnable (Blocked/Waiting) – When the thread is not able to run despite the fact of its aliveness, the thread is said to be in a NON-RUNNABLE state. Ideally, after some time of its aliveness, the thread should go to a runnable state.
A thread is said to be in a Blocked state if it wants to enter synchronized code but it is unable to as another thread is operating in that synchronized block on the same object. The first thread has to wait until the other thread exits the synchronized block.
A thread is said to be in a Waiting state if it is waiting for the signal to execute from another thread, i.e it waits for work until the signal is received.
Terminated – Once the run() method execution is completed, the thread is said to enter the TERMINATED step and is considered to not be alive.
The following flowchart clearly explains the lifecycle of the thread in Java.

----

81. What could be the tradeoff between the usage of an unordered array versus the usage of an ordered array?
The main advantage of having an ordered array is the reduced search time complexity of O(log n) whereas the time complexity in an unordered array is O(n).
The main drawback of the ordered array is its increased insertion time which is O(n) due to the fact that its element has to reordered to maintain the order of array during every insertion whereas the time complexity in the unordered array is only O(1).
Considering the above 2 key points and depending on what kind of scenario a developer requires, the appropriate data structure can be used for implementation.

----

82. Is it possible to import the same class or package twice in Java and what happens to it during runtime?
It is possible to import a class or package more than once, however, it is redundant because the JVM internally loads the package or class only once.

----

83. In case a package has sub packages, will it suffice to import only the main package? e.g. Does importing of com.myMainPackage.* also import com.myMainPackage.mySubPackage.*?
This is a big NO. We need to understand that the importing of the sub-packages of a package needs to be done explicitly. Importing the parent package only results in the import of the classes within it and not the contents of its child/sub-packages.

----

84. Will the finally block be executed if the code System.exit(0) is written at the end of try block?
NO. The control of the program post System.exit(0) is immediately gone and the program gets terminated which is why the finally block never gets executed.

----

85. What do you understand by marker interfaces in Java?
Marker interfaces, also known as tagging interfaces are those interfaces that have no methods and constants defined in them. They are there for helping the compiler and JVM to get run time-related information regarding the objects.

----

86. Explain the term “Double Brace Initialisation” in Java?
This is a convenient means of initializing any collections in Java. Consider the below example.

import java.util.HashSet;
import java.util.Set;
 
public class IBDoubleBraceDemo{
   public static void main(String[] args){
       Set<String> stringSets = new HashSet<String>()
       {
           {
               add("set1");
               add("set2");
               add("set3");
           }
       };
 
       doSomething(stringSets);
   }
 
   private static void doSomething(Set<String> stringSets){
       System.out.println(stringSets);
   }
}
In the above example, we see that the stringSets were initialized by using double braces.

The first brace does the task of creating an anonymous inner class that has the capability of accessing the parent class’s behavior. In our example, we are creating the subclass of HashSet so that it can use the add() method of HashSet.
The second braces do the task of initializing the instances.
Care should be taken while initializing through this method as the method involves the creation of anonymous inner classes which can cause problems during the garbage collection or serialization processes and may also result in memory leaks.

----

87. Why is it said that the length() method of String class doesn't return accurate results?
The length method returns the number of Unicode units of the String. Let's understand what Unicode units are and what is the confusion below.
We know that Java uses UTF-16 for String representation. With this Unicode, we need to understand the below two Unicode related terms:
Code Point: This represents an integer denoting a character in the code space.
Code Unit: This is a bit sequence used for encoding the code points. In order to do this, one or more units might be required for representing a code point.
Under the UTF-16 scheme, the code points were divided logically into 17 planes and the first plane was called the Basic Multilingual Plane (BMP). The BMP has classic characters - U+0000 to U+FFFF. The rest of the characters- U+10000 to U+10FFFF were termed as the supplementary characters as they were contained in the remaining planes.
The code points from the first plane are encoded using one 16-bit code unit
The code points from the remaining planes are encoded using two code units.
Now if a string contained supplementary characters, the length function would count that as 2 units and the result of the length() function would not be as per what is expected.

In other words, if there is 1 supplementary character of 2 units, the length of that SINGLE character is considered to be TWO - Notice the inaccuracy here? As per the java documentation, it is expected, but as per the real logic, it is inaccurate.

----

88. What is the output of the below code and why?
public class InterviewBit{
   public static void main(String[] args)
   {
       System.out.println('b' + 'i' + 't');
   }
}
“bit” would have been the result printed if the letters were used in double-quotes (or the string literals). But the question has the character literals (single quotes) being used which is why concatenation wouldn't occur. The corresponding ASCII values of each character would be added and the result of that sum would be printed.
The ASCII values of ‘b’, ‘i’, ‘t’ are:

‘b’ = 98
‘i’ = 105
‘t’ = 116
98 + 105 + 116 = 319

Hence 319 would be printed.

----

89. What are the possible ways of making object eligible for garbage collection (GC) in Java?
First Approach: Set the object references to null once the object creation purpose is served.

public class IBGarbageCollect {
  public static void main (String [] args){
       String s1 = "Some String";
           // s1 referencing String object - not yet eligible for GC
       s1 = null; // now s1 is eligible for GC
   }
 }
Second Approach: Point the reference variable to another object. Doing this, the object which the reference variable was referencing before becomes eligible for GC.

public class IBGarbageCollect {
 public static void main(String [] args){
     String s1 = "To Garbage Collect";
     String s2 = "Another Object";
     System.out.println(s1); // s1 is not yet eligible for GC
     s1 = s2; // Point s1 to other object pointed by s2
     /* Here, the string object having the content  "To Garbage Collect" is not referred by any reference variable. Therefore, it is eligible for GC */
 }
}
Third Approach: Island of Isolation Approach: When 2 reference variables pointing to instances of the same class, and these variables refer to only each other and the objects pointed by these 2 variables don't have any other references, then it is said to have formed an “Island of Isolation” and these 2 objects are eligible for GC.

public class IBGarbageCollect {
   IBGarbageCollect ib;    
   public static void main(String [] str){
       IBGarbageCollect ibgc1 = new IBGarbageCollect();
       IBGarbageCollect ibgc2 = new IBGarbageCollect();
       ibgc1.ib = ibgc2; //ibgc1 points to ibgc2
       ibgc2.ib = ibgc1; //ibgc2 points to ibgc1
       ibgc1 = null;
       ibgc2 = null;
       /* 
       * We see that ibgc1 and ibgc2 objects refer 
       * to only each other and have no valid 
       * references- these 2 objects for island of isolcation - eligible for GC
       */
   }
}

----

90. In the below Java Program, how many objects are eligible for garbage collection?
class Main{
   public static void main(String[] args){
       int[][] num = new int[3][];
       num[0] = new int[5];
       num[1] = new int[2];
       num[2] = new int[3];
       
       num[2] = new int[5];
       num[0] = new int[4];
       num[1] = new int[3];
       
       num = new int[2][];
   }
}
In the above program, a total of 7 objects will be eligible for garbage collection. Let’s visually understand what's happening in the code.



In the above figure on line 3, we can see that on each array index we are declaring a new array so the reference will be of that new array on all the 3 indexes. So the old array will be pointed to by none. So these three are eligible for garbage collection. And on line 4, we are creating a new array object on the older reference. So that will point to a new array and older multidimensional objects will become eligible for garbage collection.

----

91. What is the best way to inject dependency? Also, state the reason.
There is no boundation for using a particular dependency injection. But the recommended approach is - 

Setters are mostly recommended for optional dependencies injection, and constructor arguments are recommended for mandatory ones. This is because constructor injection enables the injection of values into immutable fields and enables reading them more easily.

----

92. How we can set the spring bean scope. And what supported scopes does it have?
A scope can be set by an annotation such as the @Scope annotation or the "scope" attribute in an XML configuration file. Spring Bean supports the following five scopes:

Singleton
Prototype
Request
Session
Global-session

----

93. What are the different categories of Java Design patterns?
Java Design patterns are categorized into the following different types. And those are also further categorized as 

Structural patterns:

Adapter
Bridge
Filter
Composite
Decorator
Facade
Flyweight
Proxy
Behavioral patterns:

Interpreter
Template method/ pattern
Chain of responsibility
Command pattern
Iterator pattern
Strategy pattern
Visitor pattern
J2EE patterns:

MVC Pattern
Data Access Object pattern
Front controller pattern
Intercepting filter pattern
Transfer object pattern
Creational patterns:

Factory method/Template
Abstract Factory
Builder
Prototype
Singleton

----

94. What is a Memory Leak? Discuss some common causes of it.
The Java Garbage Collector (GC) typically removes unused objects when they are no longer required, but when they are still referenced, the unused objects cannot be removed. So this causes the memory leak problem. Example - Consider a linked list like the structure below -


In the above image, there are unused objects that are not referenced. But then also Garbage collection will not free it. Because it is referencing some existing referenced object. So this can be the situation of memory leak.

Some common causes of Memory leaks are - 

When there are Unbounded caches.
Excessive page swapping is done by the operating system.
Improper written custom data structures.
Inserting into a collection object without first deleting it.
etc.

----

95. Assume a thread has a lock on it, calling the sleep() method on that thread will release the lock?
A thread that has a lock won't be released even after it calls sleep(). Despite the thread sleeping for a specified period of time, the lock will not be released.

Java Programming Interview Questions

----

96. Check if a given string is palindrome using recursion.
/*
* Java program to check if a given inputted string is palindrome or not using recursion.
*/
import java.util.*;
public class InterviewBit { 
   public static void main(String args[]) { 
       Scanner s = new Scanner(System.in);
       String word = s.nextLine();
       System.out.println("Is "+word+" palindrome? - "+isWordPalindrome(word));
   } 
   
   
   public static boolean isWordPalindrome(String word){ 
       String reverseWord = getReverseWord(word); 
       //if word equals its reverse, then it is a palindrome
       if(word.equals(reverseWord)){ 
           return true; 
       } 
       return false; 
   } 
   
   public static String getReverseWord(String word){ 
       if(word == null || word.isEmpty()){ 
           return word; 
       } 
       
       return word.charAt(word.length()- 1) + getReverseWord(word.substring(0, word.length() - 1)); 
   } 
} 
logo
Practice Problems
Solve these problems to ace this concept
Substring
Medium
9.47 Mins
Solve

StringBuffer
Easy
24.24 Mins
Solve

----

97. Write a Java Program to print Fibonacci Series using Recursion.
class InterviewBit {
    public static void printFibonacci(int val_1, int val_2, int num){
        //Base Case
        if(num == 0)
            return;

        //Printing the next Fibonacci number    
        System.out.print( val_1 + val_2 + " ");

        //Recursively calling for printing Fibonacci for remaining length
        printFibonacci(val_2, val_1+val_2, --num);
    }
    public static void main(String args[]) {
        System.out.println(" *** Fibonacci Series *** ");

        //Printing the first two values
        System.out.print("0 1 ");

        //Calling Method to print the fibonacci for length 10
        printFibonacci(0, 1, 10);
    }
}
In the above code, we are printing the base 2 Fibonacci values 0 and 1. And then based on the length of Fibonacci to be printed, we are using the helper function to print that.

----

98. Write a Java program to check if the two strings are anagrams.
The main idea is to validate the length of strings and then if found equal, convert the string to char array and then sort the arrays and check if both are equal.

import java.util.Arrays;
import java.util.Scanner;
public class InterviewBit {
 public static void main(String[] args) {
   Scanner s = new Scanner(System.in);
   //Input from two strings
   System.out.print("First String: ");
   String string1 = s.nextLine();
   System.out.print("Second String: ");
   String string2 = s.nextLine();
   // check for the length
   if(string1.length() == string2.length()) {
     // convert strings to char array
     char[] characterArray1 = string1.toCharArray();
     char[] characterArray2 = string2.toCharArray();
     // sort the arrays
     Arrays.sort(characterArray1);
     Arrays.sort(characterArray2);
     // check for equality, if found equal then anagram, else not an anagram
     boolean isAnagram = Arrays.equals(characterArray1, characterArray2);
     System.out.println("Anagram: "+ isAnagram);
 }
}

----

99. Write a Java Program to find the factorial of a given number.
public class FindFactorial {
   public static void main(String[] args) {
       int num = 10;
       long factorialResult = 1l;
       for(int i = 1; i <= num; ++i)
       {
           factorialResult *= i;
       }
       System.out.println("Factorial: "+factorialResult);
   }
}

----

100. Given an array of non-duplicating numbers from 1 to n where one number is missing, write an efficient java program to find that missing number.
Idea is to find the sum of n natural numbers using the formula and then finding the sum of numbers in the given array. Subtracting these two sums results in the number that is the actual missing number. This results in O(n) time complexity and O(1) space complexity.

public class IBMissingNumberProblem {

   public static void main(String[] args) {

       int[] array={4,3,8,7,5,2,6};
       int missingNumber = findMissingNum(array);
       System.out.println("Missing Number is "+ missingNumber); 
   }

   public static int findMissingNum(int[] array) {
       int n=array.length+1;
       int sumOfFirstNNums=n*(n+1)/2;
       int actualSumOfArr=0;
       for (int i = 0; i < array.length; i++) {
           actualSumOfArr+=array[i];
       }
       return sumOfFirstNNums-actualSumOfArr;
   }
}

----

101. Write a Java Program to check if any number is a magic number or not. A number is said to be a magic number if after doing sum of digits in each step and inturn doing sum of digits of that sum, the ultimate result (when there is only one digit left) is 1.
Example, consider the number:

Step 1: 163 => 1+6+3 = 10
Step 2: 10 => 1+0 = 1 => Hence 163 is a magic number
public class IBMagicNumber{

   public static void main(String[] args) { 
       int num = 163;  
       int sumOfDigits = 0;
       while (num > 0 || sumOfDigits > 9) 
       { 
           if (num == 0) 
           { 
               num = sumOfDigits; 
               sumOfDigits = 0; 
           } 
           sumOfDigits += num % 10; 
           num /= 10; 
       } 

       // If sum is 1, original number is magic number 
       if(sumOfDigits == 1) {
           System.out.println("Magic number");
       }else {
           System.out.println("Not magic number");
       }
   }
}

----

102. Write a Java program to create and throw custom exceptions.
class InterviewBit {
    public static void main(String args[]) throws CustomException {

        // Throwing the custom exception be passing the message
        throw new CustomException(" This is my custom Exception ");
    }
}
//Creating Custom Exception Class
class CustomException extends Exception{
    //Defining Constructor to throw exception message
    public CustomException(String message){
        super(message);
    }
}
We have created the exception class named with CustomException and called the base exception constructor with the error message that we want to print. And to avoid handling exceptions in the main method, we have used the throws keyword in the method declaration.

----

103. Write a Java program to reverse a string.
class InterviewBit{
    public static void main(String[] args){
        //Input String
        String str = "Welcome to InterviewBit";
        
        //Pointers.
        int i = 0, j = str.length()-1;
        
        //Result character array to store the reversed string.
        char[] revString = new char[j+1];
        
        //Looping and reversing the string.
        while(i < j){
            revString[j] = str.charAt(i);
            revString[i] = str.charAt(j);
            i++;
            j--;
        }
        //Printing the reversed String.
        System.out.println("Reversed String = " + String.valueOf(revString));
    }
}
In the above code, we are storing the last character from the string to the first and the first value to the last in the output character array. And doing the same thing in the loop for the remaining 2nd to n-1 characters. This is how the string will be reversed.

----

104. Write a Java program to rotate arrays 90 degree clockwise by taking matrices from user input.
mport java.util.Scanner;
public class InterviewBit
{
    public static void main(String[] args) {
	  Scanner sc = new Scanner(System.in);
	  int no;
        System.out.print("Enter size of Array : ");
        no = sc.nextInt();
        int[][] a = new int[no][no];
        System.out.print("Enter  "+ no*no+" Element Array : ");
        
        for(int i = 0; i<no; i++){
            for(int j = 0; j<no; j++){
                a[i][j] = sc.nextInt();
            }
        }
        System.out.print("\nArray Before Rotation\n\n");
        for(int i = 0; i<no; i++){
            for(int j = 0; j<no; j++){
                System.out.print(a[i][j] + " ");
            }
            System.out.println();
        }
    
        System.out.println("\n");
        //Rotation
        
        //Transpose
        for(int i = 0; i < no; i++){
            for(int j = i; j < no; j++){
                int temp = a[i][j];
                a[i][j] = a[j][i];
                a[j][i] = temp;
            }
        }
        
        //Reverse Each row
        for(int i = 0; i < no; i++){
            int l, j;
            for(j = 0, l = no -1; j < l; j++){
                int temp = a[i][j];
                a[i][j] = a[i][l];
                a[i][l] = temp;
                l--;
            }
        }
        
        System.out.println("Array After Rotation - \n");
    
        for(int i = 0; i<no; i++){
            for(int j = 0; j<no; j++){
                System.out.print(a[i][j] + " ");
            }
            System.out.println();
        }
    }
}
In the above code, for rotating the matrix to  90 degrees we are first transposing the matrix so the row becomes the column. And after that, we are reversing each row in the matrix. So this is how the matrix got rotated.

----

105. Write a java program to check if any number given as input is the sum of 2 prime numbers.
Example :

Input - 18

Output - 

18 = 13 + 5
18 = 11 + 7

public class InterviewBit
{
    // Method to Check Prime Number
    private static int check_prime(int num){
        int flag = 0;
        for(int i = 2; i<=num/2; i++){
            if(num%i == 0){
                flag = 1;
                return 1;
            }
        }
        if(flag == 0)
            return 0;
        return 1;
    }
    // Method to get print the prime sum
    private static void find(int num){
        for(int i = 2; i <= num/2; i++){
            if(check_prime(i) == 0){
                if(check_prime(num-i) == 0)
                    System.out.println(num + " = "+ (num-i) + " "+ i);
            }
        }
    }
	public static void main(String[] args) {
		find(18);
	}
}
In the above code, for any number n, we find all the 2 pairs of numbers that are added together resulting in n. And each checking number if it is prime. If it is prime then we are printing that.

----

106. Write a Java program for solving the Tower of Hanoi Problem.
public class InterviewBit
{
    //Recursive Method for Solving the Tower of hanoi.
    private static void TOH(char source, char auxiliary, char destination, int numOfDisk){
    	if (numOfDisk > 0){
    		TOH(source, destination, auxiliary, numOfDisk-1);
    		System.out.println("Move 1 disk from "+source+" to "+destination+" using "+auxiliary+".");
    		TOH(auxiliary, source, destination, numOfDisk-1);
    	}
    }
	public static void main(String[] args) {
		TOH('A','B','C', 3);
	}
}
In the above code we are first moving the n-1 disk from Tower A to Tower B, then moving that nth disk from Tower A to Tower C, and finally, the remaining n-1 disk from Tower B to Tower C. And we are doing this recursively for the n-1 disk.

----

107. Implement Binary Search in Java using recursion.
public class Main
{
    //Recursive method for binary search
    private static boolean binarySearch(int[] arr, int low, int high, int key){
       
        //Calculating Mid.
        int mid = (low + high)/2;
       
        //Base Case.
        if(low > high)
            return false;
       
        //Checking if the key is found in the middle.
        if(arr[mid] == key)
            return true;
       
        //Searching on the left half if a key exists there.  
        if(key < arr[mid])
            return binarySearch(arr, low, mid-1, key);
       
        //Searching on the other half otherwise.
        return binarySearch(arr, mid+1, high, key);
    }
public static void main(String[] args) {
   
   int[] arr = {2, 5, 9, 13, 17, 21, 30};
   if(binarySearch(arr, 0, (arr.length-1), 30))
       System.out.println(" Element Found. ");
   else
       System.out.println(" Element not Found.");
}
}
In the above code, we are finding the middle element each time and checking if the element is in the middle or not. If it is not, then we check on which side from the middle it exists. And Recursively searching on the particular subarray. So this way we are reducing the search space by 2 every time. So the search time is very low.

Conclusion

----

108. Conclusion
Java is one of the simple high-level languages that provides powerful tools and impressive standards required for application development. It was also one of the first languages to provide amazing threading support for tackling concurrency-based problems. The easy-to-use syntax and the built-in features of Java combined with the stability it provides to applications are the main reasons for this language to have ever-growing usage in the software community.

Join our community and share your java interview experiences.

Recommended Interview Preparation Resources
How to Become a Java Developer?
How much does a Java Developer earn in India?
Java Projects
Java Programming Questions for interview
Java 8 Interview Questions
Java String Interview Questions
Spring Interview Questions
Hibernate Interview Questions
Java Collections Interview Questions
Array Interview Questions
Design Patterns Interview Questions
Multithreading Interview Questions
Java Tutorial
Java MCQ
Advance Java MCQ
Difference Between C++ and Java
Difference Between C and Java
Difference Between Java and Javascript
Kotlin Vs Java
Java Vs Python
Features of Java 9
Java 8 Features
Java Frameworks
Java Developer Skills
Java IDE
Java 11 Features
JAVA SE Download

Additional Technical Interview Questions

Java MCQ

----

1.
What is the component used for compiling, debugging, and executing java programs?


JDK

JVM

JRE

JIT

----

2.
What component does the task of bytecode to machine code conversion?


JDK

JVM

JRE

JIT

----

3.
Which of the following is the functionality of the java interpreter?


Interpretor is nothing but the JIT compiler.

It acts as medium between JVM and JIT.

It does the conversion of byte code to machine code.

It reads the high level code and executes them.

----

4.
When an object has its own lifecycle and its child object cant belong to another parent object, what is it called?


Association

Aggregation

Composition

Encapsulation

----

5.
What is the output of the below piece of code?

class InterviewBit {
    public void method1 (int num1,float num2){
         System.out.println("int-float method");
    }
    public void method1(float num1,int num2){
         System.out.println("float-int method");
    }
     public static void main(String[] args){
           InterviewBit interviewBit=new InterviewBit();
           interviewBit.method1(40,20);
     }
}

int-float method

float-int method

Compilation Error

Run Time error

----

6.
What is the output of the following code?

class InterviewBit{
       int fun (int n) 
       {
           int result;
           result = fun (n - 1);
           return result;
       }
   } 
class Driver{
       public static void main(String args[]) 
       {
           InterviewBit ib = new InterviewBit() ;
           System.out.print(ib.fun(12));
       }
   }

0

1

Compilation Error

Run time error

----

7.
Which of the following happens when the garbage collection process kicks off during the execution of the thread?


Garbage collection does not happen during thread execution.

Thread pauses while the garbage collection process runs.

Both the process takes place simultaneously and does not interfere its execution.

Nothing happens, the thread proceeds with execution.

----

8.
What is the output of the below code?

class InterviewBit{
   public static void main(String args[])
   {
       String obj = "Hello";
       String obj1 = "InterviewBit";   
       String obj2 = "Hello";
       System.out.println(obj.equals(obj1) + " " + obj.equals(obj2));
   }
}

false false

true true

true false

false true

----

9.
What is the functionality of Class.getInstance()?


It invokes the constructor.

It has the same functionality of new operator.

It creates object if the class does not have constructor defined.

None of the above.

----

10.
What is the output of the below code?

class InterviewBit{
       public int num1;
     static int num2;
       void calculate(int a, int b)
       {
           num1 +=  a ;
           num2 +=  b;
       }        
}    
class Driver{
       public static void main(String args[])
       {
           InterviewBit obj1 = new InterviewBit();
           InterviewBit obj2 = new InterviewBit();   
           obj1.num1 = 0;
           obj1.num2 = 0;
           obj1.calculate(1, 2);
           obj2.num1 = 0;
           obj2.calculate(2, 3);
           System.out.println(obj1.num1 + " " + obj2.num2);     
       }
}

1 2

1 5

4 2

2 5

----

11.
What is the output of the following code?

class InterviewBit{
       
       int calculate(int a, int b)
       {
           try{
               return a-b;
           }catch(Exception e){
               return a+b;
           }finally{
               return a*b;
           }
       }        
}    
class Driver{
       public static void main(String args[])
       {
           InterviewBit obj1 = new InterviewBit();
           int result = obj1.calculate(2, 3);
           System.out.println("Result: " + result);     
       }
}

</https://www.interviewbit.com/java-interview-questions/>

<https://javaconceptoftheday.com/top-25-simple-basic-java-interview-questions-for-freshers/>

Top 25 Simple Basic Java Interview Questions For Freshers
Below is the list of 25 most asked simple entry level basic java interview questions for freshers.

----

1) What are the main features of Java?

Below is the list of features of Java.

a) Object Oriented
b) Simple
c) Platform Independent
d) Secured
e) Robust
f) Portable
g) Multithreaded
h) Distributed

Click here to see these features in detail.

See More : 300+ Java Interview Questions For Freshers With Detail Explanation

----

2) What are the fundamental principles of object oriented programming?

a) Inheritance

b) Abstraction

c) Polymorphism

d) Encapsulation

----

3) What do you mean by inheritance in Java?

Inheritance is one of the key principle of object oriented programming. Through inheritance, one class can inherit the properties of another class. The class from which properties are inherited is called super class and the class to which properties are inherited is called sub class.

Click here to see more info on Inheritance in Java.

----

4) What is constructor overloading? What is the use of constructor overloading?

A class can have any number of constructors. These constructors will have different list of arguments. It is called constructor overloading. Constructor overloading provides different ways to instantiate a class.

Click here to see more on constructors in Java.

----

5) What is polymorphism in Java?

Polymorphism refers to any entity whether it is a method or a constructor or an operator which takes many forms or can be used for multiple tasks.

Click here to see more info on polymorphism in Java.

----

6) What is the method overloading in Java?

If a class has more than one method with same name but with different list of arguments, then it is called method overloading.

Click here to see more on method overloading in Java.

----

7) What is the method overriding?

If a super class method is modified in the sub class then it is called method overriding.

Click here to see more info on method overriding in Java.

----

8) Does java supports multiple inheritance?

Java supports multiple inheritance but only through interfaces. That means a class can implement more than one interfaces but can not extend more than one class.

----

9) What is the difference between constructor and method?

Constructor is a special member of a class which is used to create the objects to the class. It is special because it will have same name as class. It will have no return type.

Method is ordinary member of a class which is used to implement some behavior of a class. It will have it’s own name and return type.

----

10) Can we overload the main() method?

Yes, we can overload a main() method. A class can have any number of main() methods. But, one of those must be in the form “public static void main(String[] args)” in order to start the execution.

----

11) How the exceptions are handled in java? OR Explain try, catch and finally blocks in java?

Java has it’s own mechanism to handle the exceptions. In Java, exceptions are handled using three blocks – try, catch and finally blocks.

try block – The code to be monitored for exceptions will be kept in this block.

catch block – If any exceptions occurred in try block, those exceptions will be caught by this block.

finally block – This block will be always executed whether exception is raised or not and raised exceptions are caught or not.

See the complete Exception Handling tutorial here.

----

12) What are PATH and CLASSPATH?

PATH and CLASSPATH are two environment variables which need to be set in order to compile and run the Java programs.

----

13) What is multithreaded programming?

Multithreaded programming is one of the key features of java which allows multiple threads to execute their task simultaneously.

----

14) What is the difference between error and exception in Java?

Click here to see the differences between error and exception in Java.

----

15) What are the differences between static and non-static methods?

Static method is common to all instances of a class. Static methods are stored in the class memory. Where as non-static methods are stored in the object memory. Each instance of a class will have their own copy of non-static methods.

----

16) What are the differences between method overloading and method overriding?

Click here to see the differences between method overloading and overriding.

----

17) What are the different ways of creating threads in Java?

There are two ways to create the threads in Java

a) By extending java.lang.Thread class.

b) By implementing java.lang.Runnable interface.

See more.

----

18) What is synchronization in Java?

Synchronization is a way of controlling the access of a method or a block by multiple threads. Only one thread can enter into a method or a block which has been declared as synchronized. Synchronization is one of the way to achieve thread safety.

See more..

----

19) What is the use of final keyword in Java?

final keyword in java is used to restrict the modification of a class or a method or a variable. A final class can not be extended, a final method can not be overridden and we can not change the value of a final variable.

See more…

----

20) What is static binding and dynamic binding in Java?

Click here to see what is static binding and dynamic binding in Java.

----

21) What is garbage collection in Java?

Removing unwanted objects or abandoned objects from the memory is called garbage collection. Garbage collection is done automatically in java. You need not to remove the unwanted objects explicitly. Garbage collector thread does this for you. click here to see how garbage collector thread works in Java.

----

22) What are the differences between ArrayList and Vector class in Java?

Click here to see ArrayList Vs Vector in Java.

----

23) What is cloning in Java?

Cloning is a process of creating an exact copy of an existing object in the memory. Cloning may be shallow or deep. In java, clone() method is used to create a clone of an object.

See more…

----

24) What are differences between final, finally and finalize in Java?

Click here to see the differences between final, finally and finalize in Java.

----

25) What are checked and unchecked exceptions in Java?

Click here to see about checked and unchecked exceptions in Java.

</https://javaconceptoftheday.com/top-25-simple-basic-java-interview-questions-for-freshers/>

<https://beginnersbook.com/2013/05/java-interview-questions/>

----

Q) Is Java platform independent?
Yes. Java is a platform independent language. We can write java code on one platform and run it on another platform. For e.g. we can write and compile the code on windows and can run the generated bytecode on Linux or any other supported platform. This is one of the main features of java.

----

Q) What all memory areas are allocated by JVM?
Classloader, Class area, Heap, Stack, Program Counter Register and Native Method Stack

----

Q) Java vs. C ++?
Here are the few differences between Java and C++:

Platform dependency – C++ is platform dependent while java is platform independent
No goto support – Java doesn’t support goto statement while C++ does.
Multiple inheritance – C++ supports multiple inheritance while java does not.
Multithreading – C++ does not have in-build thread support, on the other hand java supports multithreading
Virtual keyword – C++ has virtual keyword, it determines if a member function of a class can be overridden in its child class. In java there is no concept of virtual keyword.

----

Q) Explain public static void main(String args[])
Here public is an access modifier, which means that this method is accessible by any class.

static – static keyword tells that this method can be accessed without creating the instance of the class. Refer: Static keyword in java

void – this main method returns no value.

main – It is the name of the method.

String args[] – The args is an array of String type. This contains the command line arguments that we can pass while running the program.

----

Q) What is javac ?
The javac is a compiler that compiles the source code of your program and generates bytecode. In simple words javac produces the java byte code from the source code written *.java file. JVM executes the bytecode to run the program.

----

Q) What is class?
A class is a blueprint or template or prototype from which you can create the object of that class. A class has set of properties and methods that are common to its objects.

----

Q) What is the base class of all classes?
java.lang.Object is the base class (super class) of all classes in java.

----

Q) What is a wrapper class in Java?
A wrapper class converts the primitive data type such as int, byte, char, boolean etc. to the objects of their respective classes such as Integer, Byte, Character, Boolean etc. Refer: Wrapper class in Java

----

Q) What is a path and classPath in Java?
Path specifies the location of .exe files. Classpath specifies the location of bytecode (.class files).

----

Q) Different Data types in Java.
byte – 8 bit
short – 16 bit
char – 16 bit Unicode
int – 32 bit (whole number)
float – 32 bit (real number)
long – 64 bit (Single precision)
double – 64 bit (double precision)

----

Q) What is Unicode?
Java uses Unicode to represent the characters. Unicode defines a fully international character set that can represent all of the characters found in human languages.

----

Q) What are Literals?
Any constant value that is assigned to a variable is called literal in Java. For example –

// Here 101 is a literal
int num = 101

----

Q) Dynamic Initialization?
Dynamic initialization is process in which initialization value of a variable isn’t known at compile-time. It’s computed at runtime to initialize the variable.

----

Q) What is Type casting in Java?
When we assign a value of one data type to the different data type then these two data types may not be compatible and needs a conversion. If the data types are compatible (for example assigning int value to long) then java does automatic conversion and does not require casting. However if the data types are not compatible then they need to be casted for conversion.

For example:

//here in the brackets we have mentioned long keyword, this is casting
double num = 10001.99;
long num2 = (long)num;

----

Q) What is an Array?
An array is a collection (group) of fixed number of items. Array is a homogeneous data structure which means we can store multiple values of same type in an array but it can’t contain multiple values of different types. For example an array of int type can only hold integer values.

----

Q) What is BREAK statement in java?
The break statement is used to break the flow sequence in Java.

break statement is generally used with switch case data structure to come out of the statement once a case is executed.
It can be used to come out of the loop in Java

----

Q) Arrays can be defined in different ways. Write them down.
int arr[];
int[] arr;
OOPs Interview Questions

----

Q) Four main principles of OOPS Concepts?
Inheritance
Polymorphism
Data Encapsulation
Abstraction

----

Q) What is inheritance?
The process by which one class acquires the properties and functionalities of another class is called inheritance. Inheritance brings reusability of code in a java application. Refer: Guide to Inheritance in Java.

----

Q) Does Java support Multiple Inheritance?
When a class extends more than one classes then it is called multiple inheritance. Java doesn’t support multiple inheritance whereas C++ supports it, this is one of the difference between java and C++.  Refer: Why java doesn’t support multiple inheritance?

----

Q) What is Polymorphism and what are the types of it?
Polymorphism is the ability of an object to take many forms. The most common use of polymorphism in OOPs is to have more than one method with the same name in a single class. There are two types of polymorphism: static polymorphism and dynamic polymorphism. Refer these guides to understand the polymorphism concept in detail: 1) Java Polymorphism 2) Types of Polymorphism

----

Q) What is method overriding in Java?
When a sub class (child class) overrides the method of super class(parent class) then it is called overriding. To override a method, the signature of method in child class must match with the method signature in parent class. Refer: Java – Method Overriding

----

Q) Can we override a static method?
No, we cannot override a static method in Java.

----

Q) What is method overloading?
When a class has more than one methods with the same name but different number, sequence or types of arguments then it is known as method overloading. Refer: Java – Method Overloading

----

Q) Does Java support operator overloading?
Operator overloading is not supported in Java.

----

Q) Can we overload a method by just changing the return type and without changing the signature of method?
No, We cannot do this. To overload a method, the method signature must be different, return type doesn’t play any role in method overloading.

----

Q) Is it possible to overload main() method of a class?
Yes, we can overload main() method in Java.

----

Q) What is the difference between method overloading and method overriding?
Refer this guide: Overloading vs overriding in Java

----

Q) What is static and dynamic binding in Java?
Binding refers to the linking of method call to its body. A binding that happens at compile time is known as static binding while binding at runtime is known as dynamic binding. Refer: Static and Dynamic binding in Java.

----

Q) What is Encapsulation?
Wrapping of the data and code together is known as encapsulation. Refer: Java Encapsulation.

----

Q) What is an abstract class in Java?
An abstract class is a class which can’t be instantiated (we cannot create the object of abstract class), we can only extend such classes. It provides the generalised form that will be shared by all of its subclasses, leaving it to each subclass to fill in the details. We can achieve partial abstraction using abstract classes, to achieve full abstraction we use interfaces.

----

Q) What is Interface in java?
An interface is used for achieving full abstraction. A class implements an interface, thereby inheriting the abstract methods of the interface. Refer: Java Interface

----

Q) What is the difference between abstract class and interface?
1) abstract class can have abstract and non-abstract methods. An interface can only have abstract methods.
2) An abstract class can have static methods but an interface cannot have static methods.
3) abstract class can have constructors but an interface cannot have constructors.

----

Q) Name the access modifiers that can be applied to the inner classes?
public ,private , abstract, final, protected.

----

Q) What is a constructor in Java?
Constructor is used for creating an instance of a class, they are invoked when an instance of class gets created. Constructor name and class name should be same and it doesn’t have a return type. Refer this guide: Java Constructor.

----

Q) Can we inherit the constructors?
No, we cannot inherit constructors.

----

Q) Can we mark constructors final?
No, Constructor cannot be declared final.

----

Q) What is default and parameterized constructors?
Default: Constructors with no arguments are known as default constructors, when you don’t declare any constructor in a class, compiler creates a default one automatically.

Parameterized: Constructor with arguments are known as parameterized constructors.

----

Q) Can a constructor call another constructor?
Yes. A constructor can call the another constructor of same class using this keyword. For e.g. this() calls the default constructor.
Note: this() must be the first statement in the calling constructor.

----

Q) Can a constructor call the constructor of parent class?
Yes. In fact it happens by default. A child class constructor always calls the parent class constructor. However we can still call it using super keyword. For e.g. super() can be used for calling super class default constructor.

Note: super() must be the first statement in a constructor.

----

Q)THIS keyword?
The this keyword is a reference to the current object.

----

Q) Can this keyword be assigned null value?
No, this keyword cannot have null values assigned to it.

----

Q) Explain ways to pass the arguments in Java?
In java, arguments can be passed as call by value – Java only supports call by value, there is no concept of call by reference in Java.

----

Q) What is static variable in java?
Static variables are also known as class level variables. A static variable is same for all the objects of that particular class in which it is declared.

----

Q) What is static block?
A static block gets executed at the time of class loading. They are used for initializing static variables.

----

Q) What is a static method?
Static methods can be called directly without creating the instance (Object) of the class. A static method can access all the static variables of a class directly but it cannot access non-static variables without creating instance of class.

----

Q) Explain super keyword in Java?
super keyword references to the parent class. There are several uses of super keyword:

It can be used to call the superclass(Parent class) constructor.
It can be used to access a method of the superclass that has been hidden by subclass (Calling parent class version, In case of method overriding).
To call the constructor of parent class.
Q) Use of final keyword in Java?
Final methods – These methods cannot be overridden by any other method.
Final variable – Constants, the value of these variable can’t be changed, its fixed.
Final class – Such classes cannot be inherited by other classes. These type of classes will be used when application required security or someone don’t want that particular class. Final Keyword in Java.

----

Q) What is a Object class?
This is a special class defined by java; all other classes are subclasses of object class. Object class is superclass of all other classes. Object class has the following methods

objectClone () – to creates a new object that is same as the object being cloned.
boolean equals(Object obj) – determines whether one object is equal to another.
finalize() – Called by the garbage collector on an object when garbage collection determines that there are no more references to the object. A subclass overrides the finalize method to dispose of system resources or to perform other cleanup.
toString () – Returns a string representation of the object.

----

Q) What are Packages in Java?
A Package can be defined as a grouping of related types (classes, interfaces, enumerations and annotations). Refer: Package in Java.

----

Q)What is the difference between import java.util.Date and java.util.* ?
The star form (java.util.* ) includes all the classes of that package and that may increase the compilation time – especially if you import several packages. However it doesn’t have any effect run-time performance.

----

Q) What is static import?
Refer: Static Import in Java.

----

Q) Garbage collection in java?
Since objects are dynamically allocated by using the new operator, java handles the de-allocation of the memory automatically, when no references to an object exist for a long time. This whole process is called garbage collection. The whole purpose of Garbage collection is efficient memory management.

----

Q) Use of finalize() method in java?
finalize() method is used to free the allocated resource.

----

Q) How many times does the garbage collector calls the finalize() method for an object?
The garbage collector calls the finalize() method only once for an object.

----

Q) What are two different ways to call garbage collector?
System.gc() OR Runtime.getRuntime().gc().

----

Q) Can the Garbage Collection be forced by any means?
No, its not possible. you cannot force garbage collection. you can call system.gc() methods for garbage collection but it does not guarantee that garbage collection would be done.

Exception handling Interview Questions

----

Q) What is an exception?
Exceptions are abnormal conditions that arise during execution of the program. It may occur due to wrong user input or wrong logic written by programmer.

----

Q) Exceptions are defined in which java package? OR which package has definitions for all the exception classes?
Java.lang.Exception
This package contains definitions for Exceptions.

----

Q) What are the types of exceptions?
There are two types of exceptions: checked and unchecked exceptions.
Checked exceptions: These exceptions must be handled by programmer otherwise the program would throw a compilation error.
Unchecked exceptions: It is up to the programmer to write the code in such a way to avoid unchecked exceptions. You would not get a compilation error if you do not handle these exceptions. These exceptions occur at runtime.

----

Q) What is the difference between Error and Exception?
Error: Mostly a system issue. It always occur at run time and must be resolved in order to proceed further.
Exception: Mostly an input data issue or wrong logic in code. Can occur at compile time or run time.

----

Q) What is throw keyword in exception handling?
The throw keyword is used for throwing user defined or pre-defined exception.

----

Q) What is throws keyword?
If a method does not handle a checked exception, the method must declare it using the throwskeyword. The throws keyword appears at the end of a method’s signature.

----

Q) Difference between throw and throws in Java
Read the difference here: Java – throw vs throws.

----

Q) Can static block throw exception?
Yes, A static block can throw exceptions. It has its own limitations: It can throw only Runtime exception (Unchecked exceptions), In order to throw checked exceptions you can use a try-catch block inside it.

----

Q) What is finally block?
Finally block is a block of code that always executes, whether an exception occurs or not. Finally block follows try block or try-catch block.

----

Q) ClassNotFoundException vs NoClassDefFoundError?
1) ClassNotFoundException occurs when loader could not find the required class in class path.
2) NoClassDefFoundError occurs when class is loaded in classpath, but one or more of the class which are required by other class, are removed or failed to load by compiler.

----

Q) Can we have a try block without catch or finally block?
No, we cannot have a try block without catch or finally block. We must have either one of them or both.

----

Q) Can we have multiple catch blocks following a single try block?
Yes we can have multiple catch blocks in order to handle more than one exception.

----

Q) Is it possible to have finally block without catch block?
Yes, we can have try block followed by finally block without even using catch blocks in between.

When a finally block does not get executed?
The only time finally won’t be called is if you call System.exit() or if the JVM crashes first.

----

Q) Can we handle more than one exception in a single catch block?
Yes we can do that using if-else statement but it is not considered as a good practice. We should have one catch block for one exception.

----

Q) What is a Java Bean?
A JavaBean is a Java class that follows some simple conventions including conventions on the names of certain methods to get and set state called Introspection. Because it follows conventions, it can easily be processed by a software tool that connects Beans together at runtime. JavaBeans are reusable software components.

----

Java Multithreading Interview Questions
Q) What is Multithreading?
It is a process of executing two or more part of a program simultaneously. Each of these parts is known as threads. In short the process of executing multiple threads simultaneously is known as multithreading.

----

Q) What is the main purpose of having multithread environment?
Maximizing CPU usage and reducing CPU idle time

----

Q) What are the main differences between Process and thread? Explain in brief.
1)  One process can have multiple threads. A thread is a smaller part of a process.
2)  Every process has its own memory space, executable code and a unique process identifier (PID) while every thread has its own stack in Java but it uses process main memory and shares it with other threads.
3) Threads of same process can communicate with each other using keyword like wait and notify etc. This process is known as inter process communication.

----

Q) How can we create a thread in java?
There are following two ways of creating a thread:
1)  By Implementing Runnable interface.
2)  By Extending Thread class.

----

Q) Explain yield and sleep?
yield() – It causes the currently executing thread object to temporarily pause and allow other threads to execute.

sleep() – It causes the current thread to suspend execution for a specified period. When a thread goes into sleep state it doesn’t release the lock.

----

Q) What is the difference between sleep() and wait()?
sleep() – It causes the current thread to suspend execution for a specified period. When a thread goes into sleep state it doesn’t release the lock

wait() – It causes current thread to wait until either another thread invokes the notify() method or the notifyAll() method for this object, or a specified amount of time has elapsed.

----

Q) What is a daemon thread?
A daemon thread is a thread, that does not prevent the JVM from exiting when the program finishes but the thread is still running. An example for a daemon thread is the garbage collection.

----

Q) What does join( ) method do?
if you use join() ,it makes sure that as soon as a thread calls join,the current thread(yes,currently running thread) will not execute unless the thread you have called join is finished.

----

Q) Preemptive scheduling vs. time slicing?
1) The preemptive scheduling is prioritized. The highest priority process should always be the process that is currently utilized.
2) Time slicing means task executes for a defined slice/ period of time and then enter in the pool of ready state. The scheduler then determines which task execute next based on priority or other factor.

----

Q) Can we call run() method of a Thread class?
Yes, we can call run() method of a Thread class but then it will behave like a normal method. To actually execute it in a Thread, you should call Thread.start() method to start it.

----

Q) What is Starvation?
Starvation describes a situation where a thread is unable to gain regular access to shared resources and is unable to make progress. This happens when shared resources are made unavailable for long periods by “greedy” threads. For example, suppose an object provides a synchronized method that often takes a long time to return. If one thread invokes this method frequently, other threads that also need frequent synchronized access to the same object will often be blocked.

----

Q) What is deadlock?
Deadlock describes a situation where two or more threads are blocked forever, waiting for each other.

----

Serialization interview Questions
Q: What is Serialization and de-serialization?
Serialization is a process of converting an object and its attributes to the stream of bytes. De-serialization is recreating the object from stream of bytes; it is just a reverse process of serialization. To know more about serialization with example program, refer this article.

----

Q) Do we need to implement any method of Serializable interface to make an object serializable?
No. In order to make an object serializable we just need to implement the interface Serializable. We don’t need to implement any methods.

----

Q) What is a transient variable?
1) transient variables are not included in the process of serialization.
2) They are not the part of the object’s serialized state.
3) Variables which we don’t want to include in serialization are declared as transient.

----

String interview questions
Q) A string class is immutable or mutable?
String class is immutable that’s the reason once its object gets created, it cannot be changed further.

----

Q) Difference between StringBuffer and StringBuilder class?
1) StringBuffer is thread-safe but StringBuilder is not thread safe.
2) StringBuilder is faster than StringBuffer.
3) StringBuffer is synchronized whereas StringBuilder is not synchronized.

----

Q) What is toString() method in Java?
The toString() method returns the string representation of any object.

----

Java collections interview questions
Q) What is List?
Elements can be inserted or accessed by their position in the list, using a zero-based index.
A list may contain duplicate elements.

----

Q) What is Map?
Map interface maps unique keys to values. A key is an object that we use to retrieve a value later. A map cannot contain duplicate keys: Each key can map to at most one value.

----

Q) What is Set?
A Set is a Collection that cannot contain duplicate elements.

----

Q) Why ArrayList is better than Arrays?
Array can hold fixed number of elements. ArrayList can grow dynamically.

----

Q) What is the difference between ArrayList and LinkedList?
1) LinkedList store elements within a doubly-linked list data structure. ArrayList store elements within a dynamically resizing array.
2) LinkedList is preferred for add and update operations while ArrayList is a good choice for search operations. Read more here.

----

Q) For addition and deletion. Which one is most preferred: ArrayList or LinkedList?
LinkedList. Because deleting or adding a node in LinkedList is faster than ArrayList.

----

Q) For searches. Which one is most preferred: ArrayList or LinkedList?
ArrayList. Searching an element is faster in ArrayList compared to LinkedList.

----

Q) What is the difference between ArrayList and Vector?
1) Vector is synchronized while ArrayList is not synchronized.
2) By default, Vector doubles the size of its array when it is re-sized internally. ArrayList increases by half of its size when it is re-sized. More details.

----

Q) What is the difference between Iterator and ListIterator?
Following are the major differences between them:
1) Iterator can be used for traversing Set, List and Map. ListIterator can only be used for traversing a List.
2) We can traverse only in forward direction using Iterator. ListIterator can be used for traversing in both the directions(forward and backward). Read more at: ListIterator vs Iterator.

----

Q) Difference between TreeSet and SortedSet?
TreeSet implements SortedSet interface.

----

Q) What is the difference between HashMap and Hashtable?
1) Hashtable is synchronized. HashMap is not synchronized.
2) Hashtable does not allow null keys or values. HashMap allows one null key and any number of null values. Read more here.

----

Q) What is the difference between Iterator and Enumeration?
1) Iterator allows to remove elements from the underlying collection during the iteration using its remove() method. We cannot add/remove elements from a collection when using enumerator.
2) Iterator has improved method names.
Enumeration.hasMoreElement() -> Iterator.hasNext()
Enumeration.nextElement() -> Iterator.next().

----

Applet Interview Questions
Q) How do you do file I/O from an applet?
Unsigned applets are simply not allowed to read or write files on the local file system .

Unsigned applets can, however, read (but not write) non-class files bundled with your applet on the server, called resource files

----

Q) What is container ?
A component capable of holding another component is called as container.
Container
Panel
Applet
Window
Frame
Dialog

----

Q) On Windows, generally frames are invisible, how to make it visible?
Frame f = new Frame();
f.setSize(300,200);  //height and width
f.setVisible(true) ;  // Frames appears

----

Q) Listeners and corresponding Methods?
ActionListerner – actionPerformed();
ItemListerner – itemStateChanged();
TextListener – textValueChanged();
FocusListener – focusLost(); & FocusGained();
WindowListener – windowActified(); windowDEactified(); windowIconified(); windowDeiconified(); windowClosed(); windowClosing(); windowOpened();
MouseMotionListener – mouseDragged(); & mouseMoved();
MouseListener – mousePressed(); mouseReleased(); mouseEntered(); mouseExited(); mouseClicked();

----

Q) Applet Life cycle?
Following stage of any applets life cycle, starts with init(), start(), paint(), stop() and destroy().

----

Q) Use of showStatus() method in Java
To display the message at the bottom of the browser when applet is started.

----

Q) What is Event handling in Java?
Is irrespective of any component, if any action performed/done on Frame, Panel or on window, handling those actions are called Event Handling.

----

Q) What is Adapter class?
Adapter class is an abstract class.
Advantage of adapter: To perform any window listener, we need to include all the methods used by the window listener whether we use those methods are not in our class like Interfaces whereas with adapter class, its sufficient to include only the methods required to override. Straight opposite to Interface.

</https://beginnersbook.com/2013/05/java-interview-questions/>

<https://www.digitalocean.com/community/tutorials/java-programming-interview-questions>

----

1. How do you reverse a string in Java?
There is no reverse() utility method in the String class. However, you can create a character array from the string and then iterate it from the end to the start. You can append the characters to a string builder and finally return the reversed string.

The following example code shows one way to reverse a string:

public class StringPrograms {

	public static void main(String[] args) {
		String str = "123";

		System.out.println(reverse(str));
	}

	public static String reverse(String in) {
		if (in == null)
			throw new IllegalArgumentException("Null is not valid input");

		StringBuilder out = new StringBuilder();

		char[] chars = in.toCharArray();

		for (int i = chars.length - 1; i >= 0; i--)
			out.append(chars[i]);

		return out.toString();
	}

}
Bonus points for adding null check in the method and using StringBuilder for appending the characters. Note that the indexing in Java starts from 0, so you need to start at chars.length - 1 in the for loop.

----

2. How do you swap two numbers without using a third variable in Java?
Swapping numbers without using a third variable is a three-step process that’s better visualized in code:

b = b + a; // now b is sum of both the numbers
a = b - a; // b - a = (b + a) - a = b (a is swapped)
b = b - a; // (b + a) - b = a (b is swapped)
The following example code shows one way to implement the number swap method:

public class SwapNumbers {

public static void main(String[] args) {
	int a = 10;
	int b = 20;

    System.out.println("a is " + a + " and b is " + b);

	a = a + b;
	b = a - b;
	a = a - b;

    System.out.println("After swapping, a is " + a + " and b is " + b);
    }

}
The output shows that the integer values are swapped:

Output
a is 10 and b is 20
After swapping, a is 20 and b is 10

----

3. Write a Java program to check if a vowel is present in a string.
The following example code shows how to use a regular expression to check whether the string contains vowels:

public class StringContainsVowels {

	public static void main(String[] args) {
		System.out.println(stringContainsVowels("Hello")); // true
		System.out.println(stringContainsVowels("TV")); // false
	}

	public static boolean stringContainsVowels(String input) {
		return input.toLowerCase().matches(".*[aeiou].*");
	}

}

----

4. Write a Java program to check if the given number is a prime number.
You can write a program to divide the given number n, by a number from 2 to n/2 and check the remainder. If the remainder is 0, then it’s not a prime number. The following example code shows one way to check if a given number is a Prime number:

public class PrimeNumberCheck {

	public static void main(String[] args) {
		System.out.println(isPrime(19)); // true
		System.out.println(isPrime(49)); // false
	}

	public static boolean isPrime(int n) {
		if (n == 0 || n == 1) {
			return false;
		}
		if (n == 2) {
			return true;
		}
		for (int i = 2; i <= n / 2; i++) {
			if (n % i == 0) {
				return false;
			}
		}

		return true;
	}

}
Although this program works, it’s not very memory and time-efficient. Consider that, for a given number N, if there is a prime number M between 2 to √N (square root of N) that evenly divides it, then N is not a prime number.

----

5. Write a Java program to print a Fibonacci sequence using recursion.
A Fibonacci sequence is one in which each number is the sum of the two previous numbers. In this example, the sequence begins with 0 and 1. The following example code shows how to use a for loop to print a Fibonacci sequence:

public class PrintFibonacci {

	public static void printFibonacciSequence(int count) {
		int a = 0;
		int b = 1;
		int c = 1;

		for (int i = 1; i <= count; i++) {
			System.out.print(a + ", ");

            a = b;
			b = c;
			c = a + b;
		}
	}

	public static void main(String[] args) {
    	printFibonacciSequence(10);
	}

}
Output
0, 1, 1, 2, 3, 5, 8, 13, 21, 34,
You can also use recursion to print a Fibonacci sequence, because the Fibonacci number is generated by adding the previous two numbers in the sequence:

F(N) = F(N-1) + F(N-2)
The following example class shows how to use recursion to calculate a Fibonacci sequence that is 10 numbers long:

public class PrintFibonacciRecursive {

    public static int fibonacci(int count) {
		if (count <= 1)
			return count;

		return fibonacci(count - 1) + fibonacci(count - 2);
	}

	public static void main(String args[]) {
    	int seqLength = 10;

    	System.out.print("A Fibonacci sequence of " + seqLength + " numbers: ");

    	for (int i = 0; i < seqLength; i++) {
      	    System.out.print(fibonacci(i) + " ");
    	}
  	}

}
Output
A Fibonacci sequence of 10 numbers: 0 1 1 2 3 5 8 13 21 34

----

6. How do you check if a list of integers contains only odd numbers in Java?
You can use a for loop and check whether each element is odd:

public static boolean onlyOddNumbers(List<Integer> list) {
	for (int i : list) {
		if (i % 2 == 0)
			return false;
	}

	return true;
}
If the list is large, you can use parallel stream for faster processing, as shown in the following example code:

public static boolean onlyOddNumbers(List<Integer> list) {
	return list
			.parallelStream() // parallel stream for faster processing
			.anyMatch(x -> x % 2 != 0); // return as soon as any elements match the condition
}
To learn more about the math behind determining if an integer is odd, refer to the Modulo operation on Wikipedia.

----

7. How do you check whether a string is a palindrome in Java?
A palindrome string is the same string backwards or forwards. To check for a palindrome, you can reverse the input string and check if the result is equal to the input. The following example code shows how to use the String charAt(int index) method to check for palindrome strings:

boolean checkPalindromeString(String input) {
	boolean result = true;
	int length = input.length();

	for (int i = 0; i < length/2; i++) {
		if (input.charAt(i) != input.charAt(length - i - 1)) {
			result = false;
			break;
		}
	}

	return result;
}

----

8. How do you remove spaces from a string in Java?
The following example code shows one way to remove spaces from a string using with the Character.isWhitespace() method:

String removeWhiteSpaces(String input) {
	StringBuilder output = new StringBuilder();
	
	char[] charArray = input.toCharArray();
	
	for (char c : charArray) {
		if (!Character.isWhitespace(c))
			output.append(c);
	}
	
	return output.toString();
}
Learn more about removing spaces and other characters from a string in Java.

----

9. How do you remove leading and trailing spaces from a string in Java?
The String class contains two methods to remove leading and trailing whitespaces: trim() and strip(). The strip() method was added to the String class in Java 11. The strip() method uses the Character.isWhitespace() method to check if the character is a whitespace. This method uses Unicode code points, while the trim() method identifies any character with a codepoint value less than or equal to U+0020 as a whitespace character.

The strip() method is the recommended way to remove whitespaces because it uses the Unicode standard. The following example code shows how to use the strip() method to remove whitespaces:

String s = "  abc  def\t";
		
s = s.strip();
		
System.out.println(s);
Because String is immutable, you have to assign the strip() output to the string.

----

10. How do you sort an array in Java?
The Arrays utility class has many overloaded sort() methods to sort primitive and to object arrays. If you are sorting a primitive array in the natural order, then you can use the Arrays.sort() method, as shown in the following example:

int[] array = {1, 2, 3, -1, -2, 4};

Arrays.sort(array);

System.out.println(Arrays.toString(array));
However, if you want to sort an array of objects, then the object must implement the Comparable interface. If you want to specify the sorting criteria, then you can pass the Comparator for the sorting logic. Learn more about Comparable and Comparator in Java.

----

11. How do you create a deadlock scenario programmatically in Java?
Deadlock is a scenario in a multi-threaded Java environment where two or more threads are blocked forever. The deadlock situation arises with at two or more threads. The following example code creates a deadlock scenario:

public class ThreadDeadlock {

    public static void main(String[] args) throws InterruptedException {
        Object obj1 = new Object();
        Object obj2 = new Object();
        Object obj3 = new Object();
    
        Thread t1 = new Thread(new SyncThread(obj1, obj2), "t1");
        Thread t2 = new Thread(new SyncThread(obj2, obj3), "t2");
        Thread t3 = new Thread(new SyncThread(obj3, obj1), "t3");
        
        t1.start();
        Thread.sleep(5000);
        t2.start();
        Thread.sleep(5000);
        t3.start();        
    }

}

class SyncThread implements Runnable {

    private Object obj1;
    private Object obj2;

    public SyncThread(Object o1, Object o2) {
        this.obj1 = o1;
        this.obj2 = o2;
    }

    @Override
    public void run() {
        String name = Thread.currentThread().getName();

        System.out.println(name + " acquiring lock on " + obj1);
        synchronized (obj1) {
            System.out.println(name + " acquired lock on " + obj1);
            work();
            System.out.println(name + " acquiring lock on " + obj2);
            synchronized (obj2) {
                System.out.println(name + " acquired lock on " + obj2);
                work();
            }
            System.out.println(name + " released lock on " + obj2);
        }
        System.out.println(name + " released lock on " + obj1);
        System.out.println(name + " finished execution.");
    }

    private void work() {
        try {
            Thread.sleep(30000);
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
    }

}
All three threads will be able to acquire a lock on the first object. However, they are using shared resources and are started in such a way that they will keep on waiting indefinitely to acquire the lock on the second object. You can use the Java thread dump to detect the deadlocks. Learn more about deadlock in Java.

----
s
12. How can you find the factorial of an integer in Java?
The factorial of an integer is calculated by multiplying all the numbers from 1 to the given number:

F(n) = F(1)*F(2)...F(n-1)*F(n)
The following example code shows how to use recursion to find the factorial of an integer:

public static long factorial(long n) {
	if (n == 1)
		return 1;
	else
		return (n * factorial(n - 1));
}

----

13. How do you reverse a linked list in Java?
LinkedList descendingIterator() returns an iterator that iterates over the element in reverse order. The following example code shows how to use this iterator to create a new Linked List with elements listed in the reverse order:

LinkedList<Integer> ll = new LinkedList<>();

ll.add(1);
ll.add(2);
ll.add(3);

System.out.println(ll);

LinkedList<Integer> ll1 = new LinkedList<>();

ll.descendingIterator().forEachRemaining(ll1::add);

System.out.println(ll1);
Learn more about reversing a linked list from a data structures and algorithms perspective.

----

14. How do you implement a binary search in Java?
The array elements must be sorted to implement binary search. The binary search algorithm is based on the following conditions:

If the key is less than the middle element, then you now need to search only in the first half of the array.
If the key is greater than the middle element, then you need to search only in the second half of the array.
If the key is equal to the middle element in the array, then the search ends.
Finally, if the key is not found in the whole array, then it should return -1. This indicates that the element is not present.
The following example code implements a binary search:

public static int binarySearch(int arr[], int low, int high, int key) {
	int mid = (low + high) / 2;

	while (low <= high) {
		if (arr[mid] < key) {
			low = mid + 1;
		} else if (arr[mid] == key) {
			return mid;
		} else {
			high = mid - 1;
		}
		mid = (low + high) / 2;
	}

	if (low > high) {
		return -1;
	}

	return -1;
}

----

15. Write a Java program that illustrates merge sort.
Merge sort is one of the most efficient sorting algorithms. It works on the principle of “divide and conquer”. It is based on the idea of breaking down a list into several sub-lists until each sub-list consists of a single element, and then merging those sub-lists in a manner that results in a sorted list. The following example code shows one way to use merge sort:

public class MergeSort {

	public static void main(String[] args) {
		int[] arr = { 70, 50, 30, 10, 20, 40, 60 };

		int[] merged = mergeSort(arr, 0, arr.length - 1);

		for (int val : merged) {
			System.out.print(val + " ");
		}
	}

	public static int[] mergeTwoSortedArrays(int[] one, int[] two) {
		int[] sorted = new int[one.length + two.length];

		int i = 0;
		int j = 0;
		int k = 0;

		while (i < one.length && j < two.length) {
			if (one[i] < two[j]) {
				sorted[k] = one[i];
				k++;
				i++;
			} else {
				sorted[k] = two[j];
				k++;
				j++;
			}
		}

		if (i == one.length) {
			while (j < two.length) {
				sorted[k] = two[j];
				k++;
				j++;
			}
		}

		if (j == two.length) {
			while (i < one.length) {
				sorted[k] = one[i];
				k++;
				i++;
			}
		}

		return sorted;
	}

	public static int[] mergeSort(int[] arr, int lo, int hi) {
		if (lo == hi) {
			int[] br = new int[1];
			br[0] = arr[lo];

			return br;
		}

		int mid = (lo + hi) / 2;

		int[] fh = mergeSort(arr, lo, mid);
		int[] sh = mergeSort(arr, mid + 1, hi);

		int[] merged = mergeTwoSortedArrays(fh, sh);

		return merged;
	}

}

----

16. Can you create a pyramid of characters in Java?
Pattern programs are a very popular interview topic. This type of question is used to understand the logical thinking abilities of the interviewee. Refer to Pyramid Pattern Programs in Java for examples of different ways to create pyramid patterns.

----

17. Write Java program that checks if two arrays contain the same elements.
To check if two arrays contain the same elements, you need to first create a set of elements from both the arrays, and then compare the elements in these sets to find if there is an element that is not present in both sets. The following example code shows how to check if two arrays only contain common elements:

import java.util.Arrays;
import java.util.HashSet;
import java.util.Set;

public class ArraySameElements {

	public static void main(String[] args) {
		Integer[] a1 = {1,2,3,2,1};
		Integer[] a2 = {1,2,3};
		Integer[] a3 = {1,2,3,4};
		
		System.out.println(sameElements(a1, a2));
		System.out.println(sameElements(a1, a3));
	}

	static boolean sameElements(Object[] array1, Object[] array2) {
		Set<Object> uniqueElements1 = new HashSet<>(Arrays.asList(array1));
		Set<Object> uniqueElements2 = new HashSet<>(Arrays.asList(array2));
		
		// if size is different, means there will be a mismatch
		if (uniqueElements1.size() != uniqueElements2.size()) return false;
		
		for (Object obj : uniqueElements1) {
			// element not present in both?
			if (!uniqueElements2.contains(obj)) return false;
		}
		
		return true;
	}

}
Output
true
false

----

18. How do you get the sum of all elements in an integer array in Java?
You can use a for loop to iterate over the array elements and add them to get the final sum:

int[] array = { 1, 2, 3, 4, 5 };

int sum = 0;

for (int i : array)
	sum += i;

System.out.println(sum);

----

19. How do you find the second largest number in an array in Java?
There are many ways to solve this problem. You can sort the array in natural ascending order and take the second last value. However, sorting is an expensive operation. You can also use two variables to find the second largest value in a single iteration, as shown in the following example:

private static int findSecondHighest(int[] array) {
	int highest = Integer.MIN_VALUE;
	int secondHighest = Integer.MIN_VALUE;

	for (int i : array) {
		if (i > highest) {
			secondHighest = highest;
			highest = i;
		} else if (i > secondHighest) {
			secondHighest = i;
		}

	}
	return secondHighest;
}

----

20. How do you shuffle an array in Java?
The following example code shows how to use the Random class to generate random index numbers and shuffle the elements:

int[] array = { 1, 2, 3, 4, 5, 6, 7 };

Random rand = new Random();

for (int i = 0; i < array.length; i++) {
	int randomIndexToSwap = rand.nextInt(array.length);
	int temp = array[randomIndexToSwap];
	array[randomIndexToSwap] = array[i];
	array[i] = temp;
}

System.out.println(Arrays.toString(array));
You can run the shuffling code inside another for loop to shuffle multiple rounds.

----

21. How can you find a string in a text file in Java?
The following example code shows how to use the Scanner class to read the file contents line by line and then use the String contains() method to check if the string is present in the file:

boolean findStringInFile(String filePath, String str) throws FileNotFoundException {
	File file = new File(filePath);

	Scanner scanner = new Scanner(file);

	// read the file line by line
	while (scanner.hasNextLine()) {
		String line = scanner.nextLine();
		if (line.contains(str)) {
			scanner.close();
			return true;
		}
	}
	scanner.close();

	return false;
}
Note that the example code assumes that the string that you’re searching for in the file doesn’t contain newline characters.

----

22. How do you print a date in specific format in Java?
The following example code shows how to use the SimpleDateFormat class to format the date string:

String pattern = "MM-dd-yyyy";
SimpleDateFormat simpleDateFormat = new SimpleDateFormat(pattern);

String date = simpleDateFormat.format(new Date());
System.out.println(date); // 06-23-2020
Lear more about the Java SimpleDateFormat.

----

23. How do you merge two lists in Java?
The following example code shows how to use the addAll() method to merge multiple lists in Java:

List<String> list1 = new ArrayList<>();
list1.add("1");
List<String> list2 = new ArrayList<>();
list2.add("2");

List<String> mergedList = new ArrayList<>(list1);
mergedList.addAll(list2);
System.out.println(mergedList); // [1, 2]
24. Write a Java program that sorts HashMap by value.
HashMap is not an ordered collection. The following example code shows how to sort the entries based on value and store them into LinkedHashMap, which maintains the order of insertion:

import java.util.ArrayList;
import java.util.HashMap;
import java.util.LinkedHashMap;
import java.util.List;
import java.util.Map;
import java.util.Map.Entry;
import java.util.Set;

public class SortHashMapByValue {

	public static void main(String[] args) {
		Map<String, Integer> scores = new HashMap<>();

		scores.put("David", 95);
		scores.put("Jane", 80);
		scores.put("Mary", 97);
		scores.put("Lisa", 78);
		scores.put("Dino", 65);

		System.out.println(scores);

		scores = sortByValue(scores);

		System.out.println(scores);
	}

	private static Map<String, Integer> sortByValue(Map<String, Integer> scores) {
		Map<String, Integer> sortedByValue = new LinkedHashMap<>();

		// get the entry set
		Set<Entry<String, Integer>> entrySet = scores.entrySet();
		System.out.println(entrySet);

		// create a list since the set is unordered
		List<Entry<String, Integer>> entryList = new ArrayList<>(entrySet);
		System.out.println(entryList);

		// sort the list by value
		entryList.sort((x, y) -> x.getValue().compareTo(y.getValue()));
		System.out.println(entryList);

		// populate the new hash map
		for (Entry<String, Integer> e : entryList)
			sortedByValue.put(e.getKey(), e.getValue());

		return sortedByValue;
	}

}

----

25. How do you remove all occurrences of a given character from an input string in Java?
The String class doesn’t have a method to remove characters. The following example code shows how to use the replace() method to create a new string without the given character:

String str1 = "abcdABCDabcdABCD";
		
str1 = str1.replace("a", ""); 

System.out.println(str1); // bcdABCDbcdABCD
String is immutable in Java. All the string manipulation methods return a new string, which is why you need to assign it to another variable. Learn more about removing characters from a string in Java.

----

26. How do you get distinct characters and their count in a string in Java?
You can create the character array from the string. Then iterate over it and create a HashMap with the character as key and their count as value. The following example code shows how to extract and count the characters of a string:

String str1 = "abcdABCDabcd";

char[] chars = str1.toCharArray();

Map<Character, Integer> charsCount = new HashMap<>();

for (char c : chars) {
	if (charsCount.containsKey(c)) {
		charsCount.put(c, charsCount.get(c) + 1);
	} else
		charsCount.put(c, 1);
}

System.out.println(charsCount); // {a=2, A=1, b=2, B=1, c=2, C=1, d=2, D=1}

----

27. Can you prove that a String object in Java is immutable programmatically?
The following example code shows how to prove that a String object is immutable and the comments in the code explain each step:

String s1 = "Java"; // "Java" String created in pool and reference assigned to s1

String s2 = s1; //s2 also has the same reference to "Java" in the pool

System.out.println(s1 == s2); // proof that s1 and s2 have the same reference

s1 = "Python"; 
//s1 value got changed above, so how String is immutable?

//in the above case a new String "Python" got created in the pool
//s1 is now referring to the new String in the pool 
//BUT, the original String "Java" is still unchanged and remains in the pool
//s2 is still referring to the original String "Java" in the pool

// proof that s1 and s2 have different reference
System.out.println(s1 == s2); 

System.out.println(s2); 
// prints "Java" supporting the fact that original String value is unchanged, hence String is immutable

----

28. Can you write some code to showcase inheritance in Java?
The following example code shows how to use the extends keyword to create a subclass of the class Animal. The new class Cat inherits the variable from the Animal class and adds more code that only belongs to the Cat class.

class Animal {
	String color;
}

class Cat extends Animal {
	void meow() {
		System.out.println("Meow");
	}
}

----

29. How do you show a diamond problem with multiple inheritance in Java?
The diamond problem occurs when a class inherits from multiple classes and ambiguity occurs when it’s unclear which method to execute from which class. Java doesn’t allow extending multiple classes to avoid the diamond problem illustrated by the following example:

interface I {
	void foo();
}
class A implements I {
	public void foo() {}
}

class B implements I {
	public void foo() {}
}

class C extends A, B { // won't compile
	public void bar() {
		super.foo();
	}
}

----

30. How do you illustrate a try catch example in Java?
The following example code shows an example of try-catch:

try {
	FileInputStream fis = new FileInputStream("test.txt");
} catch(FileNotFoundException e) {
	e.printStackTrace();
}
From Java 7 onwards, you can also catch multiple exceptions in a single catch block, as shown in the following example. It’s useful when you have the same code in all the catch blocks.

public static void foo(int x) throws IllegalArgumentException, NullPointerException {
	// some code
}

public static void main(String[] args) {
	try {
		foo(10);
	} catch (IllegalArgumentException | NullPointerException e) {
		System.out.println(e.getMessage());
	}
}

----

31. Write a Java program to show a NullPointerException.
If you are calling a function on null, it will throw a NullPointerException, as shown in the following example code:

public static void main(String[] args) {
	printString(null, 3);
	
}

static void printString(String s, int count) {
	for (int i = 0; i < count; i++) {
		System.out.println(s.toUpperCase()); // Exception in thread "main" java.lang.NullPointerException
	}
}
You should have null check in place for early validation, as shown in the following example code:

static void printString(String s, int count) {
	if (s == null) return;
	for (int i = 0; i < count; i++) {
		System.out.println(s.toUpperCase());
	}
}
You can also throw IllegalArgumentException based on the project requirements.

----

32. How do you create a record in Java?
Records was added as a standard feature in Java 16. Records enable you to create a POJO class with minimal code. Records automatically generates hashCode(), equals(), getter methods, and toString() method code for the class. Records are final and implicitly extend the java.lang.Record class. The following example code shows one way to cerate a record:

import java.util.Map;
 
public record EmpRecord(int id, String name, long salary, Map<String, String> addresses) {
}
Learn more about records in Java. For details about POJO, refer to Plain old Java object on Wikipedia.

----

33. How do you create text blocks in Java?
Java 15 added the text blocks feature. You can create multiline strings using text blocks. The multiline string has to be written inside of a pair of triple-double quotes, as shown in the following example:

String textBlock = """
		Hi
		Hello
		Yes""";
It’s the same as creating a string, such as Hi\\nHello\\nYes.

----

34. Show an example of switch expressions and multi-label case statements in Java.
The switch expressions were added as a standard feature in Java 14. The following examples show switch expressions as well as multi-label case statements:

int choice = 2;

int x = switch (choice) {
    case 1, 2, 3:
	    yield choice;
    default:
	    yield -1;
};

System.out.println("x = " + x); // x = 2
You can also use lambda expressions in switch expressions.

String day = "TH";
String result = switch (day) {
    case "M", "W", "F" -> "MWF";
    case "T", "TH", "S" -> "TTS";

    default -> {
	    if (day.isEmpty())
		    yield "Please insert a valid day.";
	    else
		    yield "Looks like a Sunday.";
    }
};

System.out.println(result); // TTH

----

35. How do you compile and run a Java class from the command line?
This example refers to the following Java file:

public class Test {

public static void main(String args[]) {
		System.out.println("Hi");
	}

}
You can compile it using the following command in your terminal:

javac Test.java
To run the class, use the following command in your terminal:

java Test
For the recent releases, the java command will also compile the program if the class file is not present. If the class is in a package, such as com.example, then it should be inside the folder com/example. The command to compile and run is:

java com/example/Test.java
If your class requires some additional JARs to compile and run, you can use the java -cp option. For example:

java -cp .:~/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar  com/example/Test.java

----

36. How do you create an enum in Java?
The following example code shows how to create a basic enum:

public enum ThreadStates {
	START,
	RUNNING,
	WAITING,
	DEAD;
}
ThreadStates is the enum with fixed constants fields START, RUNNING, WAITING, and DEAD. All enums implicitly extend the java.lang.Enum class and implement the Serializable and Comparable interfaces. Enum can have methods also. Learn more about enums in Java.

----

37. How do you use the forEach() method in Java?
The forEach() method provides a shortcut to perform an action on all the elements of an iterable. The following example code shows how to iterate over the list elements and print them:

List<String> list = new ArrayList<>();

Iterator<String> it = list.iterator();

while (it.hasNext()) {
	System.out.println(it.next());
}
You can use the forEach() method with a lambda expression to reduce the code size, as shown in the following example code:

List<String> list = new ArrayList<>();

list.forEach(System.out::print);

----

38. How do you write an interface with default and static method?
Java 8 introduced default and static methods in interfaces. This bridged the gap between interfaces and abstract classes. The following example code shows one way to write an interface with the default and static method:

public interface Interface1 {
	
	// regular abstract method
	void method1(String str);
	
	default void log(String str) {
		System.out.println("I1 logging::" + str);
	}
	
	static boolean isNull(String str) {
		System.out.println("Interface Null Check");

		return str == null ? true : "".equals(str) ? true : false;
	}

}
Learn more about about default and static methods in interfaces in Java 8 interface changes.

----

39. How do you create a functional interface?
An interface with exactly one abstract method is called a functional interface. The major benefit of functional interfaces is that you can use lambda expressions to instantiate them and avoid using bulky anonymous class implementation. The @FunctionalInterface annotation indicates a functional interface, as shown in the following example code:

@FunctionalInterface
interface Foo {
	void test();
}

----

40. Show an example of using lambda expressions in Java.
Runnable is an excellent example of a functional interface. You can use lambda expressions to create a runnable, as shown in the following example code:

Runnable r1 = () -> System.out.println("My Runnable");

----

41. Show examples of overloading and overriding in Java.
When a class has two or more methods with the same name, they are called overloaded methods. The following example code shows as overloaded method called print:

class Foo {
	void print(String s) {
		System.out.println(s);
	}

	void print(String s, int count) {
		while (count > 0) {
			System.out.println(s);
			count--;
		}
	}

}
When a superclass method is also implemented in the child class, it’s called overriding. The following example code shows how to annotate the printname() method that’s implemented in both classes:

class Base {
	void printName() {
		System.out.println("Base Class");
	}
}

class Child extends Base {
	@Override
	void printName() {
		System.out.println("Child Class");
	}
}
Learn more about overriding and overloading in Java.

----

42.-49. Guess the Output
Test yourself by guessing the output of the following code snippets.

String s1 = "abc";
String s2 = "abc";

System.out.println("s1 == s2 is:" + s1 == s2);
Output
String s3 = "JournalDev";
int start = 1;
char end = 5;

System.out.println(s3.substring(start, end));
Output
HashSet shortSet = new HashSet();

	for (short i = 0; i < 100; i++) {
    shortSet.add(i);
    shortSet.remove(i - 1);
}

System.out.println(shortSet.size());
Output
try {
	if (flag) {
  		while (true) {
   		}
   	} else {
   		System.exit(1);
   	}
} finally {
   	System.out.println("In Finally");
}
Output
String str = null;
String str1="abc";

System.out.println(str1.equals("abc") | str.equals(null));
Output
String x = "abc";
String y = "abc";

x.concat(y);

System.out.print(x);
Output
public class MathTest {

 	public void main(String[] args) {  		
   		int x = 10 * 10 - 10;
   		
   		System.out.println(x);
   	}
   
}
Output
public class Test {
   
  	public static void main(String[] args) {
   		try {
   			throw new IOException("Hello");
   		} catch(IOException | Exception e) {
   			System.out.println(e.getMessage());
   		}
   	}
}
Output
50. Find 5 mistakes in the following code snippet.
package com.digitalocean.programming-interviews;

public class String Programs {

	static void main(String[10] args) {
		String s = "abc"
		System.out.println(s);
	}
}

</https://www.digitalocean.com/community/tutorials/java-programming-interview-questions>

<https://www.softwaretestinghelp.com/core-java-interview-questions/>

----

Q #1) What is JAVA?

Answer: Java is a high-level programming language and is platform-independent.

Java is a collection of objects. It was developed by Sun Microsystems. There are a lot of applications, websites, and games that are developed using Java.

----

Q #2) What are the features of JAVA?

Answer: Features of Java are as follows:

OOP concepts
Object-oriented
Inheritance
Encapsulation
Polymorphism
Abstraction
Platform independent: A single program works on different platforms without any modification.
High Performance: JIT (Just In Time compiler) enables high performance in Java. JIT converts the bytecode into machine language and then JVM starts the execution.
Multi-threaded: A flow of execution is known as a Thread. JVM creates a thread which is called the main thread. The user can create multiple threads by extending the thread class or by implementing the Runnable interface.

----

Q #3) How does Java enable high performance?

Answer: Java uses Just In Time compiler to enable high performance. It is used to convert the instructions into bytecodes.

----

Q #4) Name the Java IDE’s?

Answer: Eclipse and NetBeans are the IDE’s of JAVA.

----

Q #5) What do you mean by Constructor?

Answer: Constructor can be explained in detail with enlisted points:

When a new object is created in a program a constructor gets invoked corresponding to the class.
The constructor is a method which has the same name as the class name.
If a user doesn’t create a constructor implicitly a default constructor will be created.
The constructor can be overloaded.
If the user created a constructor with a parameter then he should create another constructor explicitly without a parameter.

----

Q #6) What is meant by the Local variable and the Instance variable?

Answer:

Local variables are defined in the method and scope of the variables that exist inside the method itself.

Instance variable is defined inside the class and outside the method and the scope of the variables exists throughout the class.

----

Q #7) What is a Class?

Answer: All Java codes are defined in a Class. It has variables and methods.

Variables are attributes which define the state of a class.

Methods are the place where the exact business logic has to be done. It contains a set of statements (or) instructions to satisfy the particular requirement.

Example:

public class Addition{ //Class name declaration
int a = 5; //Variable declaration
int b= 5;
public void add(){ //Method declaration
int c = a+b;
}
}

----

Q #8) What is an Object?

Answer: An instance of a class is called an object. The object has state and behavior.

Whenever the JVM reads the “new()” keyword then it will create an instance of that class.

Example:

public class Addition{
public static void main(String[] args){
Addion add = new Addition();//Object creation
}
}
The above code creates the object for the Addition class.

----

Q #9)What are the OOPs concepts?

Answer: OOPs concepts include:

Inheritance
Encapsulation
Polymorphism
Abstraction
Interface
Suggested Read =>> Top OOPs Interview Questions

----

Q #10) What is Inheritance?

Answer: Inheritance means one class can extend to another class. So that the codes can be reused from one class to another class. The existing class is known as the Super class whereas the derived class is known as a sub class.

Example:

Super class:
public class Manupulation(){
}
Sub class:
public class Addition extends Manipulation(){
}
Inheritance is only applicable to the public and protected members only. Private members can’t be inherited.

----

Q #11) What is Encapsulation?

Answer: Purpose of Encapsulation:

Protects the code from others.
Code maintainability.
Example:

We are declaring ‘a’ as an integer variable and it should not be negative.

public class Addition(){
int a=5;
}
If someone changes the exact variable as “a = -5” then it is bad.

In order to overcome the problem we need to follow the steps below:

We can make the variable private or protected.
Use public accessor methods such as set<property> and get<property>.
So that the above code can be modified as:

public class Addition(){
private int a = 5; //Here the variable is marked as private
}
The code below shows the getter and setter.

Conditions can be provided while setting the variable.

get A(){
}
set A(int a){
if(a&gt;0){// Here condition is applied
.........
}
}
For encapsulation, we need to make all the instance variables private and create setter and getter for those variables. Which in turn will force others to call the setters rather than access the data directly.

----

Q #12) What is Polymorphism?


Answer: Polymorphism means many forms.

A single object can refer to the super-class or sub-class depending on the reference type which is called polymorphism.

Example:

Public class Manipulation(){ //Super class
public void add(){
}
}
public class Addition extends Manipulation(){ // Sub class
public void add(){
}
public static void main(String args[]){
Manipulation addition = new Addition();//Manipulation is reference type and Addition is reference type
addition.add();
}
}
Using the Manipulation reference type we can call the Addition class “add()” method. This ability is known as Polymorphism. Polymorphism is applicable for overriding and not for overloading.

----

Q #13) What is meant by Method Overriding?

Answer: Method overriding happens if the sub-class method satisfies the below conditions with the Super-class method:

Method name should be the same
The argument should be the same
Return type should also be the same
The key benefit of overriding is that the Sub-class can provide some specific information about that sub-class type than the super-class.

Example:

public class Manipulation{ //Super class
public void add(){
………………
}
}
 
Public class Addition extends Manipulation(){
Public void add(){
………..
}
Public static void main(String args[]){
Manipulation addition = new Addition(); //Polimorphism is applied
addition.add(); // It calls the Sub class add() method
}
}
addition.add() method calls the add() method in the Sub-class and not the parent class. So it overrides the Super-class method and is known as Method Overriding.

----

Q #14) What is meant by Overloading?

Answer: Method overloading happens for different classes or within the same class.

For method overloading, sub-class method should satisfy the below conditions with the Super-class method (or) methods in the same class itself:

Same method name
Different argument types
There may be different return types
Example:

public class Manipulation{ //Super class
public void add(String name){ //String parameter
………………
}
}
 
Public class Addition extends Manipulation(){
Public void add(){//No Parameter
………..
}
Public void add(int a){ //integer parameter
 
}
Public static void main(String args[]){
Addition addition = new Addition();
addition.add();
}
}
Here the add() method has different parameters in the Addition class is overloaded in the same class as with the super-class.

Note: Polymorphism is not applicable for method overloading.

----

Q #15) What is meant by Interface?

Answer: Multiple inheritances cannot be achieved in java. To overcome this problem the Interface concept is introduced.

An interface is a template which has only method declarations and not the method implementation.

Example:

Public abstract interface IManupulation{ //Interface declaration
Public abstract void add();//method declaration
public abstract void subtract();
}
All the methods in the interface are internally public abstract void.
All the variables in the interface are internally public static final that is constants.
Classes can implement the interface and not extends.
The class which implements the interface should provide an implementation for all the methods declared in the interface.
public class Manupulation implements IManupulation{ //Manupulation class uses the interface
Public void add(){
……………
}
Public void subtract(){
…………….
}
}

----

Q #16) What is meant by Abstract class?

Answer: We can create the Abstract class by using the “Abstract” keyword before the class name. An abstract class can have both “Abstract” methods and “Non-abstract” methods that are a concrete class.

Abstract method:

The method which has only the declaration and not the implementation is called the abstract method and it has the keyword called “abstract”. Declarations ends with a semicolon.

Example:

public abstract class Manupulation{
public abstract void add();//Abstract method declaration
Public void subtract(){
}
}
An abstract class may have a non- abstract method also.
The concrete Subclass which extends the Abstract class should provide the implementation for abstract methods.

----

Q #17) Difference between Array and Array List.

Answer: The Difference between Array and Array List can be understood from the table below:

                        Array                                      

   Array List    
Size should be given at the time of array declaration.

String[] name = new String[2]	Size may not be required. It changes the size dynamically.

ArrayList name = new ArrayList
To put an object into array we need to specify the index.

name[1] = “book”	No index required.

name.add(“book”)
Array is not type parameterized	ArrayList in java 5.0 are parameterized.

Eg: This angle bracket is a type parameter which means a list of String.

----

Q #18) Difference between String, String Builder, and String Buffer.

Answer:

String: String variables are stored in a “constant string pool”. Once the string reference changes the old value that exists in the “constant string pool”, it cannot be erased.

Example:

String name = “book”;

Constant string pool

Constant string pool.

If the name-value has changed from “book” to “pen”.

Constant string pool

Constant string pools

Then the older value remains in the constant string pool.

String Buffer:

Here string values are stored in a stack. If the values are changed then the new value replaces the older value.
The string buffer is synchronized which is thread-safe.
Performance is slower than the String Builder.
Example:

String Buffer name =”book”;

Stack

Once the name value has been changed to “pen” then the “book” is erased in the stack.

Stack1

String Builder:

This is the same as String Buffer except for the String Builder which is not threaded safely that is not synchronized. So obviously the performance is fast.

----

Q #19) Explain about Public and Private access specifiers.

Answer: Methods and instance variables are known as members.

Public:

Public members are visible in the same package as well as the outside package that is for other packages.

Public

Public members of Class A are visible to Class B (same package) as well as Class C (different packages).

Private:

Private members are visible in the same class only and not for the other classes in the same package as well as classes in the outside packages.

Private

Private members in class A are visible only in that class. It is invisible for class  B as well as class C.

----

Q #20) Difference between Default and Protected access specifiers.

Answer:

Default: Methods and variables declared in a class without any access specifiers are called default.

Default

Default members in Class A are visible to the other classes which are inside the package and invisible to the classes which are outside the package.

So Class A members are visible to Class B and invisible to Class C.

Protected:

Protected             .

Protected is the same as Default but if a class extends then it is visible even if it is outside the package.

Class A members are visible to Class B because it is inside the package. For Class C it is invisible but if Class C extends Class A then the members are visible to Class C even if it is outside the package.

----

Q #21) Difference between HashMap and HashTable.

Answer: The difference between HashMap and HashTable can be seen below:

HashMap	HashTable
Methods are not synchronized	Key methods are synchronized
Not thread safety	Thread safety
Iterator is used to iterate the values	Enumerator is used to iterate the values
Allows one null key and multiple null values	Doesn’t allow anything that is null
Performance is high than HashTable	Performance is slow

----

Q #22) Difference between HashSet and TreeSet.

Answer: The difference between HashSet and TreeSet can be seen below:

HashSet	TreeSet
Inserted elements are in random order	Maintains the elements in the sorted order
Can able to store null objects	Couldn’t store null objects
Performance is fast	Performance is slow

----

Q #23) Difference between Abstract class and Interface.

Answer: The differences between Abstract Class and Interface are as follows:

Abstract Class:

Abstract classes have a default constructor and it is called whenever the concrete subclass is instantiated.
It contains Abstract methods as well as Non-Abstract methods.
The class which extends the Abstract class shouldn’t require the implementation of all the methods, only Abstract methods need to be implemented in the concrete sub-class.
Abstract class contains instance variables.
Interface:

It doesn’t have any constructor and couldn’t be instantiated.
The abstract method alone should be declared.
Classes that implement the interface should provide the implementation for all the methods.
The interface contains only constants.

----

Q #24)  What is the meaning of Collections in Java?

Answer: Collection is a framework that is designed to store the objects and manipulate the design to store the objects.

Collections are used to perform the following operations:

Searching
Sorting
Manipulation
Insertion
Deletion
A group of objects is known as collections. All the classes and interfaces for collecting are available in Java util package.

Further Reading => Most Popular Java Development Companies To Look For

----

Q #25) What are all the Classes and Interfaces that are available in the collections?

Answer: Given below are the Classes and Interfaces that are available in Collections:

Interfaces:

Collection
List
Set
Map
Sorted Set
Sorted Map
Queue
Classes:

Lists:
Array List
Vector
Linked List
Sets:

Hash set
Linked Hash Set
Tree Set
Maps:

Hash Map
Hash Table
TreeMap
Linked Hashed Map
Queue:

Priority Queue

----

Q #26) What is meant by Ordered and Sorted in collections?

Answer:

Ordered: It means the values that are stored in a collection is based on the values that are added to the collection. So we can iterate the values from the collection in a specific order.

Sorted: Sorting mechanisms can be applied internally or externally so that the group of objects sorted in a particular collection is based on the properties of the objects.

----

Q #27) Explain the different lists available in the collection.

Answer: Values added to the list are based on the index position and it is ordered by index position. Duplicates are allowed.

The types of Lists are:

a) Array List:

Fast iteration and fast Random Access.
It is an ordered collection (by index) and not sorted.
It implements the Random Access Interface.
Example:

public class Fruits{
public static void main (String [ ] args){
ArrayList &lt;String&gt;names=new ArrayList &lt;String&gt;();
names.add (“apple”);
names.add (“cherry”);
names.add (“kiwi”);
names.add (“banana”);
names.add (“cherry”);
System.out.println (names);
}
}
Output:

[Apple, cherry, kiwi, banana, cherry]

From the output, Array List maintains the insertion order and it accepts the duplicates. But it’s not sorted.

b) Vector:

It is the same as Array List.

Vector methods are synchronized.
Thread safety.
It also implements Random Access.
Thread safety usually causes a performance hit.
Example:

public class Fruit {
public static void main (String [ ] args){
Vector &lt;String&gt; names = new Vector &lt;String&gt; ( );
 names.add (“cherry”);
names.add (“apple”);
names.add (“banana”);
names.add (“kiwi”);
names.add (“apple”);
System.out.println (“names”);
}
}
Output:

[cherry,apple,banana,kiwi,apple]

Vector also maintains the insertion order and accepts the duplicates.

c) Linked List:

Elements are doubly linked to one another.
Performance is slower than the Array list.
Good choice for insertion and deletion.
In Java 5.0 it supports common queue methods peek( ), Pool ( ), Offer ( ) etc.
Example:

public class Fruit {
public static void main (String [ ] args){
Linkedlist &lt;String&gt; names = new linkedlist &lt;String&gt; ( ) ;
names.add(“banana”);
names.add(“cherry”);
names.add(“apple”);
names.add(“kiwi”);
names.add(“banana”);
System.out.println (names);
}
}
Output:

[ banana,cherry,apple,kiwi,banana]

Maintains the insertion order and accepts the duplicates.

----

Q #28) Explain about Set and their types in a collection.

Answer: Set cares about uniqueness. It doesn’t allow duplications. Here “equals ( )” method is used to determine whether two objects are identical or not.

a) Hash Set:

Unordered and unsorted.
Uses the hash code of the object to insert the values.
Use this when the requirement is “no duplicates and don’t care about the order”.
Example:

public class Fruit {
public static void main (String[ ] args){
HashSet&lt;String&gt; names = new HashSet &lt;=String&gt;( ) ;
names.add(“banana”);
names.add(“cherry”);
names.add(“apple”);
names.add(“kiwi”);
names.add(“banana”);
System.out.println (names);
}
}
Output:

[banana, cherry, kiwi, apple]


It doesn’t follow any insertion order. Duplicates are not allowed.

b) Linked Hash set:

An ordered version of the hash set is known as Linked Hash Set.
Maintains a doubly-Linked list of all the elements.
Use this when an iteration order is required.
Example:

public class Fruit {
public static void main (String[ ] args){
LinkedHashSet&lt;String&gt;; names = new LinkedHashSet &lt;String&gt;( ) ;
 names.add(“banana”);
 names.add(“cherry”);
 names.add(“apple”);
 names.add(“kiwi”);
 names.add(“banana”);
 System.out.println (names);
 }
}
Output:

[banana, cherry, apple, kiwi]

It maintains the insertion order in which they have been added to the Set. Duplicates are not allowed.

c) Tree Set:

It is one of the two sorted collections.
Uses the “Read-Black” tree structure and guarantees that the elements will be in ascending order.
We can construct a tree set with the constructor by using a comparable (or) comparator.
Example:

public class Fruits{
public static void main (String[ ]args) {
Treeset&lt;String&gt; names= new TreeSet&lt;String&gt;( ) ;
names.add(“cherry”);
names.add(“banana”);
names.add(“apple”);
names.add(“kiwi”);
names.add(“cherry”);
System.out.println(names);
}
}
Output:

[apple, banana, cherry, kiwi]

TreeSet sorts the elements in ascending order. And duplicates are not allowed.

----

Q #29) Explain about Map and its types.

Answer: Map cares about the unique identifier. We can map a unique key to a specific value. It is a key/value pair. We can search a value, based on the key. Like the set, the map also uses the “equals ( )” method to determine whether two keys are the same or different.

Map is of following types:

a) Hash Map:

Unordered and unsorted map.
Hashmap is a good choice when we don’t care about the order.
It allows one null key and multiple null values.
Example:

Public class Fruit{
Public static void main(String[ ] args){
HashMap&lt;Sting,String&gt; names =new HashMap&lt;String,String&gt;( );
names.put(“key1”,“cherry”);
names.put (“key2”,“banana”);
names.put (“key3”,“apple”);
names.put (“key4”,“kiwi”);
names.put (“key1”,“cherry”);
System.out.println(names);
}
 }
Output:

{key2 =banana, key1=cherry, key4 =kiwi, key3= apple}

Duplicate keys are not allowed in Map.

It doesn’t maintain any insertion order and is unsorted.

b) Hash Table:

Like the vector key, methods of the class are synchronized.
Thread safety and therefore slows the performance.
It doesn’t allow anything that is null.
Example:

public class Fruit{
public static void main(String[ ]args){
Hashtable&lt;Sting,String&gt; names =new Hashtable&lt;String,String&gt;( );
names.put(“key1”,“cherry”);
names.put(“key2”,“apple”);
names.put(“key3”,“banana”);
names.put(“key4”,“kiwi”);
names.put(“key2”,“orange”);
System.out.println(names);
}
 }
Output:

{key2=apple, key1=cherry,key4=kiwi, key3=banana}

Duplicate keys are not allowed.

c) Linked Hash Map:

Maintains insertion order.
Slower than Hash map.
I can expect a faster iteration.
Example:

public class Fruit{
public static void main(String[ ] args){
LinkedHashMap&lt;Sting,String&gt; names =new LinkedHashMap&lt;String,String&gt;( );
 names.put(“key1”,“cherry”);
 names.put(“key2”,“apple”);
 names.put(“key3”,“banana”);
 names.put(“key4”,“kiwi”);
 names.put(“key2”,“orange”);
 System.out.println(names);
 }
 }
Output:

{key2=apple, key1=cherry,key4=kiwi, key3=banana}

Duplicate keys are not allowed.

d) TreeMap:

Sorted Map.
Like Tree set, we can construct a sort order with the constructor.
Example:

public class Fruit{
public static void main(String[ ]args){
TreeMap&lt;Sting,String&gt; names =new TreeMap&lt;String,String&gt;( );
names.put(“key1”,“cherry”);
names.put(“key2”,“banana”);
names.put(“key3”,“apple”);
names.put(“key4”,“kiwi”);
names.put(“key2”,“orange”);
System.out.println(names);
}
}
Output:

{key1=cherry, key2=banana, key3 =apple, key4=kiwi}

It is sorted in ascending order based on the key. Duplicate keys are not allowed.

----

Q #30) Explain the Priority Queue.

Answer: Queue Interface

Priority Queue: Linked list class has been enhanced to implement the queue interface. Queues can be handled with a linked list. The purpose of a queue is “Priority-in, Priority-out”.

Hence elements are ordered either naturally or according to the comparator. The elements ordering represents their relative priority.

----

Q #31) What is meant by Exception?

Answer: An Exception is a problem that can occur during the normal flow of execution. A method can throw an exception when something wails at runtime. If that exception couldn’t be handled, then the execution gets terminated before it completes the task.

If we handled the exception, then the normal flow gets continued. Exceptions are a subclass of java.lang.Exception.

Example for handling Exception:

try{
//Risky codes are surrounded by this block
}catch(Exception e){
//Exceptions are caught in catch block
}

----

Q #32) What are the types of Exceptions?

Answer: There are two types of Exceptions. They are explained below in detail.

a) Checked Exception:

These exceptions are checked by the compiler at the time of compilation. Classes that extend Throwable class except Runtime exception and Error are called checked Exception.

Checked Exceptions must either declare the exception using throws keyword (or) surrounded by appropriate try/catch.

For Example, ClassNotFound Exception

b) Unchecked Exception:

These exceptions are not checked during the compile time by the compiler.  The compiler doesn’t force to handle these exceptions. It includes:

Arithmetic Exception
ArrayIndexOutOfBounds Exception

----

Q #33) What are the different ways to handle exceptions?

Answer: Two different ways to handle exceptions are explained below:

a) Using try/catch:

The risky code is surrounded by try block. If an exception occurs, then it is caught by the catch block which is followed by the try block.

Example:

class Manipulation{
public static void main(String[] args){
add();
}
Public void add(){
try{
addition();
}catch(Exception e){
e.printStacktrace();
}
}
}
b) By declaring throws keyword:

At the end of the method, we can declare the exception using throws keyword.

Example:

class Manipulation{
public static void main(String[] args){
add();
}
public void add() throws Exception{
addition();
}
}

----

Q #34) What are the advantages of Exception handling?

Answer: The advantages are as follows:

The normal flow of the execution won’t be terminated if an exception gets handled
We can identify the problem by using catch declaration

----

Q #35) What are the Exception handling keywords in Java?

Answer: Enlisted below are the two Exception Handling Keywords:

a) try:

When a risky code is surrounded by a try block. An exception occurring in the try block is caught by a catch block. Try can be followed either by catch (or) finally (or) both. But any one of the blocks is mandatory.

b) catch:

This is followed by a try block. Exceptions are caught here.

c) finally:

This is followed either by try block (or) catch block. This block gets executed regardless of an exception. So generally clean up codes are provided here.

----

Q #36) Explain about Exception Propagation.

Answer: Exception is first thrown from the method which is at the top of the stack. If it doesn’t catch, then it pops up the method and moves to the previous method and so on until they are got.

This is called Exception propagation.

Example:

public class Manipulation{
public static void main(String[] args){
add();
}
public void add(){
addition();
}
From the above example, the stack looks like as shown below:

Stack Example           

If an exception occurs in the addition() method is not caught, then it moves to the method add(). Then it is moved to the main() method and then it will stop the flow of execution. It is called Exception Propagation.

----

Q #37) What is the final keyword in Java?

Answer:

Final variable: Once a variable is declared as final, then the value of the variable could not be changed. It is like a constant.

Example:

final int = 12;

Final method: A final keyword in a method, couldn’t be overridden. If a method is marked as a final, then it can’t be overridden by the subclass.

Final class: If a class is declared as final, then the class couldn’t be subclassed. No class can extend the final class.

----

Q #38) What is a Thread?

Answer: In Java, the flow of execution is called Thread. Every java program has at least one thread called the main thread, the main thread is created by JVM. The user can define their own threads by extending the Thread class (or) by implementing the Runnable interface. Threads are executed concurrently.

Example:

public static void main(String[] args){//main thread starts here
}

----

Q #39) How do you make a thread in Java?

Answer: There are two ways available to make a thread.

a) Extend Thread class: Extending a Thread class and override the run method. The thread is available in java.lang.thread.

Example:

Public class Addition extends Thread {
public void run () {
}
}
The disadvantage of using a thread class is that we cannot extend any other classes because we have already extended the thread class. We can overload the run () method in our class.

b) Implement Runnable interface: Another way is by implementing the runnable interface. For that, we should provide the implementation for the run () method which is defined in the interface.

Example:

Public class Addition implements Runnable {
public void run () {
}
}

----

Q #40) Explain about join() method.

Answer: Join () method is used to join one thread with the end of the currently running thread.

Example:

public static void main (String[] args){
Thread t = new Thread();
t.start();
t.join();
}
Based on the above code, the main thread has started the execution. When it reaches the code t.start() then ‘thread t’ starts the own stack for the execution. JVM switches between the main thread and ‘thread t’.

Once it reaches the code t.join() then ‘thread t’ alone is executed and completes its task, then only the main thread starts the execution.

It is a non-static method. The Join () method has an overloaded version. So we can mention the time duration in join () method also “.s”.

----

Q #41) What does the yield method of the Thread class do?

Answer: A yield () method moves the currently running thread to a runnable state and allows the other threads for execution. So that equal priority threads have a chance to run. It is a static method. It doesn’t release any lock.

Yield () method moves the thread back to the Runnable state only, and not the thread to sleep (), wait () (or) block.

Example:

public static void main (String[] args){
Thread t = new Thread ();
t.start ();
}
public void run(){
Thread.yield();
}
}

----

Q #42) Explain about wait () method.

Answer: wait () method is used to make the thread to wait in the waiting pool. When the wait () method is executed during a thread execution then immediately the thread gives up the lock on the object and goes to the waiting pool. Wait () method tells the thread to wait for a given amount of time.

Then the thread will wake up after notify () (or) notify all () method is called.

Wait() and the other above-mentioned methods do not give the lock on the object immediately until the currently executing thread completes the synchronized code. It is mostly used in synchronization.

Example:

public static void main (String[] args){
Thread t = new Thread ();
t.start ();
Synchronized (t) {
Wait();
}
}

----

Q #43) Difference between notify() method and notifyAll() method in Java.

Answer: The differences between notify() method and notifyAll() method are enlisted below:

notify()	notifyAll()
This method is used to send a signal to wake up a single thread in the waiting pool.	This method sends the signal to wake up all the threads in a waiting spool.
Q #44) How to stop a thread in java? Explain about sleep () method in a thread?

----


Answer: We can stop a thread by using the following thread methods:

Sleeping
Waiting
Blocked
Sleep: Sleep () method is used to sleep the currently executing thread for the given amount of time. Once the thread is wake up it can move to the runnable state. So sleep () method is used to delay the execution for some period.

It is a static method.

Example:

Thread. Sleep (2000)

So it delays the thread to sleep 2 milliseconds. Sleep () method throws an uninterrupted exception, hence we need to surround the block with try/catch.

public class ExampleThread implements Runnable{
public static void main (String[] args){
Thread t = new Thread ();
t.start ();
}
public void run(){
try{
Thread.sleep(2000);
}catch(InterruptedException e){
}
}

----

Q #45) When to use the Runnable interface Vs Thread class in Java?

Answer: If we need our class to extend some other classes other than the thread then we can go with the runnable interface because in java we can extend only one class.

If we are not going to extend any class then we can extend the thread class.

----

Q #46) Difference between start() and run() method of thread class.

Answer: Start() method creates a new thread and the code inside the run () method is executed in the new thread. If we directly called the run() method then a new thread is not created and the currently executing thread will continue to execute the run() method.

----

Q #47) What is Multi-threading?

Answer: Multiple threads are executed simultaneously. Each thread starts its own stack based on the flow (or) priority of the threads.

Example Program:

public class MultipleThreads implements Runnable
{
public static void main (String[] args){//Main thread starts here
Runnable r = new runnable ();
Thread t=new thread ();
t.start ();//User thread starts here
Addition add=new addition ();
}
public void run(){
go();
}//User thread ends here
}
On the 1st line execution, JVM calls the main method and the main thread stack looks as shown below.

Thread1

Once the execution reaches, t.start () line then a new thread is created and the new stack for the thread is also created. Now JVM switches to the new thread and the main thread are back to the runnable state.

The two stacks look as shown below.

Thread2

Now, the user thread executed the code inside the run() method.

Thread3

Once the run() method has completed, then JVM switches back to the main thread and the user thread has completed the task and the stack was disappeared.

JVM switches between each thread until both the threads are completed. This is called Multi-threading.

----

Q #48) Explain the thread life cycle in Java.

Answer: Thread has the following states:

New
Runnable
Running
Non-runnable (Blocked)
Terminated
Thread Life Cycle in JAVA

New: In New state, a Thread instance has been created but start () method is not yet invoked. Now the thread is not considered alive.
Runnable: The Thread is in the runnable state after the invocation of the start () method, but before the run () method is invoked. But a thread can also return to the runnable state from waiting/sleeping. In this state, the thread is considered alive.
Running: The thread is in a running state after it calls the run () method. Now the thread begins the execution.
Non-Runnable(Blocked): The thread is alive but it is not eligible to run. It is not in the runnable state but also, it will return to the runnable state after some time. Example: wait, sleep, block.
Terminated: Once the run method is completed then it is terminated. Now the thread is not alive.

----

Q #49) What is Synchronization?

Answer: Synchronization makes only one thread to access a block of code at a time. If multiple threads accesses the block of code, then there is a chance for inaccurate results at the end. To avoid this issue, we can provide synchronization for the sensitive block of codes.

The synchronized keyword means that a thread needs a key in order to access the synchronized code.

Locks are per objects. Every Java object has a lock. A lock has only one key. A thread can access a synchronized method only if the thread can get the key to the objects to lock.

For this, we use the “Synchronized” keyword.

Example:

public class ExampleThread implements Runnable{
 public static void main (String[] args){
 Thread t = new Thread ();
 t.start ();
 } 
 public void run(){
 synchronized(object){
 {
 }
}

----

Q #50) What is the disadvantage of Synchronization?

Ans: Synchronization is not recommended to implement all the methods. Because if one thread accesses the synchronized code then the next thread should have to wait. So it makes a slow performance on the other end.

----

Q #51) What is meant by Serialization?

Answer: Converting a file into a byte stream is known as Serialization. The objects in the file are converted to bytes for security purposes. For this, we need to implement a java.io.Serializable interface. It has no method to define.

Variables that are marked as transient will not be a part of the serialization. So we can skip the serialization for the variables in the file by using a transient keyword.

Learn More =>> Serializable and Cloneable

----

Q #52) What is the purpose of a transient variable?

Answer: Transient variables are not part of the serialization process. During deserialization, the values of the transient variables are set to the default value. It is not used with static variables.

Example:

transient int numbers;

----

Q #53) Which methods are used during the Serialization and Deserialization process?

Answer: ObjectOutputStream and ObjectInputStream classes are higher level java.io. package. We will use them with lower level classes FileOutputStream and FileInputStream.

ObjectOutputStream.writeObject —->Serialize the object and write the serialized object to a file.

ObjectInputStream.readObject —> Reads the file and deserializes the object.

To be serialized, an object must implement the serializable interface. If superclass implements Serializable, then the subclass will automatically be serializable.

----

Q #54) What is the purpose of a Volatile Variable?

Answer: Volatile variable values are always read from the main memory and not from thread’s cache memory. This is used mainly during synchronization. It is applicable only for variables.

Example:

volatile int number;

----

Q #55) Difference between Serialization and Deserialization in Java.

Answer: These are the differences between serialization and deserialization in java:

Serialization	Deserialization
Serialization is the process which is used to convert the objects into byte stream	Deserialization is the opposite process of serialization where we can get the objects back from the byte stream.
An object is serialized by writing it an ObjectOutputStream.	An object is deserialized by reading it from an ObjectInputStream.
Q #56) What is SerialVersionUID?

Answer: Whenever an object is Serialized, the object is stamped with a version ID number for the object class. This ID is called the  SerialVersionUID. This is used during deserialization to verify that the sender and receiver that are compatible with the Serialization.

</https://www.softwaretestinghelp.com/core-java-interview-questions/>

<https://javahungry.blogspot.com/2020/05/entry-level-interview-questions.html>

----

Q1 What are the main features of Java?
a.  Java is an Object-Oriented programming language
b.  Simple
c.  Distributed
d.  Java support Multithread
e.  Java is a Platform independent programming language
f.  Java is more secured than other languages
g.  Portable
h.  Robust

----

Q2 What is an Array?
The collection of similar data types is known as Array. You can find it in detail here.

----

Q3 Is it possible to declare an Array without Array size?
It is not possible to declare an Array without Array size. If you try to do so then you will get compile-time error.

----

Q4 What do you understand by the term Object-Oriented Programming language? 
The object-oriented programming language is a language that uses objects in programming.

----

Q5 What are the basic principles of the OOPs concept?
a. Abstraction
b. Polymorphism
c. Encapsulation
d. Inheritance

----

Q6. What is the abstraction in java?
Abstraction means hiding the detailed information from the user. Abstraction can be achieved by interfaces and abstract classes.

----

Q7 What do you mean by inheritance in java?
Inheritance is the main feature of java. Inheritance means java class or interface can inherit the properties and behavior from another class or interface. Inheritance can be gained by implementing interfaces or extending classes. You can find it in detail here.

----

Q8 What do you mean by the Object in java?
The object is the instance of a class. A class contains the basic properties and behavior of a real-world object. We can instantiate this class with a new keyword to make an object.
For example, Animal.java has a class named Animal. Animal animal = new Animal() is an object or instance of this class.

----

Q9 What is a constructor?
Java provides the facility to declare a special member of the class with the same name, no return type, and with zero or many parameters is called a constructor.

----

Q10 What is polymorphism in java?
Poly means many and Morph means forms of a method or constructor or operator. So finally, Polymorphism means many forms of the same method or constructor or operators. You can find it in detail here.

----

Q11 What do you mean by the method overloading?
The method with the same name but the number of arguments are different is called method overloading. Methods return type should be the same for all methods. You can find it in detail here.

----

Q12 What do you mean by the method overriding in java?
You can find the details about method overriding here.

----

Q13 Does java support multiple inheritance?
Java classes do not support multiple inheritance but can gain multiple inheritance by using the interfaces.

----

Q14 Describe constructor vs method?
The constructor is the special member of the class with the same name as the class and no return type. But the method is the ordinary member of a class used to describe the behavior of some object or class.

----

Q15 Is it possible to overload the main() method?
Yes, the main method can be overloaded. But we should declare original one like public static void main(String args[]){} because JVM will look for this when starting execution.

----

Q16 What is the difference between String, StringBuilder and StringBuffer?
You can find the answer in detail here.

----

Q17 What is the difference between Collection and Collections.
The difference between Collection and Collections you can find it in detail here.

----

Q18 What is multithreaded programming?
Multithreaded means multiple threads will run to execute the task simultaneously.  It's important in the programming world. The operating system is an example of a multithreaded system.

----

Q19 What is the difference between Error and Exception?
Error is generated by the environment at runtime. The exception is generated by the application intentionally or mistakenly. An exception can be checked or unchecked, but the error is only unchecked. You can find the difference between Error and Exception here.

----

Q20 Difference between static and non-static methods?
Static methods belong to a class but non-static methods belong to an object. You don’t need to instantiate a class to access the static methods, but you have to instantiate the class to get access to non-static methods.

----

Q21 Difference between method overloading and method overriding?
You can find the difference between method overloading and method overriding here.

----

Q22 What are the different ways to create threads in java?
There are two ways to create threads in java. Ways are listed below:
a. Implement Runnable interface
b. By extending Thread class

----

Q23 What is the synchronization in java?
Synchronization is a technique to control access of a method with multiple threads at the same time. If we declare a method synchronized, then only one thread can use this method at a time. This is basically used for Thread safety. You can find it in detail here.

----

Q24 What is the use of the final keyword?
We cannot change the value of a final variable. We are not able to inherit a final class and cannot override a final method.

----

Q25 What is the garbage collection of java?
To clean the object from memory which has no reference is called garbage collection. It’s an important feature of java. Java automatically clears the objects from memory. We don’t need to clean the object manually from memory.

----

Q26 What is the cloning in java?
Java cloning means create an exact copy of an object. Shallow or Deep cloning is used in java to clone a java object. The clone() method is used to clone an object. You can find the difference between Shallow and Deep cloning here.

----

Q27 What is JVM? 
Java virtual machine is called JVM. JVM compiles and interprets the java code. JVM manages the garbage collection mechanism and other things efficiently. JVM manages objects in heap memory.

----

Q28 What are the difference between final, finally and finalize in java?
The keyword final is used to make a class, variable, or methods final. Final classes cannot be inherited, variables value cannot be changed, and methods cannot be overridden.
The keyword finally used in the exception handler to clear some post-task after the execution of try or catch block.
The finalize keyword used to clean up some tasks before the object is removed from memory. The finalize method mainly used in garbage collection.
You can find it in detail here.

----

Q29 What is the difference between float and double datatypes?
You can find the answer in detail here.

----

Q30 Is it possible to override the overloaded method in java?
Yes, in java it is possible to override the overloaded method.

That's all for today. Please mention in comments in case you have any questions related to top 30 entry level interview questions and answers.

</https://javahungry.blogspot.com/2020/05/entry-level-interview-questions.html>

<https://www.interviewbit.com/j2ee-interview-questions/>

----

1. What is J2EE?
J2EE or Java Enterprise Edition is a Java-based platform that is a combination of services protocols and APIs (Application Programming Interfaces) that provides capabilities to develop multi-tier, secure, stable and fast enterprise-level applications. J2EE provides web, enterprise, web service and various other specifications for developing enterprise-level web applications.


----

2. What are the main advantages of J2EE?
Following are the advantages of the J2EE platform:

Support for Web Services: J2EE provides a platform to develop and deploy web services. The JAX-RPC (Java API for XML based Remote Procedure Call) helps developers develop SOAP-based portable and interoperable web services, clients and endpoints.
Faster Time to Market: J2EE uses the concept of containers for simplifying the development. This helps in business logic separation from lifecycle management and resources which aids developers to focus on business logic than on the infrastructure. For instance, the EJB (Enterprise JavaBeans) container takes care of threading, distributed communication, transaction management, scaling etc and provides a necessary abstraction to the developers.
Compatibility: J2EE platform follows the principle of “Write Once, Run Anywhere”. It provides comprehensive standards and APIs that ensures compatibility among different application vendors resulting in the portability of applications.
Simplified connectivity: J2EE helps in easier applications connectivity which allows utilizing the capabilities of different devices. It also provides JMS (Java Message Service) to integrate diverse applications in asynchronous and loosely coupled ways. It also provides CORBA (Common Object Request Broker Architecture) support for linking systems tightly via remote calls.
Due to all the above benefits packed in one technology, it helps the developers to reduce the TCO (Total Cost of Ownership) and also focus more on actual business logic implementation.

----

3. What are some of the technologies provided by the J2EE platform?
Some of the important technologies provided by J2EE are:

Java API for XML-Based RPC (JAX-RPC): This is used to build web services and clients that make use of XML and Remote Procedure Calls.
Java Server Pages (JSP): This is used for delivering XML and HTML documents. Apart from these, we can make use of OutputStream for delivering other data types as well.
Java Servlets: Servlets are classes used for extending the server capabilities which hosts applications and can be accessed using the request-response model.

Enterprise Java Beans (EJB): This is a server-side component that is used for encapsulating the application’s business logic by providing runtime environment, security, servlet lifecycle management, transaction management and other services.
J2EE Connector Architecture: This defines standard architecture to connect J2EE platforms to different EIS (Enterprise Information Systems) such as mainframe processes, database systems and different legacy applications coded in another language.
J2EE Deployment API: Provides specifications for web services deployment
Java Management Extensions (JMX): They are used for supplying tools for monitoring and managing applications, objects, devices and networks.
J2EE Authorization Contract for Containers (JACC): This is used to define security contracts between authorization policy modules and application servers.
Java API for XML Registries (JAXR): This provides standard API to access different XML Registries to enable infrastructure for the building and deployment of web services.
Java Message Service (JMS): This is a messaging standard for allowing different JEE components for creating, sending, receiving and reading messages by enabling communication in a distributed, loosely coupled, asynchronous and reliable manner.
Java Naming and Directory Interface (JNDI): This is an API that provides naming and directory functionality for Java-based applications.
Java Transaction API (JTA): This is used for specifying Java standard interfaces between transaction systems and managers.
Common Object Request Broker Architecture (CORBA): This provides a standard for defining Object Management Group designed for facilitating system communication deployed on diverse platforms.
JDBC data access API: This provides API for getting data from any data sources like flat files, spreadsheets, relational databases etc.
You can download a PDF version of J2ee Interview Questions.

Download PDF

----

4. What are the various components of J2EE application architecture?
J2EE is made up of 3 main components (tiers) - Client tier, Middle tier, Enterprise data tier as shown in the below image:


Client Tier: This tier has programs and applications which interact with the user and they are generally located in different machines from the server. Here, different inputs are taken from the user and these requests are forwarded to the server for processing and the response will be sent back to the client.
Middle Tier: This tier comprises of Web components and EJB containers. The web components are either servlet or JSP pages that process the request and generate the response. At the time of the application’s assembly, the client’s static HTML codes, programs and applets along with the server’s components are bundled within the web components. The EJB components are present for processing inputs from the user which are sent to the Enterprise Bean that is running in the business tier.
Enterprise Data Tier: This tier includes database servers, resource planning systems and various other data sources that are located on a separate machine which are accessed by different components by the business tier. Technologies like JPA, JDBC, Java transaction API, Java Connector Architecture etc are used in this tier.

----

5. How is JDK different from JIT?
JDK (Java Development Kit) is a cross-platformed software development environment offering various collections of libraries and tools required for developing Java applications and applets. It also consists of JRE that provides tools and libraries which aids in byte code execution. JDK is needed for writing and running programs in Java. Whereas JIT stands for Just In Time Compiler which is a module inside JVM (which is inside JRE). JIT compiler is used for compiling some parts of byte code having similar functionality at the same time to machine code for optimising the compilation time and performance.

----

6. How are PATH and CLASSPATH different from each other in terms of J2EE?
PATH and CLASSPATH are key environmental variables used by Java platforms.

The PATH variable points to JDK binaries or native libraries like java.exe. Whereas The CLASSPATH variable points to the binaries of Java such as JAR files that consist of bytecode.
PATH is a system-level variable independent of Java being present in the system or not. Whereas CLASSPATH is purely Java-specific which is used by JVM for loading classes required by Java applications while running.
7. How is multi-tier client-server architectural model advantageous?
Multi-tier client-server architectural model consists of various components known as tiers that interact with each other. The below image represents the three-tier application model which has client/presentation tier, business logic tier and the database tier which interact with each other to process a request and send a response:


In the multi-tier system, we have the following advantages:

Any changes to the user interface or business logic can be done independently.
It introduces abstraction between the components. For example, the client tier can access data without knowing from where and how the response comes from, what is the server infrastructure available in the backend etc.
Each tier can be coded or developed independently. For example, the middle tier can be coded in Java or python, the client tier can be coded in Angular or React etc.
The database can have pooled connections for sharing data among multiple users without the need for creating a new connection for every user.

----

8. What do you understand by build file?
A build file is used for automating various steps involved in software development. Along with this, the build file also specifies libraries and their versions that need to be included. It also includes the type of optimizations required for the project. Whenever the project size increases, build provides a standard way to build the project.

----

9. Why do we have JDBC and JNDI in J2EE? How are they different from each other?
JDBC or Java Database Connectivity provides guidelines and APIs for connecting databases from different vendors like MySQL, Oracle, PostgreSQL etc for getting data. JNDI (Java Naming and Directory Interface) helps in providing logical structure to retrieve a resource from the database, EJB beans, messaging queues etc without knowing the actual host address or port. A resource can be registered with JNDI and then those registered application components can be accessed using the JNDI name.

----

10. What is an EJB? How can you use it in J2EE?
EJB or Enterprise Java Beans is one of the most important parts of the J2EE platform that helps to develop enterprise-level multi-tiered applications and deploy them by keeping in mind performance, scalability and robustness. EJBs can be used when we want to achieve the following:

Clustering: For deploying the application in a cluster environment, EJBs can be used to achieve high availability and fault tolerance.
Concurrency without using Threads: EJBs can be used to achieve concurrency without using actual threads since they are instantiated using the object pool and are available in the EJB container. This helps in achieving performance without involving complexities around Threads.

Transaction management: EJBs can be used for achieving transaction management for databases by using annotations provided by EJB.
Database Connection Pool: EJB can access connection pools defined in the J2EE server. The connection pools help in achieving abstraction of database connectivity and operations.
Security: EJBs use JAAS (Java Authentication and Authorization Service) to develop secure applications. EJB methods can be authenticated and authorised with only configuration changes.
Scheduler Service: EJBs can be used in the Timer Service which enables task implementation for further execution or repetitive execution.

----

11. What are the J2EE applets? Why can we use it?
Applets are J2EE client components that are written in Java and are executed in a web browser or a variety of other devices which supports the applet programming model. They are used for providing interactive features to web apps and help in providing small, portable embedded Java programs in HTML pages which will be run automatically when we view the pages.

----

12. What is the architecture model of Struts?
Strut is a combination of JSP, Java Servlets, messages and custom tags that together form an application development framework for developing enterprise-level applications. It is based on MVC (Model-View-Controller) architecture.


Model: This component defines the internal system state. It can either be a Java Beans cluster or a single bean depending on the application architecture.
View: Struts make use of JSP technology for designing views of enterprise-level applications.
Controller: It is a servlet and is used for managing user actions that process requests and respond to them.

----

13. What do you understand by ORM?
ORM stands for Object-Relational Mapping that transforms objects of Java class to tables in relational databases and vice versa using metadata describing the mapping between the database and the objects. 

This is represented as shown in the below image:


Consider an example where we have an Employee class having employeeId, firstName, lastName, contactNo as attributes. Consider we also have an Employee table that has ID, FNAME, LNAME and CONTACT_NO as columns. If we want to send data from our Java application and save it in the database, we cannot do it straightforwardly by simply saving the Java objects in the database directly. We need some sort of a mapper that maps the Java objects to the records that are compatible to be saved in the database table. This is where ORM comes into the picture. ORM helps in this transformation while writing data to the database as described in the below image:


The database records cannot be directly consumed by the Java applications as Java only deals with objects. ORM again plays a major role in the transformation of database records to Java objects.

----

14. What constitutes web components?
Java Servlets and Java Server Pages (JSP) components together constitute web components.


Java Servlets dynamically process requests and responses. JSP pages are used for executing servlets that allow a natural approach to creating static content.

----

15. What do you understand by JSF?
JSF stands for Java Server Faces which is a web framework that is intended for simplifying the development process for user interfaces. It is a standardized display technology for Java-based web applications. It is based on MVC (Model-View-Controller) pattern and provides reusable UI components.

----

16. What factors should a J2EE application possess for operating in a global economy?
Following are the factors that a J2EE application should possess to operate globally:

Financial Considerations: Each country has its taxes, restrictions and tariffs depending on the government. All these factors should be considered while developing the J2EE application.
Language Requirements: An application developed should support regional languages of the country for wider user coverage.
Legal Differences: Every government has their custom laws, privacy laws and requirements for each country. An application developed should abide by all the rules of the land.

----

17. What are the differences between JVM vs JIT vs JDK vs JRE?
JVM	JIT	JDK	JRE
Java Virtual Machine: Introduced for managing system memory and also to provide a portable execution environment for Java applications.	Just in Time Compilation: This is a part of JVM and was developed for improving JVM performance.	 Java Development Kit: JDK is a cross-platformed software development environment offering various collections of libraries and tools required for developing Java applications and applets.	Java Runtime Environment: JRE is part of JDK that consists of JVM, core classes and support libraries. It is used for providing a runtime environment for running Java programs.
Used for compiling byte code to machine code completely.	This is used for compiling only reusable byte code to machine code.	JDK is essential for writing and running programs in Java.	JRE is a subset of JDK and is like a container that consists of JVM, supporting libraries and other files. It doesn't have development tools such as compilers and debuggers.
This is used for providing platform independence.	This is used for improving the performance of JVM.	JDK is used for developing Java programs as it provides libraries and compiler tools as well as JRE for running the code.	JRE is not suitable for development. It is used for running Java Programs as it provides runtime environments and tools for supporting execution.
J2EE Interview Questions for Experienced

----

18. What are the design goals of J2EE architecture?
The design goals of J2EE architecture are as follows:

Service Availability: To ensure that the application is available 24*7 to achieve required business goals.
Data Connectivity: The connection between a J2EE application and legacy systems should remain compatible enough for ensuring business functions.
Ease of Accessibility: The user should be able to connect to applications using any device and from anywhere.
User Interaction: The user interaction should be seamless and should be able to connect to different devices like desktops, mobiles, laptops etc.
Abstraction and Flexibility: The developer should focus on business logic and the configuration details should be handled by the server.

----

19. What do you understand by Connectors? Can you describe the Connector Architecture?
Connectors are used for providing standard extension mechanisms to provide connectivity to different enterprise information systems. A connector architecture consists of resource adapters and system-level contracts, both of which are specific to enterprise information systems. The resource adapters are plugged into the container. The connector architecture defines certain contracts which a resource adapter must support for plugging into J2EE applications like security, transaction, resource management etc.

----

20. What do you understand by JRMP?
JRMP stands for Java Remote Method Protocol which is used for Remote Method Invocation (RMI) for passing Java objects as arguments. It is an underlying protocol used by RMI for marshalling objects as a stream during object serialization for transferring objects from one JVM to other.

----

21. What happens if the database connected to the Java application via connection pool suddenly goes down?
Since the Java application uses a connection pool, it has active connections that would get disconnected if the database goes down. When the queries are executed to retrieve or modify data, then we will get a Socket exception.

----

22. How is 32-bit JVM different from 64-bit JVM?
64-bit JVM is used in 64-bit operating systems whereas 32-bit JVM is used for 32-bit operating systems. In 64-bit JVM, we can specify more heap size memory up to 100G when compared to the 4G limit of 32-bit JVM. Java applications take more memory while running in 64-bit JVM when compared to running the same application in 32-bit JVM. This is because of the increased size of the Ordinary Object Pointer. However, this can be bypassed by making use of the -XXCompressedOOP option of the JVM for telling to use 32-bit pointers. Additionally, 64-bit JVM uses 12 bytes object header size and a maximum of 8 bytes of internal references whereas the 32-bit JVM uses 8 bytes headers and a maximum of 4 bytes of internal references.

----

23. How is a webserver different from an application server?
Web Server 	Application Server
Web servers are computer programs that accept requests and returns responses based on that.


Application servers are used for installing, operating and hosting associated applications and services.


It constitutes the web container.	It constitutes both a web container and an EJB container.
These are useful for getting static content for the applications.	These are useful for getting dynamic content.
This consumes and utilizes fewer resources.	It makes use of more resources.
Provide an environment for running web applications.	Provide an environment for running enterprise applications.
Web servers don’t support multithreading.	Multithreading is supported in application servers.
This server makes use of HTML and HTTP protocols.	The application server has GUI (Graphical User Interface) and also supports HTTP, RPC/RMI protocols.
24. What is the purpose of heap dumps and how do you analyze a heap dump?
Heap dumps consist of a snapshot of all live objects on Java heap memory that are used by running Java applications. Detailed information for each object like type, class name, address, size and references to other objects can be obtained in the heap dump. Various tools help in analyzing heap dumps in Java. For instance, JDK itself provides jhat tool for analysing heap dump. Heap dumps are also used for analysing memory leaks which is a phenomenon that occurs when there are objects that are not used by the application anymore and the garbage collection is not able to free that memory as they are still shown as referenced objects. Following are the causes that result in memory leaks:

Continuously instantiating objects without releasing them.
Unclosed connection objects (such as connections to the database) post the required operation.
Static variables holding on to references of objects.
Adding objects in HashMap without overriding hashCode() equals() method. If these methods are not included, then the hashmap will continuously grow without ignoring the duplicates.
Unbounded caches.
Listener methods that are uninvoked.
Due to this, the application keeps consuming more and more memory and eventually this leads to OutOfMemory Errors and can ultimately crash the application. We can make use of the Eclipse Memory Analyzer or jvisualVM tool for analysing heap dump to identify memory leaks.

----

25. How can we take a heap dump of a Java process?
There are multiple ways for taking heap dump of Java process. Tools like jCmd, jVisualVM, jmap are available for this purpose. For example, if we are using jmap, then heap dump can be taken by running the below command:

$ jmap -dump:live, file=/path/of/heap_dump.hprof  PID
This heap dump contains live objects that are stored in heap_dump.hprof file. Process ID (PID) of the Java process is needed to get the dump that can be obtained by using ps or grep commands.

----

26. How is J2EE different from Spring?
J2EE	Spring
J2EE is a standard or specification defined by Sun/Oracle which is used for web development.	Spring is a framework used for designing templates for an application.
J2EE has an Oracle-based license.	Spring is an open-source framework.
J2EE is based on a 3D framework- Logical Tiers, Client Tiers, and Presentation Tiers.	Spring is based on layered architecture having many modules that are made on top of the core container.
J2EE makes use of high-level object-oriented languages like Java.	Spring doesn’t have a specific programming model.
J2EE is faster.	Spring is slower than J2EE.
Makes use of JTA API with execution.	Spring provides a layer of abstraction to help JTA execution merchants.

----

27. What are EAR, WAR, and JAR?
EAR stands for Enterprise Archive file and it consists of web, EJB and client components all compressed and packed into a file called .ear file. EAR files allow us to deploy different modules onto the application server simultaneously.

WAR stands for Web Archive file and consists of all web components packed and compressed in a .war file. This file allows testing and deploying web applications easily in a single request.

JAR stands for Java Archive file. It consists of all libraries and class files that constitute APIs. These are packed and compressed in a file called the .jar file. These are used for deploying the entire application including classes and resources in a single request.

----

28. What do you know about Hibernate?
Hibernate is an Object Relational Mapper framework in Java that provides a layer of abstraction for retrieving or modifying data in the database. It handles all the implementations internally and the developer need not worry about how the connections to the databases are made, how the data translation from Java application to Database and vice versa happens. Hibernate supports powerful object-oriented concepts like inheritance, association, polymorphism, compositions, collections that help in making queries using the Java approach by using HQL (Hibernate Query Language).

----

29. What are deployment descriptors used for?
Servlets are server-side components that aid in developing powerful server-side applications. Ther are servers that are platform-independent and follow various protocols as per the application design. The most commonly used protocol is the HTTP protocol. In Java, we can create servlets by implementing the Servlet interface that has 3 lifecycle methods - init, service and destroy - and we can use the below classes for implementing servlets:

javax.servlet.http.HttpServletRequest
javax.servlet.http.HttpServletResponse
javax.servlet.http.HttpSession.

----

30. Can you describe the phases of the servlet lifecycle?
The below image describes the different phases of the servlet lifecycle:


There are five phases, are as follows:

Classloading phase: The first step is to load the servlet class file (.class extension) by the web container.
Instantiation phase: Next step is to instantiate the servlet by calling the default constructor.
Initialize phase: In this phase, the init() method of the servlet is run where the servlet configuration will be assigned to the servlet. This is a lifecycle method provided by the Servlet interface which is run only once in the servlet lifetime.
Request Handling phase: Here, the servlets provide services to different requests by making use of the service() method of the Servlet interface.
Removal phase: In this phase, the destroy() lifecycle method of the Servlet interface will be called that is used for clearing the configuration and closing resources before servlet destruction. Post this, the garbage collection will take place.

----

31. How does a servlet application work?
A Java servlet is typically multithreaded. This means that multiple requests can be sent to the same servlet and they can be executed at the same time. All the local variables (not pointing to shared resources) inside the servlet are automatically thread-safe and are request specific. Care has to be taken when the servlet is accessing or modifying the global shared variable. The servlet instance lifecycle for different requests are managed by the web container as follows:

User clicks on a link in a client that requests a response from a server. In this instance, consider that the client performs GET request to the server as shown in the image below:

The web container intercepts the request and identifies which servlet has to serve the request by using the deployment descriptor file and then creates two objects as shown below-
HttpServletRequest - to send servlet request
HttpServletResponse - to get the servlet response

The web container then creates and allocates a thread that inturn creates a request that calls the service() lifecycle method of the servlet and passes the request and response objects as parameters as shown below:

service() method decides which servlet method - doGet() or doPost() or doPut() or doDelete()- depending on the HTTP requests received from the client. In our case, we got the GET request from the client and hence the servlet will call the doGet() method as described below.

Servlet makes use of the response object obtained from the servlet method for writing the response to the client.

Once the request is served completely, the thread dies and the objects are made ready for garbage collection.

----

32. What do you understand by Java Message Service (JMS)?
JMS is a Java-based API that is like a gateway to the message-oriented middleware like SonicMQ, IBM MQSeries etc. It provides a mechanism for sending and receiving messages by making use of the publishing/subscribe (1 message multiple receivers) model or point-to-point (1 message 1 receiver) paradigm from one client to another. 

The following image describes how 2 clients can communicate with each other utilizing JMS providers.


Conclusion:
J2EE defines standards and specifications for various components such as e-mailing, database connectivity, security, XML parsing, CORBA communication etc that help in developing complex, reliable, secure and distributed servlets and applications that follow the client-server model. It provides various API interfaces that act as standards between different vendor adapters and J2EE components. This ensures that the application components are not dependent on vendor codes. Due to this, J2EE has been very popular among Java developers in the field of software development.

----

J2EE MCQ
1.
Which of the following exception is thrown when the initialization of servlet fails?


RemoteException

ServletException

SocketException

IOException

----

2.
Which of the following option is not a J2EE client?


JSP

Web Applications

Applets

Java Web Start clients

----

3.
What is the directory path where the classes should be present for the application’s Classloader?


/root/lib/classes/

/WEB-INF/lib/classes/

/WEB-INF/classes/

/root/classes/

----

4.
What lifecycle method is called for the first time and only once by a servlet?


start()

run()

initialize()

init()

----

5.
What is the scope of the response object?


page

session

response

request

----

6.
Which of the below files have the EJB modules of the application?


.zip

.jar

.war

.ear

----

7.
Which tier provides internal functionality to J2EE apps?


Enterprise Interface System Tier

Presentation Tier

Enterprise Java Beans Tier

Web Tier

----

8.
When is the destroy method of a filter called?


Only once at the end of the filter lifecycle

After the doFilter method is executed

Only once at the beginning of the filter lifecycle

never called

----

9.
Which of the following option is responsible for optimising byte codes to machine code?


JVM

JDK

JRE

JIT

----

10.
Which of the following bean type is defined without client view interfaces?


Stateful Session bean

Stateless Session bean

Message Driven Bean

BMP Entity bean

</https://www.interviewbit.com/j2ee-interview-questions/>

<https://www.softwaretestinghelp.com/j2ee-interview-questions-answers/>

----

Q #1) What are the components of J2EE applications?

Answer: The components of J2EE applications include:

Client-tier components: Run-on the client machine.
Web tier components: Run-on the J2EE server.
Business tier components: Run-on the J2EE server.
Enterprise Information System software (EIS software): Runs on the EIS server.

----

Q #2) What are the J2EE client types?

Answer: J2EE client types are

Applets
Application clients
Java Web Start enabled clients, by Java Web Start technology.
Wireless clients, based on the Mobile Information Device Profile (MIDP) technology.

----

Q #3) What is a J2EE container?

Answer: The interface between a component and the low-level platform with specific functionality that supports the component is called a container. The application server maintains control and provides relevant services through an interface or framework calls as a container.

----

Q #4) What are defined as web components?

Answer: Java Servlets and Java server pages technology components are identified as web components. Servlets dynamically receive requests and make responses. JSP server pages also behave as Java Servlets but facilitate to create more static content.

----

Q #5) Describe the MVC on struts?

Answer: MVC stands for Model View Controller. Each section in the Model View Controller can be described as follows:

Model: Model represents the internal state of the system as a set of single or many Java Beans.
View: Most often the view is constructed using Java Server Pages (JSP) technology.
Controller: The controller is the process that focuses on receiving client requests and produce the next level of a user interface according to the request. The primary component of the controller in the framework is the “ActionServlet” servlet class.

----

Q #6) Define JSF?

Answer: JSF stands for Java Server Faces. It is the user interface (UI) designing framework for Java Web application developments. There is a set of reusable UI components associated with JSF. Also, JSF has based on Model-View-Controller (MVC) design concepts and patterns. The automated data saving process from form to server and display at the client side is also handled by JSF.

Further reading =>> JSF Interview Questions

----

Q #7) What is Hashtable?

Answer: Hashtable is a collection synchronized object. It allows null value but not the duplicate values. Hashtable is like a HashMap.

----

Q #8) Define Hibernate?

Answer: Hibernate is an open-source object-relational mapping and query service which facilitates writing Hibernate Query Language (HQL) scripts instead of Structured Query Language (SQL) scripts.

It is a fast and easy process than writing native SQL. Hibernate has more powerful object-oriented contents like associations, inheritance, and polymorphism. Also, it has powerful compositions and collections. Hibernate allows making queries using a Java-based approach.

----

Q #9) What are the identified limitation of hibernate?

Answer:

Slower in action: In execution of HQL queries take more time than it executes directly.
Only composite key support is available and it prevents advanced query options.
No shared value type references are available.

----

Q #10) What are the identified advantages of hibernate?

Answer: Advantages are:

Database and vendor independence application.
Standard Object-relational mapping support.
Domain object mapping for a relational database.
Better performance than Java Database Connectivity.
Java Persistence API based applications.

----

Q #11) Describe ORM?

Answer: Object-Relational mapping (ORM) can be described as follows:

The mapped objects in a Java class to the tables of the relational database using metadata describes the database and object mapping. The working method is to transform data from one representation to another.

----

Q #12) What are the advantages of Object-Relational Mapping (ORM)?

Answer: Advantages are:

Productivity: Reduced time for data access coding with the help of automatic code creation base on the defined data model.
Maintainability: All code generated from ORM are well tested. Only the developer is required to create the correct functionality
Performance: The code generated from ORM completely manages the data access needs of the application. No need to create any data access code. Also, the code is optimized to speed up the data access process.
Vendor independence: The code generated from ORM does not depend on the vendor. This is to increase the portability of the application.

----

Q #13) What is the use of method save()?

Answer: In hibernate, this method is used to stores an object into the database. There is a check for duplicate records before inserting it.

----

Q #14) What is the use of method saveorupdate()?

Answer: In hibernate, method saveorupdate() is used to update an object using the identifier. When the value for the identifier is NULL then the method is directed to call save().

----

Q #15) What is the difference between load() and get()?

Answer: When the object is not available in either cache or database, the load() method throws an exception. No null values are returned from the load() method.

When the object is not available in either cache or database, get() returns null.

----

Q #16) What is meant by connection pooling?

Answer: Connection pooling is a mechanism to re-use the existing connections. The pooling mechanism maintains a number of already created object connections and when there is a demand, the mechanism directly uses the existing connection without creating a new one.

----

Q #17) Define the Collection types in Hibernate?

Answer: One-to-many reference is defined as a collection. There are five main collection types associated with J2EE. They are: Set type, List type, Array type, Map type, Bag type

----

Q #18) Define a thin client?

Answer: A program interface that does not have any operations like database queries, complex business rules or any connection to the third-party application is called a thin client.

Q #19) Describe the file types *.ear, * .jar and *.war?

Answer:


*.jar files – Property file containing libraries, resources, and accessories are included with the *.jar file extension.
*.war files – The files that are required for the development of web application (HTML, java scripts, JSP) are included with a *.war file extension.
*.ear files – The files for Enterprise Java Beans modules for the application are saved as *.ear files.

----

Q #20) How spring is related to J2EE?


Answer: Spring is an open-source application that reduces the complexity of enterprise application development. Spring is based on an inversion of control or dependency injection design patterns.

----

Q #21) What are the advantages of using spring for application development?

Answer:

Plain Old Java Object (POJO) based development facilitates to re-use existing components.
Possible to reduce development cost by improving the productivity of the application development.
Improve the testability of application with dependency injection.
Improve maintainability with reduced code coupling.
No need to have an application server and works on enterprise service.

----

Q #22) Discuss the benefit of the Spring Framework?

Answer: Benefits are as follows:

Possibility to organize middle-tier objects in an efficient way.
Easy initialization for properties.
Easily testable components.
Lightweight container.
Possibilities to use configuration management service of spring in any runtime environment with whatever architectural layer.

----

Q #23) Describe servlet?

Answer: The Server-side component that provides a powerful mechanism to create server-side programs is called a servlet. There are servlets available with a design for various protocols. Servlet is also server and platform-independent. The most commonly used protocol for the servlet is Hypertext Transfer Protocol (HTTP). Also, a servlet is a pure java object.

----

Q #24) Describe the phases of the servlet lifecycle?

Answer: The phases of servlet lifecycle are:

Classloading phase – Web container loads the servlet class file (*.class).
Instantiation phase – By calling default no-arg constructor, the servlet class gets Instantiated.
Initialize phase – The method Init () called in this phase in only one time of the lifetime of a servlet. Servlet configuration is assigned to the servlet.
Request Handling phase – In this phase, only servlets spends most of the time. Servlet provides the services to various requests by calling Service ().
Removal phase – The destroy () function is called before servlet destruction. Garbage collection occurs later.

----

Q  #25) What are the different types of JSP tags?

Answer: There are 4 different types of tags associated with JSP. They are mentioned below:

Directives
Declarations
Scriptlets
Expressions

----

Q #26) Describe the action form?

Answer: A Java bean that is associated with single or multiple action mapping is called an action form. Action form objects are automatically populated at the server end when data has been entered from the client side through a user interface (UI).

Session states of a web application are maintained by action forms.

----

Q #27) Describe the Secure Socket Layer (SSL)?

Answer: The technology that is used to communicate between the web server and the web browser is called Secure Socket Layer (SSL). More specifically, SSL is a protocol that describes how algorithms are to be used in encryption.

The technology establishes an encrypted link between two parties and this link is allowed to secure transmission of sensitive information such as login credentials, credit/debit card information and social security numbers.

----

Q #28) What is id URL?

Answer: URL stands for Uniform Resource Locator and it is the textual reference writing standard to an arbitrary piece of data in the World Wide Web (www). The general structure of the URL is as follows:

protocol://host/local info

protocol – Protocol is for fetching the object (example: HTTP, FTP)
host – Internet name of the targeted host.
local info – String is passed to the protocol handler on the remote host. In many cases, it is a file name with an extension.

----

Q #29) What is URN?

Answer: URN stands for the Uniform Resource Name. It is a unique identifier that identifies an entity. But the information on where the entity is located is not available.

----

Q #30) What are the steps associated with the servlet life cycle?

Answer: The following steps are associated with the servlet life cycle:

Loading of the servlet class.
Instantiation of Servlet.
Execution of the init method.
Request handling phase. In this phase, service methods are called.
Removal from the service phase. In this phase, the destroy method is called.

----

Q #31) Is Servlet is pure java object or not?

Answer: Yes, Servlet is a pure java object.

----

Q #32) What is EJB?

Answer: EJB stands for Enterprise Java Beans. It is the server-side component that executes in EJB container and encapsulates the business logic for the enterprise application.

----

Q #33) What are the system services of the EJB container?

Answer: EJB Container provides the following system services:

Persistence
Security
Transaction
Connection pooling
Component lifecycle management
Threading

----

Q #34) What are the design principles for EJB?

Answer: Design principle includes:

The behavior of the EJB application is specified by interfaces.
EJB applications are loosely coupled and tired.
Implementation is hidden from the client-side.
The EJB container supports the application developer.
The API to the application is in session tier.
The API to the data sources is in the entity tier.

----

Q #35) What are the advantages of EJB components?

Answer: Advantages are:

There is support for the integration of components from different vendors.
Possibility to authorize the EJB component’s detailed knowledge of the environment.
Possibility to assemble applications from separate component sources.
Interaction with its clients is entirely specified in terms of Java interfaces.
Portability support.
It does not maintain resources.

----

Q #36) What are the Basic and subtypes of Enterprise Java Beans (EJB)?

Answer: Two main types and subtypes of EJB are as follows:

Session Beans
Stateful session beans
Stateless session beans
Entity Beans
Bean Managed Persistence (BMP)
Container-Managed Persistence (CMP)
Message Driven Beans

----

Q #37) What is the description of the expression element?

Answer: The expressions used for writing dynamic content back to the client browser are called expression elements.

----

Q #38) What are the two types of comments supported by JSP?

Answer: Two types of comments supported by JSP are:

HTML comment:
HTML comment

JSP comment.:
JSP comment

----

Q #39) What is called the JSP directive?

Answer: JSP directive is the mechanism to provide metadata information to web containers about the JSP file. In the translation and compilation phases of the JSP life cycle, this Metadata is used by the web container.

----

Q #40) What are the different types of JSP directive?

Answer: There are 3 different types of JSP directives available. These are:

Page directive
Include directive
Taglib directive

</https://www.softwaretestinghelp.com/j2ee-interview-questions-answers/>

<https://www.javatpoint.com/j2ee-interview-questions>

----

1) What do you understand by J2EE?
J2EE stands for Java 2 Enterprise Edition. The functionality of J2EE is developing and deploying multi-tier web-based enterprise applications. The J2EE platform is the combination of a set of services, application programming interfaces (APIs), and protocols. The J2EE platform adds the capabilities required to provide a complete, stable, secure, and fast Java platform at the enterprise level.

----

2) What do you mean by J2EE Module?
A J2EE module is a software unit that consists of one or more J2EE components for the same container type with one deployment descriptor of that type. Modules can be easily deployed or assembled into J2EE applications.

----

3) What are the four types of J2EE modules?
J2EE defines four types of modules:

Backward Skip 10s

Play Video

Forward Skip 10s


Application Client Module
WEB Module
Enterprise JavaBeans Module
Resource Adapter Module

----

4) What does the application client module contain?
Application client module contains the following:

Class files
Client deployment descriptor
It is packaged as JAR files with a .jar extension.

----

5) What does the web module contain?
The web module contains the following:

JSP (Java Server Pages) files
Class files for servlets
Web deployment descriptor
GIF (Graphics Interchange Format) and HTML (Hypertext Markup Language) files
These modules are packaged as JAR files with a .war (Web Archive) extension.

----

6) What does Enterprise JavaBeans module contain?
The Enterprise JavaBeans (EJB) module contains the following:

Class files for enterprise beans
An EJB deployment descriptor
These modules are packaged as JAR files with a .jar extension.

----

7) What does resource adapt module contain?
The resource adapter module contains the following:

Java interfaces
Classes
Native libraries
Other documentation
Resource Adapter deployment descriptor
These modules are packaged as JAR files with a .rar (Resource Adapter Archive) extension.


----

8) What are the main components of the J2EE application?
A J2EE component is assembled into a J2EE application with its related classes and files. It can also communicate with other components. The J2EE defines the following main components:

Application clients components.
Java Servlet and JavaServer Pages technology components.
Business Components (Enterprise JavaBeans).
Resource adaptor components.

----

9) What is considered as a web component?
Java Servlet and Java Server Pages technology components are considered as web components. Servlets are based on Java programming language which dynamically receives requests and generates responses. Java Server pages execute as servlets and allow a more natural approach to creating static content.

----

10) What are the types of J2EE clients?
Applets
Application clients
Java Web Start-enabled clients
Wireless clients

----

11) What do you understand by a word applet?
An applet is a J2EE component that typically executes in a web browser. It can also be executed in a variety of other applications or devices that support the applet programming model.

----

12) What is the container?
A container is the runtime support of a system level entity. Containers provide components with features such as lifecycle management, security, deployment, and threading.

----

13) What is an "applet container"?
A container that provides support for the applet programming model is known as "applet container."


----

14) What do you understand by a thin client?
A thin client is a light-weight interface to the application that does not support operations like query database, execute complex business rules, or connect to legacy applications.

----

15) What is JavaServer Faces (JSF)?
JavaServer Faces is a user interface (UI) designing framework which is used for Java-based web applications. JavaServer Faces provides a set of reusable UI components- a standard for web applications. JSF is based on the MVC design pattern. It automatically saves the form data to the server and populates the form dates when display on the client side.

----

16) What is an EJB platform?
EJB stands for The Enterprise JavaBeans. EJB platform manages functions such as transaction and state management, resource pooling, multithreading, and simple searches while you concentrate on writing business logic.

----

17) What do you mean by the deployment descriptor?
A deployment descriptor is based on XML (Extensible Markup Language) that supports .xml extension. It is used to describe a component's deployment settings. A J2EE application and its module, both have its deployment descriptor.

----

18) Define the Struts in the J2EE framework?
Struts is an application development framework based on MVC (Model-View-Controller) architecture. It is a combination of Java Servlets, JSP, Custom tags, and messages. It is used to design applications for large enterprises. It can be described as:

Model
The model defines the internal state of a system. It can be either single or a cluster of Java Beans based on app architecture.

View
JSP technology is used to design a view of any enterprise application.

Controller
A controller is used to manage the actions of users. It processes the client request and responds based on the request. The main component in the framework is a servlet of class ActionServlet. This servlet is configured by defining a set of ActionMappings.

----

19) Define Hashtable in J2EE?
Hashtable is similar to HashMap except that Hashtable is synchronized. Hashtable is a cluster of synchronized objects where null values and duplicate values are not allowed.

----

20) Define Hibernate and HQL?
Hibernate is an object-relational mapping and query service. In hibernate, we can write HQL (Hibernate Query Language) scripts instead of SQL, which saves lots of time and effort. Hibernate provides a more powerful association, inheritance, polymorphism, composition, and collections. We can process queries easily into the database using the Java objects. Hibernate also allows us to express queries using Java-based criteria.

----

21) What are the limitations of Hibernate?
Following are some limitations of hibernate:

Slower execution of queries.
Only HQL support is available for composite keys.
No shared references are available to the value type.

----

22) What are the major benefits of hibernate?
Following are some major benefits of hibernate:


Hibernate is independent of database and vendor so it is the portable framework.
Domain objects can be mapped to the relational database.
JPA support for standard ORM.
Better database connectivity in Hibernate when compared to JDBC.

----

23) Define ORM and its working in J2EE?
ORM refers to Object-Relational mapping. It is the object in a Java class which is mapped into the tables of a relational database using the metadata that describes the mapping between the objects and database. It transforms the data from one representation to another.

----

24) What is authorization?
An authorization is a process by which access to a method or resource is determined. It relies on the determination of whether the principal associated with a request through authentication is in a given security role. A security role can be explained as a logical grouping of users defined by the person who assembles the application. A deployer maps the security roles to security identities. Security identities may be principles or groups in the operational environment.

----

25) Define authorization constraint?
An authorization rule which determines who is permitted to access Web resource collection is known as authorization constraint.

----

26) How will you explain save() and saveorupdate() methods in hibernate?
The Save() method in hibernate is used to store an object in the database. It creates a new entry if the record doesn't exist.

The Saveorupdate() method in hibernate is used for updating the object using the identifier. If the identifier is unavailable, this method calls save(). If the identifier is available, it will call the update method.

----

27) How will you explain load() and get() methods?
Load(): If an object is missing in the Cache or database, Load() method will throw an exception. Load() method never returns null.

Get(): If an object is missing in the Cache or database, Get() method returns a null value, not the exception.

----

28) What is a web container in J2EE?
An interface between a component and the low-level platform with defined functionality that is designed to support the component is defined as the web container in J2EE.

----

29) What is the concept of connection pooling?
Connection pooling is a simple concept which is popular to reuse existing connections. It means that if object connections are already well-defined and connected, then they can be reused whenever there is a requirement instead of generating a new one.

----

30) What do you understand by the servlet?
Servlet is a server-side component which provides full functionalities to create a server-side program. There are different servlets available with a specific design for a variety of protocols. The most popular type of protocol for the servlet is HTTP.Servlets, which use the classes in the java packages javax.servlet, javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse, javax.servlet.http.HttpSession;. All servlets must include the Servlet interface, which defines life-cycle methods.

----

31) Give some advantages of ORM (object-relational mapping)?
Productivity
The automatic code is generated to reduce the overall data access time based on the data model defined.

Performance
The complete requirements of an application are managed by the automated code generated by the ORM, which means that there is no need for any extra code, and the overall data access process is made faster and optimized.

Vendor Independent
The generated code is independent of the vendor, which increases the overall portability of an application.
Maintainability
The code is well tested and generated by the ORM, and only a developer can understand the code perfectly.

----

32) Tell about the core interfaces of the hibernate framework?
Session Interface
SessionFactory Interface
Configuration Interface
Transaction Interface
Query and Criteria Interface

----

33) What is B2b?
B2b indicates to business-to-business.

----

34) What is the file extension used for hibernate mapping file and hibernate configuration file?
For hibernate mapping, the file name should be like filename.hbm.xml.

For hibernate configuration, the file name should be like hibernate.cfg.xml.

----

35) Define a way to add Hibernate mapping file in hibernate configuration file?
It can be easily performed by:

<mapping resource="filename.hbm.xml"/>  

----

36) What are the main components of multi-tier architecture?
The main components of multi-tier architecture are:

Presentation Tier
The front-end component existing in this tier is used to display the presentation.

Resource Tier
The back-end component existing in this tier is used to communicate with the database.

Business Tier
The component existing in this tier is used to provide business logic for the system.

----

37) Explain JTA, JNDI, and JMS.
JTA represents JAVA Transaction API, which is used for coordinating and managing transactions across the enterprise information system.

JNDI represents Java Naming Directory Interface, which is used for accessing data from directory services.

JMS represents the Java Messaging Service, which is used for receiving and sending messages through messaging systems.

----

38) Explain the J2EE tiers.
J2EE has the following tiers:

Client Tier
It indicates to the browser from which request is processed to the server. The interfaces that are available in this tier are HTML browser, Java application, an applet, or a non-java application.


Middle Tier
It comprises of a presentation tier and integration tier. The UI (User Interface) is created in the presentation tier using JavaServer Pages. The business logic is written inside the business tier with the help of Enterprise Java Bean. The objects of the database are created in the integration tier.

Backend
It constitutes the Enterprise Information System (EIS) which is used to store the data.

----

39) Describe the EAR, WAR, and JAR.
EAR stands for Enterprise Archive file. It consists of the components of the web, EJB, and client. All the components of the EAR are packed in a compressed file with the extension .ear.

WAR stands for a Web Archive file. It consists of all the components related to the web application. All the components are packed in a compressed file with the extension .war.

JAR stands for Java Archive file. It consists of all the class files and library files, which constitute an API (Application Programming Interface). All the components are packed in a compressed file with the extension .jar.

Each type of file (.ear, .war, and .jar) is processed uniquely by application servers, servlet containers, EJB containers, etc.

----

40) What do you understand by Spring?
Spring is a light-weight open source framework for developing enterprise applications. It resolves the complexity of enterprise application development and provides easy development for the J2EE. It was initially written by Rod Johnson. It was released under the Apache 2.0 license in June 2003.

----

41) What are the different modules used in Spring?
There are mainly seven core modules in spring:

The Core container module
Object/Relational mapping module
DAO module
Application context module
Aspect Oriented Programming
Web module
MVC module

----

42) What is action mapping?
In action mapping, a user specifies action class for a particular URL, i.e., path and different target view, which means, forwards on to which request-response is forwarded. The ActionMapping defines the information that the ActionServlet knows about the mapping of a particular request to an instance of a specific Action class. The mapping is transferred to the execute() method of the Action class, enabling access to this information directly.

----

43) What do you understand by ActionForm?
ActionForm is a Java bean which may associate one or more ActionMappings. A java bean changes to FormBean when a user extends a class org.apache.struts.action.ActionForm. ActionForm object is generally populated on the server side automatically, and the client enters data from UI. ActionForm manages the session state for a web application.

----

44) What is backing bean?
A backing bean is a JavaBeans component which corresponds to JavaServer Pages that includes JavaServer Faces components. The backing bean describes the properties for the components on the page and methods which perform processing for the component.

This processing may include event handling, validation, and processing associated with navigation.

----

45) What is the build file?
A build file is an XML file that consists of one or more asant targets. A target is a set of tasks that a user wants to get executed. When starting asant, a user can select which target is to be executed. If there is no target, then the default target of the project is executed.

----

46) What do you understand by business logic?
Business logic is the code that includes the functionality of an application. In the EJB (Enterprise JavaBeans) architecture, this logic is implemented by the methods of an enterprise bean.

----

47) How will you explain CDATA?
A CDATA is a predefined XML tag for the character data, which means "don't interpret these characters," it is similar to parsed character data (PCDATA), in which the standard rules of XML syntax apply. CDATA sections are used to show examples of XML syntax.

----

48) What do you mean by the Component Contract?
The contract between the J2EE component and its container is known as the component contract. This type of contract includes:

Life-cycle management of the component
An interface which is used by instance to obtain various information and services from its container
List of services that every container must provide for its components.

----

49) What do you understand by Connector? Explain Connector Architecture.
A connector is a standard extension mechanism for containers, which provides connectivity to enterprise information systems. It is specific to an enterprise information system and contains a resource adapter and application development tools for enterprise information system connectivity. The resource adapter is plugged into a container through its support for system-level contracts, defined in the Connector architecture.

An architecture for the integration of J2EE products with enterprise information systems is known as the connector architecture. A connector architecture consists of:

A resource adapter which is given by an enterprise information system vendor
A J2EE product that allows this resource adapter to plug in.
Connector architecture also defines a set of contracts which a resource adapter must support to plug into a J2EE product (e.g., transactions, security, and resource management).

</https://www.javatpoint.com/j2ee-interview-questions>

<https://www.interviewkickstart.com/interview-questions/java-and-j2ee-interview-questions>

----

Q1. What’s the difference between JVM Spec, JVM Runtime, and JVM Implementation?
JVM spec is simply the specification of JVM. JVM implementation is the actual implementation of JVM by vendors. Meanwhile, JVM runtime is a running program supporting Java specified programs.

----

Q2. What is JIT?
The Just-in-Time compiler improves the performance of Java apps by combining platform-neutral bytecode to the native machine code during run time.

----

Q3. What are JRE and JDK?
JDK is a kit providing an environment to execute and develop the Java program. On the other hand, JRE is a kit that provides an environment to run (not develop) the Java program.

----

Q4. Define Locale.
A locale object shows a specific political, cultural, or geographical region. An operation that requires locale is called locale-sensitive.

Apart from these, do prepare for the below Java and J2EE interview questions as well:

What is a ResourceBundle class?
Can you force a garbage collector? How does it decide which objects need to be removed?
How can you obtain platform-dependent values, such as path separator or line separator?
Mention the methods in the object.
What is the final keyword denoting w.r.t. class, variable, and method?
Are you able to instantiate math class?
Can you declare the main method as final?
Mention the difference between getclass and instanceof. Are they the same or not?
Do you know whether Java provides any construct to determine an object’s size?
Define native method.
Is it okay for a Java file to have more than one Java class?
Is an empty Java file a valid source?
Mention the difference between a parameter and an argument.
Mention the various scopes for Java variables.
Define wrapper classes.
The interviewer also includes a few advanced-level Java and J2EE interview questions during a typical Java interview. You must take these questions seriously and prepare for them accordingly.

Advanced Java and J2EE Interview Questions
Mentioned below are a few advanced level Java and J2EE programming interview questions for senior software developers:

----

Q1. Define HQL.
HQL (Hibernate Query Language) is an object-oriented query language. Unlike SQL, which works on tables and columns, HQL works on persistent objects and properties. HQL is a superset of Java Persistence Query Language (JPQL). This means that all JPQL queries are valid HQL queries, but all HQL queries are not JPQL queries

----

Q2. What is a Java thin client?
Thin client is a lightweight client. A thin client connects to the cluster through a standard socket connection without becoming a part of the cluster topology. Thin client does not hold any data and is not used for computing calculations. It performs all operations through the standard node​.

----

Q3. What does URN mean?
URN is an abbreviation for Uniform Resource Name. It is a unique identifier that identifies an entity. 

----

Q4. What are the uses of Spring?
Spring is an open-source application development framework for enterprise Java. It is one of the most widely used frameworks for Java. Developers use Spring to develop high-performing, testable, and reusable code

----

Q5. What are the different phases that fall under the life cycle of a servlet?
Request handling, Servlet installation, The init method, Servlet class loading, and Removal from the service.

Here are a few other Java and J2EE interview questions for experienced professionals:

What must servlets execute?
Do you know whether servlet is pure Java or not?
Mention the method to create objects without using ‘new’ in Java.
Mention the scope of default in spring.
What are the components of the J2EE app?
Mention the types of j2EE clients.
Define JSF.
What is a Hash table?
Define hibernate.
What is the difference between saveorupdate and save?
Define ORM and mention a few of its benefits.
What is the difference between the get and load method?
Mention the core interfaces of hibernate framework.
What file extension will you use for mapping a hibernate file?
Mention the difference between .jar, .war, and .ear files.
Read our Top Advanced Java Interview Questions for your coding interview.

Java and J2EE Interview Questions on Design Patterns
Here are some design patterns for Java and J2EE interview questions:

----

Q1. What are the different components in the multi-tier architecture?
The presentation tier, Resource tier, and Business tier are the components of multi-tier architecture.

----

Q2. What are the different modules in Spring?
The list of spring modules is

Aspect-oriented programming
DAO module
O/R mapping module
Core container module
Web module
Application context module.

----

Q3. What is a servlet?
A servlet is a server-side component that provides development mechanisms for server-side programs. It makes use of classes available under a Java package.

----

Q4. Define the various phases in the life cycle of a servlet.
The different phases are:

Servlet instantiation
Servlet class loading
The init method
Removal from the service
Request handling
Q5. Define JMS, JNDI, and JTA.
JNDI: It is Java Naming Directory Interface. It helps access information from the directory services.
JMS: It is a Java Messaging Service. It is responsible for receiving and sending messages through various messaging systems.
JTA: It is a Java Transaction API. It coordinates and manages the transaction in an enterprise information system.
You can also go through the following Java and J2EE technical architect interview questions:

Explain the terms - EDI and EAI.
What are the roles of third-party software in the EJB framework?
Explain the difference between load and get.
What are the benefits of using spring for developing applications?
Mention the different types of JSP tags.
Briefly define SSL or secure socket layer.
What does EJB mean? Mention the subtypes and basics of the same.
What does the JSP directive mean? Mention the different types of JSP directives.
These Java and J2EE interview questions will assist aspiring architects in their upcoming tech interview prep. You can also take a look at some of the Top Java Programming Interview Questions and Answers.

Miscellaneous Java and J2EE Interview Questions
Apart from the above-mentioned questions, the following miscellaneous Java and J2EE interview questions might be asked by an interviewer:

----

Q1. What is connection pooling?
Connection pooling is a practice generally used to extract already existing connections. These connections can be used instead of generating new connections.

----

Q2. Define hibernate proxy.
It is an object proxy that includes the process of retrieving the objects until and unless you require them.

----

Q3. How will you create a SessionFactory?
Configuration cfg = new Configuration(); cfg.addResource("dir/hibernate.hbm.xml"); cfg.setProperties( System.getProperties() ); SessionFactory sessions = cfg.buildSessionFactory();

----

Q4. Mention the collection types in hibernate.
List, array, map, bag, set are the collection types in hibernate.

----

Q5. Mention the JSP tag types.
JSP tags are divided into four categories:

Declarations
Directives
Expressions
Scriptlets
Go through the following additional miscellaneous Java and J2EE interview questions:

How can you access web.xml parameters from the JSP page?
What is the EAR file?
Define JSP Directives.
Define ActionErrors.
What are struts?
What is action mapping?
Define ActionForm.
What are the different spring modules?
Define Bean Factory. Have you used it before?
Define MCV on struts.
What does authorization constraint and authorization mean?
What is the difference between savings and update or save?
Define design objectives of the J2EE architecture.
What are the core design goals of J2EE architecture?
What is the role of a J2EE architect?
That said, brushing up your overall skills related to Java and J2EE interview questions is of paramount importance and can help you secure your dream job in Tier-1 tech companies. You can practice some Java Interview Questions for Software Developers With 5 Years of Experience too.

----

FAQs on Java and J2EE Interview Questions 
Q1. How much does a Java developer earn in the US?

The average annual salary of a Java developer is around $106,019 in the US.

----

Q2. What is the minimum eligibility to become a Java developer?

Becoming a Java developer requires a Bachelor’s degree in Computer Science or any related field. However, experience is equally important to appear for Java and J2EE interview questions.

----

Q3. Are Java and J2EE the same?

Before appearing for Java and J2EE interview questions, you should have a common understanding of the difference between both these programming languages. J2EE is just an extension of Java SE, which is based on the Java programming language. In simple words, J2EE is a part of Java featuring a powerful library set.

----

Q4. What are the four types of J2EE modules?

The four types of J2EE modules are Application Client Module, WEB Module, Enterprise JavaBeans Module, and Resource Adapter Module.

----

Q5. What is J2EE?

J2EE stands for Java 2 Platform, Enterprise Edition. The J2EE platform is used to create multi-tier, web-based applications by utilizing a set of protocols and application programming interfaces (APIs).

</https://www.interviewkickstart.com/interview-questions/java-and-j2ee-interview-questions>

<https://career.guru99.com/top-50-j2ee-interview-questions/>

----

1) What is J2EE?
J2EE means Java 2 Enterprise Edition. The functionality of J2EE is developing multitier web-based applications. The J2EE platform is consists of a set of services, application programming interfaces (APIs), and protocols.

----

2) What are the four components of J2EE application?
Application clients components.
Servlet and JSP technology are web components.
Business components (JavaBeans).
Resource adapter components

----

3) What are types of J2EE clients?
Applets
Application clients
Java Web Start-enabled clients, by Java Web Start technology.
Wireless clients, based on MIDP technology.
The video player is currently playing an ad. You can skip the ad in 5 sec with a mouse or keyboard

----

4) What is considered as a web component?
Java Servlet and Java Server Pages technology components are web components. Servlets are Java programming language that dynamically receives requests and makes responses. JSP pages execute as servlets but allow a more natural approach to creating static content.

----

5) What is JSF?
JavaServer Faces (JSF) is a user interface (UI) designing framework for Java web applications. JSF provides a set of reusable UI components, a standard for web applications. JSF is based on MVC design pattern. It automatically saves the form data to the server and populates the form date when display on the client side.

J2EE Interview Questions and Answers
J2EE Interview Questions and Answers

----

6) Define Hash table
HashTable is just like Hash Map, Collection having a key(Unique), value pairs. Hashtable is a collection Synchronized object. It does not allow duplicate values or null values.

----

7) What is Hibernate?
Hibernate is an open source object-relational mapping and query service. In hibernate we can write HQL instead of SQL which save developers to spend more time on writing the native SQL.

Hibernate has a more powerful association, inheritance, polymorphism, composition, and collections. It is a beautiful approach for persisting into the database using the Java objects. Hibernate also allows you to express queries using Java-based criteria.

----

8) What is the limitation of hibernate?
Slower in executing the queries than queries are used directly.
Only query language support for composite keys.
No shared references to value types.

----

9) What are the advantages of hibernate?
 Hibernate is portable i mean database independent, Vendor independence.
 Standard ORM also supports JPA
 Mapping of the Domain object to the relational database.
 Hibernate is better than plain JDBC.
 JPA provider in JPA based applications.
10) What is ORM?
Java 2 Platform Enterprise Edition (J2EE)
Java 2 Platform Enterprise Edition (J2EE)
ORM stands for Object-Relational mapping. The objects in a Java class which is mapped into the tables of a relational database using the metadata that describes the mapping between the objects and the database. It works by transforming the data from one representation to another.

----

11) Difference between save and saveorupdate
save() – This method in Hibernate is used to stores an object in the database. It inserts an entry if the record doesn’t exist, otherwise not.
saveorupdate () -This method in the hibernate is used for updating the object using identifier. If the identifier is missing this method calls save(). If the identifier exists, it will call update method.

----

12) Difference between load and get method?
load() can’t find the object from cache or database, an exception is thrown, and the load() method never returns null.
get() method returns null if the object can’t be found. The load() method may return a proxy instead of a real persistent instance get() never returns a proxy.

----

13) How to invoke a stored procedure in hibernate?
{ ? = call thisISTheProcedure() }

----

14) What are the benefits of ORM?
Productivity
Maintainability
Performance
Vendor independence

----

15) What are the Core interfaces of Hibernate framework?
Session Interface
SessionFactory Interface
Configuration Interface
Transaction Interface
Query and Criteria Interface

----

16) What is the file extension used for hibernate mapping file?
The name of the file should be like this: filename.hbm.xml

----

17) What is the file name of hibernate configuration file?
The name of the file should be like this: hibernate.cfg.xml

----

18) How Hibernate is database independent explain?
Only changing the full property full database can be replaced.

<property name="hibernate.dialect">org.hibernate.dialect.Oracle9Dialect</property> and

<property name="hibernate.connection.driver_class">oracle.jdbc.driver.OracleDriver</property>

----

19) How to add Hibernate mapping file in hibernate configuration file?
By <mapping resource=” filename.hbm.xml”/>

----

20) Define connection pooling?
Connection pooling is a mechanism reuse the connection which contains the number of already created object connection. So whenever it is necessary for an object, this mechanism is used to get objects without creating it.

----

21) What is the Hibernate proxy?
An object proxy is just a way to avoid retrieving an object until you need it. Hibernate 2 does not proxy objects by default.

----

22) What do you create a SessionFactory?
Configuration cfg = new Configuration(); cfg.addResource("dir/hibernate.hbm.xml"); cfg.setProperties( System.getProperties() ); SessionFactory sessions = cfg.buildSessionFactory();

----

23) What is HQL?
HQL stands for Hibernate Query Language. Hibernate allows to the user to express queries in its portable SQL extension, and this is called as HQL. It also allows the user to express in native SQL.

----

24) What are the Collection types in Hibernate?
Set, List, Array, Map, Bag are collection type in Hibernate.

----

25) What is a thin client?
A thin client is a program interface to the application that does not have any operations like the query of databases, execute complex business rules, or connect to legacy applications.

----

26) Differentiate between .ear,  .jar and .war files.
.jar files: These files are with the .jar extension. The .jar files contain the libraries, resources and accessories files like property files.
.war files: These files are with the .war extension. The .war file contains JSP, HTML, javascript and other files necessary for the development of web applications.
.ear files: The .ear file contains the EJB modules of the application.

----

27) What is the JSP tag?
In JSP tags can be divided into four different types.

Directives
Declarations
Scriplets
Expressions

----

28) How to access web.xml init parameters from JSP page?
For example, if you have:
<context-param> <param-name>Id</param-name> <param-value>this is the value</param-value></context-param>
You can access this parameter

Id: <h:outputText value="#{initParam['Id']}"/>

----

29) What are JSP Directives?
1.page Directives <%@page language=”java” %>
2. include Directives: <%@ include file=”/header.jsp” %>
3. taglib Directives <%@ taglib uri=”tlds/taglib.tld” prefix=”html” %>

----

30) What is the EAR file?
An EAR file is a JAR file with an .ear extension. A J2EE application with all of its modules is delivered in an EAR file.

----

31) What will happen when you compile and run the following code?
public class MyClass { public static void main(String argv[]){ int array[]=new int[]{1,2,3}; System.out.println(array [1]); } } Answer: Compiled and shows output : 2

----

32) What are Struts?
Struts framework is a Model-View-Controller(MVC) architecture for designing large-scale applications. It is a combination of Java Servlets, JSP, Custom tags, and message. Struts help you to create an extensible development environment for your application, based on published standards and proven design patterns. Model in many applications represents the internal state of the system as a set of one or more JavaBeans.The View is most often constructed using JavaServer Pages (JSP) technology.The Controller is focused on receiving requests from the client and producing the next phase of the user interface to an appropriate View component. The primary component of the Controller in the framework is a servlet of class ActionServlet. This servlet is configured by defining a set of ActionMappings.

----

33) What is ActionErrors?
ActionErrors object that encapsulates any validation errors that have been found. If no errors are found, return null or an ActionErrors object with no recorded error messages.The default implementation attempts to forward to the HTTP version of this method. Holding request parameters  mapping and request  and returns set of validation errors, if validation failed; an empty set or null

----

34) What is ActionForm?
ActionForm is a Java bean that associates one or more ActionMappings. A java bean become FormBean when extend org.apache.struts.action.ActionForm class. ActionForm object is automatically populated on the server side which data has been entered by the client from UI. ActionForm maintains the session state for a web application.

----

35) What is action mapping??
In action mapping, we specify action class for particular URL ie path and different target view ie forwards on to which request response will be forwarded.The ActionMapping represents the information that the ActionServlet knows about the mapping of a particular request to an instance of a particular Action class. The mapping is passed to the execute() method of the Action class, enabling access to this information directly.

----

36) What is the MVC on struts?
MVC stands Model-View-Controller.

Model: Model in many applications represent the internal state of the system as a set of one or more JavaBeans.

View: The View is most often constructed using JavaServer Pages (JSP) technology.

Controller: The Controller is focused on receiving requests from the client and producing the next phase of the user interface to an appropriate View component. The primary component of the Controller in the framework is a servlet of class ActionServlet. This servlet is configured by defining a set of ActionMappings.

----

37) What are different modules in spring?
There are seven core modules in spring

The Core container module
O/R mapping module (Object/Relational)
DAO module
Application context module
Aspect Oriented Programming
Web module
MVC module

----

38) What is Bean Factory, have you used XMLBean factory?
XmlBeanFactory is one of the implementation of bean Factory org.springframework.beans.factory.xml.XmlBeanFactory is used to creat bean instance defined in our xml file. BeanFactory factory = new XmlBeanFactory(new FileInputStream("beans.xml")); Or ClassPathResource resorce = new ClassPathResource("beans.xml"); XmlBeanFactory factory = new XmlBeanFactory(resorce);

----

39) What is Spring?
Spring is a lightweight open source framework for the development of enterprise application that resolves the complexity of enterprise application development is also providing a cohesive framework for J2EE application development which is primarily based on IOC (inversion of control) or DI (dependency injection) design pattern.

----

40) What is the functionality of ActionServlet and RequestProcessor?
Receiving the HttpServletRequest
Populating JavaBean from the request parameters
Displaying response on the web page Issues
Content type issues handling
Provide extension points

----

41) ActionServlet, RequestProcessor, and Action classes are the components of
Controller

----

42) What is default scope in Spring?
Singleton.

----

43) What are advantages of Spring usage?
Pojo based programming enables reuse component.
Improve productivity and subsequently reduce development cost.
Dependency Injection can be used to improve testability.
Spring required enterprise services without a need for the expensive application server.
It reduces coupling in code and improves maintainability.

----

44) What are the Benefits Spring Framework?
Lightweight container
Spring can effectively organize your middle tier objects
Initialization of properties is easy. No need to read from a properties file
application code is much easier to unit test
Objects are created Lazily, Singleton – configuration
Spring’s configuration management services can be used in any architectural layer, in whatever runtime environment

----

45) Lifecycle interfaces in spring?
1) InitializingBean <bean id="expInitBean" init-method="init"/> public class ExpBean { public void init() { // do some initialization code } } OR <bean id=" expInitBean "/> public class ExpBean implements InitializingBean { public void afterPropertiesSet() { // do some initialization code } } 2) DisposableBean <bean id="expInitBean" destroy-method="cleanup"/> public class ExpBean { public void cleanup() { // do some destruction code (like releasing pooled connections) } } OR <bean id="expInitBean"/> public class ExpBean implements DisposableBean { public void destroy() { // do some destruction code (like releasing pooled connections) } }

----

46) How to Create Object without using the keyword “new” in java?
Without new, the Factory methods are used to create objects for a class. For example
Calender c=Calender.getInstance();
Here Calender is a class, and the method getInstance() is a Factory method which can create an object for Calendar class.

----

47) What is a servlet?
Servlets is a server-side component that provides a powerful mechanism for developing server side programs. Servlets is a server, as well as platform-independent and Servlets, are designed for various protocols. Most commonly used HTTP protocols. Servlets use the classes in the java packages javax.servlet, javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse, javax.servlet.http.HttpSession;. All servlets must implement the Servlet interface, which defines life-cycle methods.

----

48) Servlet is pure java object or not?
Yes, pure java object.

----

49) What are the phases of the servlet life cycle?
The life cycle of a servlet consists of the following phases:

Servlet class loading
Servlet instantiation
 the init method
Request handling (call the service method)
Removal from service (call the destroy method)

</https://career.guru99.com/top-50-j2ee-interview-questions/>

<https://www.simplilearn.com/j2ee-interview-questions-answers-article>

1. What is J2EE?
J2EE, or Java Enterprise Edition, is a Java-based platform that combines services protocols with APIs (Application Programming Interfaces), giving users the ability to create enterprise-level applications that are multi-tiered, safe, stable, and quick. J2EE offers a variety of specifications for creating enterprise-level online applications, including web, enterprise, web service, and others.

----

2. What are the benefits of J2EE?
Given below are the benefits of J2EE:

Faster time to market: J2EE employs the idea of containers to make development simpler. This supports the separation of business logic from lifecycle management and resources, allowing developers to concentrate more on the business logic than the infrastructure. The EJB (Enterprise JavaBeans) container, for example, handles threading, distributed communication, transaction management, scaling, etc. and offers the developers the necessary abstraction.
Support for Web Series: A platform for creating and deploying web services is offered by J2EE. The Java API for XML-based Remote Procedure Call, or JAX-RPC, assists programmers in creating SOAP-based web services, clients, and endpoints that are portable and interoperable.
Compatibility: The "Write Once, Run Anywhere" guiding philosophy is used by the J2EE platform. It offers thorough standards and APIs that guarantee interoperability between various application providers and, as a result, the portability of programmes.
Simplified Connectivity: J2EE facilitates applications' connectivity, enabling the use of various devices' capabilities. Additionally, it offers JMS (Java Message Service) for asynchronous, loosely linked application integration. Additionally, it offers support for CORBA (Common Object Request Broker Architecture), which enables close system integration through remote calls.

----

3. Name various components of J2EE application architecture.
J2EE is made up of 3 main components (tiers) - Client tier, Middle tier, Enterprise data tier:

Client Tier: Programs and apps in this tier typically run on machines other than the server and interact with users. Different user inputs are taken in this instance, and the requests are submitted to the server for processing before being returned to the client with the result.
Middle Tier: Web components and EJB containers make up this tier. The web components that process the request and produce the response are either servlet or JSP pages. Static HTML codes, programmes, and applets from the client are packed with the server's components when the application is put together, along with the web components. The Enterprise Bean, which is running on the business tier, needs the EJB components to handle input from the user.
Enterprise Data Tier: Database servers, resource management programmes, and several other data sources are included in this tier and are accessible by various business tier components via a separate workstation. This tier makes use of technologies like JPA, JDBC, Java transaction API, Java Connector Architecture, etc.

----

4. What are the different technologies provided to the J2EE platform?
Given below are the important technologies provided to J2EE platform:

Java Server Pages (JSP): Delivering XML and HTML documents makes use of this. In addition to these, we may use other sorts of data using OutputStream.
Java API for XML Based RPC (JAX-RPC): This is used to create web applications and clients that employ Remote Procedure Calls and XML.
Java Servlets: The request-response approach can be used to access applications hosted by servers, which are extended by classes known as servlets.
Enterprise Java Beans: This is a server-side component that provides runtime environment, security, servlet lifecycle management, transaction management, and other services in order to encapsulate the business logic of the application.
J2EE Deployment API: It offers specifications for web services deployment.
J2EE Connector Architecture: This establishes a common framework for linking J2EE platforms with other EIS (Enterprise Information Systems), including mainframe operations, database systems, and many legacy applications written in other languages.
J2EE Authorization Contract for Containers: This is used to specify security agreements between application servers and authorization policy modules.
Java Management Extensions (JMX): They are used to provide tools for managing and monitoring networks, objects, devices, and applications.
Java API for XML Registries: This gives users a consistent API to access several XML Registries, enabling the infrastructure needed to create and deploy web services.
Java Message Service (JMS): This messaging standard enables distributed, loosely coupled, asynchronous, and reliable communication across various J2EE components so that they can create, send, receive, and read messages.
Java Transaction API (JTA): This is used to specify the Java standard interfaces for managers and transaction systems.
Java Naming and Directory Interface (JNDI): For Java-based applications, this API offers name and directory functionality.
JDBC Data Access API: This offers APIs for obtaining data from several data sources, including relational databases, flat files, and spreadsheets.
Common Object Request Broker Architecture (CORBA): In order to facilitate system communication implemented on many platforms, this standard for establishing Object Management Groups is provided.
Get Access to 200+ Hiring Partners in Our Bootcamp
Full Stack Java Developer Career BootcampEXPLORE COURSEGet Access to 200+ Hiring Partners in Our Bootcamp

----

5. How is JDK different from JIT?
A cross-platform software development environment called JDK (Java Development Kit) provides diverse collections of libraries and tools needed to create Java programmes and applets. It also includes JRE, which offers tools and libraries that support the execution of byte code. JDK is required for creating and executing Java programmes. while JIT refers to the Just In Time Compiler, a module found inside the JVM (which is inside JRE). For the purpose of reducing compilation time and improving speed, JIT compilers are used to compile some portions of byte code that perform similarly to machine code simultaneously.

----

6. What do you understand by build file?
A build file is used to automate numerous software development processes. The build file additionally specifies the versions of libraries that must be included in addition to this. The kinds of optimizations needed for the project are also included. When the project size grows, build offers a standardized method for building the project.

----

7. How are CLASSPATH and PATH different from each other in terms of J2EE?
Key environmental variables utilized by Java systems include PATH and CLASSPATH.

Whether Java is installed on the system or not has no bearing on PATH, a system-level variable. While JVM uses CLASSPATH, which is entirely Java-specific, to load the classes needed by running Java programmes.
The JDK binaries or native libraries like java.exe are referenced by the PATH variable. In contrast, the CLASSPATH variable directs users to Java binaries, such as bytecode-filled JAR files.

----

8. How is a multi tier client server architectural model advantageous?
The tiers that make up a multi-tier client-server architectural model all communicate with one another. The three-tier application paradigm shown below shows how the client/presentation, business logic, and database tiers interact with one another to handle requests and provide responses:

The user interface and business logic can both be altered independently.
Each tier may be individually coded or designed. Java or Python, for instance, can be used to code the intermediate tier, while Angular or React can be used to code the client tier, etc.
Between the components, abstraction is introduced. As an illustration, the client tier can access data without being aware of the origin of the response, the server infrastructure in the backend, etc.
Instead of needing to create a new connection for each user, the database may feature pooled connections that allow users to share data.

----

9. Why do we have JNDI and JDBC in J2EE?
JDBC, or Java Database Connectivity, offers instructions and APIs for establishing connections to databases from many vendors, including MySQL, Oracle, PostgreSQL, etc., in order to obtain data. Without knowing the precise host address or port, JNDI (Java Naming and Directory Interface) assists in creating a logical framework to access a resource from the database, EJB beans, messaging queues, etc. After registering a resource with JNDI, application components can subsequently be accessed by using the JNDI name.

----

10. What are the J2EE aplets? Why can we use it?
Applets are Java-based J2EE client components that run in a web browser or on a number of other platforms that support the applet development model. They assist in providing small, portable embedded Java programmes in HTML pages that will be run automatically when we browse the pages and are used to provide interactive capabilities to online apps.

----

11. What is EJB? How can you use it in J2EE?
One of the most crucial components of the J2EE platform, EJB, or Enterprise Java Beans, enables the creation and deployment of enterprise-level multi-tiered applications while keeping performance, scalability, and robustness in mind. When we wish to accomplish the following, we can utilize EJBs:

Clustering: EJBs can be utilized for the application's deployment in a cluster environment to provide high availability and fault tolerance.
Concurrency without using Threads: Due to the fact that EJBs are available in the EJB container and are instantiated using the object pool, concurrency can be achieved without the usage of actual threads. This aids in achieving performance without engaging Threads-related complexity.
Full Stack Web Developer Course
To become an expert in MEAN StackVIEW COURSEFull Stack Web Developer Course

----

12. What is the architecture model of Struts?
Strut is an application development framework for creating enterprise-level applications that combines JSP, Java Servlets, messages, and custom tags. MVC (Model-View-Controller) architecture is the foundation of it.

View: JSP technology is used by Struts to develop views for enterprise-level applications.
Model: The internal system state is defined by this component. Depending on the architecture of the application, it could either be a Java Beans cluster or a single bean.
Controller:It manages user actions that process requests and give answers to them. It is a servlet.

----

13. What is ORM?
By leveraging metadata that describes the relationship between the database and the objects, object-relational mapping, or ORM, converts Java class objects to tables in relational databases and vice versa.

----

14. What constitutes web components?
Web components are made up of Java Servlets and Java Server Pages (JSP) elements. Java Servlets process requests and responses on the fly. Servlets that enable a natural method to create static content are executed through JSP pages.

----

15. What is EJB platform?
The Enterprise JavaBeans are referred to as EJBs. While you focus on building business logic, the EJB platform handles tasks like transaction and state management, resource pooling, multithreading, and simple searches.

----

16. What is JSF?
JSF, or Java Server Faces, is a web framework designed to make the creation of user interfaces more straightforward. It is a common display solution for web applications with a Java foundation. It offers reusable UI components and is built on the MVC (Model-View-Controller) pattern.

----

17. What factors should a J2EE application possess for operating in a global economy?
The following are the factors that a J2EE application possess for operating in a global economy:

Language Requirements: For a wider user base, a programme should support the national language as well as regional ones.
Financial Consideration: Depending on the government, every nation has its own taxes, regulations, and tariffs. When creating a J2EE application, all of these elements should be taken into account.
Legal Differences: Every government has its own set of customary laws, privacy laws, and demands for every nation. A designed application must abide by all applicable laws.

----

18. What are Connectors? Describe the Connector Architecture.
Connectors are used to offer connectivity to various enterprise information systems through standard extension protocols. Resource adapters and system-level contracts, both of which are unique to enterprise information systems, make up a connector architecture. Plugging the resource adapters into the container. For a resource adapter to be plugged into J2EE applications, it must satisfy certain contracts that the connector architecture prescribes, such as security, transaction, resource management, etc.

----

19. What are the design goals of J2EE architecture?
The following are the design goals of J2EE architecture:

User Interaction: The user experience should be smooth and connect to a variety of devices, including computers, mobile phones, laptops, etc.
Data Connectivity: A J2EE application's link to legacy systems needs to be stable enough to support business operations.
Service Availability: To guarantee that the application is accessible around-the-clock in order to meet necessary business objectives.
Ease of Accessibility: Applications should be accessible to users from any location and on any device.
Abstraction and Flexibility: The server should handle the configuration details while the developer should concentrate on the business logic.
New Course: Full Stack Development for Beginners
Learn Git Command, Angular, NodeJS, Maven & MoreENROLL NOWNew Course: Full Stack Development for Beginners

----

20. What is JRMP?
JRMP, or Java Remote Method Protocol, is a tool used for Remote Method Invocation (RMI), which allows Java objects to be passed as arguments. When moving items from one JVM to another using object serialization, RMI uses this underlying protocol to marshal objects as a stream.

----

21. How is 32-bit JVM different from 64-bit JVM?
In contrast to 32-bit operating systems, 64-bit operating systems use the 64-bit JVM. As opposed to the 4G limit of 32-bit JVM, we can select higher heap size memory in 64-bit JVM up to 100G. When running in a 64-bit JVM, Java programmes consume more memory than when running in a 32-bit JVM. The Ordinary Object Pointer's larger size is to blame for this. However, this can be avoided by instructing the JVM to utilize 32-bit pointers by using the -XXCompressedOOP option. In contrast to the 32-bit JVM, which utilizes 8-byte headers and a maximum of 4-byte internal references, the 64-bit JVM employs 12-byte object headers and a maximum of 8-byte internal references.

----

22. What is the purpose of heap dumps and how do you analyze a heap dump?
Heap dumps are a snapshot of all active objects being used by active Java programmes on the Java heap memory. The heap dump contains comprehensive information for each item, including type, class name, address, size, and relationships to other objects. Numerous tools are useful when examining Java heap dumps. For instance, JDK itself offers the jhat tool for heap dump analysis. Heap dumps are also used for memory leak analysis. Memory leaks are a phenomenon that happens when there are objects that are no longer needed by the application but are still represented as referenced objects by the garbage collection, making it impossible to free that memory. Following are the causes that result in memory leaks:

Constantly creating new instances of objects without relinquishing them.
Open connection objects, such as database connections, post the necessary operation.
Static variables preserving object references.
Adding objects to a hashmap without modifying the equals() method of the hash code. If these techniques are left out, the hashmap will continue to expand while taking duplicates into account.
Infinite caches.
Techniques that are uninvoked by listeners.
As a result, the application keeps using more and more memory, which finally causes OutOfMemory Errors and can cause the application to crash. To find memory leaks in heap dumps, we can analyze the data using the visualVM for Eclipse Memory Analyzer tools.

----

23. What are EAR, WAR, and JAR?
Enterprise Archive File, or EAR, is a compressed and packaged file that contains client, EJB, and web components. Its extension is.ear. We can deploy many modules simultaneously to the application server using EAR files.

The term "WAR" refers to a file that contains all web components that have been compressed and packaged together. This file makes it simple to test and deploy web apps with just one request.

Java Archive file is referred to as a JAR. It includes all of the class files and libraries that make up APIs. The.jar file contains these compressed and packaged together. These are employed for the single-request deployment of the full application, including classes and resources.

----

24. What is Spring?
A lightweight open source framework for creating enterprise apps is called Spring. It solves the enterprise application development complexity and offers simple J2EE development. Rod Johnson was the author of the original draught. In June 2003, it was made available under the Apache 2.0 license.

----

25. What is Hibernate?
Hibernate is a Java-based Object Relational Mapper technology that offers an abstraction layer for accessing or changing database data. The developer should not worry about how the connections to the databases are formed, how the data translation from Java application to Database and vice versa occurs because it handles all implementations inside. Strong object-oriented concepts supported by Hibernate include inheritance, association, polymorphism, compositions, and collections that aid in query creation when using the Java method and HQL (Hibernate Query Language).

----

26. Can you describe the phases of the servlet life cycle?
Given below are the five phases:

Classloading phases: The web container must first load the servlet class file with the.class extension.
Instantiation phases: The servlet must then be instantiated by executing the default function Object.
Initialize phases: This stage involves running the servlet's init() method, where the servlet configuration will be given to it. This is a lifecycle method offered by the Servlet interface that is only executed once during the lifetime of the servlet.
Request handling: By utilizing the service() function of the Servlet interface, the servlets in this instance deliver services to various requests.
Remove phases: The Servlet interface destroy() lifecycle method, which is used to clear the configuration and close resources before servlet destruction, will be called during this phase. The waste will then be picked up after this.

----

27. What are different modules used in Spring?
Given below are the various modules used in Spring:

The Core container module
Object/Relational mapping module
DAO module
Application context module
Aspect Oriented Programming
Web module
MVC module
FREE Java Certification Training
Learn A-Z of Java like never beforeENROLL NOWFREE Java Certification Training

----

28. What is a backing bean?
Backing beans are JavaBeans components that relate to JavaServer Pages and contain JavaServer Faces components. The backing bean outlines the characteristics for the page components as well as the methods that process them. Event handling, validation, and navigational processing are a few examples of this processing.

----

29. What is the build file?
An XML file with one or more asant targets is referred to as a build file. A target is a list of assignments that a user hopes to complete. A user can specify which target should be executed when asant is started. If there isn't a target, the project's default target is carried out.

----

30. Explain business logic.
The code that contains an application's functionality is known as business logic. This logic is implemented in the EJB (Enterprise JavaBeans) architecture by the enterprise bean's methods.

</https://www.simplilearn.com/j2ee-interview-questions-answers-article>

<https://engineeringinterviewquestions.com/java-swing-interview-questions-and-answers/>
</https://engineeringinterviewquestions.com/java-swing-interview-questions-and-answers/>

<http://www.a2zinterviews.com/java-questions/swing-questions/>


----

1.	What are differences between Swing and AWT?
 	There is couple of differences between swing and AWT.
AWT component are considered to be heavyweight while Swing component are lightweights.
Swing has plug gable look and feel.
AWT is platform dependent same GUI will look different platform while Swing is developed in Java and is platform dependent.

----

 	DISCUSS
2.	Why Swing components are called lightweight component?
 	
AWT component are associated with native screen resource and called heavyweight component.
While Swing components is uses the screen resource of an ancestor instead of having their own and that's why called lightweight or lighter component.
 	DISCUSS

----

3.	What is the difference between a scrollbar and a scrollpane?
 	
A Scrollbar is just a component, but not a container.
A Scrolpane is a container.
A Scrollpane handles its own events and performs its own scrolling.
 	DISCUSS

----

4.	What is a container in a GUI?
 	A container contains and arranges other components (including other container) through the use of layout managers, which use specific layout policies to determine where components should go as a function of the size of the container.

----

5.	What is Event Driven Thread (EDT) is Swing?
 	
Event Driven Thread or EDT is a special thread in Swing and AWT. Event Driven Thread is used to draw graphics and listen for events in Swing.
You will get a bonus point if you able to highlight that time consuming operations like connecting to database, opening a file or connecting to network should not be done on EDT thread because it could lead to freezing GUI because of blocking and time consuming nature of these operations instead they should be done on separate thread and EDT can just be used o spawn those thread on a button click or mouse click.
 	DISCUSS

----

6.	What is a layout manager and what are different types of layout managers available in Java Swing?
 	A layout manager is an object that is used to organize components in a container.
FlowLayout: The elements of a Flow Layout are organized in a top to bottom, left to right fashion.
Border Layout: The elements of a BorderLayout are organized at the borders(North, South East and West) and the center of a container.
Card Layout: The elements of a CardLayout are stacked, on top of the other, like a deck of cards.
Grid Layout: The elements of a GridLayout are of equal size and laid out using the square of a grid.
Grid Bag Layout: The elements of a GridBagLayout are organized according to a grid. However, the elements may be different sizes and may occupy more than one row or column of the grid. In addition, the rows and columns may have different sizes.
 	DISCUSS

----

7.	What is the difference between a Window and a Frame?
 	The Frame extends Window to define a main application window that can have a menu bar.
 	DISCUSS

----

8.	What is the difference between the paint() and repaint() methods?
 	
The paint() method supports painting via a Graphics object.
The repaint() method is used to cause paint() to be invoked by the AWT painting thread.

----

9.	Does Swing is thread safe?
 	
Since Swing components are not thread safe it means you cannot update these components in any thread other than Event Driven Thread.
If you do so you will get unexpected behavior.
Some time interviewer will also ask what are thread safe methods in swing which can be safely called from any thread only few like repaint() and revalidate().
 	DISCUSS

----

10.	What are peerless components?
 	The peerless components are called light weight components.
 	DISCUSS

----

11.	What advantage do Java's layout managers provide over traditional windowing systems?
 	
Java uses layout managers to lay out components in a consistent manner across all windowing platforms.
Since Java's layout managers aren't tied to absolute sizing and positioning, they are able to accommodate platform specific differences among windowing systems.
 	DISCUSS

----

12.	Which package has light weight component?
 	
javax.Swing package contains light weight components.
All components in Swing, except JApplet, JDialog, JFrame and JWindow are lightweight components.


----

13.	What is the difference between the Font and FontMetrics classes?
 	The FontMetrics class is used to define implementation specific properties, such as ascent and descent of a Font object.


----

13.	What is the difference between the Font and FontMetrics classes?
 	The FontMetrics class is used to define implementation specific properties, such as ascent and descent of a Font object.
 	DISCUSS

----

14.	How can a GUI component handle its own events?
 	A component can handle its own events by implementing the required event listener interface and adding itself as its own event listener.
 	DISCUSS

----

15.	Why swing is not thread safe?
 	
The Swing API was designed to be powerful, flexible and easy of use.
In particular, we wanted to make it easy for programmers to build new Swing components, whether from scratch or by extending components that we provide.
For this reason, we do not require Swing components to support access from multiple threads.
Instead, we make it easy to send requests to a component so that the requests run on a single thread.
 	DISCUSS

----

16.	Name Container classes?
 	
Window
Frame
Dialog
File Dialog
Panel
Applet or ScrollPane


----

17.	What method is used to specify a container's layout?
 	
The setLayout() method is used to specify a container's layout.
For example, setLayout(new Flow Layout()); will be set the layout as Flow Layout.
 	DISCUSS

----

18.	Which containers use a Flow Layout as their default layout?
 	The Panel and Applet classes use the Flow Layout as their default layout.
 	DISCUSS

----

19.	Name Components subclasses that support painting?
 	
The Canvas
Frame
Panel and
Applet classes support painting
 	DISCUSS

----

20.	What is the preferred size of a component?
 	The preferred size of a component is the minimum component size that will allow the component to display normally.


----

21.	Which container method is used to cause a container to be laid out and redisplayed?
 	validate()
 	DISCUSS

----

22.	Name the containers which use Border Layouts as their default layout?
 	
Window
Frame and
Dialog classes
 	DISCUSS

----

23.	What do heavy weight components mean?
 	
Heavy weight components like Abstract Window Toolkit (AWT) depend on the local windowing toolkit.
For example, java.awt. Button is a heavy weight component.
 	DISCUSS

----

24.	What is the purpose of the enableEvents() method?
 	
The enableEvents() method is used to enable an event for a particular component.
Normally, an event is enabled when a listener is added to an object for a particular event.
The enableEvents() method is used by objects that handle events by overriding their event dispatch methods.

----

25.	What is swing?
 	Swing is a comprehensive set of user interface components whose look and feel can be defined at runtime. Swing is a set of classes that provide more powerful and flexible components that are possible with the AWT.
 	DISCUSS

----

26.	Explain the JTable and TableDateModel interface in Swing?
 	
JTable is one of the powerful features given by Swing. This class, present in the swing.table package, shows the data in the form of tables, in a much better way. We can also select an entire column or row at a time.
JTable (TableDataaModel) is the constructor for a JTable.
The method addColumn (JTableColumn) appends a column to the end of the JTable's array of columns and JTableHeader's getTableHeader () method gives a Header to the table.
The TableDataModel interface specifies the interface for objects that provides data for cells in a JTable. We can have an object of this interface by creating an object of JTableDataModelAdapter after overriding the methods.
 	DISCUSS

----

27.	How different is Swing from AWT?
 	
In addition to familiar components, such as buttons, check boxes, labels, etc. Swing supplies several exciting additions, including tabbed panes, scroll panes, trees, and tables. Even familiar components, such as buttons, have more capabilities in Swing. For example, a button may have both an image and a text string associated with it. Also, the image can be changed as the state of the button changes.
Unlike AWT components, Swing components are not implemented by platform-specific code. Instead, they are written entirely in Java and, therefore, are platform-independent.
Swing components can be treated as lightweight components. One of the most important features of Swing components is their pluggable look and feel design, which increases the reliability and consistency of applications and applets deployed across platforms.

----

28.	How do you classify Swing Components?
 	Swing components are classified under the following headings:
Top level containers – The containers at the top of any swing component hierarchy are:
Applet
Dialog
Frame
. General purpose containers – The intermediate containers are
Panel
Scroll pane
Split pane
Tabbed pane
Tool bar
Special purpose containers – These are intermediate containers which play specific roles in the user interface:
Internal frame
Layered pane
Root pane
Basic controls : The atomic components that exist primarily to get input from the user are
Buttons
Combo box
List
Menu
Slider
Spinner
TextField
Uneditable information displays: The atomic components which give information to the user are
Label
Progress bar
Tool tip
Interactive displays of highly formatted information – The atomic components that display formatted information that can be modified by the user are
Color chooser
File chooser
Table
Text
Tree

----

29.	What is MVC?
 	Model-View-Controller (MVC) is a well known object oriented design for GUI components. The architecture of swing components is based on MVC design. When a GUI component is developed using MVC architecture, it is divided into three parts:
Model-An object that defines the component's state
View-The visual screen representation of component.
Controller-An object that controls a component in such a way that it responds to user input.
The model part of an MVC-based component provides information that can be used to specify the component's value, provided the component has any value properties, e.g. the min and max values of a slider control are stored in the component's model part.
The Controller part modifies information maintained by the component's model part in response to input from the user.
The View part manages the way in which the object is drawn on the screen.

----

30.	What is the main difference between Dialog and Frame?
 	
In AWT, the top level window, which is itself not contained in another window, is called a FRAME.
On the other hand, a window that appears over existing window (mostly Frame) and forces the user to respond is called a DIALOG.
Frame f = new Frame(); // creates an object of type Frame.
A FRAME can exists on its own , where as a DIALOG cannot exist on its own. In other words, FRAME is a primary window, where as the DIALOG box is secondary window. The dialog boxes are of two types:
modal – This dialog won't let the user interact with the remaining containers/windows until he deals with it.
modeless - The user can interact with other windows as well as the dialog box, e.g. the toolbox.
There is no default constructor for a DIALOG. The following statement constructs a dialog box:
public Dialog( Frame parent, String title, boolean modal) Here:
parent – The container to which the dialog belongs.
title – Title of the dialog
modal – True for modal type, false for modeless type.

----

31.	Explain Thread Rule in Swing?
 	Once a swing component has been realized, i.e. the component has been painted on screen or it is ready to painted, all the code that might affect or depend on the state of that component should be executed in the event dispatching thread. This is called thread rule in swing.
 	
</http://www.a2zinterviews.com/java-questions/swing-questions/>

<https://quescol.com/interview-preparation/core-java-coding-questions>

Java Coding Questions on Numbers
Write a program to reverse an integer in Java.
Write a program in Java to check whether an integer is Armstrong number or not.
Write a program in Java to check given number is prime or not.
Write a program in Java to print the Fibonacci series using iteration.
Write a program in Java to print the Fibonacci series using recursion.
Write a program in Java to check whether a number is Palindrome or not using iteration.
Write a program in Java to check whether a number is Palindrome or not using recursion.
Write a program in Java to find greatest among three integers.
Write a program in Java to find sum of digits of a number using recursion?
Write a program in Java to swap two numbers without using third variable?
Write a program in Java to swap two numbers using third variable?
Write a program in Java to find prime factors of a given integer.
Write a program in Java to add two integer without using arithmetic operator?
Write a program in Java to find given number is perfect or not?
Java Program to Calculate the Average of Integer Array.
Java Program to calculate the Average of number taken from user.
Java Program to calculate factorial using iterative method.
Java Program to calculate factorial using recursion.
Java Program to check a given number is even or odd.
Java program to print first n Prime Number with explanation.
Java Program to print Prime Number in a given range.
Java Program to find Smallest number among three.
Java program to calculate the power using the POW method.
Java Program to calculate the power without using POW function.
Java Program to calculate the square of a given number.
Java Program to calculate the cube of a given number.
Java Program to calculate the square root of a given number.
Java program to calculate LCM of given two numbers.

Java Program to find GCD or HCF of two numbers.
Java Program to find GCD of two numbers using recursion.
Java Program to check the given year is a leap year or not.
Java Program to convert Celsius to Fahrenheit.
Java Program to convert Fahrenheit to Celsius.
Java program to calculate Simple Interest with explanation.
Java Coding Questions on String
Write a method in Java which will remove any given character from a String.
Write a program in Java to count occurrence of a given character in a String?
Write a program in Java to check if two String are Anagram.
Write a program in Java to check a String is palindrome or not.
Java program to check given character is vowel or consonant.
Java program to check given character is digit or not.
Java program to replace the string space with a given character.
Java program to convert lowercase char to uppercase of string.
Java program to convert lowercase vowel to uppercase in string.
Java program to delete vowels in a given string.
Java program to count Occurrence Of Vowels & Consonants in a String.
Java program to print the highest frequency character in a String.
Java program to Replace First Occurrence Of Vowel With ‘-‘ in String.
Java program to count alphabets, digits and special characters.
Java program to remove blank space from string.
Java program to Concatenate two strings.
Java Program to remove repeated character from string.
Java program to calculate sum of integers in string.
Java program to print all non repeating character in string.
Java Program to sort characters of string in Ascending Order.
Java Program to sort character of string in descending order.
Java Interview Questions for Freshe...

Write a program in Java for, In array 1-100 numbers are stored, one number is missing how do you find it.
Write a program in Java for, In a array 1-100 multiple numbers are duplicates, how do you find it.
Write a program in Java for, How to find all pairs in array of integers whose sum is equal to given number.
Write a program in Java for, In a array 1-100 exactly one number is duplicate how do you find it.
Write a program in Java for, Given two arrays 1,2,3,4,5 and 2,3,1,0,5 find which number is not present in the second array.
Write a program in Java for, How to compare two array is equal in size or not.
Write a program in Java to find largest and smallest number in array.
Write a program in Java to find second highest number in an integer array.
Write a program in Java to find top two maximum number in array?
Java program to print array in reverse Order.
Java program to reverse array without using second array.
Java Program to calculate length of an array.
Java program to insert an element at end of an Array.
Java program to insert element at a given location in Array.
Java Program to delete element at end of Array.
Java Program to delete given element from Array.
Java Program to delete element from array at given index.
Java Program to find sum of array elements.
Java Program to print all even numbers in array.
Java Program to print all odd numbers in array.
Java program to perform left rotation of array elements by two positions.
Java program to perform right rotation in array by 2 positions.
Java program to find all pairs in array of integers whose sum is equal to given number.
Java Program to remove duplicate elements form array.

</https://quescol.com/interview-preparation/core-java-coding-questions>

<https://quescol.com/interview-preparation/core-java-pattern-questions>

Pattern Programs In Java: 25+ types that asked most often
One of the most important areas you should have a focus on when you are preparing for the interview is a pattern printing program. I don’t think that in an interview if your recruiter is recruiting you as a software developer/software engineering profile will not ask to write a program to print given pattern (maybe in some interview not).

Writing program is all about how efficiently and fast you can think logics
Basically, Writing a program of any pattern is not tough. It only requires time and practices.

When you are going to write a program of any pattern for the first time then you will surely realize that it is taking time to build a logic and writing program to print that particularly given pattern. Here 80-90% is only the game of thinking the logic and once you imagine the logic then very quickly you can write a program.

14 Popular Programming Languages an...

Play

Unmute
Remaining Time -1:46


Fullscreen

Advertisement: 0:00
14 Popular Programming Languages and Their Uses Explained
Below I have collected the list if most important and most frequently asked pattern program and also I have provided their program in Java. Solution contains nested for loops and if else block etc.


You should also prepare pattern program in C language.

NOTE:-I kindly request to all readers and my website lovers please try to make all programs by self before go for the solution.

Different Types of Pyramid Patterns
half pyramid pattern programquescol
Half Pyramid Pattern Using *

right inverted half pyramid program in c quescol
Right Inverted Half Pyramid Pattern


half pyramid using number in C
Half Pyramid Pattern

inverted half pyramid program quescol
Inverted Half Pyramid Pattern

full pyramid pattern program in c using star quescol
Full Pyramid Pattern

inverted half pyramid using number program in c
Inverted Half Pyramid Pattern

right half pyramid program quescol
Right Half Pyramid Pattern

inverted full pyramid pattern program in c using star
Inverted Full Pyramid Pattern

full pyramid using number program in c
Full Pyramid Pattern


Click Here To See Pyramid Pattern Program In Java

Different Types of Diamond Patterns
solid right half diamond pattern program in C
Right Half Diamond Pattern

solid left half diamond pattern program in c
Left Half Diamond Pattern

solid diamond using star program in c
Full Diamond Pattern


Click here To See Diamond Pattern Program In Java

Pascal’s Triangle
pascal triangle pattern program in c
Pascal’s Traingle


Click here To See Pascal’s Triangle Program In Java

Print Floyd’s Triangle
floyd triangle pattern program in c
Print Floyd’s Triangle


Click here To See Floyd’s Triangle Program In Java

Different Types of Rhombus Patterns
solid rhombus right inclined pattern program in c
Solid Rhombus Right Inclined

solid rhombus left inclined pattern program in C
Solid Rhombus Left Inclined


Click here To See Rhombus Pattern Program In Java

Different Types of Rectangle Patterns
solid rectangle pattern program in C
Solid Rectangle

hollow rectangle pattern program in C
Hollow Rectangle


Click here To See Rectangle Pattern Program In Java

Different Types of Patterns Using Star And Hyphen
star hyphen combination pattern program in c
star hyphen combination pattern 1

star hyphen combination 3 pattern program in C
Triangle Using Star Hyphen

star hyphen combination pattern program in c
star hyphen combination pattern 2

inverted Triangle Using Star Hyphen pattern program in C
Inverted Triangle Using Star Hyphen

star hyphen combination full pattern program in c
Daimond Using Star Hyphen

</https://quescol.com/interview-preparation/core-java-pattern-questions>

<https://quescol.com/interview-preparation/java-interview-question-experienced>

MNCs Choice Java Interview Question For Experienced
If Your are struggling to find the most important and frequently asked face two face c interview questions, Then hold down and take a deep breath because you are at the right place.

I know that It is very tough for fresher students to prepare for an interview as well as finding some great bunch of right questions that cover the most important topics.
In this section, I have tried to cover all important and most asked c programming interview questions topics wise.
Let us start Preparing.

Java interview questions for Experienced MNCs
Q1). Tell me something about HashMap in Java
Ans:

HashMap is a Collection classes in java which implementation is based on the hash table data structure. HashMap class extends AbstractMap class and AbstractMap  class implements the Map interface.


Some Important point about Hashmap:

HashMap allows only one null key and multiple null value.
HashMap does not maintain the order of insertion into the map.
Initial size of hashmap bucket is 16 which grows to 32 when the map entries crosses  75%.
HashMap uses hashCode() and equals() methods on keys  to perform put and get operations. It internally check the key is already exist or not?
Hashmap is not a thread safe. This is the reason it won’t uses in multithreaded environment. 
Q2). What is load Factor, Threshold, Rehashing and collision in hashmap?
Ans:

Load factor is the measure to decide when to increase the size of the Map. By default, the load factor is 75% of the capacity.

The threshold can be calculated by multiplying the current capacity and load factor. 


Rehashing means, re-calculating the hash code of already stored entries. When entries in the hash table exceed the threshold, the Map is rehashed and increases the size of buckets.

Collision is a condition when a hash function returns the same bucket location for two different keys.

For example:


Suppose Our HashMap has an initial capacity is 16 and a load factor is 0.75. 

Threshold will be 16 * 0.75 = 12, 

It means after the 12th entry in the hashmap, the capacity of the hashmap will increase from 16 to 32.

----

Q3). How HashMap Internally works in Java?
Ans:

----

Q4). Explain how hashcode will be calculated for String Key.
Ans:

Hashmap has hashCode() method. This method is used to calculate the hashcode value of the String as an Integer.

Syntax of hascode:
public int hashCode()

Program

import java.io.*; 
class Main {
public static void main(String[] args)
{
  String str = "Name";
  System.out.println(str);
  int hashCode = str.hashCode();
  System.out.println(hashCode);
 }
}
Output

Name
2420395
Here we got Output 2420395 for String “Name”. Below is the way to calculate hashcode of string.

How hashcode is calculated for string key?

Below  is the formula to calculate the hashcode value of a String:

s[0]*31^(n-1) + s[1]*31^(n-2) + … + s[n-1]

Here:

s[i] is the ith character of the string
^ is a the exponential operator
n shows the length of the string

----

Q5). What is the Difference between HashMap and LinkedHashMap.
Ans:

The difference between HashMap and LinkedHashMap is that LinkedHashMap maintains the insertion order of keys but HashMap doesn’t maintain the insertion order of keys.
LinkedHashMap requires more memory than HashMap to keep the record of insertion order. Basically LinkedHashMap  uses doubly LinkedList to keep track of the insertion order of keys.
LinkedHashMap extends HashMap and implements the Map interface and Hashmap extends AbstractMap class and implements the Map interface.
Hashmap were introduced in JDK 2.0 but LinkedHashMap introduced in JDK 4.0.
Here is the Program of HashMap and LinkedHashMap.

Example of Hashmap

import java.util.HashMap;
public class Main {
public static void main(String[] args)
{
  HashMap<String,String> map = new HashMap<>();
  map.put("firstName","Interview");
  map.put("lastName","Expert");
  map.put("rollNo","1");
  System.out.println(map.size());
  if(map.containsKey("firstName")){
    System.out.println(map.get("firstName"));
  }
  if(Integer.parseInt(map.get("rollNo"))<20){
    System.out.println(map.get("lastName"));
  } 
 }
}
﻿
Output:

3

Interview

Expert
Example Of LinkedHashMap:

import java.util.LinkedHashMap;
public class Main {
public static void main(String[] args)
{
  LinkedHashMap<String,String> map = new LinkedHashMap<>();
  map.put("firstName","Interview");
  map.put("lastName","Expert");
  map.put("rollNo","1");
  System.out.println(map.size());
  if(map.containsKey("firstName")){
    System.out.println(map.get("firstName"));
  }
  if(Integer.parseInt(map.get("rollNo"))<10){
    System.out.println(map.get("lastName"));
  } 
 }
}
Output:

3

Interview

Expert

----

Q6). What is Concurrent HashMap?
Ans:

ConcurrentHashMap is a class of Collection Framework that provides a concurrent version of HashMap. It is a thread safe i.e multiple threads can access the single object of the map.

At a time any number of threads can perform the read operations without locking. But for write/update operation at a single time thread must lock the particular segment in which the thread wants to operate.

Functionality wise HashMap and ConcurrentHashMap are same, except ConcurrentHashMap maintains concurrency. Hashmap Can have a null key and value but concurrentHashMap Cannot have null key and value pair.

ConcurrentHashMap uses a Hashtable data structure. 

ConcurrentHashMap Example

import java.util.concurrent.ConcurrentHashMap;
import java.util.Map;
public class Main {
public static void main(String[] args)
{
  Map<String,String> chm = new ConcurrentHashMap<>();
  chm.put(null,null);
}
}
Output

Exception in thread "main" java.lang.NullPointerException
at java.base/java.util.concurrent.ConcurrentHashMap.putVal(ConcurrentHashMap.java:1011)
at java.base/java.util.concurrent.ConcurrentHashMap.put(ConcurrentHashMap.java:1006)
at Main.main(Main.java:7)
Here we will get an NullPointerException because we are trying to insert null key value in concurrent hashmap which is not allowed.

----

Q7). What is the Time Complexity of HashMap.
Ans : 

Usually Time complexity of Hashmap is O(1). But in some cases it might change. Let’s assume a scenario in hashmap when hashcode will return same index value for each enteries. In that case at single index of hashtable, a singly linked list will create to store the key value pair of hashmap.

This is a worst case scenario in HashMap which will be O(n) complexity to lookup. Here we have to walk through all entries in the same hash bucket. This situation is very rare.

There are some improvements done in java 8 to improve the time compelxity from O(n) to O(log n). Instead of using singly linked list, Hashmap in Java 8 uses self balancing tree like RB tree and AVL tree.

----

Q8) Tell me some difference between ArrayList and LinkedList.
Ans:

ArrayList uses a dynamic array/Array object data strucutre to store the elements but LinkedList internally uses a doubly linked list to store the elements. 
ArrayList Manipulation is slow because it uses an array and if we remove any element from the array we have to shift other elements in memory. But LinkedList Manipulation is faster because it uses a doubly linked list so no shift is required when we remove any element.
ArrayList is better for storing and accessing elements but LinkedList is better for manipulating elements.
ArrayList takes memory in a contiguous fashion but the linked list does not takes memory in a contiguous.

----

Q9) When you will prefer ArrayList and when LinkedList in your RealTime projects.
Ans:

As We know Accessing an element in ArrayList takes constant time [O(1)] and adding an element takes O(n) in the worst case. And in LinkedList inserting an element takes O(n) time and accessing also takes O(n) time but LinkedList needs some more memory than ArrayList.

Accessing elements in ArrayList is faster because it is index based. But Accessing elements in LinkedList is slower because we need to traverse each node. Insertion and deletion in Linked List are much faster because here we need to change the pointer of the node only. We need not shift the element as we do in ArrayList. 

So here we are at the conclusion, if we need to perform more manipulation work on the element and memory is not a problem then we can prefer Linked List over ArrayList.

But When we require more searching of the element then we can choose ArrayList over LinkedList.

Time complexity with operations

 For ArrayList<E>

get(int index) takes O(1).
add(E element) operation takes O(1) amortized, but in the worst case it will be O(n) since the array must be resized and copied.
add(int index, E element) takes O(n) Complexity (with n/2 steps on average).
remove(int index) operation takes O(n) (with n/2 steps on average).
Iterator.remove() have O(n) Complexity (with n/2 steps on average). 
ListIterator.add(E element) operation takes O(n) (with n/2 steps on average)
For LinkedList<E>

get(int index) operation takes O(n) , It will take O(1) when index = 0 or index = list.size() -1 .
add(int index, E element) take O(n) and It will take O(1) when index = 0 or index = list.size() – 1
remove(int index) takes O(n) and It will take O(1) when index = 0 or index = list.size() – 1. 

----

Q10) What is the difference between Hashset and LinkedHashSet.
Ans:

HashSet uses Hashtable to store the elements. LinkedHashSet uses HashTable and a doubly linked list to store and maintain the insertion order of the elements.
HashSet extends AbstractSet class but LinkedHashSet extends HashSet.
HashSet won’t maintain the insertion order of the element but LinkedHashSet maintains the insertion order of an element.
HashSet takes less memory in comparison to LinkedHashSet because HashSet won’t maintain insertion order but LinkedHashSet maintains the insertion order.
HashSet provides faster performance than LinkedHashSet.

----

Q11) Differences between HashMap and HashSet.
Ans:

Hashmap is the implementation of the Map interface But HashSet is the implementation of the Set interface.
HashSet internally uses Hashmap for its implementation But HashMap Won’t.
HashMap stores value in key-value pair But HashSet Stores only object no key-value pair.
HashMap uses the put(k,v) method to add elements to the map whereas HashSet uses add(K) method.
HashMap Allows duplicate values not key But HashSet won’t allow duplicate values.
HashMap allows a single null key and multiple null values but HashSet allow only one null value.
Multi-threading Questions

----

Q12) What is the Different ways to create threads in java?
Ans:

There are two ways to create threads in Java:

By extending Thread class
By implementing Runnable interface.
1). By Extending Thread Class

class Main extends Thread{  
    public void run(){  
        System.out.println("thread is running");  
    }  
    public static void main(String args[]){  
        Main thread1 = new Main();  
        thread1.start();  
    }  
} 
Output:

Thread is running
2). By implementing Runnable interface

class Main implements Runnable{  
  public void run(){  
    System.out.println("thread is running");  
  }    
  public static void main(String args[]){  
    Main obj=new Main();  
    // Here we are Using the constructor Thread(Runnable r)
    Thread tobj =new Thread(obj);     
    tobj.start();  
  }  
}  
Output:

Thread is running

----

Q13). Difference between Thread and Runnable.
Ans:

Thread is a class used to create a thread Whereas Runnable is an interface that is used to create a thread.
Thread has methods like start() and run() but Runnable has only one method run().
Thread won’t allow multiple inheritance but Runnable allows multiple inheritance.
Thread requires more memory but Runnable requires less memory.
In Thread Each thread creates a unique object but in Runnable same object is shared with multiple threads.

----

Q14) Tell some Difference between Callable & Runnable in Java.
Ans: 

Callable belongs to java.util.concurrent package whereas Runnable belongs to java.lang package.
Thread will not create by passing callable as a parameter but Runnable will create a thread by passing runnable as a parameter.
Callable has call() method whereas Runnable has run() method.
Callable might return some output but Runnable does not return anything.
By invoking invokeAll() method bulk execution of the task is possible in callable but in runnable we can’t use it for bulk execution of the task.

----

Q15). What is the Difference between sleep() & wait() method in java.
Ans:

Sleep() method belongs to the Thread class whereas Wait() method belongs to the Object class.
Sleep() method is used to pause the execution of the current thread for a given time in Milliseconds. But the wait() method tells the thread to wait until another thread invoke’s the notify() or notifyAll() method for this object.
Sleep() method will not release the lock on the object during Synchronization but Wait() method can release the lock on the object during Synchronization.
Sleep() is a static method but wait() is not a static method.
Sleep() has two overloaded methods sleep(long millis) and sleep(long millis, int nanos), Whereas Wait() has Three Overloaded methods wait(), wait(long timeout), wait(long timeout, int nanos).
Example of Sleep method

import java.lang.Thread;
class Main {
    public static void main(String[] args)
    {
        try {
            for (int i = 1; i <=10; i++) {
                Thread.sleep(1000);
                System.out.println(i);
            }
        }
        catch (Exception e) {
            System.out.println(e);
        }
    }
}
Output

1
2
3
4
5
6
7
8
9
10
Exceptional Handling in Java
Q16). What is exceptional handling in java?
Ans:

In Java, Exception Handling is a mechanism to handle the runtime errors and protect the program from abnormal termination. It help to maintain the normal flow of the application in case any exceptions come.

There are multiple type of Exceptions such as ClassNotFoundException, IOException, SQLException.

java.lang.Throwable class is the root class of Java Exception hierarchy. It is inherited by two subclasses Exception and Error. The hierarchy of Java Exception classes is given below:

java interview question for mncs experienced

----

Q17). Difference between Checked and Unchecked Exceptions.
Ans: 

Checked exception occurs at compile time whereas the Unchecked exception occurs at run time.
Checked Exception is checked by the compiler but the Unchecked exception is not.
Checked Exception can be handled at compile time but Unchecked Exception can be handled at runtime.
Checked Exception is a sub-class of the Exception class but Unchecked Exception is not a part of the Exception class.
Some Checked Exceptions are ClassNotFoundException, IOException, SQLException, etc. Some Unchecked Exceptions are ArithmeticException, NullPointerException, ArrayIndexOutOfBoundExceptions.
java interview questions for experienced

----

Q18). How many ways you can print exceptions in java?
Ans:

There are multiple ways to print the exceptions in Java. Here we will see 3 methods to print the exceptions.

1). printStackTrace()

2). toString()

3). getMessage()

1.printStackTrace()

printStackTrace method prints exception information printStackTrace() is a method of Java.lang.Throwable class. It is used to print the details of exceptions like class name and line number where the exception occurred.

Program to demonstrate printStackTrace() method

import java.io.*;
class Main {
    public static void main (String[] args) {
      int a=5, b=0;
        try{
          System.out.println(a/b);
        }
        catch(ArithmeticException e){
          e.printStackTrace();
        }
    }
}
Output:

java.lang.ArithmeticException: / by zero

at Main.main(Main.java:6)

2. toString() 

toString() method is also used to  prints exception. It prints exception information in the format of Name of the exception along with description of the exception.

Program to demonstrate toString() method

import java.io.*;
class Main {
    public static void main (String[] args) {
      int a=5, b=0;
        try{
          System.out.println(a/b);
        }
        catch(ArithmeticException e){
            System.out.println(e.toString());
        }
    }
}
Output:

java.lang.ArithmeticException: / by zero

3. getMessage()

getMessage() method prints only the description of the exception message.

Program to demonstrate  getMessage() method


import java.io.*;
class Main {
    public static void main (String[] args) {
      int a=5, b=0;
        try{
          System.out.println(a/b);
        }
        catch(ArithmeticException e){
            System.out.println(e.getMessage());
        }
    }
}
Output:

/ by zero

----

Q19). What is the process to create custom exception in java?
Ans: Here we are showing two examples to show how you can create you own custom exception class in Java. 

Example 1: 

class CustomException extends Exception{
    public CustomException(String ex){
        super(ex);
    }
}

public class Main{
    public static void main(String ...a){
        int age = 13;
        try{
            if(age<18){
                throw new CustomException("no valid Age");
            }else{
                System.out.println("Age is valid");
            }
        }
        catch(CustomException e){
             System.out.println("Exception occured: " + e); 
        }
        System.out.println("Rest Code is running"); 
    }
}
Output


Exception occured: CustomException: no valid Age
Rest Code is running
Example 2:


class CustomException extends Exception {
   String message;
   CustomException(String str) {
      message = str;
   }
   public String toString() {
      return ("Custom Exception Occurred : " + message);
   }
}
public class Main {
   public static void main(String args[]) {
      try {
         throw new CustomException("This is CustomException");
      } catch(CustomException e) {
         System.out.println(e);
      }
   }
}
Output

Custom Exception Occurred : This is CustomException

----

Q20). Write the difference between Throw Vs Throws.
Ans:

throw keyword is used inside the function or the block of code to throw an exception explicitly when an exception occurs. Whereas throws keyword is used with method signature with exception means exception might be thrown by the function during the execution if an exception occurs.
throw keyword is followed by an instance of Exception that will be thrown whereas throws keyword is followed by class names of Exceptions to be thrown.
throw keyword can be used to throw only one exception at a time but in throws keywords, we can use multiple Exception classes separated by a comma.
throw keyword is used to propagate unchecked Exceptions whereas the throws keyword is used to propagate checked Exceptions.
Example of using throw keyword

public class Main{
   public void checkAge(int age){
      if(age<18)
         throw new ArithmeticException("Age is not valid for voting");
      else
         System.out.println("Age is valid for voting");
   }
   public static void main(String args[]){
      Main obj = new Main();
      obj.checkAge(10);
      System.out.println("Execution continue");
   }
}
Output

Exception in thread "main" java.lang.ArithmeticException: Age is not valid for voting
at Main.checkAge(Main.java:4)
at Main.main(Main.java:10)
Example of using throws keywords

public class Main{
   public int division(int a, int b) throws ArithmeticException{
      int result = a/b;
      return result;
   }
   public static void main(String args[]){
      Main obj = new Main();
      try{
         System.out.println(obj.division(15,0));
      }
      catch(ArithmeticException e){
         System.out.println("We can't divide number by zero");
      }
   }
}
Output

We can't divide number by zero

----

Q21). What is Serialization and why we use it?
Ans:

Serialization is used to convert the object into a byte stream so that it can be sent over the network. Deserialization is the reverse process where the byte stream is converted into an actual Java object. 

Serialization is required because Network infrastructure and Hard disk or any other hardware components can understand bits and bytes only but not the JAVA objects.

So we use Serialization as a translation to translate our Java object’s values/states to bytes to send it over the network or save it.

SerialVersionUID is used here for identity purpose. It must be static, final, and of type long.

Java Program for Serialization and Deserialization 

import java.io.*;
public class Main {
    public static void main(String[] args) {
        Student student = new Student("quescol", 2);
        byte[] bytes = convertObjectToBytes(student);
        System.out.println(bytes);
        Student s = (Student) convertBytesToObject(bytes);
        System.out.println(s);
    }
    public static byte[] convertObjectToBytes(Object obj) {
        ByteArrayOutputStream boas = new ByteArrayOutputStream();
        try (ObjectOutputStream ois = new ObjectOutputStream(boas)) {
            ois.writeObject(obj);
            return boas.toByteArray();
        } catch (IOException ioe) {
            ioe.printStackTrace();
        }
        throw new RuntimeException();
    }
    public static Object convertBytesToObject(byte[] bytes) {
        InputStream is = new ByteArrayInputStream(bytes);
        try (ObjectInputStream ois = new ObjectInputStream(is)) {
            return ois.readObject();
        } catch (IOException | ClassNotFoundException ioe) {
            ioe.printStackTrace();
        }
        throw new RuntimeException();
    }
}

class Student implements Serializable {
    private String name;
    private int age;
    public Student( String name, int id) {  
        this.age = age;  
        this.name = name;  
    }
}
Output

[B@7d4793a8
Student@721e0f4f

----

Q22). What is volatile and Transient keyword in java?
Ans:

A volatile keyword is used in a multithreading environment. When two threads are performing reading and writing operations on the same variable, a volatile keyword is used. It flushes the changes directly to the main memory instead of the CPU cache. A transient keyword is used in serialization. Variable where transient is used, cannot be part of the serialization and deserialization.
Volatile variable is not initialized with any default value whereas transient variables are initialized with a default value during deserialization.
Volatile variable can be used with the final keyword whereas Transient cannot be used with the final keyword.
Volatile variable can be used with static keyword whereas Transient cannot be used with the static keyword.

----

Q23). How you will create Immutable class in java
Ans:
In Java, an Immutable class means once the object is created in the class, its fields cannot be changed or modified. 
All the wrapper classes like Boolean, Byte, Long, Short, Integer, Float, Double, Char, and String are immutable.
There are some steps by following we can create an immutable class in Java

First Declare the class with the final keyword so it can’t be extended.
Make all the classes private. It will not allow direct access.
Don’t make any setter methods for variables.
Make all mutable fields final so that their value can be assigned only once.
Initialize the all fields value using the constructor. 
Example of Immutable java Class

final class Student{
  private String name;
  private int roll;
  Student(String name, int roll) {
    this.name = name;
    this.roll = roll;
  }
  public String getName() {
    return name;
  }
  public int getRoll() {
    return roll;
  }
}
class Main {
  public static void main(String[] args) {
    Student obj = new Student("quescol", 1);
    System.out.println("Name: " + obj.getName());
    System.out.println("Roll: " + obj.getRoll());
  }
}

----

Q24). How you will Create Singleton class in Java.
Ans:


Singleton class is a class in oops that can have only one object at a time and can be globally accessible.

It Saves memory because Only a single instance is created and reused again and again.

Single Class is mostly used in the multi-threaded system, database application, logging, caching, configuration settings, etc.

There are two forms of singleton design pattern

Early Instantiation: In this Singleton design pattern object will create at the load time.

Lazy Instantiation: In this Singleton design pattern object will create according to the requirement.


Early Instantiation Example

class Singlton {
    //Instance will be created at load time  
    private static Singlton obj=new Singlton();
    private Singlton(){}  
    public static Singlton getSinglton(){  
        return obj;  
    }  
}
class Main {
   public static void main(String[] args) {
      Singlton s1;
      s1= Singlton.getSinglton();
      Singlton s2;
      s2= Singlton.getSinglton();
      System.out.println(s1);
      System.out.println(s2);
   }
}
Output


Singlton@1e81f4dc
Singlton@1e81f4dc
Lazy Instantiation example

class Singlton {
    private static Singlton singlton;
    private Singlton(){
        
    }
    public static Singlton getInstance() {
        if(null == singlton){
            singlton = new Singlton();
        }
    return singlton;
    }
}
class Main {
   public static void main(String[] args) {
      Singlton s1;
      s1= Singlton.getInstance();
      Singlton s2;
      s2= Singlton.getInstance();
      System.out.println(s1);
      System.out.println(s2);
   }
}

</https://quescol.com/interview-preparation/java-interview-question-experienced>

<https://quescol.com/interview-preparation/spring-boot-interview-questions>

----

Q0) What is Java Spring Boot?
What is Spring Boot?
Java Spring Boot is an open-source tool that makes it easier to use Java-based frameworks to create microservices and web apps.
For any definition of Spring Boot, the conversation has to start with Java—one of the most popular and widely used development
languages and computing platforms for app development. Developers all over the world start their coding journey learning Java.
Flexible and user-friendly, Java is a developer favorite for a variety of apps—everything from social media, web, and gaming
apps to networking and enterprise applications.

----

Q1). Explain the Spring Boot key components?
6 MOST DIFFICULT INTERVIEW QUESTION...

Pause

Unmute
Remaining Time -12:06


Fullscreen

----

6 MOST DIFFICULT INTERVIEW QUESTIONS & ANSWERS! (How to ANSWER the HARDEST Interview Questions!)
Ans:


There are four important key components of spring-boot are

Spring Boot auto-configuration.
Spring Boot CLI.
Spring Boot starter POMs.
Spring Boot Actuators.
There are two more Spring Boot components

Spring initializr: To quick start new Spring Boot projects
Spring Boot IDEs: We have multiple Spring Boot IDEs for example : Eclipse IDE, IntelliJ IDEA, Spring STS Suite etc
Now we will discuss these Spring Boot four components one by one in detail.

Spring Boot AutoConfigurator

Spring Boot AutoConfigurator is an important key component of Spring Boot. Spring-based application requires a lot of configuration in development of the project. For example XML Configuration and Annotation Configuration.


To Minimize this configuration problem and save the time, Spring Boot bring with AutoConfiguraton. The main responsibility of the Spring Boot AutoConfigurator is to reduce the Spring XML Configuration and Annotation Configuration. In Development of any Spring Boot, We need to do some minimal Annotation configuration and no any single XML configuration.

In Spring Application XML Configuration requires for views, view resolvers etc But in  Spring Boot Framework  we dont need to define those XML Configuration. This application configuration will be taken care by Spring Boot AutoConfigurator.

Similarly   Spring Boot requires @SpringBootApplication annotation at class level. And this Spring Boot AutoConfigurator annotation will automatically add all required annotations to Java Class ByteCode.

@SpringBootApplication = @Configuration + @ComponentScan + @EnableAutoConfiration

That’s it about Spring Boot AutoConfigurate component.

NOTE:

Spring Boot Starter reduces build’s dependencies and Spring Boot AutoConfigurator reduces the Spring Configuration.
As we discussed that Spring Boot Starter has a dependency on Spring Boot AutoConfigurator, Spring Boot Starter triggers Spring Boot AutoConfigurator automatically.
Spring Boot Starter

Spring Boot Starters is important components of Spring Boot Framework. Spring Boot Starter  combines similar types of dependencies into single dependencies.

For an example if you want to develop a Spring WebApplication with Tomcat WebServer. For this development we have to add some jar dependencies in  Maven’s pom.xml file or Gradle’s build.gradle file like

Spring core Jar file(spring-core-xx.jar)
Spring Web Jar file(spring-web-xx.jar)
Spring Web MVC Jar file(spring-webmvc-xx.jar)
Servlet Jar file(servlet-xx.jar)
Suppose if we want to work with database in spring application then we need to add database related jars like Spring JDBC jar file, Spring ORM jar files, Spring Transaction Jar file etc.

Spring JDBC Jar file(spring-jdbc-xx.jar)
Spring ORM Jar file(spring-orm-xx.jar)
Spring Transaction Jar file(spring-transaction-xx.jar)
As we are seeing that we need lot of dependencies configurations in our build files. And adding this list of jar dependencies is tedious task for the Developers. Adding that much dependency makes build file complex and big in size.

To save us from the lots of dependencies configurations, we have Spring Boot Starter component.

Spring Boot Starter component combines all related jars into single jar file so that we required to add only one jar file dependency to our build files.

In above we have seen, to develop web application we need to add 4 jars. Now Instead of adding above 4 jars our build file, we need to add only one jar file: “spring-boot-starter-web” in our build file.

When we add “spring-boot-starter-web” jar file dependency to our build file, then Spring Boot Framework will automatically download all required jars and add to our project classpath.

That’s it about Spring Boot Starter component.

Spring Boot CLI

Spring Boot CLI also known as Spring Boot Command Line Interface. It is a Spring Boot tool that allow to run and test Spring Boot applications using command prompt.

When we run Spring Boot applications using CLI, it internally uses Spring Boot Starter and Spring Boot AutoConfigurate components to resolve all dependencies and execute the application.

We can run even Spring Web Applications with simple Spring Boot CLI Commands.

Spring Boot CLI basically run the Groovy scripts. It allows you to quickly develop Spring Framework applications. Groovy scripts is very similar to Java but without boilerplate code.

Spring Boot Actuator

Spring Boot Actuator is also a very important Component of the Spring Boot. It helps to monitor the sprint boot applications health , understand traffics, knowing the state of the database, operational information about the running application like metrics, info, dump, env. Spring Boot Actuator also Provides production-grade tools without having to actually implement these features ourselves.

The Three main features of Spring Boot Actuator are

Endpoints
Metrics
Audit
Whenever we run  the Spring Boot Web Application, Spring Boot Actuator provides hostname as “localhost” and default port number as “8080”. We can access this application using “https://localhost:8080/” end point.

----

Q2). Tell some List of Sprint Boot Actuator EndPoints
Ans: Some of Spring Boot Actuator End Point are:

auditevents: This endpoint Exposes the audit events information for the current application.
beans: Displays the list of all the Spring beans of application.
health: Display the health information of spring boot application.
caches: Exposes the all available caches.
env: Exposes the  all properties from Spring’s ConfigurableEnvironment.
metrics: It Shows the ‘metrics’ information for the current application.
There are some more Spring Actuator endpoints are loggers, mappings, sessions, shutdown, flyway, conditions, etc

----

Q3). Tell us some benefits of Spring Boot over Spring?
Ans: Spring boot framework is the extension of spring framework to help developers to start coding with low configuration. It eliminates the boilerplate configurations required for setting up a Spring application. 

Spring Boot comes with multiple starter dependencies for different Spring modules. 

Some of the most commonly used dependencies are :

spring-boot-starter-web
spring-boot-starter-data-jpa
spring-boot-starter-security
spring-boot-starter-test
spring-boot-starter-thymeleaf
spring-boot-starter-actuator
Below are the features provided by spring boot but spring doesn’t

Starter POM
Auto Configuration
Component Scanning
Embedded server
InMemory DB
Actuators
Version Management

----

Q4). What is the starter dependency of the Spring boot module?
Ans:

Some of Spring Boot Starter Dependencies are

Spring Boot Starter web: Important features of spring-boot-starter-web are It is compatible for web development and Provides Auto configuration. This spring-boot-starter-web dependency pulls all dependencies which is used in the Spring Boot web development.

Below is the code to add Spring Boot Starter web in Spring Boot project using POM.xml.

<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-web</artifactId>
</dependency>
Spring Boot Starter Actuator : This dependency is used to monitor and manage the Spring Boot application. Below is the code to add Spring Boot Starter Actuator in Spring Boot project using POM.xml.

<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-actuator</artifactId>
</dependency> 
Spring Boot Starter Security: This dependency is used in Spring Boot application    to add the Security in Spring Boot Application.

Below is the code to add Spring Boot Starter Security in Spring Boot project using POM.xml.

<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-security</artifactId>
</dependency> 
Spring Boot Starter ThymeLeaf : Spring Boot Starter ThymeLeaf Dependency  is used to create a web application. It provides a good support for serving a XHTML/HTML5 in web applications.

Below is the code to add Spring Boot Starter ThymeLeaf in Spring Boot project using POM.xml.

<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-thymeleaf</artifactId>
</dependency> 
Spring Boot Starter Test: This dependency is used in Spring Boot Application to write the Unit Test cases of Java methods. Below is the code to add Spring Boot Starter Test in Spring Boot project using POM.xml.

<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-test</artifactId>
</dependency>

----

Q5). What is Spring Boot dependency management.
Ans: Spring Boot dependency management system manages dependencies and configuration automatically. We need not to specify the version of the dependencies in our configuration file. Spring Boot automatically upgrades all dependencies added in configuration file when we update the Spring Boot version.

----

Q6) How does Spring Boot works Internally?
Ans:

When we Create Spring Boot Application we add the starter Dependencies in it. This Starter Dependencies automatically configures Spring Boot application based on the dependencies you have added to the project. We add @EnableAutoConfiguration annotation for the configuration.

Suppose if you have not configured any database connection, Spring Boot auto-configures an in-memory database.

The entry point of the spring boot application is the class contains @SpringBootApplication annotation and the main method.

@ComponentScan annotation scans all the components included in the Spring Boot Application automatically.

----

Q7). Explain Auto Configuration in Spring Boot.
Ans:

Spring Boot Auto Configuration , configures Spring application based on the dependencies we have added in the project.

For Autoconfiguration we will add @EnableAutoConfiguration

annotation or @SpringBootApplication annotation in main class file. This annotation will automatically automatically configure Spring Boot application.

Lets see the below example for better understanding.

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.EnableAutoConfiguration;
@EnableAutoConfiguration
public class SpringBootApplicationDemo {
   public static void main(String[] args) {
      SpringApplication.run(SpringBootApplicationDemo.class, args);
   }
}
Spring Boot Application

Class that  contains  @SpringBootApplication annotation denotes the entry point of the Spring Boot Application. This class should have the main method to run the Spring Boot application. @SpringBootApplication annotation includes Auto- Configuration, Component Scan, and Spring Boot Configuration.

If we add @SpringBootApplication annotation in java class, we need not to add any other annotation like @EnableAutoConfiguration, @ComponentScan and @SpringBootConfiguration.

We can say SpringBootApplication  = EnableAutoConfiguration + ComponentScan + SpringBootConfiguration.

Below example show how we can use SpringBootApplication annotations.

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
@SpringBootApplication
public class SpringBootApplicationDemo {
   public static void main(String[] args) {
      SpringApplication.run(SpringBootApplicationDemo.class, args);
   }
}
Component Scan

In Spring Boot application @ComponentScan annotation scan all your components that is added in your project. This annotation scans all the beans and package declarations when the application initializes.

Without writing any explicit code, Spring will Scan our application for classes annotated with @Component, Instantiate them and inject any specified dependencies into them and Inject them wherever needed.

Below is the example of using component scan

import org.springframework.boot.SpringApplication;
import org.springframework.context.annotation.ComponentScan;
@ComponentScan
public class SpringBootApplicationDemo {
   public static void main(String[] args) {
      SpringApplication.run(SpringBootApplicationDemo.class, args);
   }
}

----

Q8) How does a spring boot application get started?
Ans:

Spring Boot application Looks for the class having @SpringBootApplication annotation with main method. This method serves as an entry point, which invokes the SpringApplication.run method to start the application.

@SpringBootApplication 
public class SpringBootApplicationDemo{    
       public static void main(String[] args) {        
             SpringApplication.run(SpringBootApplicationDemo.class); 
       } 
}

----

Q9) Tell some commonly used Spring Boot CLI commands?
Ans:

Some commonly used Spring Boot CLI Commands Are:
-run, -test, -install, -uninstall, -grap, -jar, -war, –init, -shell, -help etc

----

Q10) Tell Some Basic Annotations used in Spring Boot?
Ans:

The Spring Boot annotations reside in its org.springframework.boot.autoconfigure package and its sub-packages.

Some Common and Important Spring Boot Annotations are:

@EnableAutoConfiguration – It makes Spring Boot look for auto-configuration beans on its classpath and automatically apply them.

@SpringBootApplication – This annotation is used to denote the main class of a Boot Application. This annotation combines @Configuration, @EnableAutoConfiguration, and @ComponentScan annotations with their default attributes.

Some More annotations of Spring Boot are:

For Application Basic Setup

@SpringBootApplication

@ComponentScan

@Configuration

@EnableAutoConfiguration

For Request Response

@GetMapping

@PostMapping

@RequestMapping

For Component Types

@Repository

@Service

@Component

@Controller

----

Q11) What is Spring Boot dependency management?
Ans:

Spring Boot manages dependencies and configuration automatically. We don’t need to mention the version of the dependencies in our configuration. We can say Dependency Management as it is a way to manage the dependencies efficiently in one place. When we update the Spring Boot version Spring Boot upgrades all dependencies automatically.

----

Q12) How you can change the port of embedded Tomcat server in Spring Boot?
Ans:

There are two ways to change the default port of server in Spring Boot

1). Using application.properties file

server.port = 8081

In the application.properties file just change the default value of port to value what you wanted to be. Here we have given 8081 as a new port value.

2). Using application.yaml file

Server:

   Port:8081

Also you can change the port value from application.yaml by changing the default value of port to value what you wanted to be. Here we have also given 8081 as a new port value.

----

Q13). How you can change the tomcat server to any other Server in Spring Boot?
Ans:

To Replace the embedded tomcat server in Spring Boot first we have to exclude the default server from the pom.xml. And to  add new server we will add the new dependency.

For example:

To exclude tomcat from starter dependency add below code in pom.xml

<dependency>  
  <groupId>org.springframework.boot</groupId>  
  <artifactId>spring-boot-starter-web</artifactId>
  <exclusions>    
   <exclusion>      
    <groupId>org.springframework.boot</groupId>      
    <artifactId>spring-boot-starter-tomcat</artifactId>    
   </exclusion>  
  </exclusions>
</dependency>
And to include new server add as a dependency. Below is the example to add jetty server.

<dependency>  
  <groupId>org.springframework.boot</groupId>  
  <artifactId>spring-boot-starter-jetty</artifactId>
</dependency>

----

Q14) What is @RestController annotation in Sprint boot?
Ans: 

@RestController  annotation is a combination of @Controller and @ResponseBody annotation. It is used to make restful web services and also it converts the response to JSON or XML. This annotation is used at the class level and it allows class to handle the requests made by the client.

----

Q15). What is the difference between @Controller and @RestController?
Ans: 

With @controller annotation class is responsible for preparing a model Map with data to be displayed by the view But @RestController annotation class is responsible  for creating Restful controllers.
@controller only behave as controller, we need to add @responsebody annotation with method to return value and writes it to the HTTP response. But @RestController annotation is a combination of @controller and @responsebody which by default converts return as HTTP Response.
@Controller is used to mark classes as Spring MVC Controller whereas @RestController annotation mark class as RESTful Web services.
In @Controller, we need to use @ResponseBody on every handler method but in @RestController we don’t need to use @ResponseBody on every handler method.
@Controller annotation added in Spring 2.0 version whereas @RestController annotation added in Spring 4.0 version.

----

Q16). What is the difference between RequestMapping and GetMapping?
Ans:


RequestMapping annotation is used with GET, POST, PUT, and other request methods. getMapping is an extension of RequestMapping which helps you to improve on clarity of requests.
@RequestMapping annotation is used on a class level but the @GetMapping is used on method-level

----

Q17). What is Actuator in Spring Boot?
Ans: An actuator in Spring boot is a feature  that helps you to monitor and manage your application when you push it to production. These actuators include auditing, health, CPU usage, HTTP hits, metric gathering, and many more that are automatically applied to your application.

----

Q18). What is the process to enable Actuator in Spring boot application?
Ans:

To enable the spring actuator feature, we need to add the dependency of “spring-boot-starter-actuator” in pom.xml.

Below is the xml snippet that can be added 

<dependency>
<groupId> org.springframework.boot</groupId>
<artifactId> spring-boot-starter-actuator </artifactId>
</dependency>

----

Q19). Tell some endpoint actuator-provide to monitor the Spring boot application?
Ans:

Actuators provide below pre-defined endpoints to monitor our application –

Health
Info
Beans
Mappings
Configprops
Httptrace
Heapdump
Threaddump
Shutdown
Q20). What is the use of Profiles in spring boot?
Ans:

To Complete the development process of an application  or we can say during  the development of any application, we deal with multiple environments such as dev, test and Prod. Sometime we need specific configuration at each environment level. Suppose we are using an embedded H2 database for dev but for prod, we might have proprietary Oracle.

A profile is a set of configuration settings. Spring Boot allows to define profile specific property files in the form of application-{profile}.properties. It automatically loads the properties in an application.properties file for all profiles, and the ones in profile-specific property files only for the specified profile. 


spring boot interview question

----

Q21). What is dependency Injection in Spring Boot?
Ans:

The process of injecting dependent objects into target class is called dependency injection. Suppose our one class is dependent on the another class object. In that case we will provide the other class object to our class. This process is known as dependency injections.

There are multiple ways to inject the dependencies.

Setter Injection: The IOC container will inject the dependent bean object into the target bean object by calling the setter method.
Constructor Injection: Here IOC container will pass the dependent object via constructor of the class.
Class Student(private val school:School){
    Fun markAttendence(){
        school.mark();
    }
}
Field Injection: Here dependency object will directly pass in a field in the target class.
Class Student {
  Public val school :School;
  Fun markAttendence(){
    school.mark();
  }
}
Q22). What is an IOC container?

----

Ans: IoC Container is a framework for implementing automatic dependency injection. It manages object creation and its life-time and also injects dependencies into the class.

Q23). Tell the steps how you will create spring boot project using Spring Initializer.

----

Ans:

Spring Initializr is a web tool provided by Spring. Using this tool we can create Spring boot projects by providing project details and giving the jar dependencies details needed for our project.

Let’s see the procedure step by step to create a spring boot project:

First, go to the browser and browse for spring intializr.
Now Choose the project type maven. Give the details like project name, Group and Artifact details, etc. Now select the required dependencies for the projects. Click on Generate Project and it will download a project to your system.
After the download of the project extracts this project into your system.
Open your IDE like eclipse or STS and import the downloaded and extracted project file using the import project option in IDE.
After the import project will take some time to internal build and download the dependencies.
Now you are done with the creation of the spring boot project.
Q24). Tell me the Advantages of the YAML file Over Properties file.
Ans:The advantage of the YAML file over the properties file in Spring Boot is, that YAML Stores data in a hierarchical format but the properties file does not. YAML file makes easy to read and debug the file for developers. The SpringApplication class supports the YAML file as an alternative to properties whenever you use the SnakeYAML library on your classpath. One more great advantage of YAML is suppose we have different deployment profiles such as  development, testing, or production,  so instead of creating new files for each environment we can place all the details in a single YAML file. Which is not possible in the case of properties file.

----

Q25). Tell some difference between @RequestParam vs @PathVariable Annotations.
Ans:


1). @RequestParams extract values from the query string and @PathVariables extract values from the URI path.

Example of Pathvariable:

Suppose our url structure is http://localhost:8080/springproject/xyz
Then we will use @pathVariable annotation like below to extract some value from the URLs

@GetMapping("/springproject/{id}")
@ResponseBody
public String getIdUsingPathVariable (@PathVariable String id) {
return "ID: " + id;
}
Here id will be print as “xyz”

Or we can also write

@GetMapping("/springproject/{id}")
@ResponseBody
public String getIdUsingPathVariable (@PathVariable("id") String id) {
return "ID: " + id;
}
Example of @RequestParam

Suppose our url structure is http://localhost:8080/springproject?id=xyz
Then we will use @ RequestParam annotation like below to extract some value from the URLs

@GetMapping("/foos")
@ResponseBody
public String getIdUsingRequestParam(@RequestParam("id") String id) {
return "ID: " + id;
}
Here id will be return as “xyz”.

2). @RequestParam encoded the value from url but @PathVariable extracting values from the URI path is not encoded.

@PathVariable Example:
If the url will be like http://localhost:8080/springproject/x+y
Output will be x+y
Here url value is not decoded.

@RequestParam Example:
http://localhost:8080/springproject?id=x+y

Output will be x y
Here url value is decoded

3). We can make @RequestParam and @PathVariable optional with the help of required attribute.
Below is a example

@GetMapping("/optional/{id}")
@ResponseBody
public String getIdUsingPathVariable(@PathVariable(required = false) String id) {    
  return "ID: " + id;
}
For Url http://localhost:8080/optional/xyz
Output will be xyz
And for Url http://localhost:8080/optional/
Ouput will be null

Q26). Tell something about Spring @GetMapping, @PostMapping, @PutMapping, @DeleteMapping and @PatchMapping
Ans:

@GetMapping – It is a shortcut for @RequestMapping(method = RequestMethod.GET)


It is used to get single or all values from the database in Spring Application.

@PostMapping – It is a shortcut for @RequestMapping(method = RequestMethod.POST)

Method that has @PostMapping annotation is responsible to Create single or multiple entries in the database.

It is used to create single or multiple value in the database in Spring Application.

@PutMapping – It is a shortcut for @RequestMapping(method = RequestMethod.PUT)

Method that has @PutMapping annotation is responsible to update the data in the database.

@PatchMapping – It is a shortcut for @RequestMapping(method = RequestMethod.PATCH)

@PatchMapping  annotation is used when we want to apply a partial update on the database.

@DeleteMapping – It is a shortcut for @RequestMapping(method =RequestMethod.DELETE)

It is used to Delete single or multiple value from the database in the Spring Application.

----

Q27). What is Thymeleaf in Spring Boot?
Ans:Thymeleaf is a server-side Java-based template engine. It is used for both web and standalone environments. It is capable of processing HTML, XML, JavaScript, CSS and even plain text. 

----

Q28). Tell some embedded containers supported by Spring Boot.
Ans:

There are three embedded containers supported by Spring Boot are :

Tomcat (used by default)
Undertow
Jetty

----

Q4). Are exit () and return statements same in function definition?
Ans:No, both are different as we used exit() to immediately exit from the program, where as return is used to return the control of programs execution from the called function to calling function.

----

Q5). When is the “void” keyword used in a function?
Ans:When we declare the function we have to decide whether we want some return value from the function or not, if we only want to print some value or statements on the screen we use void on the left side of function name otherwise we place the data type of the value on the left side of function name.

----

Q6). Differentiate between call by value and call by reference.
Ans:

Factor

Call by Value

Call by Reference

Safety

In call by value actual parameters are safe because operations are performed on formal parameter.

In call by value operations are performed on actual parameters so it is not safe here.

Memory Location

In this separate memory locations are created for actual and formal parameters

In this actual and Formal parameters share the same memory space.

Parameters

In this copy of actual parameters are passed.


In this actual parameters are passed.

----

Q7). Explain rand() function in c. Write a program in c to generate a random number.
Ans: The rand() function in c is used to generate a random number.

</https://quescol.com/interview-preparation/spring-boot-interview-questions>

<https://javarevisited.blogspot.com/2015/10/133-java-interview-questions-answers-from-last-5-years.html#axzz80dfcO0nd>

130+ Java Interview Questions Answers for 2 to 7 Year Experienced Programmers

Time is changing and so is Java interviews. Gone are the days, when knowing the difference between String and StringBuffer can help you to go through the second round of interview, questions are becoming more advanced and interviewers are asking more deep questions. When I started my career, questions like Vector vs Array and HashMap vs Hashtable were the most popular ones and just memorizing them gives you a good chance to do well in interviews, but not anymore. Nowadays, you will get questions from the areas where not many Java programmer looks e.g. NIO, patterns, sophisticated unit testing or those which are hard to master e.g. concurrency, algorithms, data structures and coding.

Since I like to explore interview questions, I have got this huge list of questions with me, which contains lots and lots of questions on different topics. I have been preparing this MEGA list for quite some time and now It's ready to share with you guys.

It contains interview questions not only from classic topics like threads, collections, equals and hashcode, sockets but also from NIO, array, string, Java 8, and much more.

It has questions for both entry-level Java programmers and senior developers with years of experience. No matter whether you are a Java developer of 1, 2, 3, 4, 5, 6, 8, 9, or even 10 years of experience, you will find something interesting in this list. 

It contains questions that are super easy to answer, and also, a question that is tricky enough for even seasoned Java programmers. If you need more questions then you can also check out these Java Interview Courses and books to better prepare yourself. 


Top 5 Courses to Learn Eclipse IDE for Java Programmers - Best of Lot
Given the list is long and we have questions from everywhere, it's imperative that answers must be short, concise, and crisp, with no fluffing at all. So apart from this paragraph, you will only hear from me in the questions and answers, no more context, no more feedback, and no more evaluation.

For that, I have already written blog posts, where you can find my views on a particular question, e.g. why I like that question, what makes them challenging, and what kind of answer you should expect from candidates.

This list is a little bit different and I encourage you to share questions and answers in a similar way so that it should be easy to revise. 

I hope this list can be of great use for both interviewer and candidates, the interviewer can, of course, but a little variety on questions to bring novelty and surprise element, which is important for a good interview. While a candidate, can expand and test their knowledge about key areas of Java programming language and platform.

Nowadays and in coming years the focus will be more on advanced concurrency concepts, JVM internals, 32-bit vs 64-bit JVM, unit testing, and clean code. I am sure, once you read through this MEGA list of Java interview questions, you should be able to do well on both telephonic and face-to-face programming interviews.

I have also written a book for Java interviews, Grokking the Java Interview, and Grokking the Spring Boot Interview, where I have shared tips, tricks and frequently asked Java questions from different topics. If you are keen to do well and better prepare for Java interviews, you can also take a look at that. If you want to buy, use the code - friends20 to get a 20% discount because you are already my reader. 


Important Topics for Java Interviews
Apart from quantity, as you can see with a huge number of questions, I have worked hard to maintain quality as well. I have not only shared questions from all important topics but also ensured to include so-called advanced topics which many programmers do not prefer to prepare or just left out because they have not worked on that.

Java NIO and JVM internals questions are the best examples of that. You can keep design patterns also on the same list but a growing number of experienced programmers are now well aware of GOF design patterns and when to use them. 

I have also worked hard to keep this list up-to-date to include what interviewers are asking nowadays and what will be their core focus in the coming years. To give you an idea, this list of Java interview questions includes the following topics:
Multithreading, concurrency, and thread basics
Date type conversion and fundamentals
Garbage Collection
Java Collections Framework
Array
String
GOF Design Patterns
SOLID design principles
Abstract class and interface
Java basics like equals() and hashcode
Generics and Enum
Java IO and NIO
Common Networking protocols
Data structure and algorithm in Java
Regular expressions
JVM internals
Java Best Practices
JDBC
Date, Time, and Calendar
XML Processing in Java
JUnit
Programming

You guys are also lucky that nowadays there are some good books available to prepare for Java interviews, one of them which I particularly find useful and interesting to read is Java Programming Interview Exposed by Markham. It will take you to some of the most important topics for Java and JEE interviews, worth reading even if you are not preparing for a Java interview.

Top 120 Java Interview Questions Answers
So now the time has come to introduce you to this MEGA list of 120 Java questions collected from various interviews of last 5 years. I am sure you have seen many of these questions personally on your interviews and many of you would have answered them correctly as well.


Multithreading, Concurrency and Thread basics Questions

----

1) Can we make array volatile in Java?
This is one of the tricky Java multi-threading questions you will see in senior Java developer Interview. Yes, you can make an array volatile in Java but only the reference which is pointing to an array, not the whole array. What I mean, if one thread changes the reference variable to points to another array, that will provide a volatile guarantee, but if multiple threads are changing individual array elements they won't be having happens before guarantee provided by the volatile modifier.

----

2) Can volatile make a non-atomic operation to atomic?
This another good question I love to ask on volatile, mostly as a follow-up of the previous question. This question is also not easy to answer because volatile is not about atomicity, but there are cases where you can use a volatile variable to make the operation atomic.

One example I have seen is having a long field in your class. If you know that a long field is accessed by more than one thread e.g. a counter, a price field or anything, you better make it volatile. Why? because reading to a long variable is not atomic in Java and done in two steps, If one thread is writing or updating long value, it's possible for another thread to see half value (fist 32-bit). While reading/writing a volatile long or double (64 bit) is atomic.

----


3) What are practical uses of volatile modifier? 
One of the practical use of the volatile variable is to make reading double and long atomic. Both double and long are 64-bit wide and they are read in two parts, first 32-bit first time and next 32-bit second time, which is non-atomic but volatile double and long read is atomic in Java. Another use of the volatile variable is to provide a memory barrier, just like it is used in Disrupter framework. Basically, Java Memory model inserts a write barrier after you write to a volatile variable and a read barrier before you read it. Which means, if you write to volatile field then it's guaranteed that any thread accessing that variable will see the value you wrote and anything you did before doing that right into the thread is guaranteed to have happened and any updated data values will also be visible to all threads, because the memory barrier flushed all other writes to the cache.

----

4) What guarantee volatile variable provides? (answer)
volatile variables provide the guarantee about ordering and visibility e.g. volatile assignment cannot be re-ordered with other statements but in the absence of any synchronization instruction compiler, JVM or JIT are free to reorder statements for better performance. volatile also provides the happens-before guarantee which ensures changes made in one thread is visible to others. In some cases volatile also provide atomicity e.g. reading 64-bit data types like long and double are not atomic but read of volatile double or long is atomic.




5) Which one would be easy to write? synchronization code for 10 threads or 2 threads?
In terms of writing code, both will be of same complexity because synchronization code is independent of a number of threads. Choice of synchronization though depends upon a number of threads because the number of thread present more contention, so you go for advanced synchronization technique e.g. lock stripping, which requires more complex code and expertise.


6) How do you call wait() method? using if block or loop? Why? (answer)
wait() method should always be called in loop because it's possible that until thread gets CPU to start running again the condition might not hold, so it's always better to check condition in loop before proceeding. Here is the standard idiom of using wait and notify method in Java:
// The standard idiom for using the wait method
synchronized (obj) {
   while (condition does not hold)
      obj.wait(); // (Releases lock, and reacquires on wakeup)
      ... // Perform action appropriate to condition
}
See Effective Java Item 69 to learn more about why wait method should call in the loop.

----


7)  What is false sharing in the context of multi-threading? 
false sharing is one of the well-known performance issues on multi-core systems, where each process has its local cache. false sharing occurs when threads on different processor modify variables that reside on same cache line as shown in the following image:

Java Interview questions for experienced programmers

False sharing is very hard to detect because the thread may be accessing completely different global variables that happen to be relatively close together in memory. Like many concurrency issues, the primary way to avoid false sharing is careful code review and aligning your data structure with the size of a cache line.


----

8) What is busy spin? Why should you use it?
Busy spin is one of the technique to wait for events without releasing CPU. It's often done to avoid losing data in CPU cached which is lost if the thread is paused and resumed in some other core. So, if you are working on low latency system where your order processing thread currently doesn't have any order, instead of sleeping or calling wait(), you can just loop and then again check the queue for new messages. It's only beneficial if you need to wait for a very small amount of time e.g. in micro seconds or nano seconds. LMAX Disrupter framework, a high-performance inter-thread messaging library has a BusySpinWaitStrategy which is based on this concept and uses a busy spin loop for EventProcessors waiting on the barrier.


----

9) How do you take thread dump in Java?
You can take a thread dump of Java application in Linux by using kill -3 PID, where PID is the process id of Java process. In Windows, you can press Ctrl + Break. This will instruct JVM to print thread dump in standard out or err and it could go to console or log file depending upon your application configuration. If you have used Tomcat then when


----


10) is Swing thread-safe? (answer)
No, Swing is not thread-safe. You cannot update Swing components e.g. JTable, JList or JPanel from any thread, in fact, they must be updated from GUI or AWT thread. That's why swings provide invokeAndWait() and invokeLater() method to request GUI update from any other threads. This methods put update request in AWT threads queue and can wait till update or return immediately for an asynchronous update. You can also check the detailed answer to learn more.


----

11) What is a thread local variable in Java? (answer)
Thread-local variables are variables confined to a thread, its like thread's own copy which is not shared between multiple threads. Java provides a ThreadLocal class to support thread-local variables. It's one of the many ways to achieve thread-safety. Though be careful while using thread local variable in manged environment e.g. with web servers where worker thread out lives any application variable. Any thread local variable which is not removed once its work is done can potentially cause a memory leak in Java application.


----

12) Write wait-notify code for producer-consumer problem? (answer)
Please see the answer for a code example. Just remember to call wait() and notify() method from synchronized block and test waiting for condition on the loop instead of if block.


----

13) Write code for thread-safe Singleton in Java? (answer)
Please see the answer for a code example and step by step guide to creating thread-safe singleton class in Java. When we say thread-safe, which means Singleton should remain singleton even if initialization occurs in the case of multiple threads. Using Java enum as Singleton class is one of the easiest ways to create a thread-safe singleton in Java.

----


14) The difference between sleep and wait in Java? (answer)
Though both are used to pause currently running thread, sleep() is actually meant for short pause because it doesn't release lock, while wait() is meant for conditional wait and that's why it release lock which can then be acquired by another thread to change the condition on which it is waiting.

----


15) What is an immutable object? How do you create an Immutable object in Java? (answer)
Immutable objects are those whose state cannot be changed once created. Any modification will result in a new object e.g. String, Integer, and other wrapper class. Please see the answer for step by step guide to creating Immutable class in Java.

----


16) Can we create an Immutable object, which contains a mutable object?
Yes, its possible to create an Immutable object which may contain a mutable object, you just need to be a little bit careful not to share the reference of the mutable component, instead, you should return a copy of it if you have to. Most common example is an Object which contain the reference of java.util.Date object.



Date types and Basic Java Interview Questions

----

17) What is the right data type to represent a price in Java? (answer)
BigDecimal if memory is not a concern and Performance is not critical, otherwise double with predefined precision.


----

18) How do you convert bytes to String? (answer)
you can convert bytes to the string using string constructor which accepts byte[], just make sure that right character encoding otherwise platform's default character encoding will be used which may or may not be same.


----

19) How do you convert bytes to long in Java? (answer)
This questions if for you to answer :-)

----


20) Can we cast an int value into byte variable? what will happen if the value of int is larger than byte?
Yes, we can cast but int is 32 bit long in java while byte is 8 bit long in java so when you cast an int to byte higher 24 bits are lost and a byte can only hold a value from -128 to 128.

----


21) There are two classes B extends A and C extends B, Can we cast B into C e.g. C = (C) B; (answer)

----


22) Which class contains clone method? Cloneable or Object? (answer)
java.lang.Cloneable is marker interface and doesn't contain any method clone method is defined in the object class. It is also knowing that clone() is a native method means it's implemented in C or C++ or any other native language.


----

23) Is ++ operator is thread-safe in Java? (answer)
 No it's not a thread safe operator because its involve multiple instructions like reading a value, incriminating it and storing it back into memory which can be overlapped between multiple threads.

----


24) Difference between a = a + b and a += b ? (answer)
The += operator implicitly cast the result of addition into the type of variable used to hold the result. When you add two integral variable e.g. variable of type byte, short, or int then they are first promoted to int and them addition happens. If result of addition is more than maximum value of a then a + b will give compile time error but a += b will be ok as shown below
byte a = 127;
byte b = 127;
b = a + b; // error : cannot convert from int to byte
b += a; // ok

----


25) Can I store a double value in a long variable without casting? (answer)
No, you cannot store a double value into a long variable without casting because the range of double is more  that long and you we need to type cast. It's not dificult to answer this question but many develoepr get it wrong due to confusion on which one is bigger between double and long in Java.


----

26) What will this return 3*0.1 == 0.3? true or false? (answer)
This is one of the really tricky questions. Out of 100, only 5 developers answered this question and only of them have explained the concept correctly. The short answer is false because some floating point numbers can not be represented exactly.

----


27) Which one will take more memory, an int or Integer? (answer)
An Integer object will take more memory an Integer is the an object and it  store meta data overhead about the object and int is primitive type so its takes less space.

----


28) Why is String Immutable in Java? (answer)
One of my favorite Java interview question. The String is Immutable in java because java designer thought that string will be heavily used and making it immutable allow some optimization easy sharing same String object between multiple clients. See the link for the more detailed answer. This is a great question for Java programmers with less experience as it gives them food for thought, to think about how things works in Java, what Jave designers might have thought when they created String class etc.

----

29) Can we use String in the switch case? (answer)
Yes from Java 7 onward we can use String in switch case but it is just syntactic sugar. Internally string hash code is used for the switch. See the detaiedl answer for more explanation and discussion.

----

30) What is constructor chaining in Java? (answer)
When you call one constructor from other than it's known as constructor chaining in Java. This happens when you have multiple, overloaded constructor in the class.



JVM Internals and Garbage Collection Interview Questions
In last a couple of years I have seen increased focus on JVM internal and Garbage collection tuning, monitoring Java appliation, dealing with Java performance issues on various Java interviews. This is actually become the prime topic for interviewing any experienced Java developer for senior position e.g. technical lead, VP or team lead. If you feel you are short of experience and knowledge in this area then you should read atleast one book mentioned in my list of Java Performance books. I vote goes to Java Performance, The Definitive guide by Scott.

----

31) What is the size of int in 64-bit JVM?
The size of an int variable is constant in Java, it's always 32-bit irrespective of platform. Which means the size of primitive int is same in both 32-bit and 64-bit Java virtual machine.

----

32) The difference between Serial and Parallel Garbage Collector? (answer)
Even though both the serial and parallel collectors cause a stop-the-world pause during Garbage collection. The main difference between them is that a serial collector is a default copying collector which uses only one GC thread for garbage collection while a parallel collector uses multiple GC threads for garbage collection.

----

33) What is the size of an int variable in 32-bit and 64-bit JVM? (answer)
The size of int is same in both 32-bit and 64-bit JVM, it's always 32 bits or 4 bytes.

----

34) A difference between WeakReference and SoftReference in Java? (answer)
Though both WeakReference and SoftReference helps garbage collector and memory efficient, WeakReference becomes eligible for garbage collection as soon as last strong reference is lost but SoftReference even thought it can not prevent GC, it can delay it until JVM absolutely need memory.

----

35) How do WeakHashMap works? (answer)
WeakHashMap works like a normal HashMap but uses WeakReference for keys, which means if the key object doesn't have any reference then both key/value mapping will become eligible for garbage collection.

----

36) What is -XX:+UseCompressedOops JVM option? Why use it? (answer)
When you go migrate your Java application from 32-bit to 64-bit JVM, the heap requirement suddenly increases, almost double, due to increasing size of ordinary object pointer from 32 bit to 64 bit. This also adversely affect how much data you can keep in CPU cache, which is much smaller than memory. Since main motivation for moving to 64-bit JVM is to specify large heap size, you can save some memory by using compressed OOP. By using -XX:+UseCompressedOops, JVM uses 32-bit OOP instead of 64-bit OOP.

----


37) How do you find if JVM is 32-bit or 64-bit from Java Program? (answer)
You can find that by checking some system properties like sun.arch.data.model or os.arch


----

38) What is the maximum heap size of 32-bit and 64-bit JVM? (answer)
Theoretically, the maximum heap memory you can assign to a 32-bit JVM is 2^32 which is 4GB but practically the limit is much smaller. It also varies between operating systems e.g. form 1.5GB in Windows to almost 3GB in Solaris. 64-bit JVM allows you to specify larger heap size, theoretically 2^64 which is quite large but practically you can specify heap space up to 100GBs. There are even JVM e.g. Azul where heap space of 1000 gigs is also possible.

----


39) What is the difference between JRE, JDK, JVM and JIT? (answer)
JRE stands for Java run-time and it's required to run Java application. JDK stands for Java development kit and provides tools to develop Java program e.g. Java compiler. It also contains JRE. The JVM stands for Java virtual machine and it's the process responsible for running Java application. The JIT stands for Just In Time compilation and helps to boost the performance of Java application by converting Java byte code into native code when the crossed certain threshold i.e. mainly hot code is converted into native code.

Java Interview Questions for 3 years experience


----

40) Explain Java Heap space and Garbage collection? (answer)
When a Java process is started using java command, memory is allocated to it. Part of this memory is used to create heap space, which is used to allocate memory to objects whenever they are created in the program. Garbage collection is the process inside JVM which reclaims memory from dead objects for future allocation.

JVM Internals Java Interview Questions Answers

----


41) Can you guarantee the garbage collection process? (answer)
No, you cannot guarantee the garbage collection, though you can make a request using System.gc() or Runtime.gc() method.


----

42) How do you find memory usage from Java program? How much percent of the heap is used?
You can use memory related methods from java.lang.Runtime class to get the free memory, total memory and maximum heap memory in Java.  By using these methods, you can find out how many percents of the heap is used and how much heap space is remaining. Runtime.freeMemory() return amount of free memory in bytes, Runtime.totalMemory() returns total memory in bytes and Runtime.maxMemory() returns maximum memory in bytes.


----

43) What is the difference between stack and heap in Java? (answer)
Stack and heap are different memory areas in the JVM and they are used for different purposes. The stack is used to hold method frames and local variables while objects are always allocated memory from the heap. The stack is usually much smaller than heap memory and also didn't shared between multiple threads, but heap is shared among all threads in JVM.

Java Interview Questions and Answers on Memory


----


Basic Java concepts Interview Questions
44) What's the difference between "a == b" and "a.equals(b)"? (answer)
The a = b does object reference matching if both a and b are an object and only return true if both are pointing to the same object in the heap space, on the other hand, a.equals(b) is used for logical mapping and its expected from an object to override this method to provide logical equality. For example, String class overrides this equals() method so that you can compare two Strings, which are the different object but contains same letters.

----


45) What is a.hashCode() used for? How is it related to a.equals(b)? (answer)
hashCode() method returns an int hash value corresponding to an object. It's used in hash based collection classes e.g Hashtable, HashMap, LinkedHashMap and so on. It's very tightly related to equals() method. According to Java specification, two objects which are equal to each other using equals() method must have same hash code.


----

46) Difference between final, finalize and finally? (answer)
The final is a modifier which you can apply to variable, methods and classes. If you make a variable final it means its value cannot be changed once initialized. finalize is a method, which is called just before an object is a garbage collected, giving it last chance to resurrect itself, but the call to finalize is not guaranteed. finally is a keyword which is used in exception handling along with try and catch. the finally block is always executed irrespective of whether an exception is thrown from try block or not.

----


47) What is a compile time constant in Java? What is the risk of using it?
public static final variables are also known as a compile time constant, the public is optional there. They are replaced with actual values at compile time because compiler know their value up-front and also knows that it cannot be changed during run-time. One of the problem with this is that if you happened to use a public static final variable from some in-house or third party library and their value changed later than your client will still be using old value even after you deploy a new version of JARs. To avoid that, make sure you compile your program when you upgrade dependency JAR files.


Java Collections Framework Interview Questions
It also contains Data structure and algorithm Interview question in Java, questions on array, linked list, HashMap, ArrayList, Hashtable, Stack, Queue, PriorityQueue, LinkedHashMap and ConcurrentHashMap.

----

48) The difference between List, Set, Map, and Queue in Java? (answer)
The list is an ordered collection which allows duplicate. It also has an implementation which provides constant time index based access, but that is not guaranteed by List interface. Set is unordered collection which

----


49) Difference between poll() and remove() method?
Both poll() and remove() take out the object from the Queue but if poll() fails then it returns null but if remove fails it throws Exception.

----


50) The difference between LinkedHashMap and PriorityQueue in Java? (answer)
PriorityQueue guarantees that lowest or highest priority element always remain at the head of the queue, but LinkedHashMap maintains the order on which elements are inserted. When you iterate over a PriorityQueue, iterator doesn't guarantee any order but iterator of LinkedHashMap does guarantee the order on which elements are inserted.

----


51) Difference between ArrayList and LinkedList in Java? (answer)
The obvious difference between them is that ArrrayList is backed by array data structure, supprots random access and LinkedList is backed by linked list data structure and doesn't supprot random access. Accessing an element with the index is O(1) in ArrayList but its O(n) in LinkedList. See the answer for more detailed discussion.


52) What is a couple of ways that you could sort a collection? (answer)
You can either use the Sorted collection like TreeSet or TreeMap or you can sort using the ordered collection like a list and using Collections.sort() method.


53) How do you print Array in Java? (answer)
You can print an array by using the Arrays.toString() and Arrays.deepToString() method. Since array doesn't implement toString() by itself, just passing an array to System.out.println() will not print its contents but Arrays.toString() will print each element.

54) LinkedList in Java is doubly or singly linked list? (answer)
It's a doubly linked list, you can check the code in JDK. In Eclipse, you can use the shortcut, Ctrl + T to directly open this class in Editor.

55) Which kind of tree is used to implement TreeMap in Java? (answer)
A Red Black tree is used to implement TreeMap in Java.


----

56) What is the difference between Hashtable and HashMap? (answer)
There are many differences between these two classes, some of them are following:
a) Hashtable is a legacy class and present from JDK 1, HashMap was added later.
b) Hashtable is synchronized and slower but HashMap is not synchronized and faster.
c) Hashtable doesn't allow null keys but HashMap allows one null key.
See the answer for more differences between HashMap and Hashtable in Java.


----

57) How HashSet works internally in Java? (answer)
HashSet is internally implemented using an HashMap. Since a Map needs key and value, a default value is used for all keys. Similar to HashMap, HashSet doesn't allow duplicate keys and only one null key, I mean you can only store one null object in HashSet.

----


58) Write code to remove elements from ArrayList while iterating? (answer)
 Key here is to check whether candidate uses ArrayList's remove() or Iterator's remove(). Here is the sample code which uses right way o remove elements from ArrayList while looping over and avoids ConcurrentModificationException.


----

59) Can I write my own container class and use it in the for-each loop?
Yes, you can write your own container class. You need to implement the Iterable interface if you want to loop over advanced for loop in Java, though. If you implement Collection then you by default get that property.


----

60) What is default size of ArrayList and HashMap in Java? (answer)
As of Java 7 now, default size of ArrayList is 10 and default capacity of HashMap is 16, it must be power of 2. Here is code snippet from ArrayList  and HashMap class :
// from ArrayList.java JDK 1.7
private static final int DEFAULT_CAPACITY = 10;  

//from HashMap.java JDK 7
static final int DEFAULT_INITIAL_CAPACITY = 1 << 4; // aka 16


----


61) Is it possible for two unequal objects to have the same hashcode?
Yes, two unequal objects can have same hashcode that's why collision happen in a hashmap.
the equal hashcode contract only says that two equal objects must have the same hashcode it doesn't say anything about the unequal object.

----

62) Can two equal object have the different hash code?
No, thats not possible according to hash code contract.

----


63) Can we use random numbers in the hashcode() method? (answer)
No, because hashcode of an object should be always same. See the answer to learning more about things to remember while overriding hashCode() method in Java.

----


64) What is the difference between Comparator and Comparable in Java? (answer)
The Comparable interface is used to define the  natural order of object while Comparator is used to define custom order. Comparable can be always one, but we can have multiple comparators to define customized order for objects.

----

65) Why you need to override hashcode, when you override equals in Java? (answer)
 Because equals have code contract mandates to override equals and hashcode together .since many container class like HashMap or HashSet depends on hashcode and equals contract.

Java IO and NIO Interview questions
IO is very important from Java interview point of view. You should have a good knowledge of old Java IO, NIO, and NIO2 alsong with some operating system and disk IO fundamentals. Here are some frequently asked questions form Java IO.

66) In my Java program, I have three sockets? How many threads I will need to handle that

67) How do you create ByteBuffer in Java?

68) How do you write and read from ByteBuffer in Java?

69) Is Java BIG endian or LITTLE endian?

70) What is the byte order of ByteBuffer?

71) The difference between direct buffer and non-direct buffer in Java? (answer)

72) What is the memory mapped buffer in Java? (answer)

73) What is TCP NO DELAY socket option?

74) What is the difference between TCP and UDP protocol? (answer)

75) The difference between ByteBuffer and StringBuffer in Java? (answer)



Java Best Practices Interview question
Contains best practices from different parts of Java programming e.g. Collections, String, IO, Multi-threading, Error and Exception handling, design patterns etc. This section is mostly for experience Java developer, technical lead,  AVP, team lead and coders who are responsible for products. If you want to create quality products you must know and follow the best practices.

----

76) What best practices you follow while writing multi-threaded code in Java? (answer)
Here are couple of best practices which I follow while writing concurrent code in Java:
a) Always name your thread, this will help in debugging.
b) minimize the scope of synchronization, instead of making whole method synchronized, only critical section should be synchronized.
c) prefer volatile over synchronized if you can can.
e) use higher level concurrency utilities instead of waitn() and notify for inter thread communication e.g. BlockingQueue, CountDownLatch and Semeaphore.
e) Prefer concurrent collection over synchronized collection in Java. They provide better scalability.

----


77) Tell me few best practices you apply while using Collections in Java? (answer)
Here are couple of best practices I follow while using Collectionc classes from Java:
a) Always use the right collection e.g. if you need non-synchronized list then use ArrayList and not Vector.
b) Prefer concurrent collection over synchronized collection because they are more scalable.
c) Always use interface to a represent and access a collection e.g. use List to store ArrayList, Map to store HashMap and so on.
d) Use iterator to loop over collection.
e) Always use generics with collection.

----


78) Can you tell us at least 5 best practice you use while using threads in Java? (answer)
This is similar to the previous question and you can use the answer given there. Particularly with thread, you should:
a) name your thread
b) keep your task and thread separate, use Runnable or Callable with thread pool executor.
c) use thread pool
d) use volatile to indicate compiler about ordering, visibility, and atomicity.
e) avoid thread local variable because incorrect use of ThreadLocal class in Java can create a memory leak.
Look there are many best practices and I give extra points to the developer which bring something new, something even I don't know. I make sure to ask this question to Java developers of 8 to 10 years of experience just to gauge his hands on experience and knowledge.


----

79) Name 5 IO best practices? (answer)
IO is very important for performance of your Java application. Ideally you should avoid IO in critical path of your application. Here are couple of Java IO best practices you can follow:
a) Use buffered IO classes instead of reading individual bytes and char.
b) Use classes from NIO and NIO2
c) Always close streams in finally block or use try-with-resource statements.
d) use memory mapped file for faster IO.
If a Java candidate doesn't know about IO and NIO, especially if he has at least 2 to 4 years of experience, he needs some reading.


80) Name 5 JDBC best practices your follow? (answer)
Another good Java best practices for experienced Java developer of 7 to 8 years experience. Why it's important? because they are the ones which set the trend in the code and educate junior developers. There are many best practices and you can name as per your confort and conviniece. Here are some of the more common ones:
a) use batch statement for inserting and updating data.
b) use PreparedStatement to avoid SQL exception and better performance.
c) use database connection pool
d) access resultset using column name instead of column indexes.
e) Don't generate dynamic SQL by concatenating String with user input.

----


81) Name couple of method overloading best practices in Java? (answer)
Here are some best practices you can follow while overloading a method in Java to avoid confusion with auto-boxing:
a) Don't overload method where one accepts int and other accepts Integer.
b) Don't overload method where number of argument is same and only order of argument is different.
c) Use varargs after overloaded methods has more than 5 arguments.



Date, Time and Calendar Interview questions in Java

----

82) Does SimpleDateFormat is safe to use in the multi-threaded program? (answer)
No, unfortunately, DateFormat and all its implementations including SimpleDateFormat is not thread-safe, hence should not be used in the multi-threaded program until external thread-safety measures are applied e.g. confining SimpleDateFormat object into a ThreadLocal variable. If you don't do that, you will get an incorrect result while parsing or formatting dates in Java. Though, for all practical date time purpose, I highly recommend joda-time library.

----


83) How do you format a date in Java? e.g. in the ddMMyyyy format? (answer)
You can either use SimpleDateFormat class or joda-time library to format date in Java. DateFormat class allows you to format date on many popular formats. Please see the answer for code samples to format date into different formats e.g. dd-MM-yyyy or ddMMyyyy.


84) How do you show timezone in formatted date in Java? (answer)

----

85) The difference between java.util.Date and java.sql.Date in Java? (answer)

----

86) How to you calculate the difference between two dates in Java? (program)

----

87) How do you convert a String(YYYYMMDD) to date in Java? (answer)



----


Unit testing JUnit Interview questions
89) How do you test static method? (answer)
You can use PowerMock library to test static methods in Java.

----

90) How to do you test a method for an exception using JUnit? (answer)

----

91) Which unit testing libraries you have used for testing Java programs? (answer)

----

92) What is the difference between @Before and @BeforeClass annotation? (answer)


----


Programming and Coding Questions
93) How to check if a String contains only numeric digits? (solution)

----

94) How to write LRU cache in Java using Generics? (answer)

----

95) Write a Java program to convert bytes to long? (answer)

----

96) How to reverse a String in Java without using StringBuffer? (solution)

----

97) How to find the word with the highest frequency from a file in Java? (solution)

----

98) How do you check if two given String are anagrams? (solution)

----

99) How to print all permutation of a String in Java? (solution)

----

100) How do you print duplicate elements from an array in Java? (solution)

----

101) How to convert String to int in Java? (solution)

----

102) How to swap two integers without using temp variable? (solution)



Java Interview questions from OOP and Design Patterns
It contains Java Interview questions from SOLID design principles, OOP fundamentals e.g. class, object, interface, Inheritance, Polymorphism, Encapsulation, and Abstraction as well as more advanced concepts like Composition, Aggregation, and Association. It also contains questions from GOF design patterns.

----

103) What is the interface? Why you use it if you cannot write anything concrete on it?
The interface is used to define API. It tells about the contract your classes will follow. It also supports abstraction because a client can use interface method to leverage multiple implementations e.g. by using List interface you can take advantage of random access of ArrayList as well as flexible insertion and deletion of LinkedList. The interface doesn't allow you to write code to keep things abstract but from Java 8 you can declare static and default methods inside interface which are concrete.


----

104) The difference between abstract class and interface in Java? (answer)
There are multiple differences between abstract class and interface in Java, but the most important one is Java's restriction on allowing a class to extend just one class but allows it to implement multiple interfaces. An abstract class is good to define default behavior for a family of class, but the interface is good to define Type which is later used to leverage Polymorphism. Please check the answer for a more thorough discussion of this question.

----


105) Which design pattern have you used in your production code? apart from Singleton?
This is something you can answer from your experience. You can generally say about dependency injection, factory pattern, decorator pattern or observer pattern, whichever you have used. Though be prepared to answer follow-up question based upon the pattern you choose.


----

106) Can you explain Liskov Substitution principle? (answer)
This is one of the toughest questions I have asked in Java interviews. Out of 50 candidates, I have almost asked only 5 have managed to answer it. I am not posting an answer to this question as I like you to do some research, practice and spend some time to understand this confusing principle well.


----

107) What is Law of Demeter violation? Why it matters? (answer)
Believe it or not, Java is all about application programming and structuring code. If  you have good knowledge of common coding best practices, patterns and what not to do than only you can write quality code.  Law of Demeter suggests you "talk to friends and not stranger", hence used to reduce coupling between classes.


----

108) What is Adapter pattern? When to use it?
Another frequently asked Java design pattern questions. It provides interface conversion. If your client is using some interface but you have something else, you can write an Adapter to bridge them together. This is good for Java software engineer having 2 to 3 years experience because the question is neither difficult nor tricky but requires knowledge of OOP design patterns.


----

109) What is "dependency injection" and "inversion of control"? Why would someone use it? (answer)

----

110) What is an abstract class? How is it different from an interface? Why would you use it? (answer)
One more classic question from Programming Job interviews, it is as old as chuck Norris. An abstract class is a class which can have state, code and implementation, but an interface is a contract which is totally abstract. Since I have answered it many times, I am only giving you the gist here but you should read the article linked to answer to learn this useful concept in much more detail.


----

111) Which one is better constructor injection or setter dependency injection? (answer)
Each has their own advantage and disadvantage. Constructor injection guaranteed that class will be initialized with all its dependency, but setter injection provides flexibility to set an optional dependency. Setter injection is also more readable if you are using an XML file to describe dependency. Rule of thumb is to use constructor injection for mandatory dependency and use setter injection for optional dependency.


----

112) What is difference between dependency injection and factory design pattern? (answer)
Though both patterns help to take out object creation part from application logic, use of dependency injection results in cleaner code than factory pattern. By using dependency injection, your classes are nothing but POJO which only knows about dependency but doesn't care how they are acquired. In the case of factory pattern, the class also needs to know about factory to acquire dependency. hence, DI results in more testable classes than factory pattern. Please see the answer for a more detailed discussion on this topic.

----


113) Difference between Adapter and Decorator pattern? (answer)
Though the structure of Adapter and Decorator pattern is similar, the difference comes on the intent of each pattern. The adapter pattern is used to bridge the gap between two interfaces, but Decorator pattern is used to add new functionality into the class without the modifying existing code.

----


114) Difference between Adapter and Proxy Pattern? (answer)
Similar to the previous question, the difference between Adapter and Proxy patterns is in their intent. Since both Adapter and Proxy pattern encapsulate the class which actually does the job, hence result in the same structure, but Adapter pattern is used for interface conversion while the Proxy pattern is used to add an extra level of indirection to support distribute, controlled or intelligent access.

----


115) What is Template method pattern? (answer)
Template pattern provides an outline of an algorithm and lets you configure or customize its steps. For examples, you can view a sorting algorithm as a template to sort object. It defines steps for sorting but let you configure how to compare them using Comparable or something similar in another language. The method which outlines the algorithms is also known as template method.


----

116) When do you use Visitor design pattern? (answer)
The visitor pattern is a solution of problem where you need to add operation on a class hierarchy but without touching them. This pattern uses double dispatch to add another level of indirection.


----

117) When do you use Composite design pattern? (answer)
Composite design pattern arranges objects into tree structures to represent part-whole hierarchies. It allows clients treat individual objects and container of objects uniformly. Use Composite pattern when you want to represent part-whole hierarchies of objects.


----

118) The difference between Inheritance and Composition? (answer)
Though both allows code reuse, Composition is more flexible than Inheritance because it allows you to switch to another implementation at run-time. Code written using Composition is also easier to test than code involving inheritance hierarchies.


----

119) Describe overloading and overriding in Java? (answer)
Both overloading and overriding allow you to write two methods of different functionality but with the same name, but overloading is compile time activity while overriding is run-time activity. Though you can overload a method in the same class, but you can only override a method in child classes. Inheritance is necessary for overriding.


----

120) The difference between nested public static class and a top level class in Java? (answer)
You can have more than one nested public static class inside one class, but you can only have one top-level public class in a Java source file and its name must be same as the name of Java source file.


----

121) Difference between Composition, Aggregation and Association in OOP? (answer)
If two objects are related to each other, they are said to be associated with each other. Composition and Aggregation are two forms of association in object-oriented programming. The composition is stronger association than Aggregation. In Composition, one object is OWNER of another object while in Aggregation one object is just USER of another object. If an object A is composed of object B then B doesn't exist if A ceased to exists, but if object A is just an aggregation of object B then B can exists even if A ceased to exist.

----


122) Give me an example of design pattern which is based upon open closed principle? (answer)
This is one of the practical questions I ask experienced Java programmer. I expect them to know about OOP design principles as well as patterns. Open closed design principle asserts that your code should be open for extension but closed for modification. Which means if you want to add new functionality, you can add it easily using the new code but without touching already tried and tested code.  There are several design patterns which are based upon open closed design principle e.g. Strategy pattern if you need a new strategy, just implement the interface and configure, no need to modify core logic. One working example is Collections.sort() method which is based on Strategy pattern and follows the open-closed principle, you don't modify sort() method to sort a new object, what you do is just implement Comparator in your own way.

----


123) Difference between Abstract factory and Prototype design pattern? (answer)
This is the practice question for you, If you are feeling bored just reading and itching to write something, why not write the answer to this question. I would love to see an example the, which should answer where you should use the Abstract factory pattern and where is the Prototype pattern is more suitable.

----


124) When do you use Flyweight pattern? (answer)
This is another popular question from the design pattern. Many Java developers with 4 to 6 years of experience know the definition but failed to give any concrete example. Since many of you might not have used this pattern, it's better to look examples from JDK. You are more likely have used them before and they are easy to remember as well. Now let's see the answer.
Flyweight pattern allows you to share object to support large numbers without actually creating too many objects. In order to use Flyweight pattern, you need to make your object Immutable so that they can be safely shared. String pool and pool of Integer and Long object in JDK are good examples of Flyweight pattern.



Miscellaneous Java Interview Questions
It contains XML Processing in Java Interview question, JDBC Interview question, Regular expressions Interview questions, Java Error and Exception Interview Questions, Serialization,

----

125) The difference between nested static class and top level class? (answer)
One of the fundamental questions from Java basics. I ask this question only to junior Java developers of 1 to 2 years of experience as it's too easy for an experience Java programmers. The answer is simple, a public top level class must have the same name as the name of the source file, there is no such requirement for nested static class. A nested class is always inside a top level class and you need to use the name of the top-level class to refer nested static class e.g. HashMap.Entry is a nested static class, where HashMap is a top level class and Entry is nested static class.

----


126) Can you write a regular expression to check if String is a number? (solution)
If you are taking Java interviews then you should ask at least one question on the regular expression. This clearly differentiates an average programmer with a good programmer. Since one of the traits of a good developer is to know tools, regex is the best tool for searching something in the log file, preparing reports etc. Anyway, answer to this question is, a numeric String can only contain digits i.e. 0 to 9 and + and - sign that too at start of the String, by using this information you can write following regular expression to check if given String is number or not

----


127) The difference between checked and unchecked Exception in Java? (answer)
checked exception is checked by the compiler at compile time. It's mandatory for a method to either handle the checked exception or declare them in their throws clause. These are the ones which are a sub class of Exception but doesn't descend from RuntimeException. The unchecked exception is the descendant of RuntimeException and not checked by the compiler at compile time. This question is now becoming less popular and you would only find this with interviews with small companies, both investment banks and startups are moved on from this question.


----

128) The difference between throw and throws in Java? (answer)
the throw is used to actually throw an instance of java.lang.Throwable class, which means you can throw both Error and Exception using throw keyword e.g.

throw new IllegalArgumentException("size must be multiple of 2")

On the other hand, throws is used as part of method declaration and signals which kind of exceptions are thrown by this method so that its caller can handle them. It's mandatory to declare any unhandled checked exception in throws clause in Java. Like the previous question, this is another frequently asked Java interview question from errors and exception topic but too easy to answer.

----


129) The difference between Serializable and Externalizable in Java? (answer)
This is one of the frequently asked questions from Java Serialization. The interviewer has been asking this question since the day Serialization was introduced in Java, but yet only a few good candidate can answer this question with some confidence and practical knowledge. Serializable interface is used to make Java classes serializable so that they can be transferred over network or their state can be saved on disk, but it leverages default serialization built-in JVM, which is expensive, fragile and not secure. Externalizable allows you to fully control the Serialization process, specify a custom binary format and add more security measure.


----

130) The difference between DOM and SAX parser in Java? (answer)
Another common Java question but from XML parsing topic. It's rather simple to answer and that's why many interviewers prefers to ask this question on the telephonic round. DOM parser loads the whole XML into memory to create a tree based DOM model which helps it quickly locate nodes and make a change in the structure of XML while SAX parser is an event based parser and doesn't load the whole XML into memory. Due to this reason DOM is faster than SAX but require more memory and not suitable to parse large XML files.


----

131) Tell me 3 features introduced on JDK 1.7? (answer)
This is one of the good questions I ask to check whether the candidate is aware of recent development in Java technology space or not. Even though JDK 7 was not a big bang release like JDK 5 or JDK 8, it still has a lot of good feature to count on e.g. try-with-resource statements, which free you from closing streams and resources when you are done with that, Java automatically closes that. Fork-Join pool to implement something like the Map-reduce pattern in Java. Allowing String variable and literal into switch statements. Diamond operator for improved type inference, no need to declare generic type on the right-hand side of variable declaration anymore, results in more readable and succinct code. Another worth noting feature introduced was improved exception handling e.g. allowing you to catch multiple exceptions in the same catch block.

----


132) Tell me 5 features introduced in JDK 1.8? (answer)
This is the follow-up question of the previous one. Java 8 is path breaking release in Java's history, here are the top 5 features from JDK 8 release
Lambda expression, which allows you pass an anonymous function as object.
Stream API, take advantage of multiple cores of modern CPU and allows you to write succinct code.
Date and Time API, finally you have a solid and easy to use date and time library right into JDK
Extension methods, now you can have static and default method into your interface
Repeated annotation, allows you apply the same annotation multiple times on a type

----

133) What is the difference between Maven and ANT in Java? (answer)
Another great question to check the all round knowledge of Java developers. It's easy to answer questions from core Java but when you ask about setting things up, building Java artifacts, many Java software engineer struggles. 

Coming back to the answer of this question, Though both are build tools and used to create Java application build, Maven is much more than that. It provides a standard structure for Java project based upon the "convention over configuration" concept and automatically manages dependencies (JAR files on which your application is dependent) for Java applications. Please see the answer for more differences between the Maven and ANT tools.


That's all guys, lots of Java Interview questions? isn't it? I am sure if you can answer this list of Java questions you can easily crack any core Java or advanced Java interview. Though I have not included questions from Java EE or J2EE topics e.g. Servlet, JSP, JSF, JPA, JMS, EJB, or any other Java EE technology or from major web frameworks like Spring MVC, Struts 2.0, Hibernate, or both SOAP and RESTful web services, it's still useful for Java developers preparing for Java web developer position, because every Java interview starts with questions from fundamentals and JDK API. 

If you think, I have missed any popular Java question here and you think it should be in this list then feel free to suggest me. My goal is to create the best list of Java Interview Questions with the latest and greatest questions from recent interviews.

In case you don't know, I  have also written a book for Java interviews, Grokking the Java Interview, and Grokking the Spring Boot Interview, where I have shared tips, tricks and frequently asked Java questions from different topics. You can read the book to better prepare for your Java interviews. You can also use the code - friends20 to get a 20% discount because you are already my reader. 



Related Java EE Interview Questions
For my Java EE friends, here are web development specific questions, which you can use to prepare for JEE part:
Top 10 Spring Framework Interview Questions with Answers (see here)
10 Great XML Interview Questions for Java Programmers (read here)
20 Great Java Design Pattern Questions asked on Interviews (see here)
10 popular Struts Interview Questions for Java developers (list)
20 Tibco Rendezvous and EMS Interview Questions (read more)
10 frequently asked Servlet Interview Questions with Answers (see here)
20 jQuery Interview Questions for Java Web Developers (list)
10 Great Oracle Interview Questions for Java developers (see here)
Top 10 JSP Questions  from J2EE Interviews (read here)
12 Good RESTful Web Services Questions from Interviews (read here)
Top 10 EJB Interview Questions and Answers (see here)
Top 10 JMS and MQ Series Interview Questions and Answers (list)
10 Great Hibernate Interview Questions for Java EE developers (see here)
10 Great JDBC Interview Questions for Java Programmers (questions)
15 Java NIO and Networking Interview Questions with Answers (see here)
Top 10 XSLT Interview Questions with Answers (read more)
15 Data Structure and Algorithm Questions from Java Interviews (read here)
Top 10 Trick Java Interview Questions and Answers (see here)
Top 40 Core Java Phone Interview Questions with Answers (list)


Recommended Books for Java Programmers
If you are looking for some goods to prepare for your Java Interviews, You can take a look at the following books to cover both theory and coding questions:
9 Must-Read Books for Java Developers (see book)
5 Java Performance Tuning Books for Experienced Programmers (see book)
5 Good Books for Java JEE Interviews (see book)
5 Books to learn Data Structure and Algorithms (see book)
5 Hibernate Books for Java Developers (see book)
5 Spring Books for Java Developers (see book)
References
The Java Virtual Machine Specification (see here)
The Java Language Specification (Java SE 8) (see here)
Java SE 8 API Specification (see here)
Thanks a lot, for reading this article so far. All the best for your Java interviews. If you have any interesting questions to share or want to share your interview experience, please drop a note so that others can benefit from it. 


Read more: https://javarevisited.blogspot.com/2015/10/133-java-interview-questions-answers-from-last-5-years.html#ixzz80dhIw3nT

</https://javarevisited.blogspot.com/2015/10/133-java-interview-questions-answers-from-last-5-years.html#axzz80dfcO0nd>

<https://javarevisited.blogspot.com/2014/07/top-50-java-multithreading-interview-questions-answers.html#axzz80dfcO0nd>

Top 50 Java Thread and Concurrency Interview Questions Answers for 2 to 5 Years Experienced

You go to any Java interview, senior or junior, experience or freshers,  you are bound to see a couple of questions from the thread, concurrency, and multi-threading. In fact, this built-in concurrency support is one of the strongest points of the Java programming language and helped it to gain popularity among the enterprise world and programmers equally. Most of the lucrative Java developer position demands excellent core Java multi-threading skills and experience in developing, debugging, and tuning high-performance low latency concurrent Java applications. This is the reason, it is one of the most important topics in Java interviews. Multithreading and concurrency are also hard to master the concept and only good developers with solid experience can effectively deal with concurrency issues.

PauseUnmute
Fullscreen


In a typical Java interview, the Interviewer slowly starts from basic concepts of Thread by asking questions like, why you need threads, how to create threads, which one is a better way to create threads like by extending thread class or implementing Runnable, and then slowly goes into Concurrency issues, challenges faced during the development of concurrent Java applications.

Java memory model, higher-order concurrency utilities introduced in JDK 1.5, principles and design patterns of concurrent Java applications, classical multithreading problems like producer-consumer, dining philosopher, reader-writer, or simply bounded buffer problems.

Since it's also not enough just to know the basics of threading, you must know how to deal with concurrency problems like deadlock, race conditions, memory inconsistency, and various thread safety-related issues. These skills are thoroughly get tested by presenting various multi-threading and concurrency problems.


Many Java developers are used to only looking and reading interview questions before going for the interview, which is not bad but you should not be too far away. Also collecting questions and going through the same exercise is too time-consuming, that's why I have created this list of the top 50 Java multi-threading and concurrency-related questions, collected from various interviews. I am only going to add new and recent interview questions as and when I am going to discover them.

Though you need good knowledge and solid experience to do well on Java interviews focused on advanced multithreading and concurrency skill, I strongly recommend Java programmers to read Effective Java and Java Concurrency in Practice twice before going to an interview. They do not only help you to answer questions better but also help you to present your idea clearly.
Top 5 Courses to Learn Eclipse IDE for Java Programmers - Best of Lot

And, if you are serious about mastering Java multi-threading and concurrency then I also suggest you take a look at these best Java Multithreading courses for experienced developers. It's a collection of advanced Java courses to become an expert in Multithreading, concurrency, and Parallel programming in Java with a strong emphasis on high performance

By the way, I have not provided answers to some questions here, Why? because I expect most Java developers to know the answers to this question and if not, also answers are widely available by using Google. 

If you don't find the answer to any particular question, you can always ask me in the comments section. You can even find answers to a few questions on the link provided or my earlier post Top 12 Java Thread Questions with Answers.




50 Interview questions from Java Multithreading and Concurrency with Answers 
Here is our list of top questions from Java thread, concurrency, and multi-threading. You can use this list to prepare well for your Java interview.


----

1)  What is Thread in Java? (answer)
The thread is an independent path of execution. It's a way to take advantage of multiple CPUs available on a machine. By employing multiple threads you can speed up CPU-bound tasks. For example, if one thread takes 100 milliseconds to do a job, you can use 10 threads to reduce that task into 10 milliseconds. Java provides excellent support for multithreading at the language level, and it's also one of the strong selling points.

----


2)  What is the difference between Thread and Process in Java? (answer)
The thread is a subset of Process, in other words, one process can contain multiple threads. Two processes run on different memory spaces, but all threads share the same memory space. Don't confuse this with stack memory, which is different for the different threads and used to store local data to that thread. For more detail see the answer.

What is the difference between Thread and Process in Java?



----


3)  How do you implement Thread in Java? (answer)
At the language level, there are two ways to implement Thread in Java. An instance of java.lang.Thread represents a thread but it needs a task to execute, which is an instance of interface java.lang.Runnable. 

Since the Thread class itself implement Runnable, you can override the run() method either by extending the Thread class or just implementing the Runnable interface. For a detailed answer and discussion see this article.


----

4)  When to use Runnable vs Thread in Java? (answer)
This is a follow-up to a previous multi-threading interview question. As we know we can implement thread either by extending the Thread class or implementing Runnable interface, the question arises, which one is better and when to use one? This question will be easy to answer if you know that the Java programming language doesn't support multiple inheritances of class, but it allows you to implement multiple interfaces. 

This means it's better to implement Runnable than extend Thread if you also want to extend another class e.g. Canvas or CommandListener. For more points and discussion you can also refer to this post.



----


6)  What is the difference between the start() and run() method of the Thread class?  (answer)
One of trick Java questions from early days, but still good enough to differentiate between shallow understanding of Java threading model start() method is used to start a newly created thread, while start() internally calls run() method, there is difference calling run() method directly. 

When you invoke run() as a normal method, it's called in the same thread, no new thread is started, which is the case when you call the start() method. Read this answer for a much more detailed discussion.

----


7)  What is the difference between Runnable and Callable in Java? (answer)
Both Runnable and Callable represent task which is intended to be executed in a separate thread. Runnable is there from JDK 1.0 while Callable was added on JDK 1.5. The main difference between these two is that Callable's call() method can return value and throw Exception, which was not possible with Runnable's run() method. Callable return Future object, which can hold the result of the computation. See my blog post on the same topic for a more in-depth answer to this question.

----


8)  What is the difference between CyclicBarrier and CountDownLatch in Java?  (answer)
Though both CyclicBarrier and CountDownLatch wait for a number of threads on one or more events, the main difference between them is that you can not re-use CountDownLatch once the count reaches to zero, but you can reuse the same CyclicBarrier even after the barrier is broken.  See this answer for a few more points and a sample code example.

----


9)  What is the Java Memory model? (answer)
Java Memory model is a set of rules and guidelines which allows Java programs to behave deterministically across multiple memory architecture, CPU, and operating systems. It's particularly important in the case of multi-threading. 

Java Memory Model provides some guarantee on which changes made by one thread should be visible to others, one of them is the happens-before relationship. This relationship defines several rules which allow programmers to anticipate and reason the behavior of concurrent Java programs. For example, happens-before relationship guarantees :
Each action in a thread happens-before every action in that thread that comes later in the program order, this is known as the program order rule.
An unlock on a monitor lock happens before every subsequent lock on that same monitor lock, also known as the Monitor lock rule.
A write to a volatile field happens before every subsequent read of that same field, known as the Volatile variable rule.
A call to Thread.start on a thread happens-before any other thread detects that thread has terminated, either by successfully returning from Thread.join() or by Thread.isAlive() returning false, also known as Thread start rule.
A thread calling interrupt() on another thread happens before the interrupted thread detects the interrupt( either by having InterruptedException thrown, or invoking interrupted or interrupted), popularly known as the Thread Interruption rule.
The end of a constructor for an object happens before the start of the finalizer for that object is known as the Finalizer rule.
If A happens before B, and B happens before C, then A happens-before C, which means happens-before guarantees Transitivity.
I strongly suggest reading Chapter 16 of Java Concurrency in Practice to understand the Java Memory model in more detail.

What is the Java Memory model? (answer)




----

10) What is a volatile variable in Java? (answer)
volatile is a special modifier, which can only be used with instance variables. In concurrent Java programs, changes made by multiple threads on instance variables are not visible to others in absence of any synchronizers like synchronized keywords or locks. 

Volatile variable guarantees that a write will happen before any subsequent read: as stated: "volatile variable rule" in the previous question. Read this answer to learn more about volatile variables and when to use them.



----


11) What is thread-safety? is Vector a thread-safe class? (Yes, see details)
Thread safety is a property of an object or code which guarantees that if executed or used by multiple threads in any manner e.g. read vs writing it will behave as expected. For example, a thread-safe counter object will not miss any count if the same instance of that counter is shared among multiple threads.

Apparently, you can also divide collection classes into two categories, thread-safe and non-thread-safe. Vector is indeed a thread-safe class and it achieves thread-safety by synchronizing methods that modify the state of Vector, on the other hand, its counterpart ArrayList is not thread-safe.


----

12) What is a race condition in Java? Given one example?  (answer)
Race conditions are caused by some subtle programming bugs when Java programs are exposed to a concurrent execution environment. As the name suggests, a race condition occurs due to race between multiple threads, if a thread that is supposed to execute first lost the race and is executed second, the behavior of code changes, which surface as non-deterministic bugs. 

This is one of the hardest bugs to find and re-produce because of the random nature of racing between threads. One example of race conditions is out-of-order processing, see this answer for some more examples of race conditions in Java programs.


----

13) How to stop a thread in Java? (answer(answer)
I always said that Java provides rich APIs for everything but ironically Java doesn't provide a sure-shot way of stopping the thread. There were some control methods in JDK 1.0 e.g. stop(), suspend(), and resume() which were deprecated in later releases due to potential deadlock threats, then Java API designers have not made any effort to provide a consistent, thread-safe, and elegant way to stop threads. 

Programmers mainly rely on the fact that thread stops automatically as soon as they finish execution of run() or call() method. To manually stop, programmers either take advantage of volatile boolean variables and check in every iteration if the run method has loops or interrupt threads to abruptly cancel tasks. See this tutorial for a sample code of stopping thread in Java.


----

14) What happens when an Exception occurs in a thread? (answer)
This is one of the good tricky Java questions I have seen in interviews. In simple words, If not caught thread will die, if an uncaught exception handler is registered then it will get a callback. Thread.UncaughtExceptionHandler is an interface, defined as a nested interface for handlers invoked when a Thread abruptly terminates due to an uncaught exception. 

When a thread is about to terminate due to an uncaught exception the Java Virtual Machine will query the thread for its UncaughtExceptionHandler using Thread.getUncaughtExceptionHandler() and will invoke the handler's uncaughtException() method, passing the thread and the exception as arguments.


----

15) How do you share data between two threads in Java? (answer)
You can share data between threads by using shared objects, or concurrent data structures like BlockingQueue. See this tutorial to learn inter-thread communication in Java. It implements the Producer consumer pattern using wait and notify methods, which involves sharing objects between two threads.


Java concurrency questions for experienced programmers


----

16) What is the difference between notify and notifyAll in Java? (answer)
This is another tricky question from core Java interviews since multiple threads can wait on a single monitor lock, Java API designer provides a method to inform only one of them or all of them, once the waiting condition changes, but they provide the half implementation. 

There notify() method doesn't provide any way to choose a particular thread, that's why it's only useful when you know that there is only one thread is waiting. 

On the other hand, notifyAll() sends a notification to all threads and allows them to compete for locks, which ensures that at least one thread will proceed further. See my blog post on a similar topic for a more detailed answer and code example.


----

17) Why wait, notify, and notifyAll are not inside the thread class?  (answer)
This is a design-related question, which checks what the candidate thinks about the existing system or does he ever thought of something which is so common but looks inappropriate at first. In order to answer this question, you have to give some reasons why it makes sense for these three methods to be in the Object class, and why not on Thread class. 

One reason which is obvious is that Java provides lock at the object level, not at the thread level. Every object has a lock, which is acquired by a thread. Now if the thread needs to wait for a certain lock it makes sense to call wait() on that object rather than on that thread.

Had wait() method declared on Thread class, it was not clear for which lock thread was waiting. In short, since wait, notify and notifyAll operate at lock level, it makes sense to define it on object class because the lock belongs to object. You can also see this article for a more elaborate answer to this question.


----

18) What is the ThreadLocal variable in Java?  (answer)
ThreadLocal variables are a special kind of variable available to Java programmers. Just like instance, the variable is per instance, ThreadLocal variable is per thread. It's a nice way to achieve thread-safety of expensive-to-create objects, for example, you can make SimpleDateFormat thread-safe using ThreadLocal. Since that class is expensive, it's not good to use it in local scope, which requires separate instances on each invocation. 

By providing each thread their own copy, you shoot two birds with one arrow. First, you reduce the number of instances of expensive objects by reusing a fixed number of instances, and Second, you achieve thread safety without paying the cost of synchronization or immutability. 

Another good example of a thread-local variable is ThreadLocalRandom class, which reduces the number of instances of expensive-to-create Random objects in a multi-threading environment. See this answer to learn more about thread-local variables in Java.



----


19) What is FutureTask in Java? (answer)
FutureTask represents a cancellable asynchronous computation in concurrent Java applications. This class provides a base implementation of Future, with methods to start and cancel a computation, query to see if the computation is complete and retrieve the result of the computation. 

The result can only be retrieved when the computation has been completed; the get methods will block if the computation has not yet been completed. A FutureTask object can be used to wrap a Callable or Runnable object. Since FutureTask also implements Runnable, it can be submitted to an Executor for execution.


----

20) What is the difference between the interrupted() and isInterrupted() method in Java? (answer)
The main difference between interrupted() and isInterrupted() is that the former clears the interrupt status while the latter does not. The interrupt mechanism in Java multi-threading is implemented using an internal flag known as the interrupt status. Interrupting a thread by calling Thread.interrupt() sets this flag. 

When interrupted thread checks for an interrupt by invoking the static method Thread.interrupted(), interrupt status is cleared. The non-static isInterrupted() method, which is used by one thread to query the interrupt status of another, does not change the interrupt status flag. 

By convention, any method that exits by throwing an InterruptedException clears interrupt status when it does so. However, it's always possible that interrupt status will immediately be set again, by another thread invoking interrupt


----

21) Why wait and notify methods are called from the synchronized block? (answer)
The main reason for calling the wait and notify method from either synchronized block or method is that it is made mandatory by Java API. If you don't call them from a synchronized context, your code will throw IllegalMonitorStateException. A more subtle reason is to avoid the race condition between wait and notify calls. To learn more about this, check my similarly titled post here.


----

22) Why should you check the condition for waiting in a loop? (answer)
It's possible for a waiting thread to receive false alerts and spurious wake-up calls, if it doesn't check the waiting condition in a loop, it will simply exit even if the condition is not met. As such, when awaiting thread wakes up, it cannot assume that the state it was waiting for is still valid. It may have been valid in the past, but the state may have been changed after the notify() method was called and before the waiting thread woke up. 

That's why it is always better to call the wait() method from a loop, you can even create a template for calling wait and notify in Eclipse. To learn more about this question, I would recommend you to read Effective Java items on thread and synchronization.


----

23) What is the difference between synchronized and concurrent collection in Java? (answer)
Though both synchronized and concurrent collection provides thread-safe collection suitable for multi-threaded and concurrent access, later is more scalable than former. Before Java 1.5, Java programmers only had synchronized collection which becomes a source of contention if multiple threads access them concurrently, which hampers the scalability of the system. 

Java 5 introduced concurrent collections like ConcurrentHashMap, which not only provides thread safety but also improves scalability by using modern techniques like lock stripping and partitioning internal tables. See this answer for more differences between synchronized and concurrent collection in Java.


----

24) What is the difference between Stack and Heap in Java? (answer)
Why does someone this question as part of multi-threading and concurrency? because Stack is a memory area that is closely associated with threads. To answer this question, both stack and heap are specific memories in Java applications. 

Each thread has its own stack, which is used to store local variables, method parameters, and call stack. Variable stored in one Thread's stack is not visible to other. On another hand, the heap is a common memory area that is shared by all threads. 

Objects whether local or at any level is created inside the heap. To improve performance thread tends to cache values from the heap into their stack, which can create problems if that variable is modified by more than one thread, this is where volatile variables come into the picture. volatile suggest threads read the value of variable always from main memory. See this article for learning more about stack and heap in Java to answer this question in greater detail.


Java thread interview questions with answers difficult ones


----


25) What is a thread pool? Why should you thread pool in Java?  (answer)
Creating a thread is expensive in terms of time and resources. If you create a thread at the time of request processing it will slow down your response time, also there is only a limited number of threads a process can create. To avoid both of these issues, a spool of threads is created when the application starts up and threads are reused for request processing.

This pool of thread is known as "thread pool" and threads are known as a worker thread. From JDK 1.5 release, Java API provides Executor framework, which allows you to create different types of thread pools e.g. single thread pool, which processes one task at a time, fixed thread pool (a pool of fixed number of threads), or cached thread pool (an expandable thread pool suitable for applications with many short-lived tasks). See this article to learn more about thread pools in Java to prepare a detailed answer to this question.

----


26) Write code to solve Producer Consumer problems in Java? (answer)
Most of the threading problems you solved in the real world are of the category of Producer consumer pattern, where one thread is producing a task and another thread is consuming that. You must know how to do inter-thread communication to solve this problem. At the lowest level, you can use wait and notify to solve this problem, and at a high level, you can leverage Semaphore or BlockingQueue to implement a Producer consumer pattern, as shown in this tutorial.


----

27) How do you avoid deadlock in Java? Write Code? (answer)
Deadlock is a condition in which two threads wait for each other to take action which allows them to move further. It's a serious issue because when it happens your program hangs and doesn't do the task it is intended for. 

In order for the deadlock to happen, the following four conditions must be true:
Mutual Exclusion: At least one resource must be held in a non-shareable mode. Only one process can use the resource at any given instant of time.
Hold and Wait: A process is currently holding, at least, one resource and requesting additional resources which are being held by other processes.
No Pre-emption: The operating system must not de-allocate resources once they have been allocated; they must be released by the holding process voluntarily.
Circular Wait: A process must be waiting for a resource that is being held by another process, which in turn is waiting for the first process to release the resource.

The easiest way to avoid deadlock is to prevent Circular wait, and this can be done by acquiring locks in a particular order and releasing them in reverse order so that a thread can only proceed to acquire a lock if it held the other one. Check this tutorial for the actual code example and detailed discussion on techniques for avoiding deadlock in Java.

deadlock in multithreading Java


----


28) What is the difference between livelock and deadlock in Java? (answer)
This question is an extension of the previous interview question. A livelock is similar to a deadlock, except that the states of the threads or processes involved in the livelock constantly change with regard to one another, without anyone progressing further. 

Livelock is a special case of resource starvation. A real-world example of livelock occurs when two people meet in a narrow corridor, and each tries to be polite by moving aside to let the other pass, but they end up swaying from side to side without making any progress because they both repeatedly move the same way at the same time. In short, the main difference between livelock and deadlock is that in the former state of process change but no progress is made.



----


29) How do you check if a thread holds a lock or not? (answer)
I didn't even know that you can check if a Thread already holds a lock before this question hits me in a telephonic round of Java interviews. There is a method called holdsLock() on java.lang.Thread, it returns true if and only if the current thread holds the monitor lock on the specified object. You can also check this article for a more detailed answer.


----

30) How do you take thread dump in Java? (answer)
There are multiple ways to take a thread dump of the Java process depending upon the operating system. When you take thread dump, JVM dumps the state of all threads in log files or standard error console. In windows, you can use Ctrl + Break key combination to take thread dump, on Linux you can use the kill -3 command for the same. You can also use a tool called jstack for taking thread dump, it operates on process id, which can be found using another tool called jps.


----

31) Which JVM parameter is used to control the stack size of a thread? (answer)
This is the simple one, -Xss parameter is used to control the stack size of Thread in Java. You can see this list of JVM options to learn more about this parameter.

----


32) What is the difference between synchronized and ReentrantLock in Java? (answer)
There were days when the only way to provide mutual exclusion in Java was via synchronized keyword, but it has several shortcomings e.g. you can not extend lock beyond a method or block boundary, you can not give up trying for a lock, etc.

Java 5 solves this problem by providing more sophisticated control via the Lock interface. ReentrantLock is a common implementation of the Lock interface and provides re-entrant mutual exclusion Lock with the same basic behavior and semantics as the implicit monitor lock accessed using synchronized methods and statements, but with extended capabilities. See this article to learn about those capabilities and some more differences between synchronized vs ReentrantLock in Java.



----


33) There are three threads T1, T2, and T3? How do you ensure sequence T1, T2, T3 in Java? (answer)
Sequencing in multi-threading can be achieved by different means but you can simply use the join() method of thread class to start a thread when another one has finished its execution. To ensure three threads execute you need to start the last one first e.g. T3 and then call join methods in reverse order e.g. T3 calls T2. join and T2 calls T1.join, these ways T1 will finish first and T3 will finish last. To learn more about the join method, see this tutorial.


----

34) What does the yield method of the Thread class do? (answer)
The yield method is one way to request the current thread to relinquish CPU so that other threads can get a chance to execute. Yield is a static method and only guarantees that the current thread will relinquish the CPU but doesn't say anything about which other thread will get CPU. It's possible for the same thread to get the CPU back and start its execution again. See this article to learn more about the yield method and to answer this question better.

----


35) What is the concurrency level of ConcurrentHashMap in Java? (answer)
ConcurrentHashMap achieves its scalability and thread-safety by partitioning the actual map into a number of sections. This partitioning is achieved using a concurrency level.

Its optional parameter of ConcurrentHashMap constructor and its default value is 16. The table is internally partitioned to try to permit the indicated number of concurrent updates without contention. To learn more about concurrency level and internal resizing, see my post How ConcurrentHashMap works in Java.



----


36) What is Semaphore in Java? (answer)
Semaphore in Java is a new kind of synchronizer. It's a counting semaphore. Conceptually, a semaphore maintains a set of permits. Each acquire() blocks if necessary until a permit is available and then takes it. Each release() adds a permit, potentially releasing a blocking acquirer. 

However, no actual permit objects are used; the Semaphore just keeps a count of the number available and acts accordingly. Semaphore is used to protect an expensive resource that is available in fixed numbers e.g. database connection in the pool. See this article to learn more about counting Semaphore in Java.

----


37) What happens if you submit a task when the queue of the thread pool is already filled? (answer)
This is another tricky question on my list. Many programmers will think that it will block until a task is cleared but it's true. ThreadPoolExecutor's submit() method throws RejectedExecutionException if the task cannot be scheduled for execution.

----


38) What is the difference between the submit() and execute() method thread pool in Java? (answer)
Both methods are ways to submit a task to thread pools but there is a slight difference between them. execute(Runnable command) is defined in Executor interface and executes given task in future, but more importantly, it does not return anything. Its return type is void. 

On other hand submit() is an overloaded method, it can take either Runnable or Callable task and can return Future object which can hold the pending result of the computation. 

This method is defined on ExecutorService interface, which extends Executor interface, and every other thread pool class e.g. ThreadPoolExecutor or ScheduledThreadPoolExecutor gets these methods. To learn more about thread pools you can check this article.

----


39) What is the blocking method in Java? (answer)
A blocking method is a method that blocks until the task is done, for example, accept() method of ServerSocket blocks until a client is connected. here blocking means control will not return to the caller until the task is finished. On the other hand, there is an asynchronous or non-blocking method that returns even before the task is finished. To learn more about the blocking method see this answer.


----

40) Is Swing thread-safe? What do you mean by Swing thread-safe? (answer)
You can simply this question as No, Swing is not thread-safe, but you have to explain what you mean by that even if the interviewer doesn't ask about it. When we say swing is not thread-safe we usually refer to its component, which can not be modified in multiple threads. 

All updates to GUI components have to be done on the AWT thread, and Swing provides synchronous and asynchronous callback methods to schedule such updates. You can also read my article to learn more about swing and thread safety to better answer this question. Even next two questions are also related to this concept.


----

41) What is the difference between invokeAndWait and invokeLater in Java? (answer)
These are two methods Swing API provides Java developers for updating GUI components from threads other than the Event dispatcher thread. InvokeAndWait() synchronously update GUI component, for example, a progress bar, once progress is made, the bar should also be updated to reflect that change. 

If progress is tracked in a different thread, it has to call invokeAndWait() to schedule an update of that component by the Event dispatcher thread. On another hand, invokeLater() is an asynchronous call to update components. You can also refer to this answer for more points.


----

42) Which method of Swing API is thread-safe in Java? (answer)
This question is again related to swing and thread-safety though components are not thread-safe there is a certain method that can be safely called from multiple threads. I know about repaint(), and revalidate() being thread-safe but there are other methods on different swing components e.g. setText() method of JTextComponent, insert() and append() method of JTextArea class.

----


43) How to create an Immutable object in Java? (answer)
This question might not look related to multi-threading and concurrency, but it is. Immutability helps to simplify already complex concurrent code in Java. Since immutable objects can be shared without any synchronization it's very dear to Java developers. Core value object, which is meant to be shared among threads should be immutable for performance and simplicity. 

Unfortunately, there is no @Immutable annotation in Java, which can make your object immutable, hard work must be done by Java developers. You need to keep basics like initializing state in the constructor, no setter methods, no leaking of reference, keeping a separate copy of the mutable object to create an Immutable object. For step by step guide see my post, how to make an object Immutable in Java. This will give you enough material to answer this question with confidence.


----

44) What is ReadWriteLock in Java? (answer)
In general, the read-write lock is the result of the lock stripping technique to improve the performance of concurrent applications. In Java, ReadWriteLock is an interface that was added in Java 5 release. 

A ReadWriteLock maintains a pair of associated locks, one for read-only operations and one for writing. The read lock may be held simultaneously by multiple reader threads, so long as there are no writers. 

The write lock is exclusive. If you want you can implement this interface with your own set of rules, otherwise you can use ReentrantReadWriteLock, which comes along with JDK and supports a maximum of 65535 recursive write locks and 65535 read locks.


----

45) What is a busy spin in multi-threading? (answer)
Busy spin is a technique that concurrent programmers employ to make a thread wait on certain conditions. Unlike traditional methods e.g. wait(), sleep(), or yield() which all involve relinquishing CPU control, this method does not relinquish CPU, instead, it just runs the empty loop. Why would someone do that? to preserve CPU caches. 

In a multi-core system, it's possible for a paused thread to resume on a different core, which means rebuilding the cache again. To avoid the cost of rebuilding cache, programmers prefer to wait for a much smaller time doing busy spin. You can also see this answer to learn more about this question.



----


46) What is the difference between the volatile and atomic variables in Java? (answer)
This is an interesting question for Java programmers, at first, volatile and atomic variables look very similar, but they are different. A volatile variable provides you happens-before guarantee that a write will happen before any subsequent write, it doesn't guarantee atomicity. 

For example, the count++ operation will not become atomic just by declaring the count variable as volatile.  On the other hand, AtomicInteger class provides an atomic method to perform such compound operation atomically e.g. getAndIncrement() is the atomic replacement of increment operator. It can be used to atomically increment the current value by one. 

Similarly, you have an atomic version for other data types and reference variables as well.


----

47) What happens if a thread throws an Exception inside a synchronized block? (answer)
This is one more tricky question for the average Java programmer if he can bring the fact about whether the lock is released or not is a key indicator of his understanding. 

To answer this question, no matter how you exist synchronized block, either normally by finishing execution or abruptly by throwing an exception, the thread releases the lock it acquired while entering that synchronized block. 

This is actually one of the reasons I like synchronized block over lock interface, which requires explicit attention to release lock, generally, this is achieved by releasing the lock in a finally block.


----

48) What is double-checked locking of Singleton? (answer)
This is one of the very popular questions on Java interviews, and despite its popularity, the chances of candidates answering this question satisfactory is only 50%. Half of the time, they failed to write code for double-checked locking, and half of the time they failed how it was broken and fixed on Java 1.5.

This is actually an old way of creating a thread-safe singleton, which tries to optimize performance by only locking when the Singleton instance is created the first time, but because of complexity and the fact it was broken for JDK 1.4,  I personally don't like it. 

Anyway, even if you do not prefer this approach it's good to know from an interview point of view. Since this question deserves a detailed answer, I have answered in a separate post, you can read my post how double-checked locking on Singleton works to learn more about it.

----


49) How to create thread-safe Singleton in Java? (answer)
This question is actually a follow-up to the previous question. If you say you don't like double-checked locking then the Interviewer is bound to ask about alternative ways of creating a thread-safe Singleton class. 

There is actually man, you can take advantage of class loading and static variable initialization feature of JVM to create an instance of Singleton, or you can leverage powerful enumeration type in Java to create Singleton. I actually preferred that way, you can also read this article to learn more about it and see some sample code.


----

50) List down 3 multi-threading best practices you follow? (answer)
This is my favorite question because I believe that you must follow certain best practices while writing concurrent code which helps in performance, debugging, and maintenance. Following are three best practices, I think an average Java programmer should follow:
Always give a meaningful name to your thread 
This goes a long way to find a bug or trace execution in concurrent code. OrderProcessor, QuoteProcessor, or TradeProcessor is much better than Thread-1. Thread-2 and Thread-3. The name should say about task done by that thread. All major frameworks and even JDK follow this best practice.
Avoid locking or Reduce scope of Synchronization
Locking is costly and context switching is even costlier. Try to avoid synchronization and locking as much as possible and at a bare minimum, you should reduce critical sections. That's why I prefer synchronized block over synchronized method because it gives you absolute control over the scope of locking.
Prefer Synchronizers over wait and notify
Synchronizers like CountDownLatch, Semaphore, CyclicBarrier or Exchanger simplify coding. It's very difficult to implement complex control flow right using wait and notify. Secondly, these classes are written and maintained by the best in business and there is a good chance that they are optimized or replaced by better performance code in subsequent JDK releases. By using higher-level synchronization utilities, you automatically get all these benefits.
Prefer Concurrent Collection over Synchronized Collection
This is another simple best practice that is easy to follow but reap good benefits. Concurrent collections are more scalable than their synchronized counterpart, that's why it's better to use them while writing concurrent code. So next time if you need a map, think about ConcurrentHashMap before thinking Hashtable. See my article Concurrent Collections in Java, to learn more about modern collection classes and how to make best use of them.



----


51) How do you force to start a thread in Java? (answer)
This question is like how do you force garbage collection in Java, there is no way though you can make a request using System.gc() but it's not guaranteed. On Java multi-threading there is absolutely no way to force start a thread, this is controlled by thread scheduler and Java exposes no API to control thread scheduling. This is still a random bit in Java.


----

52) What is the fork-join framework in Java? (answer)
The fork-join framework, introduced in JDK 7 is a powerful tool available to Java developers to take advantage of multiple processors of modern-day servers. It is designed for work that can be broken into smaller pieces recursively. 

The goal is to use all the available processing power to enhance the performance of your application. One significant advantage of The fork/join framework is that it uses a work-stealing algorithm. Worker threads that run out of things to do can steal tasks from other threads that are still busy. See this article for a much more detailed answer to this question.


----

53) What is the difference between the calling wait() and sleep() method in Java multi-threading? (answer)
Though both wait and sleep introduce some form of pause in Java applications, they are tools for different needs. The wait method is used for inter-thread communication, it relinquishes lock if waiting for a condition is true and waits for notification when due to an action of another thread waiting condition becomes false. 

On the other hand sleep() method is just to relinquish CPU or stop the execution of the current thread for a specified time duration. The calling sleep method doesn't release the lock held by the current thread. You can also take look at this article to answer this question with more details.


That's all on this list of top 50 Java multi-threading and concurrency interview questions. I have not shared answers to all the questions but provided enough hints and links to explore further and find answers by yourself. As I said, let me know if you don't find an answer to any particular question and I will add an answer here.

You can use this list not only to prepare for your core Java and programming interviews but also to check your knowledge about the basics of threads, multi-threading, concurrency, design patterns, and threading issues like race conditions, deadlock, and thread-safety problems.

My intention is to make this list of questions as the mother of all list of Java Multi-threading questions, but this can not be done without your help. You can also share any question with us, which has been asked to you or any question for which you have yet to find an answer.

This master list is equally useful to Java developers of all levels of experience. You can read through this list even if you have 2 to 3 years of working experience as a junior developer or 5 to 6 years as a senior developer. 

It's even useful for freshers and beginners to expand their knowledge. I will add new and latest multi-threading questions as and when I come across them, and I request you all to ask, share and answer questions via comments to keep this list relevant to all Java programmers.


Other Java Interview Questions list you may want to check
50 Java Programs from Coding Interviews (list)
15 Spring Boot Interview Questions with answers (spring boot questions)
21 Java ArrayList Interview Questions with Answers (list)
21 String Coding Problems for Java Programmers (string questions)
21 Java Final modifier Interview Questions (list)
19 Java Overloading and Overriding Interview Questions (list)
15 Java NIO and Networking Interview Questions with Answers (see here)
21 Java Inheritance Interview Questions with Answers (list)
75 Coding Interview Questions for Programmers (questions) 
21 String Algorithms Questions from Interviews (questions)
20+ binary tree Coding problems from Interviews (questions)
10 Date, Time, and Calendar based Interview Questions with Answers (list)
5 main() method interview questions (list)
25 Software Design Interview Questions for programmers (questions)
15 Java Enum based Interview Questions (list)
21 HashMap Interview Questions for Java developers (answers)
15 SQL and UNIX questions from Java Interviews (list)
22 array concept interview questions from Java (list)
25 Spring Security Interview Question with Answers (spring security questions)
15 Microservice Interview Questions with answers (microservice questions)

These questions will not only help you to understand multithreading and concurrency in Java better but also encourage you to find out more about Thread and various related classes and concurrency design patterns. If you have any other Thread or Concurrency based Java questions, which were asked to you in an interview, feel free to share with us.

P. S. - If you are preparing for Java Interviews and looking for some interesting questions for practice, then you can also check out these best Java Interview online courses, and books that contain more than 200+ real-world questions from Java interviews and their explanation.


Read more: https://javarevisited.blogspot.com/2014/07/top-50-java-multithreading-interview-questions-answers.html#ixzz80dhR0l1K

</https://javarevisited.blogspot.com/2014/07/top-50-java-multithreading-interview-questions-answers.html#axzz80dfcO0nd>

<https://javarevisited.blogspot.com/2015/02/50-programmer-phone-interview-questions-answers.html#axzz80dfcO0nd>

Top 42 Programming Interview Questions with Answers for 1 to 3 Years Experienced

For the last few years, phone interviews also known as the telephonic round is the single most popular way to screen candidates in a programming job interview. It's easy for both parties to gauge each other, the candidate doesn't need to travel to the prospective Employer's premises and the Interviewer also doesn't need to make any necessary arrangements. This is the second part of my article on programming interview questions, in the first part, I got feedback that it is a little bit heavy on coding-based questions and many programmers asked me to share a similar list for the telephonic round of programming Interviews. In order to clear the telephonic round and proceed to the next round, you must be good enough to answer all the questions related to your Job description.




In most of the phone interviews for Java or C++ developers, you will not only find questions from respective programming languages but also from other technology like SQL, XML, UNIX, General Programming, Object-oriented programming, Data Structure, and Algorithm, Networking, Coding, and other areas of work.

Because of this vast nature of the phone round of programming job interviews, you need to come up with a special strategy to present yourself in a manner Interviewer is expecting.

Also, basic knowledge of essential data structure and algorithms is also very important and that's why I suggest all Java programmers join these online Data structures and Algorithms courses to improve their knowledge and algorithms skills.

One of the most important things to remember, while answering questions on a phone interview is to mention key points early and always give the point answer. Since most interviewers like to cover lots of topics to screen the candidate, they usually like to-the-point answers rather than blah blah and OK I know the stuff, you will get your chance to explain things in deep in the face to face interview.

By the way, this is not the hard and fast rule and you can actually understand what the interviewer is expecting from you by noting his response to your answers. If he asks follow-up or expects you to speak more then go ahead, but it quickly jumps to the next question then be clear and concise.
Top 5 Books to Learn DevOps for Developers - Best of Lot

In this article, I am sharing some popular and interesting programming questions especially tailored for phone interviews. Most of them are actually from the telephonic round of various tech companies including banks like Barclays, Citi, Nomura, and various service-based companies like Infosys, TCS, CTS, Tech Mahindra, and HCL.

As I mentioned before questions are randomly picked from the various topics but mostly based upon fundamentals because that is what the Interviewer tests on phone interviews. Though these questions are mostly for less experienced developers like 2 to 5 years, Senior and experienced programmers can also use these for their interview purpose.

If you are seriously preparing for Job interviews, I also suggest you take a look at either Programming Interviews Exposed by Wrox or Cracking the coding Interview, two of the good books I have found for preparing any programming job interviews.

The first one is my favorite and I have read it almost 7 years back, but still, it's quite relevant because of an excellent explanation of data structure and algorithm questions. If you are an interviewer, you can also use these questions to quickly screen candidates for development positions. I have provided the short answer here and a pointer for a more detailed answer.




42 Programming and Tech Questions for Telephonic Interviews
Here is a list of almost 50 questions from the phone round of programming job interviews. These questions are good for any programmers, developers, software engineer, QA, and support engineer because they are based upon fundamentals of programming, but most suited for programmers and developers.

By the way, If you are a Java developer and looking for Java Questions for Phone interviews, check out that list. This list is more general and applicable for all programmers including Python, Ruby, Perl, and C# developers.


----

1. How much time does it take to retrieve an element if stored in HashMap, Binary tree, and a Linked list? how it change if you have millions of records?
In HashMap it takes O(1) time, in the binary tree it takes O(logN) where N is a number of nodes in the tree and in linked list it takes O(n) time where n is a number of element in the list. Millions of records don't affect the performance if the data structure is working as expected e.g. HashMap has no or relatively less number of collision or binary tree is balanced. If that's not the case then their performance degrades as a number of records grows.




----



2. What is the difference between Overriding and Overloading? (detailed answer)
Overriding is resolved at runtime while overloading is compile time. Also, rules of overriding and overloading are different, for example in Java, method signature of the overloaded method must be different than original method, but in the case of overriding it must be exactly same as an overriding method.

----


3. What is the difference between forking a process and spawning a thread? (answer)
When you fork a process, the new process will run the same code as the parent process but in different memory space, but when you spawn a new thread in existing process, it just creates another independent path of execution but share same memory space.


----

4. What is a critical section? (answer)
A critical section is the part of a code, which is very important and in multi-threading must be exclusively modified by any thread. Semaphore or mutex is used to protect critical section. In Java, you can use synchronized keyword or ReentrantLock to protect a critical section.


----


5. What is the difference between a value type and a reference type? (answer)
A value type is a more optimized type and always immutable e.g. primitive int, long, double and float in Java while a reference type points to an object, which can be mutable or Immutable. You can also say that value type points to a value while reference type points to an object.


----

6. What is heap and stack in a process? (detailed answer)
They are two separate areas of memory in the same process. Talking about Java, the stack is used to store primitive values and reference type to object but actual object is always created in heap. One critical difference between heap and stack is that heap memory is shared by all threads but each thread has their own stack.

----


7. What is revision/version control? (answer)
Version control is software which is used to store code and manage versions of codebase e.g. SVN, CVS, Git, Perforce, and ClearCase. They are very effective while comparing code, reviewing code and creating a build from previous stable version. All professional development use some sort of revision or version control tool, without them, you cannot manage code effectively, especially if 20 developers are working on same code base at the same time. Version control tool plays very important role to keep code base consistent and resolving code conflicts.

----


8. What is a strongly typed programming language? (answer)
In a strongly typed language compiler ensure type correctness, for example, you can not store the number in String or vice-versa. Java is a strongly typed language, that's why you have different data types e.g. int, float, String, char, boolean etc. You can only store compatible values in respective types. 

On the other hand, weakly typed language don't enforce type checking at compile time and they tree values based upon context. Python and Perl are two popular example of weakly typed programming language, where you can store a numeric string in number type.

----


9. Can you describe the difference between valid and well-formed XML?
A well-formed XML is the one which has root element and all tags are closed properly, attributes are defined properly, their value is also quoted properly. On another hand, a valid XML is the one which can be validated against an XSD file or schema. So it's possible for an XML to be well-formed but not valid because they contain tags which may not be allowed by their schema.


----

10. What is the difference between DOM and SAX parser? (detailed answer)
DOM parser is an in-memory parser so it loads whole XML file in memory and create a DOM tree to parse. SAX parser is an event based parser, so it parses XML document based on the event received e.g. opening tag, closing tag, the start of attribute or end of the attribute. 

Because of their working methodology, DOM parser is not suitable for large XML file as they will take a lot of space in memory and your process may run out of memory, SAX is the one which should be used to parse large files. For small files, DOM is usually much faster than SAX.

----



11. What is the relationship between threads and processes? (detailed answer)
A process can have multiple threads but a thread always belongs to a single process. Two processes cannot share memory space until they are purposefully doing inter-process communication via shared memory but two threads from the same process always share the same memory.


----

12. What is Immutable class mean? (detailed answer)
A class is said to be Immutable if its state cannot be changed once created, for example, String in Java is immutable. Once you create a String say "Java", you cannot change its content. Any modification in this string e.g. converting into upper case,  concatenating with another String will result in the new object. 

An immutable object is very useful for concurrent programming because they can be shared between multiple threads without worrying about synchronization. In fact, the whole model of functional programming is built on top of Immutable objects.

----


13. Why would you ever want to create a mock object? (answer)
A mock object is very useful to test an individual unit in your Software, in fact, stub and mocks a are a powerful tool for creating automated unit tests. Suppose you write a program to display currency conversion rates but you don't have a URL to connect to, now if you want to test your code, you can use mock objects. In Java world, there are a lot of frameworks which can create powerful mock objects for you e.g. Mockito and PowerMock.


----

14. What is SQL injection?
SQL injection is a security vulnerability which allows an intruder to steal data from the system. Any system which takes input from the user and creates SQL query without validating or sanitizing that input is vulnerable to SQL injection. In such system, an intruder can inject SQL code instead of data to retrieve more than expected data. 

There are many instances on which sensitive information e.g. user id, password, and personal details are stolen by exploiting this vulnerability. In Java, you can avoid SQL injection by using Prepared statement.

----


15. What is the difference between an inner join and a left join in SQL? (answer)
In SQL, there are mainly two types of joins, inner join, and outer join. Again outer joins can be two types right and left outer join. 

The main difference between inner join and left join is that in the case of former only matching records from both tables are selected while in the case of left join, all records from left table are selected in addition to matching records from both tables. 

Always watch out for queries which have "all" in it, they usually require left join like to write SQL query to find all departments and a number of employees on it. If you use inner join to solve this query, you will miss empty departments where no one works.

What is the difference between an inner join and a left join in SQL



----



16. What does the V in MVC stand for, and what does it signify? (answer)
V stands for View in MVC pattern. The view is what user sees  like web pages. This is a very important design pattern of web development which is based upon segregation of concern so that each area can be modified without impacting other areas. 

In Java world, there are lots of open source framework which provides an implementation of MVC pattern like Struts 2 and Spring MVC. 

By the way, M stands the for model and C stands the for controller. Modes are actual business objects like User, Employee, Order; while the controller is used for the routing request to correct processor.


----

17. What is the difference between a class and an object? (detailed answer)
A class is a blueprint on which objects are created. A class has code and behavior but an object has both the state and behavior. You cannot create an object without creating a class to represent its structure. The class is also used to map an object in memory, in Java, JVM does that for you.


----

18. What is loose-coupling?
Loose coupling is a desirable quality of software, which allows one part of the software to modify without affecting another part of the software. For example, in a loosely coupled software, a change in UI layout should not affect the back-end class structure.


----

19. What is the difference between composition, aggregation, and association? (detailed answer)
Association means two objects are related to each other but can exist without each other, Composition is a form of association where one object is composed of multiple objects, but they only exists together e.g. human body is the composition of organs, individual organs cannot live they only useful in the body. Aggregation is a collection of object e.g. city is an aggregation of citizens.

What is the difference between composition, aggregation, and association?


----



20. What is the difference between an interface and an abstract class? (detailed answer)
This is the most classical question of all programming interviews. An interface is the purest form of abstraction with nothing concrete in place while an abstract class is a combination of some abstraction and concrete things. The difference may vary depending upon language e.g. in Java you can extend multiple interface but you can only extend on the abstract class. For a more comprehensive discussion see the detailed answer.


----

21. What is unit testing? (answer)
Unit testing is a way to test individual unit for their functionality instead of testing whole application. There are a lot of tools to do the unit testing in different programming language e.g. in Java, you can use JUnit or TestNG to write unit tests. It is often run automatically during the build process or in a continuous environment like Jenkins.


----

22. Can you describe three different kinds of testing that might be performed on an application before it goes live?
unit testing, integration testing and smoke testing. Unit testing is used to test individual units to verify whether they are working as expected, integration testing is done to verify whether individually tested module can work together or not and smoke testing is a way to test whether most common functionality of software is working properly or not like in a flight booking website, you should be able to book, cancel or change flights.

----


23. What is the difference between iteration and recursion? (detailed answer)
Iteration uses a loop to perform the same step again and again while recursion calls the function itself to do the repetitive task. Many times recursion result in a clear and concise solution to a complex problem like tower of Hanoi, reversing a linked list or reversing a String itself. 

One drawback of recursion is depth  since recursion stores intermediate result in the stack you can only go up to a certain depth, after that your program will die with StackOverFlowError, this is why iteration is preferred over recursion in production code.


----

24. What is difference between & and && operator? (detailed answer)
& is a bitwise operator while && is a logical operator. One difference between & and && is that bitwise operator (&) can be applied to both integer and boolean but logical operator (&&) can only be applied to boolean variables. 

When you do a & b then AND operator is applied to each bit of both integer number, while in the case of a && b, the second argument may or may not be evaluated, that's why it is also known as short circuit operator, at least in Java. I like this question and often asked it to junior or developer and college graduates.

----


25. What is the result of 1 XOR 1? (example)
The answer is zero because XOR returns 1 if two operands are distinct and zero if two operands are same, for example, 0 XOR 0 is also zero, but 0 XOR 1 or 1 XOR 0 is always 1.

----


26. How do you get the last digit of an integer? (answer)
By using modulus operator, number % 10 returns the last digit of the number, for example, 2345%10 will return 5 and 567%10 will return 7.  Similarly, division operator can be used to get rid of the last digit of  a number e.g. 2345/10 will give 234 and 567/10 will return 56. This is an important technique to know and useful to solve problems like number palindrome or reversing numbers.

----


27. What is test-driven development?
Test driven is one of the popular development methodologies in which tests are written before writing any function code. In fact, test drives the structure of your program. Purists never wrote a single line of application code without writing a test for that. It greatly improve code quality and often attributed as a quality of Rockstar developers.

What is test-driven development?


----



28. What is the Liskov substitution principle? (answer)
Liskov substitution principle is one of the five principle introduced by Uncle Bob as SOLID design principles. It's the 'L' in SOLID. Liskov substitution principle asserts that every subtype should be able to work as the proxy for parent type. 

For example, if a method except object of Parent class then it should work as expected if you pass an object of the Child class. 

Any class which cannot stand in place of its parent violate LSP or Liskov substitution principle. This is actually a tough question to answer and if you do that you end up with creating a good impression on the interviewer's mind.


----

29. What is the Open closed design principle? (answer)
Open closed is another principle from SOLID, which asserts that a system should be open for extension but closed for modification. This means if new functionality is required in a stable system then your tried and tested code should not be touched and new functionality should be provided by adding new classes only. 


----

30. What is the difference between a binary tree and a binary search tree? (answer)
Binary search tree is an ordered binary tree, where the value of all nodes in the left tree are less than or equal to node and values of all nodes in right subtree is greater than or equal to the node (e.g. root). It's an important data structure and can be used to represent a sorted structure.

----


31. Can you give a practical example of a recursive algorithm? (example)
There are lots of places where recursive algorithm fits e.g. algorithm related to binary and linked list. A couple of examples of a recursive algorithm is reversing String and calculating Fibonacci series. Other examples include reversing linked list, tree traversal, and quick sort algorithm. 


----

31. What is the time complexity of an algorithm?
Time complexity specifies the ratio of time to the input. It shows how much time an algorithm will take to complete for a given number of input. It's approximated valued but enough to give you an indication that how your algorithm will perform if the number of input is increased from 10 to 10 million?

What is the time complexity of an algorithm?




----

32. What are some important differences between a linked list and an array? (detailed answer)
linked list and array are two of the most important data structure in the programming world. The most significant difference between them is that array stores its element at the contiguous location while linked list stores its data anywhere in memory. 

This gives linked list enormous flexibility to expand itself because memory is always scattered. 

It's always possible that you wouldn't be able to create an array to store 1M integers but can do by using linked list because space is available but not as contiguous chunk. All other differences are the result of this fact.

For example, you can search an element in array with O(1) time if you know the index but searching will take O(n) time in linked list. For more differences see the detailed answer.


----

33. What is a couple of ways to resolve collision in the hash table?  (answer)
linear probing, double hashing, and chaining. In linear probing, if the bucket is already occupied then function check next bucket linearly until it finds an empty one, while in chaining, multiple elements are stored in same bucket location.

----


34. What is a regular expression? (answer)
A regular expression is a way to perform pattern matching on text data. It's very powerful tool to find something like some character in a long string e.g. finding if a book contains some word or not. Almost all major programming language supports regular expression but Perl has been renowned for its enormous capability. 

Java also supports Perl-like regular expression using java.util.regex package. 

You can use the regular expression to check if an email is valid or not, if a phone number is valid, or if a zip code is valid, or even an SSN number is valid or not. One of the simplest examples of the regular expression is to check if a String is a number or not.

----


35. What is a stateless system?
A stateless system is a system which doesn't maintain any internal state. Such system will produce the same output for same input at any point of time. It's always easier to code and optimize a stateless system, so you should always strive for one if possible.

Programming Phone  Interview Questions answers


----


36. Write SQL query to find second highest salary in employee table? (solution)
This is one of the classic questions from SQL interviews, the event it's quite old it is still interesting and has lots of follow-ups you can use to check the depth of candidate's knowledge. You can find second highest salary by using the correlated and non-correlated subquery. 

You can also use keyword's like TOP or LIMIT if you are using SQL Server or MySQL, given Interviewer allows you. The simplest way to find 2nd highest salary is following:

SELECT MAX(Salary) FROM Employee 
WHERE Salary NOT IN (SELECT MAX(Salary) FROM Employee)

This query first finds maximum salary and then exclude that from the list and again finds maximum salary. Obviously second time, it would be second highest salary.


----

37. Can you describe the difference between correlated and non-correlated subquery? (answer)
In correlated sub-query, the inner query depends upon the outer query and executes for each row in the outer query. While non-correlated subquery doesn't depend upon the outer query and can be executed independently. 

Due to this reason, former is slow and later is fast. BTW, correlated subquery has some nice applications, one of them is finding Nth highest salary in Employee table, as seen on previous SQL question as well.


----

39. How do you find if a number is a power of two, without using an arithmetic operator? (solution)
Assume it's a question of using the bitwise operator as soon as you hear restriction about not allowed to use arithmetic operator. If that restriction is not in place then you can easily check if a number is a power of two by using modulus and division operator. By the using bitwise operator, there is a nice trick to do this.  You can use following code to check if a number if power of two or not

public static boolean powerOfTwo(int x) {
        return (x & (x - 1)) == 0;
}

x & (x-1) is a nice trick to convert right most bit to zero if it's on, I learned from hackers delight book.


----

40. How do you find a  running Java process on UNIX? (command)
You can use the combination of 'ps' and 'grep' command to find any process running on UNIX machine. Suppose your Java process has a name or any text which you can use to match against just use following command.

ps -ef | grep "myJavaApp"

ps -e will list every process i.e. process from all user not just you and  ps -f will give you full details including PID, which will be required if you want to investigate more or would like to kill this process using kill command.

----


41. How do you find large files in UNIX  like more than 1GB? (command)
You can easily find big files by using the find command because it provides an option to search files based upon their size. Use this if your file system is full and your Java process is crashing with no more space. This command will list all files which are more than 1GB. You can tweak the size easily like to find all files with more than 100 MB just use +100M.

find . - type f -size +1G -print


----

42. What is the shell script? (courses)
A shell script is a set of shell commands with some programming constructs e.g. if and for loop, which allows you to automate some repetitive task. For example, you can write a shell script to the daily cleanup of logs files,  for backing up data for historical use and for other housekeeping jobs, releases, and monitoring.


That's all in this list of programming questions for phone interviews. You might have noticed that there are only 42 questions but the title mentioned about 50 questions, where are the remaining 8 questions? Well Instead of sharing 8 questions I am sharing with you guys 8 more articles where you can find the remaining programming questions.  here you go:
20 String Coding Questions for Programmers ( read here)
15 Data Structure and Algorithm questions for Software developers (see here)
25 Spring Security Interview questions (Spring security questions)
10 Interview Questions Every Developer Should Know (read more)
20 Core Java Question from Programmers for 2 to 3 years experienced (check here)
30 System Design Interview Questions with answers (System design questions)
21 SQL Query Interview Questions with Answers (read more)
23 Tricky Questions for Java Programmers  (read here)
10 XML Interview Questions for Programmers (see here)
50 Multithreading and Concurrency Questions from Java Interviews (check here)
20 Software design Questions from Programming Interviews (read more)
18 Java Design Pattern Interview questions. (see here)
100+ Data Structure Interview Questions with answers (data structure questions)
75 Programming Interview Questions with answers (programming questions)
10 Dynamic Programming Problems for interview (dynamic programming questions)
25 Recursion based coding problems with answers (recursion questions)
50 SQL and Database Questions for Interviews (SQL questions)
50+ OOP Questions with answers (object oriented programming questions)

Thanks for reading this far, If you like this article and found it useful for your telephonic interviews, please share it with your friends and colleges.  Any feedback to improve the quality of interview questions will be highly appreciated.

P. S. - If you are preparing for coding interviews and need resources to prepare well then I also suggest you to take a look at these best coding interview courses from Udemy, Coursera, Educative, and ZTM Academy. I have collected them and arranged them based upon how I found them effective for coding interview preparation. 


Read more: https://javarevisited.blogspot.com/2015/02/50-programmer-phone-interview-questions-answers.html#ixzz80dhW7mB9

</https://javarevisited.blogspot.com/2015/02/50-programmer-phone-interview-questions-answers.html#axzz80dfcO0nd>