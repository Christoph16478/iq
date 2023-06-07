### https://quescol.com/interview-preparation/core-java-interview-questions

## **Name most important websites to get Java related information/updates/trends/ etc.?**

* [Java basics](https://www.javatpoint.com/java-basics)

* [Java Platform, Standard Edition Documentation](https://docs.oracle.com/en/java/javase/)
    * [The Java Compiler (javac)](https://docs.oracle.com/en/java/javase/20/docs/specs/man/javac.html)
    * [JVM](https://docs.oracle.com/javase/specs/jvms/se7/html/)
    * [JRE](https://www.oracle.com/java/technologies/javase/jre8-readme.html)

* [OOP in Java](https://docs.oracle.com/javase/tutorial/java/concepts/)

* [Java Platform, Standard Edition & Java Development Kit Version 20 API Specification](https://docs.oracle.com/en/java/javase/20/docs/api/)
    * [Introduction of Java Swing](https://www.geeksforgeeks.org/introduction-to-java-swing/)
    * [JavaFX](https://docs.oracle.com/javase/8/javase-clienttechnologies.htm)
    * [JDBC API](https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/)

* Java development tools:
    * [Maven Getting Started Guide](https://maven.apache.org/guides/getting-started/)
    * [Gradle Build Tool](https://gradle.org/guides/#close-notification)
    * [Git - Documentation](https://git-scm.com/doc)

* [Java Multithreading](https://www.geeksforgeeks.org/multithreading-in-java/)

* [Java Concurrency](https://www.geeksforgeeks.org/java-concurrency-yield-sleep-and-join-methods/)

* [Java Exception Handling](https://www.geeksforgeeks.org/exceptions-in-java/)

* [Software Design Patterns](https://www.geeksforgeeks.org/software-design-patterns/)

* [Java Memory Management](https://www.geeksforgeeks.org/java-memory-management/)

* [12 Tips to Optimize Java Code Performance](https://www.geeksforgeeks.org/12-tips-to-optimize-java-code-performance/)
    * [How to Optimize Your Code for Performance](https://dev.to/roy8/how-to-optimize-your-code-for-performance-1km5)

* [Java EE](https://docs.oracle.com/javaee/7/index.html)

* Frameworks and Libraries
    * [Java Spring](https://de.wikipedia.org/wiki/Spring_(Framework))
    * [Hibernate](https://www.geeksforgeeks.org/introduction-to-hibernate-framework/)
    * [Apache Struts](https://www.geeksforgeeks.org/introduction-and-working-of-struts-web-framework/)
    * [JavaFX](https://docs.oracle.com/javase/8/javase-clienttechnologies.htm)

* Testing
    * [JUnit](https://www.geeksforgeeks.org/how-to-write-test-cases-in-java-application-using-mockito-and-junit/)
    * [Behavior-driven development](https://www.geeksforgeeks.org/behavioral-driven-development-bdd-in-software-engineering/)
        * [Cucumber](https://www.tutorialspoint.com/cucumber/index.htm)
            * [Gherkin](https://cucumber.io/docs/gherkin/)
    * [Unit tests](https://www.geeksforgeeks.org/unit-testing-software-testing/)
    * [Integration tests](https://www.geeksforgeeks.org/software-engineering-integration-testing/)
    * [Automated tests](https://www.geeksforgeeks.org/software-testing-automation-testing/)
        
* CI/CD
    * [Jenkins](https://www.geeksforgeeks.org/what-is-jenkins/)
    * [Travis CI](https://docs.travis-ci.com/user/languages/java/)
    * [GitLab CI/CD](https://docs.gitlab.com/ee/ci/)

* Industry Best-Practices
    * [Java Oracle Documentation](https://docs.oracle.com/en/java/)
        * [Java Documentation on tutorialspoint.com](https://www.tutorialspoint.com/java/java_documentation.htm)
        * [9 - Naming Conventions](https://www.oracle.com/java/technologies/javase/codeconventions-namingconventions.html)
        * [Java Code Style Guidelines](https://www.cs.cornell.edu/courses/JavaAndDS/JavaStyle.html)
    * [How to Write Doc Comments for the Javadoc Tool](https://www.oracle.com/technical-resources/articles/java/javadoc-tool.html) 
    * [2 Java Language Best Practices](https://docs.oracle.com/cd/A97688_16/generic.903/bp/java.htm)
    * Latest trends in Java:
        * [https://blogs.oracle.com/java/](https://blogs.oracle.com/java/)
        * [https://www.baeldung.com/](https://www.baeldung.com/)
        * [https://www.infoq.com/java/](https://www.infoq.com/java/)
        * [https://dzone.com/java](https://dzone.com/java)
        * [https://www.infoworld.com/category/java/](https://www.infoworld.com/category/java/)
        * [https://www.reddit.com/r/java/](https://www.reddit.com/r/java/)
        * [https://www.javacodegeeks.com/](https://www.javacodegeeks.com/)
        * [https://blogs.oracle.com/javamagazine/](https://blogs.oracle.com/javamagazine/)

----

## **For what can Java be used for?**

- Desktop Applications: Java FX, Swing
- Web Applications: JavaEE(JSF, JSP), Java Servlets
- Mobile Applications: Android SDK
- Server-Side Development: Java Serverlets, JSP, JSF, JavaEE
- Big Data: Apache Hadoop
- Scientific Coputing: Python or MATLAB
- Internet of Things (IoT): JavaME(Micro Edition)


----

## **What do you understand by Class in Java?**

A class is a blueprint from which objects are created. We can also define it as it is a group of objects which
have common properties. This properties is set by class for all method and properties of class.

Class declaration have components mentioned below:

__Class name__

```java
/**
* <h1>Main</h1>
* The Main program implements an application that
* simply returns a new Person object.
* <p>
* her can get another part of the comment if necessary.
*
* @author  ch
* @version 1.0
*/
class Person { // class name
    // body of the class
}

/**
* <h1>Main</h1>
* The Main program implements an application that
* simply returns a new Person object.
* <p>
* Giving proper comments in your program makes it more
* user friendly and it is assumed as a high quality code.
*
* @author  ch
* @version 1.0
* @since   2023-06-06 
*/
public class Main {
   /**
   * This is the main method which makes use of method X.
   * @param args Unused
   * @return Nothing
   * @exception IOException On input error
   */    
    public static void main(String argv[]) {
        // Brings new object to live.
        Person P1 = new Person();
    }
}
```

[__Modifiers__](https://www.w3schools.com/java/java_modifiers.asp)

```java
/**
 * Main class
 */
public class Main {
    public static void main(String argv[]) {
        // code
    }
}
```

__Interface__

```java
/**
* Returns an Image object that can then be painted on the screen. 
* The url argument must specify an absolute <a href="#{@link}">{@link URL}</a>. The name
* argument is a specifier that is relative to the url argument. 
* <p>
* This method always returns immediately, whether or not the 
* image exists. When this applet attempts to draw the image on
* the screen, the data will be loaded. The graphics primitives 
* that draw the image will incrementally paint on the screen. 
*
* @author (classes and interfaces only, required)
* @version (classes and interfaces only, required. See footnote 1)
* @param (methods and constructors only)
* @return (methods only)
* @exception (@throws is a synonym added in Javadoc 1.2)
* @see
* @since
* @serial (or @serialField or @serialData)
* @deprecated (see How and When To Deprecate APIs)
*/
interface Image {
    public void imageSize(); // interface method (does not have a body)
    public void run(); // interface method (does not have a body)
}

/**
 * Main class
 */
public class Main {
    public static void main(String argv[]) {
        // code
    }
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
import java.io?*;
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
        System.out.println("salary : " + salary);
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
public class Main {
    public static void main(String[] args)
    {
        // accessing a static nested class
        OuterClass.StaticNestedClass nestedObject = new OuterClass.StaticNestedClass();

        nestedObject.display();
    }
}

// Output:
// outer_x = 10
// outer_private = 30
// outer_y = 20
```

__Nested Interface__

```java
// Java program to demonstrate working of
// interface inside a class.

class Test {
    interface Yes {
        void show();
    }
}

class Testing implements Test.Yes {
    public void show() {
        System.out.println("show method of interface");
    }
}

class Main {
    public static void main(String[] args) {
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
class {
    // body of the class
	field;
	method;
}
```

----

## **What do you understand by Object?**

Object is a basic unit of OOPs. It is also an instance of a class. Everything in OOPs is
represented using Objects. In General we can define Object as it is a real world entity
that has its own some states and behaviour.

For Example: Cat is a suitable example of an objects. Cat has its own states and
behaviour and its is also a real world entity. Cat can walk, eat is its behaviour
and Cat can be white, black is its states.

Objects have some characteristics :

1. State : State Reflects the properties of Objects. Just like Cat can be white,
black or may be combination of both is its properties. State can be denoted by
attributes.

2. Behaviour : Behaviours shows that how object is responding to other objects.
Behaviour can be denoted by Methods.

3. Identity: Every objects should have unique identity. Like if we say cat
then it may be a group of cat but If we talk about a particular cat then we
need a identity for that particular cat.

---

## **Explain JDK, JVM and JRE?**

__JDK:__ JDK stands for Java Development Kit which contains JRE. It gives a
development environment for Java applications where developer can code and
run java programs.

__JRE:__ JRE Stands for Java Runtime Environment that contains class libraries, loader class
and JVM. Its main function is to run Java Program. If you don’t want to develop program
then you don’t need JDK But, for only the purpose of execution of java program you only need
JRE. JRE comes with JDK bundle you don’t need to download it separately.

__JVM:__ JVM stands for Java Virtual Machine that provide the runtime environment to java code
where Java code is executed. JVM is a part of JRE that converts java byte code into
machine code. In java, compiler produces code for JVM.

----

## **Explain Public Static void Main(String args[]) in Java?**

It is an entry point of any Java program from where Execution starts.

__Public:__ Public is a access modifier that define the accessibility of method. If any method have Public access modifier it means that it can access by any other class.

__Static:__ static is a keyword in java that define class level member. It means that without
creating any instance it can be accessible using class name.

__void:__ void is also a keyword that define the return type of any methods. If method have void
keyword it means that method will not return any value.

__Main:__ It is a method from where execution starts. It is searched by JVM to start the execution.

__String args[]:__ it is a main method argument.

---

## **What is the different between Final, finally and finilize?**

__Final:__
final is a modifier which is used with classes, methods and variables. If the class is declared as final then that class is not extended by other class. If the method is declared as final then we cannot override that method in the child class. i.e. final method is not overridden by child class. If the variable is declared as final then it behave as a constant and we cannot re-assingment for that variable.

__finally:__
finally is a block which is always associated with try-catch block.finally block is always executed whether exception is handled or not.finally block is used to execute important code such as closing connection, stream when any exception arise.

__finalize()__
finalize() method is used to perform cleanup operation just before destroying any object. This finalize() method is always invoked by garbage collector. 

----

## **What is the difference between "==" and "equals()" method?**

"==" is used for address/reference comparison.

Example:

```java
String str1=new String("prakash");
String str2=new String("prakash");
System.out.println(str1==str2);
// Output: false
```

equals() is used for content comparision.

Example:

```java
String str1=new String("prakash");
String Str2=new String("prakash");
System.out.println(str1.equals(str2));
// Output: true
```

----

## **Why Java is called as platform independent?**

After the compilation of Java code, code is converted into byte code. This byte code
can be executed in any other system and environment. Because of that it is known as
platform independent.

----

## **What is meant by Local variable and Instance variable?**

Local variables are defined in the method and scope of the variables that have existed
inside the method itself.

An instance variable is defined inside the class and outside the method and scope of the
variables exist throughout the class.

----

## **Define Constructor?**

We can define as constructor is a method or block which is use to initialise the objects. Constructor should have same name as a name
of class which have no return type. It is automatically called by java at the time of object creation.

__There are 3 types of constructor:__
1. Default constructor: It is automatically inserted by Java when we not declared any constructor. It is not visible in your source code.
2. Parameterised constructor : Constructor with arguments are known as Parameterised constructor.
3. No-arg Constructor : it is very similar to default constructor. We declare it when we want to perform some operation at a time of object creation then we write that code in no-args constructor. For example some initialization of value.

----

## **Explain access modifiers in Java?**

Access modifiers is a keywords in Java that define the accessibility of any class, methods and member variables.

__There are 4 types of access modifiers in Java:__
- Public
- Private
- Protected
- Default

| Modifier | Default | Private | Protected | Public |
| -------- | ------- | ------- | --------- | ----- |
| Same class | YES | YES | YES | YES |
| Same Package subclass | YES | NO | YES | YES |
| Same Package non-subclass | YES | NO | YES | YES |
| Different package subclass | NO | NO | YES | YES |
| Different package non-subclass | NO | NO | NO | YES |

----

## **Explain some features of oops?**

__Inheritance:__ Inheritance is process in which child objects of child class acquires the all properties and behaviour of its parent class. It improves the code reusability.


```java
// Parent class
class Vehicle {
    protected String brand;

    public Vehicle(String brand) {
        this.brand = brand;
    }

    public void drive() {
        System.out.println("Driving the vehicle");
    }
}

// Child class inheriting from the parent class
class Car extends Vehicle {
    private int numberOfSeats;

    public Car(String brand, int numberOfSeats) {
        super(brand);
        this.numberOfSeats = numberOfSeats;
    }

    public void displayInfo() {
        System.out.println("Brand: " + brand);
        System.out.println("Number of Seats: " + numberOfSeats);
    }
}

// Main class
public class Main {
    public static void main(String[] args) {
        Car car = new Car("Toyota", 5);
        car.displayInfo();
        car.drive();
    }
}
```

__Abstraction:__ Abstraction means hide the complexity and show the functionality. For examples in education portal
you just sign up and then login by giving credential and then access your dashboard but you won’t aware of
how its happening in backend. It is known as abstraction.

```java
// Abstract parent class
abstract class Shape {
    abstract double calculateArea(); // Abstract method
    abstract double calculatePerimeter(); // Abstract method
}

// Concrete child class implementing the Shape abstract class
class Circle extends Shape {
    private double radius;

    public Circle(double radius) {
        this.radius = radius;
    }

    @Override
    double calculateArea() {
        return Math.PI * radius * radius;
    }

    @Override
    double calculatePerimeter() {
        return 2 * Math.PI * radius;
    }
}

// Concrete child class implementing the Shape abstract class
class Rectangle extends Shape {
    private double length;
    private double width;

    public Rectangle(double length, double width) {
        this.length = length;
        this.width = width;
    }

    @Override
    double calculateArea() {
        return length * width;
    }

    @Override
    double calculatePerimeter() {
        return 2 * (length + width);
    }
}

// Main class
public class Main {
    public static void main(String[] args) {
        Circle circle = new Circle(5);
        System.out.println("Circle Area: " + circle.calculateArea());
        System.out.println("Circle Perimeter: " + circle.calculatePerimeter());

        Rectangle rectangle = new Rectangle(4, 6);
        System.out.println("Rectangle Area: " + rectangle.calculateArea());
        System.out.println("Rectangle Perimeter: " + rectangle.calculatePerimeter());
    }
}
```

__Encapsulation:__ Encapsulation is a process of binding the data and methods together in a single entity
known as class for data safety.

```java
// Encapsulated class
class Person {
    private String name;
    private int age;

    // Getter methods
    public String getName() {
        return name;
    }

    public int getAge() {
        return age;
    }

    // Setter methods
    public void setName(String name) {
        this.name = name;
    }

    public void setAge(int age) {
        if (age >= 0) {
            this.age = age;
        }
    }
}

// Main class
public class Main {
    public static void main(String[] args) {
        Person person = new Person();

        // Accessing and setting private fields using public getter and setter methods
        person.setName("John");
        person.setAge(25);

        // Accessing private fields using public getter methods
        System.out.println("Name: " + person.getName());
        System.out.println("Age: " + person.getAge());
    }
}
```

__Polymorphism:__ Polymorphism defines to perform single actions in multiple form. It is derived from two
word Poly + morphs that means many forms.

```java
// Parent class
class Animal {
    public void makeSound() {
        System.out.println("Animal is making a sound");
    }
}

// Child class 1
class Dog extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Dog is barking");
    }
}

// Child class 2
class Cat extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Cat is meowing");
    }
}

// Main class
public class Main {
    public static void main(String[] args) {
        Animal animal1 = new Dog();
        Animal animal2 = new Cat();

        animal1.makeSound(); // Output: Dog is barking
        animal2.makeSound(); // Output: Cat is meowing
    }
}
```

It is of two types:

- Method overloading

In method overloading a class have different methods with same name but different number of arguments. In Overloading case methods should have different signature. It is also known as compile time polymorphism.

```java
class Calculator {
    public int add(int a, int b) {
        return a + b;
    }

    public double add(double a, double b) {
        return a + b;
    }

    public int add(int a, int b, int c) {
        return a + b + c;
    }
}

public class Main {
    public static void main(String[] args) {
        Calculator calculator = new Calculator();

        int sum1 = calculator.add(5, 10);
        System.out.println("Sum 1: " + sum1);

        double sum2 = calculator.add(3.5, 2.5);
        System.out.println("Sum 2: " + sum2);

        int sum3 = calculator.add(2, 4, 6);
        System.out.println("Sum 3: " + sum3);
    }
}
```

- Method Overriding

In Method Overriding sub class have similar method as parent class. Similar mean name, return type, parameter of methods for both parent and sub class method.

```java
// Parent class
class Animal {
    public void makeSound() {
        System.out.println("Animal is making a sound");
    }
}

// Child class
class Dog extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Dog is barking");
    }
}

// Main class
public class Main {
    public static void main(String[] args) {
        Animal animal = new Dog();
        animal.makeSound(); // Output: Dog is barking
    }
}
```

----

## **What is this and super keyword in Java?**

__this:__ this is a keyword is use to access the member of present class.

```java
class Person {
    private String name;

    public Person(String name) {
        this.name = name;
    }

    public void printName() {
        System.out.println("Name: " + this.name);
    }

    public void changeName(String newName) {
        this.name = newName;
    }
}

public class Main {
    public static void main(String[] args) {
        Person person = new Person("John");
        person.printName(); // Output: Name: John

        person.changeName("David");
        person.printName(); // Output: Name: David
    }
}
```

__super:__ super keyword is used to access the member of parent class.

```java
class Vehicle {
    protected String brand;

    public Vehicle(String brand) {
        this.brand = brand;
    }

    public void displayInfo() {
        System.out.println("Brand: " + brand);
    }
}

class Car extends Vehicle {
    private int numberOfSeats;

    public Car(String brand, int numberOfSeats) {
        super(brand);
        this.numberOfSeats = numberOfSeats;
    }

    public void displayInfo() {
        super.displayInfo();
        System.out.println("Number of Seats: " + numberOfSeats);
    }
}

public class Main {
    public static void main(String[] args) {
        Car car = new Car("Toyota", 5);
        car.displayInfo();
    }
}
```

----

## **What is the different between static and non-static method of java?**

__Static method:__ static method is a class level method. We need not required any instance to access them we can access it directly using class. A static method can only access static variable.

```java
class MathUtils {
    public static int add(int a, int b) {
        return a + b;
    }

    public static double multiply(double a, double b) {
        return a * b;
    }
}

public class Main {
    public static void main(String[] args) {
        int sum = MathUtils.add(5, 3);
        System.out.println("Sum: " + sum); // Output: Sum: 8

        double product = MathUtils.multiply(2.5, 4.0);
        System.out.println("Product: " + product); // Output: Product: 10.0
    }
}
```

__Non-static method:__ non-static method belongs to objects of the class. It can be accessible inside the static method with the help of class instance.

```java
class Circle {
    private double radius;

    public Circle(double radius) {
        this.radius = radius;
    }

    public double calculateArea() {
        return Math.PI * radius * radius;
    }

    public double calculateCircumference() {
        return 2 * Math.PI * radius;
    }
}

public class Main {
    public static void main(String[] args) {
        Circle circle = new Circle(5.0);
        double area = circle.calculateArea();
        double circumference = circle.calculateCircumference();

        System.out.println("Area: " + area); // Output: Area: 78.53981633974483
        System.out.println("Circumference: " + circumference); // Output: Circumference: 31.41592653589793
    }
}
```

----

## **What do you mean by Polymorphism?**

Polymorphism is derived from two greek word “poly” and “morphs” means many form. It allows to perform single task in
multiple form. In Java term we can say that there can be multiple methods with same name but different functionality.

It is of two types:

1. Compile time polymorphism

```java
class Calculator {
    public int add(int a, int b) {
        return a + b;
    }

    public double add(double a, double b) {
        return a + b;
    }

    public int add(int a, int b, int c) {
        return a + b + c;
    }
}

public class Main {
    public static void main(String[] args) {
        Calculator calculator = new Calculator();

        // compiler chooses at runtime what method
        // to use
        int sum1 = calculator.add(5, 10);
        System.out.println("Sum 1: " + sum1);

        double sum2 = calculator.add(3.5, 2.5);
        System.out.println("Sum 2: " + sum2);

        int sum3 = calculator.add(2, 4, 6);
        System.out.println("Sum 3: " + sum3);
    }
}
```

1. Runtime Polymorphism

```java
class Animal {
    public void makeSound() {
        System.out.println("Animal is making a sound");
    }
}

class Dog extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Dog is barking");
    }
}

class Cat extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Cat is meowing");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal animal1 = new Dog();
        Animal animal2 = new Cat();

        // at runtime method is chosen
        animal1.makeSound(); // Output: Dog is barking
        animal2.makeSound(); // Output: Cat is meowing
    }
}
```

__NOTE: Compile time polymorphism is also known as method overloading and Runtime polymorphism is known as overriding.__

----

How many ways you can overload method?

1. By number of passing parameters the valid case for overloading the method is

```java
add(int,int)
add(int,int,int)
```

2. By changing the data type of parameter

```java
add(int,int)
add(float,int)
```

3. By changing the sequence of data type

```java
add(int, float)
add(float,int)
```

----

## **What is the some invalid cases of method overloading in Java?**

In java if two methods having the same name, same parameters but different return type,
then this is not a valid method overloading. Also if two methods having the same name,
same parameters and different return type, then this is also not a valid method
overloading. This will throw compilation error.

Example:

```java
int sum(int,int)
float sum(int,int)
```

----

## **What do you mean by abstract class?**

Abstract class is declared with the help of Abstract Keyword. It can have both abstract and non-abstract method. We cannot instantiate abstract method. It is extended by another class which can implement its methods to use. It can have static and final methods.

Data abstraction is the process of hiding certain details and showing only essential information to the user.
Abstraction can be achieved with either abstract classes or interfaces (which you will learn more about in the next chapter).

The abstract keyword is a non-access modifier, used for classes and methods:

Abstract class: is a restricted class that cannot be used to create objects (to access it, it must be inherited from another class).

Abstract method: can only be used in an abstract class, and it does not have a body. The body is provided by the subclass (inherited from).

```java
abstract class Animal {
  public abstract void animalSound();
  public void sleep() {
    System.out.println("Zzz");
  }
}
```

----

## **What do you mean by Interface?**

Interface is a blueprint of class that have abstract and public methods without body. Class that implements interface should implement all methods of interface.

```java
public interface Man
{
	public void eat();
	public void sleep();
	public void walk();
}
```

----

## **Difference between String and StringBuffer?**

String: String object is immutable but the StringBuffer objects are mutable.
Immutable means once we create a String object we cannot perform any changes
on object.

Example of String:

```java
String str=new String("prakash");
str.concat("kumar");
System.out.println(str);
output:- prakash
```

Example of StringBuffer:

```java
StringBuffer strbfr=new StringBuffer("prakash");
strbfr.append("kumar");
System.out.println(strbfr);
output:- prakash kumar
```

----

## **Difference between StringBuffer and StringBuilder?**

Both StringBuffer and StringBuilder are mutable.

__StringBuffer:__

All method of StringBuffer is synchronized. As it is synchronized, it is also thread-safe. Thread-Safe means two
threads can’t call the StringBuffer method simultaneously. Its performance is low because every task is dependent on the other.

Example:

```java
StringBuffer strbuffer = new StringBuffer("java"); 
strbuffer.append("developer"); 
System.out.println(strbuffer); 
```

__StringBuilder:__

Methods are not synchronized so it is not thread-safe. It means two threads can call the string builder method simultaneously. Its performance is high because more than one thread can be allowed.

Example:

```java
StringBuilder strBuilder=new StringBuilder("java"); 
strBuilder.append("developer"); 
System.out.println(strBuilder);
```

----

## **Difference between String, StringBuilder and StringBuffer?**

__Factor__
- String
- StringBuilder
- StringBuffer

__Storage Area__
- Constant String Pool
- Heap Area
- Heap Area

__Mutability__
- Immutable
- Mutable
- Mutable

__Thread Safety__
- Yes
- No
- Yes

__Performance__
- Fast
- More efficient
- Less efficient

----

## **Difference between Array and ArrayList?**

__Arrays:__

Array is fixed in size which is decided at a time of array declaration.
Array can contain both primitives data and objects.

Example:

```java
int arr[] = new int[3];
arr[0]=10; 
arr[1]=20; 
arr[2]=70;
Arrays.stream(arr).forEach(e->System.out.print(e + " "));
```

__ArrayList:__

Size of ArrayList is dynamic.
It is a part of the collection framework of java.
ArrayList can contain the only object. After Java 5 It converts primitive data into object itself.

```java
ArrayList<Integer> arrList = new ArrayList<Integer>(3);
for (int i = 1; i <= 3; i++)
{
    arrList.add(i);
}
arrList.stream().forEach(e->System.out.print(e + " ")); 
```

----

## **What do you mean by Collections in Java?**

Collection is a Java framework that have some predefined class and interfaces to store and manipulate the group of objects.

__Interfaces comes with Collection framework:__

- Set

```java
import java.util.HashSet;
import java.util.Set;

public class Main {
    public static void main(String[] args) {
        // Create a new set
        Set<String> fruits = new HashSet<>();

        // Add elements to the set
        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Orange");

        // Print the set
        System.out.println("Set: " + fruits); // Output: Set: [Apple, Banana, Orange]

        // Check if an element exists in the set
        boolean containsBanana = fruits.contains("Banana");
        System.out.println("Contains Banana? " + containsBanana); // Output: Contains Banana? true

        // Remove an element from the set
        boolean removedApple = fruits.remove("Apple");
        System.out.println("Removed Apple? " + removedApple); // Output: Removed Apple? true

        // Print the updated set
        System.out.println("Set: " + fruits); // Output: Set: [Banana, Orange]

        // Get the size of the set
        int size = fruits.size();
        System.out.println("Size: " + size); // Output: Size: 2

        // Iterate over the elements in the set
        System.out.println("Elements:");
        for (String fruit : fruits) {
            System.out.println(fruit);
        }
        /* Output:
           Elements:
           Banana
           Orange
         */
    }
}
```

- List

```java
import java.util.ArrayList;
import java.util.List;

public class Main {
    public static void main(String[] args) {
        // Create a new list
        List<String> fruits = new ArrayList<>();

        // Add elements to the list
        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Orange");

        // Print the list
        System.out.println("List: " + fruits); // Output: List: [Apple, Banana, Orange]

        // Access elements by index
        String firstFruit = fruits.get(0);
        System.out.println("First Fruit: " + firstFruit); // Output: First Fruit: Apple

        // Update an element in the list
        fruits.set(2, "Grapes");
        System.out.println("Updated List: " + fruits); // Output: Updated List: [Apple, Banana, Grapes]

        // Remove an element from the list
        boolean removed = fruits.remove("Banana");
        System.out.println("Removed Banana? " + removed); // Output: Removed Banana? true

        // Check if an element exists in the list
        boolean containsGrapes = fruits.contains("Grapes");
        System.out.println("Contains Grapes? " + containsGrapes); // Output: Contains Grapes? true

        // Get the size of the list
        int size = fruits.size();
        System.out.println("Size: " + size); // Output: Size: 2

        // Iterate over the elements in the list
        System.out.println("Elements:");
        for (String fruit : fruits) {
            System.out.println(fruit);
        }
        /* Output:
           Elements:
           Apple
           Grapes
         */
    }
}
```

- Queue

```java
import java.util.LinkedList;
import java.util.Queue;

public class Main {
    public static void main(String[] args) {
        // Create a new queue
        Queue<String> queue = new LinkedList<>();

        // Add elements to the queue
        queue.offer("Apple");
        queue.offer("Banana");
        queue.offer("Orange");

        // Print the queue
        System.out.println("Queue: " + queue); // Output: Queue: [Apple, Banana, Orange]

        // Access the element at the front of the queue
        String frontElement = queue.peek();
        System.out.println("Front Element: " + frontElement); // Output: Front Element: Apple

        // Remove the element at the front of the queue
        String removedElement = queue.poll();
        System.out.println("Removed Element: " + removedElement); // Output: Removed Element: Apple

        // Print the updated queue
        System.out.println("Updated Queue: " + queue); // Output: Updated Queue: [Banana, Orange]

        // Check if the queue contains an element
        boolean containsBanana = queue.contains("Banana");
        System.out.println("Contains Banana? " + containsBanana); // Output: Contains Banana? true

        // Get the size of the queue
        int size = queue.size();
        System.out.println("Size: " + size); // Output: Size: 2

        // Iterate over the elements in the queue
        System.out.println("Elements:");
        for (String fruit : queue) {
            System.out.println(fruit);
        }
        /* Output:
           Elements:
           Banana
           Orange
         */
    }
}
```

- Dequeue

```java
import java.util.Deque;
import java.util.LinkedList;

public class Main {
    public static void main(String[] args) {
        // Create a new deque
        Deque<String> deque = new LinkedList<>();

        // Add elements to the front of the deque
        deque.addFirst("Apple");
        deque.addFirst("Banana");

        // Add elements to the end of the deque
        deque.addLast("Orange");
        deque.addLast("Grapes");

        // Print the deque
        System.out.println("Deque: " + deque); // Output: Deque: [Banana, Apple, Orange, Grapes]

        // Access the element at the front of the deque
        String frontElement = deque.peekFirst();
        System.out.println("Front Element: " + frontElement); // Output: Front Element: Banana

        // Access the element at the end of the deque
        String rearElement = deque.peekLast();
        System.out.println("Rear Element: " + rearElement); // Output: Rear Element: Grapes

        // Remove the element at the front of the deque
        String removedFrontElement = deque.pollFirst();
        System.out.println("Removed Front Element: " + removedFrontElement); // Output: Removed Front Element: Banana

        // Remove the element at the end of the deque
        String removedRearElement = deque.pollLast();
        System.out.println("Removed Rear Element: " + removedRearElement); // Output: Removed Rear Element: Grapes

        // Print the updated deque
        System.out.println("Updated Deque: " + deque); // Output: Updated Deque: [Apple, Orange]

        // Check if the deque contains an element
        boolean containsOrange = deque.contains("Orange");
        System.out.println("Contains Orange? " + containsOrange); // Output: Contains Orange? true

        // Get the size of the deque
        int size = deque.size();
        System.out.println("Size: " + size); // Output: Size: 2

        // Iterate over the elements in the deque
        System.out.println("Elements:");
        for (String fruit : deque) {
            System.out.println(fruit);
        }
        /* Output:
           Elements:
           Apple
           Orange
         */
    }
}
```

__Classes comes with Collection framework:__

- ArrayList

```java
import java.util.ArrayList;

public class Main {
    public static void main(String[] args) {
        // Create a new ArrayList
        ArrayList<String> fruits = new ArrayList<>();

        // Add elements to the ArrayList
        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Orange");

        // Print the ArrayList
        System.out.println("ArrayList: " + fruits); // Output: ArrayList: [Apple, Banana, Orange]

        // Access elements by index
        String firstFruit = fruits.get(0);
        System.out.println("First Fruit: " + firstFruit); // Output: First Fruit: Apple

        // Update an element in the ArrayList
        fruits.set(2, "Grapes");
        System.out.println("Updated ArrayList: " + fruits); // Output: Updated ArrayList: [Apple, Banana, Grapes]

        // Remove an element from the ArrayList
        boolean removed = fruits.remove("Banana");
        System.out.println("Removed Banana? " + removed); // Output: Removed Banana? true

        // Check if an element exists in the ArrayList
        boolean containsGrapes = fruits.contains("Grapes");
        System.out.println("Contains Grapes? " + containsGrapes); // Output: Contains Grapes? true

        // Get the size of the ArrayList
        int size = fruits.size();
        System.out.println("Size: " + size); // Output: Size: 2

        // Iterate over the elements in the ArrayList
        System.out.println("Elements:");
        for (String fruit : fruits) {
            System.out.println(fruit);
        }
        /* Output:
           Elements:
           Apple
           Grapes
         */
    }
}
```

- LinkedList

```java
import java.util.LinkedList;

public class Main {
    public static void main(String[] args) {
        // Create a new LinkedList
        LinkedList<String> linkedList = new LinkedList<>();

        // Add elements to the LinkedList
        linkedList.add("Apple");
        linkedList.add("Banana");
        linkedList.add("Orange");

        // Print the LinkedList
        System.out.println("LinkedList: " + linkedList); // Output: LinkedList: [Apple, Banana, Orange]

        // Access elements by index
        String firstElement = linkedList.get(0);
        System.out.println("First Element: " + firstElement); // Output: First Element: Apple

        // Update an element in the LinkedList
        linkedList.set(2, "Grapes");
        System.out.println("Updated LinkedList: " + linkedList); // Output: Updated LinkedList: [Apple, Banana, Grapes]

        // Remove an element from the LinkedList
        boolean removed = linkedList.remove("Banana");
        System.out.println("Removed Banana? " + removed); // Output: Removed Banana? true

        // Check if an element exists in the LinkedList
        boolean containsGrapes = linkedList.contains("Grapes");
        System.out.println("Contains Grapes? " + containsGrapes); // Output: Contains Grapes? true

        // Get the size of the LinkedList
        int size = linkedList.size();
        System.out.println("Size: " + size); // Output: Size: 2

        // Iterate over the elements in the LinkedList
        System.out.println("Elements:");
        for (String element : linkedList) {
            System.out.println(element);
        }
        /* Output:
           Elements:
           Apple
           Grapes
         */
    }
}
```

- HashSet

```java
import java.util.HashSet;

public class Main {
    public static void main(String[] args) {
        // Create a new HashSet
        HashSet<String> set = new HashSet<>();

        // Add elements to the HashSet
        set.add("Apple");
        set.add("Banana");
        set.add("Orange");
        set.add("Apple"); // Adding duplicate element

        // Print the HashSet
        System.out.println("HashSet: " + set); // Output: HashSet: [Orange, Apple, Banana]

        // Check if an element exists in the HashSet
        boolean containsBanana = set.contains("Banana");
        System.out.println("Contains Banana? " + containsBanana); // Output: Contains Banana? true

        // Remove an element from the HashSet
        boolean removed = set.remove("Apple");
        System.out.println("Removed Apple? " + removed); // Output: Removed Apple? true

        // Get the size of the HashSet
        int size = set.size();
        System.out.println("Size: " + size); // Output: Size: 2

        // Iterate over the elements in the HashSet
        System.out.println("Elements:");
        for (String element : set) {
            System.out.println(element);
        }
        /* Output:
           Elements:
           Orange
           Banana
         */
    }
}
```

- TreeSet

```java
import java.util.TreeSet;

public class Main {
    public static void main(String[] args) {
        // Create a new TreeSet
        TreeSet<String> set = new TreeSet<>();

        // Add elements to the TreeSet
        set.add("Apple");
        set.add("Banana");
        set.add("Orange");
        set.add("Apple"); // Adding duplicate element

        // Print the TreeSet
        System.out.println("TreeSet: " + set); // Output: TreeSet: [Apple, Banana, Orange]

        // Check if an element exists in the TreeSet
        boolean containsBanana = set.contains("Banana");
        System.out.println("Contains Banana? " + containsBanana); // Output: Contains Banana? true

        // Remove an element from the TreeSet
        boolean removed = set.remove("Apple");
        System.out.println("Removed Apple? " + removed); // Output: Removed Apple? true

        // Get the size of the TreeSet
        int size = set.size();
        System.out.println("Size: " + size); // Output: Size: 2

        // Iterate over the elements in the TreeSet
        System.out.println("Elements:");
        for (String element : set) {
            System.out.println(element);
        }
        /* Output:
           Elements:
           Banana
           Orange
         */
    }
}
```

- LinkedHashSet

```java
import java.util.LinkedHashSet;

public class Main {
    public static void main(String[] args) {
        // Create a new LinkedHashSet
        LinkedHashSet<String> set = new LinkedHashSet<>();

        // Add elements to the LinkedHashSet
        set.add("Apple");
        set.add("Banana");
        set.add("Orange");
        set.add("Apple"); // Adding duplicate element

        // Print the LinkedHashSet
        System.out.println("LinkedHashSet: " + set); // Output: LinkedHashSet: [Apple, Banana, Orange]

        // Check if an element exists in the LinkedHashSet
        boolean containsBanana = set.contains("Banana");
        System.out.println("Contains Banana? " + containsBanana); // Output: Contains Banana? true

        // Remove an element from the LinkedHashSet
        boolean removed = set.remove("Apple");
        System.out.println("Removed Apple? " + removed); // Output: Removed Apple? true

        // Get the size of the LinkedHashSet
        int size = set.size();
        System.out.println("Size: " + size); // Output: Size: 2

        // Iterate over the elements in the LinkedHashSet
        System.out.println("Elements:");
        for (String element : set) {
            System.out.println(element);
        }
        /* Output:
           Elements:
           Banana
           Orange
         */
    }
}
```

----

## **Explain the lists that are present in Java Collection?**

Types of Lists are:

1. Vector

Similar as ArrayList. Maintain the Insertion Order. It can have duplicate values. Its Methods are Synchronized.

```java
import java.util.Vector;

public class Main {
    public static void main(String[] args) {
        // Create a new Vector
        Vector<String> vector = new Vector<>();

        // Add elements to the Vector
        vector.add("Apple");
        vector.add("Banana");
        vector.add("Orange");

        // Print the Vector
        System.out.println("Vector: " + vector); // Output: Vector: [Apple, Banana, Orange]

        // Access elements by index
        String firstElement = vector.get(0);
        System.out.println("First Element: " + firstElement); // Output: First Element: Apple

        // Update an element in the Vector
        vector.set(2, "Grapes");
        System.out.println("Updated Vector: " + vector); // Output: Updated Vector: [Apple, Banana, Grapes]

        // Remove an element from the Vector
        boolean removed = vector.remove("Banana");
        System.out.println("Removed Banana? " + removed); // Output: Removed Banana? true

        // Check if an element exists in the Vector
        boolean containsGrapes = vector.contains("Grapes");
        System.out.println("Contains Grapes? " + containsGrapes); // Output: Contains Grapes? true

        // Get the size of the Vector
        int size = vector.size();
        System.out.println("Size: " + size); // Output: Size: 2

        // Iterate over the elements in the Vector
        System.out.println("Elements:");
        for (String element : vector) {
            System.out.println(element);
        }
        /* Output:
           Elements:
           Apple
           Grapes
         */
    }
}
```

----

## **Difference between HashMap and HashTable?**

HashMap	HashTable
1. HashMap is non synchronized	1. HashTable is synchronized
2. HashMap allows NULL Key and Value.	2. HashTable does not allows any NULL Key and Value.
3. Performance of HashMap is fast.	3. HashTable is slow.
4. HashMap inherits class AbstractMap.	4. HashTable inherits class Dictionary.
5. We can traverse HashMap using Iterator.	5. We can traverse HashTable using Iterator and Enumerator.

----

## **Difference between HashSet and TreeSet?**

HashSet	TreeSet
1. HashSet is faster and gives better performace.	1. TreeSet is little bit slower than HashSet.
2. HashSet performs operation in constant time	2. TreeSet performs operation in Log(n) time.
3. HashSet does not follow any order	3. TreeSet elements are arranged in ascending order.
4. HashSet does not hold duplicate value.	4. TreeSet also does not hold duplicate value.

----

## **Difference between Collection and Collections in Java?**

__Collection:__

The collection is an interface in Java. It represents a group of individual objects as a single unit. 

After java8, Collection can contain a static method. and abstract and default method.

__Collections:__

The collections is a utility class in Java. It defines several utility methods that are used to operate on collection.

Collections includes only static methods. 

### https://quescol.com/interview-preparation/core-java-interview-questions

### https://www.simplilearn.com/tutorials/java-tutorial/java-interview-questions

## **What are the differences between C++ and Java?**

__Concept__

C++ is not platform-independent; the principle behind C++ programming is “write once, compile anywhere.”
In contrast, because the byte code generated by the Java compiler is platform-independent, it can run on any
machine, Java programs are written once and run everywhere.

__Languages Compatibility__

C++ is a programming language that is based on the C programming language. Most other high-level languages are
compatible with C++. Most of the languages of Java are incompatible. Java is comparable to those of C and C++.

__Interaction with the library__

It can access the native system libraries directly in C++. As a result, it’s better for programming at the system level.
Java’s native libraries do not provide direct call support. You can use Java Native Interface or access the libraries.

__Characteristics__

C++ distinguishes itself by having features that are similar to procedural and object-oriented languages.
The characteristic that sets Java apart is automatic garbage collection. Java doesn’t support destructors
at the moment.

__The semantics of the type__

Primitive and object types in C++ have the same kind of semantics. The primitive and object and classes of Java, on the other hand, are not consistent.

__In the context of Compiler and Interpreter__

Java refers to a compiled and interpreted language. In contrast, C++ is only a compiled language.

In Java, the source code is the compiled output is a platform-independent byte code.
In C++, the source program is compiled into an object code that is further executed to produce an output.

----

## **List the features of the Java Programming language?**

A few of the significant features of Java Programming Language are:

__Easy:__ Java is a language that is considered easy to learn. One fundamental concept of OOP Java has a catch to understand.

__Secured Feature:__ Java has a secured feature that helps develop a virus-free and tamper-free system for the users.

__OOP:__ OOP stands for Object-Oriented Programming language. OOP signifies that, in Java, everything is considered an object.

__Independent Platform:__ Java is not compiled into a platform-specific machine; instead, it is compiled into

__platform-independent bytecode:__ This code is interpreted by the Virtual Machine on which the platform runs.

----

## **What do you get in the Java download file? How do they differ from one another?**

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

## **What is a ClassLoader?**

A classloader in Java is a subsystem of Java Virtual Machine, dedicated to loading class files when a program is executed; ClassLoader is the first to load the executable file.

Java has Bootstrap, Extension, and Application classloaders.

Also Read: What is Bootstrap and How to Embed Bootstrap into Angular?

----

## **What are the Memory Allocations available in Java?**

Java has five significant types of memory allocations.

Class Memory
Heap Memory
Stack Memory
Program Counter-Memory
Native Method Stack Memory

----

## **What are the differences between Heap and Stack Memory in Java?**

Stack memory in data structures is the amount of memory allocated to each individual programme. It is a fixed memory space.

Heap memory, in contrast, is the portion that was not assigned to the Java code but will be available for use by the Java code when it is required, which is generally during the program's runtime.

----

## **Will the program run if we write static public void main?**

Yes, the program will successfully execute if written so. Because, in Java, there is no specific rule
for the order of specifiers

----

## **What is the default value stored in Local Variables?**

Neither the Local Variables nor any primitives and Object references have any default
value stored in them. 

----

## **Explain the expected output of the following code segment?**

```java
// Main class
public class Main {
    public static void main(String[] args) {
        System.out.println(100 + 100 + "Simplilearn");
        System.out.println("E-Learning Company" + 100 + 100);
        // Output:
        // 200Simplilearn
        // E-Learning Company100100
        // FIXME: Why? Missing instantiation of the class.
    }
}
```

----

## **What is an Association?**

An Association can be defined as a relationship that has no ownership over another.
For example, a person can be associated with multiple banks, and a bank can be related
to various people, but no one can own the other.

```java
class School {
    private String name;

    public School(String name) {
        this.name = name;
    }

    public String getName() {
        return name;
    }
}

class Student {
    private String name;
    private School school;

    public Student(String name, School school) {
        this.name = name;
        this.school = school;
    }

    public String getName() {
        return name;
    }

    public School getSchool() {
        return school;
    }
}

public class Main {
    public static void main(String[] args) {
        School school = new School("ABC School");
        Student student = new Student("John Doe", school);

        System.out.println("Student: " + student.getName());
        System.out.println("School: " + student.getSchool().getName());
    }
}
```

----

## **What do you mean by aggregation?**

The term aggregation refers to the relationship between two classes best described as a “whole/part” and “has-a” relationship. This kind is the
most specialized version of an association relationship. It contains the reference to another class and is said to have ownership of that class.

```java
class Address {
    private String street;
    private String city;
    private String state;

    public Address(String street, String city, String state) {
        this.street = street;
        this.city = city;
        this.state = state;
    }

    public String getStreet() {
        return street;
    }

    public String getCity() {
        return city;
    }

    public String getState() {
        return state;
    }
}

class Employee {
    private String name;
    private Address address;

    public Employee(String name, Address address) {
        this.name = name;
        this.address = address;
    }

    public String getName() {
        return name;
    }

    public Address getAddress() {
        return address;
    }
}

public class Main {
    public static void main(String[] args) {
        Address address = new Address("123 Main Street", "Cityville", "State");
        Employee employee = new Employee("John Doe", address);

        System.out.println("Employee: " + employee.getName());
        System.out.println("Address: " + employee.getAddress().getStreet() +
                           ", " + employee.getAddress().getCity() +
                           ", " + employee.getAddress().getState());
    }
}
```

----

## **Define Copy Constructor in Java?**

A Copy Constructor in Java is a constructor that initializes an object through another object of the same class.

```java
class Car {
    private String make;
    private String model;
    private int year;

    // Constructor with parameters
    public Car(String make, String model, int year) {
        this.make = make;
        this.model = model;
        this.year = year;
    }

    // Getter methods

    public String getMake() {
        return make;
    }

    public String getModel() {
        return model;
    }

    public int getYear() {
        return year;
    }
}

public class Main {
    public static void main(String[] args) {
        // Create a new Car object using the constructor
        Car myCar = new Car("Toyota", "Camry", 2021);

        // Access the object's properties using getter methods
        System.out.println("Make: " + myCar.getMake());
        System.out.println("Model: " + myCar.getModel());
        System.out.println("Year: " + myCar.getYear());
    }
}
```

----

## **What is a Marker Interface?**

An empty interface in Java is referred to as a Marker interface. Serializable and Cloneable are
some famous examples of Marker Interface. 

```java
interface Maker {
    void make();
}

class Car implements Maker {
    @Override
    public void make() {
        System.out.println("Making a car");
    }
}

class Phone implements Maker {
    @Override
    public void make() {
        System.out.println("Making a phone");
    }
}

public class Main {
    public static void main(String[] args) {
        Maker carMaker = new Car();
        carMaker.make(); // Output: Making a car

        Maker phoneMaker = new Phone();
        phoneMaker.make(); // Output: Making a phone
    }
}
```

----

## **What is Object Cloning?**

An ability to recreate an object entirely similar to an existing object is known as Object
Cloning in Java. Java provides a clone() method to clone a current object offering the same
functionality as the original object.

```java
class Person implements Cloneable {
    private String name;
    private int age;

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }

    public int getAge() {
        return age;
    }

    @Override
    public Object clone() throws CloneNotSupportedException {
        return super.clone();
    }
}

public class Main {
    public static void main(String[] args) {
        try {
            // Create an instance of Person
            Person person1 = new Person("John", 30);

            // Clone the person object
            Person person2 = (Person) person1.clone();

            // Print the details of both objects
            System.out.println("Original Person: " + person1.getName() + ", " + person1.getAge());
            System.out.println("Cloned Person: " + person2.getName() + ", " + person2.getAge());
        } catch (CloneNotSupportedException e) {
            e.printStackTrace();
        }
    }
}
```

----

## **Can Java be said to be the complete object-oriented programming language?**

No, Java cannot be treated as a complete object-oriented programming language.

----

## **What is an object-oriented paradigm?**

A Paradigm that is based on the concepts of “Objects.” It contains data and code. Data that is
in the form of fields, and regulation, that is in the form of procedures. The exciting feature
of this paradigm is that the object’s procedures can access and often modify the data
fields themselves.

----

## **Define Wrapper Classes in Java?**

In Java, when you declare primitive datatypes, then Wrapper classes are responsible for converting
them into objects(Reference types). 

```java
public class Main {
    public static void main(String[] args) {
        // Boxing: Converting int to Integer
        int primitiveInt = 10;
        Integer wrappedInt = Integer.valueOf(primitiveInt);

        System.out.println("Primitive int: " + primitiveInt);
        System.out.println("Wrapped Integer: " + wrappedInt);

        // Unboxing: Converting Integer to int
        Integer anotherWrappedInt = Integer.valueOf(20);
        int unboxedInt = anotherWrappedInt.intValue();

        System.out.println("Wrapped Integer: " + anotherWrappedInt);
        System.out.println("Unboxed int: " + unboxedInt);

        // Autoboxing: Implicit conversion of int to Integer
        int autoboxedInt = 30;
        Integer autoboxedWrapper = autoboxedInt;

        System.out.println("Autoboxed Integer: " + autoboxedWrapper);

        // Autounboxing: Implicit conversion of Integer to int
        Integer autounboxedWrapper = Integer.valueOf(40);
        int autounboxedInt = autounboxedWrapper;

        System.out.println("Autounboxed int: " + autounboxedInt);
    }
}
```

----

## **What is a singleton class in Java? And How to implement a singleton class?**

A class that can possess only one object at a time is called a singleton class. To implement a singleton
class given steps are to be followed:

* Make sure that the class has only one object
* Give global access to that object

```java
public class Singleton {
    private static Singleton instance;

    // Private constructor to prevent instantiation from outside the class
    private Singleton() {
    }

    // Public static method to get the singleton instance
    public static Singleton getInstance() {
        if (instance == null) {
            instance = new Singleton();
        }
        return instance;
    }

    // Other methods of the singleton class
    public void doSomething() {
        System.out.println("Singleton instance is doing something.");
    }
}

public class Main {
    public static void main(String[] args) {
        // Get the singleton instance
        Singleton singleton = Singleton.getInstance();

        // Call methods on the singleton instance
        singleton.doSomething();
    }
}
```

----

## **Define package in Java?**

The package is a collective bundle of classes and interfaces and the necessary libraries and JAR files.
The use of packages helps in code reusability.

---

## **Can you implement pointers in a Java Program?**

Java Virtual Machine takes care of memory management implicitly. Java's primary motto was to keep
programming simple. So, accessing memory directly through pointers is not a recommended action.
Hence, pointers are eliminated in Java. 

----

## **Differentiate between instance and local variables?**

For instance, variables are declared inside a class, and the scope of variables in javascript is
limited to only a specific object.

```java
public class Circle {
    private double radius; // Instance variable

    public Circle(double radius) {
        this.radius = radius;
    }

    public double calculateArea() {
        return Math.PI * radius * radius;
    }

    public static void main(String[] args) {
        Circle circle1 = new Circle(3.5); // Creating an instance of Circle
        double area1 = circle1.calculateArea();
        System.out.println("Area of circle1: " + area1);

        Circle circle2 = new Circle(5.2); // Creating another instance of Circle
        double area2 = circle2.calculateArea();
        System.out.println("Area of circle2: " + area2);
    }
}
```

A local variable can be anywhere inside a method or a specific block of code. Also, the scope
is limited to the code segment where the variable is declared. 

```java
public class Rectangle {
    public void calculateArea(double length, double width) {
        double area = length * width; // Local variable
        System.out.println("Area of the rectangle: " + area);
    }

    public static void main(String[] args) {
        Rectangle rectangle = new Rectangle();
        rectangle.calculateArea(4.5, 3.2);
    }
}
```

----

## **Explain Java String Pool**

A collection of strings in Java's Heap memory is referred to as Java String Pool. In case you try
to create a new string object, JVM first checks for the presence of the object in the pool. If
available, the same object reference is shared with the variable, else a new object is created.

----

## **What is an Exception?**

An Exception handling in Java is considered an unexpected event that can disrupt the program's
normal flow. These events can be fixed through the process of Exception Handling.

```java
import java.util.Scanner;

public class DivideByZeroExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter a dividend: ");
        int dividend = scanner.nextInt();

        System.out.print("Enter a divisor: ");
        int divisor = scanner.nextInt();

        try {
            int quotient = divide(dividend, divisor);
            System.out.println("Quotient: " + quotient);
        } catch (ArithmeticException e) {
            System.out.println("Error: " + e.getMessage());
        }

        scanner.close();
    }

    public static int divide(int dividend, int divisor) {
        if (divisor == 0) {
            throw new ArithmeticException("Cannot divide by zero.");
        }

        return dividend / divisor;
    }
}
```

----

## **What is the final keyword in Java?**

The term final is a predefined word in Java that is used while declaring values to variables.
When a value is declared using the final keyword, then the variable's value remains constant
throughout the program's execution.

```java
public class Example {
    public static void main(String[] args) {
        final int constantValue = 10; // Declaring a final variable
        // constantValue = 20; // Error: Cannot modify final variable
        System.out.println("Constant value: " + constantValue);
    }
}
```

----

## **What happens when the main() isn't declared as static?**

When the main method is not declared as static, then the program may be compiled correctly but ends
up with a severe ambiguity and throws a run time error that reads "NoSuchMethodError."

```java
// Main class
public class Main {
    public void main(String[] args) {
        System.out.println("Not a static method");
    }
}
```

----

## **Why is Java a platform independent language?**

One of the most well-known and widely used programming languages is Java. It is a programming
language that is independent of platforms. Java doesn't demand that the complete programme be
rewritten for every possible platform. The Java Virtual Machine and Java Bytecode are used to
support platform independence. Any JVM operating system can run this platform-neutral byte code.
The application is run after JVM translates the byte code into machine code. Because Java
programmes can operate on numerous systems without having to be individually rewritten for
each platform, the language is referred to as "Write Once, Run Anywhere" (WORA).

----

## **Why is the main method static in Java?**

Java's main() function is static by default, allowing the compiler to call it either before or after creating a class object.
The main () function is where the compiler begins programme execution in every Java programme. Thus, the main () method needs to
be called by the compiler. If the main () method is permitted to be non-static, the JVM must instantiate its class when calling the function. 

----

## **What part of memory - Stack or Heap - is cleaned in the garbage collection process?**

On Heap memory, garbage collection is employed to release the memory used by objects with no references. Every object created in the Heap
space has access to the entire application and may be referred to from anywhere.

----

## **What is the difference between the program and the process?**

A programme is a non-active entity that includes the collection of codes necessary to carry out a specific operation. When a programme is run,
an active instance of the programme called a process is launched. A process is begun by a programme once it has been run. The process carries
out the program's specified instructions.

----

## **What are the differences between constructor and method of a class in Java?**

Initializing the state of the object is done by constructors. A function Object () { [native code] }, like methods, contains a group of statements (or instructions) that are carried out when an object is created. A method is a group of statements that work together to complete a certain task and return the outcome to the caller. A method has the option of working without returning anything.

----

## **Which among String or String Buffer should be preferred when there are a lot of updates required to be done in the data?**

Because StringBuilder is quicker than StringBuffer, it is advised to utilize it wherever possible. However, StringBuffer objects are the best choice if thread safety is required.

----

## **What happens if the static modifier is not included in the main method signature in Java?**

The main function is called by the JVM even before the objects are created, thus even if the code correctly compiles, there will still be an error at runtime.

----

## **Can we make the main() thread a daemon thread?**

This technique designates whether the active thread is a user thread or a daemon thread. For instance, tU.setDaemon(true) would convert a user thread named tU into a daemon thread. On the other side, executing tD.setDaemon(false) would convert a Daemon thread, tD, into a user thread.

----

## **What happens if there are multiple main methods inside one class in Java?**

There is no limit to the number of major approaches you can use. Overloading is the ability to have main methods with
different signatures than main (String []), and the JVM will disregard those main methods.

----

## **How does an exception propagate in the code?**

In the event that an exception is not caught, it is initially thrown from the top of the stack and then moves down the call stack to the preceding method.
The runtime system looks for a way to handle an exception that a method throws. The ordered list of methods that were called to get to the method where the
error occurred is the collection of potential "somethings" that can be used to manage the exception. The call stack is the list of methods, and exception
propagation is the search technique.

----

## **How do exceptions affect the program if it doesn't handle them?**

If you don't deal with an exception once it occurs, the programme will end abruptly and the code after the line where the exception occurred won't run.

----

## **Is it mandatory for a catch block to be followed after a try block?**

Each attempt block does not necessarily have to be followed by a catch block. Either a catch block or a final block ought to come after it. Additionally,
any exceptions that are expected to be thrown should be mentioned in the method's throws clause.

----

## **Can you call a constructor of a class inside another constructor?**

Yes, a class may include any number of constructors, and each function Object () {[native code] } may call the others using
the this() function Object() { [native code] } call function [please do not mix the this() function Object() { [native code] }
call function with this keyword]. The constructor's first line should be either this () or this(args). Overloading of
constructors is what this is called.

----

## **Contiguous memory locations are usually used for storing actual values in an array but not in ArrayList. Explain?**

Primitive data types like int, float, and others are typically present in an array. In such circumstances, the array immediately saves these elements at contiguous memory regions.

While an ArrayList does not contain primitive data types. Instead of the actual object, an ArrayList includes the references to the objects' many locations in memory.
The objects are not kept in consecutive memory regions because of this.

----

## **Why does the java array index start with 0?**

The distance from the array's beginning is just an offset. There is no distance because the first element is at the beginning of the array. Consequently, the offset is 0.

----

## **Why is the remove method faster in the linked list than in an array?**

Because there is no background scaling of an array, insertion, addition, and removal operations are quicker with a LinkedList.
Only references in adjacent items need to update when a new item is added in the middle of the list.

----

## **How many overloaded add() and addAll() methods are available in the List interface? Describe the need and uses?**

List is an interface in the Java Collections Framework. The add() and addAll() methods are the main methods at the List interface.

The add() method is used to add an element to the list, while the addAll() method is used to add a collection of elements to the list.

The List interface contains two overloaded versions of the add() method:

The first add() method accepts a single argument of type E, the element to be added to the list.

The second add() method accepts a variable number of arguments of type E, which are the elements to be added to the list.

The List interface also contains two overloaded versions of the addAll() method:

The first addAll() method accepts a single argument of type Collection (pointed bracket)? Extends E(pointed bracket), which is the collection of elements to be added to the list.

The second addAll() method accepts a variable number of arguments of type E, which are the elements to be added to the list.

----

## **How does the size of ArrayList grow dynamically? And also state how it is implemented internally?**

A resizable array implementation in Java is called ArrayList. Dynamically expanding array lists make it
possible to add new elements at any time. The underlying data structure of the ArrayList is an array of
the Object class. The ArrayList class in Java has three constructors. There are available readObject
and writeObject methods specific to it. The Object Array in an ArrayList is temporary. There are
implemented and Serialization-capable versions of RandomAccess, Cloneable, and java.io (that are Marker Interface in Java).

----

## **Although inheritance is a popular OOPs concept, it is less advantageous than composition? Explain?**

A class's testability is improved through composition over inheritance. If a class is comprised of another class,
it is simple to create a mock object to simulate the combined class for testing purposes. This privilege is not
given by inheritance. Even while Composition and Inheritance both let you reuse code, Inheritance has the
drawback of breaking encapsulation. If the function of the subclass depends on the superclass's action,
it suddenly becomes vulnerable. Sub-class functionality may be broken without any alteration on the part
of the super-class when its behaviour changes.

```java
public class Engine {
    public void start() {
        System.out.println("Engine started");
    }

    public void stop() {
        System.out.println("Engine stopped");
    }
}

public class Car {
    private Engine engine; // Composition: Car has an Engine

    public Car() {
        engine = new Engine(); // Create an instance of Engine
    }

    public void startCar() {
        engine.start(); // Delegate the start operation to the Engine
    }

    public void stopCar() {
        engine.stop(); // Delegate the stop operation to the Engine
    }
}

public class Main {
    public static void main(String[] args) {
        Car car = new Car();
        car.startCar(); // Start the car
        car.stopCar(); // Stop the car
    }
}
```

----

## **What are Composition and Aggregation? State the difference?**

Aggregation (HAS-A) and composition are its two forms (Belongs-to). In contrast to composition, which has a significant correlation, the aggregation has a very modest association.
Aggregation can be thought of as a more confined version of the composition.

Since all compositions are aggregates but not all aggregates are compositions, aggregate can be thought of as the superset of composition.

----

## **How is the creation of a String using new() different from that of a literal?**

The new () operator always produces a new object in heap memory when creating a String object. The String pool may return an existing object
if we build an object using the String literal syntax, such as "Baeldung," on the other hand.

----

## **How is the ‘new' operator different from the 'newInstance()' operator in java?**

Both the new operator and the newInstance() method are used to create objects in Java. If we already know the kind of object to create,
we can use the new operator; however, if the type of object to create is supplied to us at runtime, we must use the newInstance() function.

----

## **Is exceeding the memory limit possible in a program despite having a garbage collector?**

Yes, even with a garbage collector in place, the programme could still run out of memory. Garbage collection aids in identifying and removing programme
objects that are no longer needed in order to release the resources they use. When an object in a programme cannot be reached, trash collection is executed
with respect to that object. If there is not enough memory available to create new objects, a garbage collector is used to free up memory for things that have
been removed from the scope. When the amount of memory released is insufficient for the creation of new objects, the program's memory limit is exceeded.

----

## **Why is synchronization necessary? Explain with the help of a relevant example?**

Multiple threads trying to access the same resources in a multi-threaded software may frequently result in unexpected and incorrect outcomes. Therefore, it must be ensured through some form of synchronization that only one thread can access the resource at any given time. Java offers a method for setting up threads and synchronizing their operations with the aid of synchronized blocks. The synchronized keyword in Java is used to identify synchronized blocks. In Java, a synchronized block is one that is tied to an object. Only one thread can be running at a time inside synchronized blocks since they are all synchronized on the same object. Until the thread inside the synchronized block exits the block, all other threads trying to enter the block are blocked. 

```java
public class Counter {
    private int count;

    public synchronized void increment() {
        count++; // Increment the count
    }

    public synchronized void decrement() {
        count--; // Decrement the count
    }

    public synchronized int getCount() {
        return count; // Get the current count
    }
}

public class CounterThread extends Thread {
    private Counter counter;

    public CounterThread(Counter counter) {
        this.counter = counter;
    }

    public void run() {
        for (int i = 0; i < 1000; i++) {
            counter.increment(); // Increment the counter
        }
    }
}

public class Main {
    public static void main(String[] args) throws InterruptedException {
        Counter counter = new Counter();

        CounterThread thread1 = new CounterThread(counter);
        CounterThread thread2 = new CounterThread(counter);

        thread1.start();
        thread2.start();

        thread1.join();
        thread2.join();

        System.out.println("Count: " + counter.getCount());
    }
}
```

----

## **Define System.out.println()?**

System.out.println() in Java outputs the argument that was supplied to it. On the monitor, the println() method displays the findings. An objectname is typically used to call a method.

----

## **Can you explain the Java thread lifecycle?**

A thread can be in any of the following states in Java.

These are the states:

New: A new thread is always in the new state when it is first formed. The function hasn't been run yet, thus it hasn't started to execute for a thread in the new state.

Active: A thread switches from the new state to the active state when it calls the start() method. The runnable state and the running state are both contained within the active state.

Blocked or Waiting: A thread is either in the blocked state or the waiting state when it is inactive for a while (but not indefinitely).

Timed waiting: When we use the sleep () method on a particular thread, we are actually engaging in timed waiting. The thread enters the timed wait state using the sleep () function. The thread awakens when the allotted time has passed and resumes execution where it left off.

Termination: A thread that has been terminated means it is no longer active in the system. In other words, the thread is inactive and cannot be revived (made active again after being killed).

```java
public class ThreadLifecycleExample {
    public static void main(String[] args) {
        Thread thread = new Thread(new MyRunnable());

        // New state: The thread is created but not started yet
        System.out.println("Thread state: " + thread.getState());

        thread.start();

        // Runnable state: The thread is ready to run but may not be executing at this moment
        System.out.println("Thread state: " + thread.getState());

        try {
            Thread.sleep(1000); // Sleep for 1 second
        } catch (InterruptedException e) {
            e.printStackTrace();
        }

        // Blocked state: The thread is blocked/waiting for a resource or lock
        System.out.println("Thread state: " + thread.getState());

        try {
            Thread.sleep(2000); // Sleep for 2 seconds
        } catch (InterruptedException e) {
            e.printStackTrace();
        }

        // Waiting state: The thread is waiting for another thread to notify or for a specific condition
        System.out.println("Thread state: " + thread.getState());

        thread.interrupt(); // Interrupt the thread

        // Timed Waiting state: The thread is waiting for a specified time period
        System.out.println("Thread state: " + thread.getState());

        try {
            thread.join(); // Wait for the thread to terminate
        } catch (InterruptedException e) {
            e.printStackTrace();
        }

        // Terminated state: The thread has completed its execution
        System.out.println("Thread state: " + thread.getState());
    }
}

class MyRunnable implements Runnable {
    public void run() {
        try {
            Thread.sleep(3000); // Sleep for 3 seconds
        } catch (InterruptedException e) {
            // Handle interrupt and exit the thread
            return;
        }
    }
}
```

## **What could be the tradeoff between the usage of an unordered array versus the usage of an ordered array?**

When opposed to an unordered array, which has a time complexity of O, an ordered array's search times have a time complexity of O(log n) (n).

Due to the need to shift the elements with higher values to create room for the new member, an ordered array has a temporal complexity of O(n)
during the insertion process. Instead, an unordered array's insertion operation requires a constant O amount of time (1).

----

## **Is it possible to import the same class or package twice in Java and what happens to it during runtime?**

The same package or class may be imported more than once. Neither the JVM nor the compiler raise an objection. Even if you import the same class several times, the JVM will only internally load it once.

----

## **In case a package has sub packages, will it suffice to import only the main package? e.g. Does importing of com.myMainPackage?* also import com.myMainPackage.mySubPackage?*?**

Sub-packages won't be imported when a package is imported. When you import a package, all of its classes and interfaces—with the exception of those from its sub-packages—are imported.

----

## **Will the final block be executed if the code System.exit(0) is written at the end of the try block?**

The system is established as the last line to be run, after which nothing will happen, therefore both the catch and finally blocks are essentially ignored.

----

## **Explain the term “Double Brace Initialisation” in Java?**

The outer braces of the double-brace initialization construct an anonymous class that is descended from the provided class and gives an initializer block for that class (the inner braces).

----

## **Why is it said that the length() method of String class doesn't return accurate results?**

Since this char[] array is used by the Java String class internally, the length variable cannot be made public.

----

## **What are the possible ways of making objects eligible for garbage collection (GC) in Java?**

If a reference variable for an object is removed from the programme while it is running, the object may be trash collected. They are also
referred to as inaccessible objects occasionally.  The new operator returns a reference to an object after dynamically allocating memory for it.

----

## **In the below Java Program, how many objects are eligible for garbage collection?**

I don't know about the program, but generally, three objects are eligible for garbage collection. 

The first object is created when the program is started and is no longer needed when the program ends. 

The second object is created when the user inputs their name and is no longer required when the program ends. 

The third object is created when the user inputs their address and is no longer needed when the program ends.

----

## **What is the best way to inject dependency? Also, state the reason?**

Constructor injection. A class requesting its dependencies through its function Object() { [native code] } is the most typical instance of dependency
injection. Since the client cannot be constructed without the required dependencies, this guarantees that it is always in a correct state.

----

## **How we can set the spring bean scope. And what supported scopes does it have?**

what is a "bean" - The objects that form the backbone of your application and that are managed by the Spring IoC container are called beans. A bean is an
object that is instantiated, assembled, and otherwise managed by a Spring IoC container. These beans are created with the configuration metadata that you
supply to the container. For example, in the form of XML <bean/> definitions which you have already seen in the previous chapters.

Bean definition contains the information called configuration metadata, which is needed for the container to know the following −
- How to create a bean
- Bean's lifecycle details
- Bean's dependencies

There are four ways to set the scope of a Spring bean: singleton, prototype, request, and session.

__The singleton scope__ creates a single instance of a bean, which is shared by all objects that request it. 

__The prototype scope__ creates a new instance of a bean for each object that requests it.

__The request and session scopes__ are only available in a web-based context. The request scope creates a new bean instance for each HTTP request, and the session scope creates a single instance of a bean shared by all objects in a single HTTP session.

----

## **What are the different categories of Java Design patterns?**

The three categories of Java design patterns are creational, structural, and behavioural design patterns.

----

## **What is a Memory Leak? Discuss some common causes of it?**

A memory leak is the slow degradation of system performance over time brought on by the fragmentation of a computer's RAM as a result of shoddy application
design or programming that fails to release memory chunks when they are no longer required. These memory leaks frequently result from session items in excess,
insertion into Collection objects without deletion, infinite caches, excessive page switching on the operating system, listener methods that are not called,
and bespoke data structures that are poorly written.

----

## **Assume a thread has a lock on it, calling the sleep() method on that thread will release the lock?**

No, the thread might release the locks using notify, notifyAll(), and wait() methods.

----

## **Write a Java Program to print Fibonacci Series using Recursion?**

```java
// Java program to demonstrate working of
// interface

class Main{
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

// Output:
// 0 1 1 2 3 5 8 13 21 34
```

----

## **Write a Java program to check if the two strings are anagrams?**

```java
import java.util.Arrays;

public class Main {
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

// Output:
// Keep and Peek are anagrams
// MotherInLaw and HitlerWoman are anagrams
```

----

## **Write a Java Program to find the factorial of a given number?**

Tests:
4! = 4*3*2*1 = 24  
5! = 5*4*3*2*1 = 120  

```java
import java.util.Scanner;

public class Factorial {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int number = scanner.nextInt();

        long factorial = calculateFactorial(number);
        System.out.println("Factorial of " + number + " is: " + factorial);

        scanner.close();
    }

    public static long calculateFactorial(int number) {
        if (number == 0 || number == 1) {
            return 1; // Base case: factorial of 0 and 1 is 1
        } else {
            return number * calculateFactorial(number - 1); // Recursive call to calculate factorial
        }
    }
}
```

----

## **Given an array of non-duplicating numbers from 1 to n where one number is missing, write an efficient java program to find that missing number?**

Input: arr[] = {1, 2, 4, 6, 3, 7, 8}, N = 8
Explanation: The missing number between 1 to 8 is 5

```java
public class MissingNumber {
    public static void main(String[] args) {
        int[] arr = {1, 2, 4, 6, 3, 7, 8};
        int n = arr.length + 1; // Total number of elements in the sequence (including the missing number)

        int expectedSum = (n * (n + 1)) / 2; // Calculate the sum of numbers from 1 to n
        int actualSum = 0;

        for (int i = 0; i < arr.length; i++) {
            actualSum += arr[i]; // Calculate the sum of the given array
        }

        int missingNumber = expectedSum - actualSum;
        System.out.println("Missing number: " + missingNumber);
    }
}
```

----

## **Write a Java Program to check if any number is a magic number or not. A number is said to be a magic number if after doing the sum of digits in each step and in turn doing the sum of digits of that sum, the ultimate result (when there is only one digit left) is 1?**

```java
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

    public static void main(String args[])
    {
        int n = 1234;
        if (isMagic(n))
            System.out.printf("%s is a Magic Number%n", n);
        else
            System.out.printf("%s is not a Magic Number%n", n);
    }
}

// Output:
// 1234 is a Magic Number
```

----

## **Write a Java program to create and throw custom exceptions?**

```java
// class that uses custom exception InvalidAgeException  
class InvalidAgeException extends Exception
{
    public InvalidAgeException (String str)
    {
        // calling the constructor of parent Exception
        super(str);
    }
}

public class Main
{
    // method to check the age
    static void validate (int age) throws InvalidAgeException{
        if(age < 18){
            // throw an object of user defined exception
            throw new InvalidAgeException("age is not valid to vote");
        } else {
            System.out.println("welcome to vote");
        }
    }

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

// Output:
// 1234 is a Magic Number
```

----

## **Write a Java program to rotate arrays 90 degree clockwise by taking matrices from user input?**

```java
public class Main
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
            System.out.println(a[i]);
            for(int j=2;j>=0;j--)
            {
                //prints the elements of the rotated matrix
                System.out.println(a[j]);
                System.out.print(""+a[j][i]+"\t");
            }
            System.out.println("\n");
        }
    }
}

// Output:
// Original Matrix: 
// 
//  1	 2	 3	
// 
//  4	 5	 6	
// 
//  7	 8	 9	
// 
// Rotate Matrix by 90 Degrees Clockwise: 
// 
// 7	4	1	
// 
// 8	5	2	
// 
// 9	6	3	

```

----

## **Write a java program to check if any number given as input is the sum of 2 prime numbers?**

```c++
// TestApplication.cpp : Program to check whether a number is prime or not.
//

#include <iostream>
#include <string>
#include <stdio.h>
#include <math.h>
#include <stdbool.h>

using namespace std;

// Function to check whether a number
// is prime or not
bool isPrime(int x)
{
    if (x <= 1)
        return false;

    for (int i = 2; i <= sqrt(x); i++)
    {
        if (x % i == 0)
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

int main() {
    int a = 13;
    if (isPossible(a))
        printf("%s", "Yes");
    else
        printf("%s", "No");

    return 0;
}

```

----

## **Write a Java program for solving the Tower of Hanoi Problem?**



```java
class Main
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
        towerOfHanoi(n, 'A', 'C', 'B'); // A, B and C are names of rods
    }
}
```

----

## **Implement Binary Search in Java using recursion?**

```java
// Java Program to Illustrate Recursive Binary Search

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
            System.out.println("Element found at index " + result);
    }
}
```

----

## **Is delete, next, main, exit or null keyword in java?**

No, these keywords do not exist in Java. Delete, Next, Exit are the operations performed in the Java program, Main is the predefined method, and Null is the default String type.

With this we are done with the first section that is Basic Java Interview Question, Now, lets move on to our next section of Intermediate Java Interview Questions.

----

## **What is JDK? Mention the variants of JDK?**

JDK is an abbreviation for Java Development Kit. It is a combined Package of JRE and Developer tools used for designing Java Applications and Applets. Oracle has the following variants.
- JDK Standard Edition
- JDK Enterprise Edition
- JDK Micro Edition

----

## **What is the difference between JDK, JRE, and JVM?**

JVM has a Just in Time (JIT) compiler tool that converts all the Java source code into the low-level compatible machine language. Therefore, it runs faster than the regular application.

JRE has class libraries and other JVM supporting files. But it doesn’t have any tool for java development such as compiler or debugger.

JDK has tools that are required to write Java Programs and uses JRE to execute them. It has a compiler, Java application launcher, and an applet viewer.

----

## **What is a JIT compiler?**

JIT compiler refers to Just in Time compiler. It is the simplest way of executing the computer code that takes in compilation during the execution
of a program rather than before performance. It commonly uses bytecode translation to machine code. It is then executed directly.

----

## **What are Brief Access Specifiers and Types of Access Specifiers?**

Access specifiers are predefined keywords used to help JVM understand the scope of a variable, method, and class. We have four access specifiers.
- Public Access Specifier 
- Private Access Specifier 
- Protected Access Specifier 
- Default Access Specifier

----

## **How many types of constructors are used in Java?**

There are two types of constructors in Java.
- __Parameterized Constructors:__ Parameterized constructor accepts the parameters with which users can initialize the instance variables. Users can initialize the class variables dynamically at the time of instantiating the class.
- __Default constructors:__ This type doesn’t accept any parameters; rather, it instantiates the class variables with their default values. It is used mainly for object creation.

----

## **Can a constructor return a value?**

Yes, a constructor can return a value. It replaces the class's current instance implicitly; you cannot make a constructor return a value explicitly.

----

## **Explain 'this' keyword in Java?**

The term "this" is a particular keyword designated as a reference keyword. The "this" keyword is used to refer to the current class properties like method, instance, variable, and constructors.

----

## **Explain 'super' keyword in Java?**

The term "super" is a particular keyword designated as a reference keyword. The "super" keyword refers to the immediate parent class object.

----

## ***Explain Method Overloading in Java?**

The process of creating multiple method signatures using one method name is called Method Overloading in Java. Two ways to achieve method overloading are:
- Varying the number of arguments.
- Changing the return type of the Method.

----

## **Can we overload a static method?**

No, Java does not support the Overloading of a static method. The process would throw an error reading __"static method cannot be referenced."__

----

## **Define Late Binding?**

Binding is a process of unifying the method call with the method's code segment. Late binding (also known as dynamic binding or runtime polymorphism) happens when the method's code segment is unknown until it is called during the runtime. 

Static Binding:

```java
class Animal {
    public void makeSound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    public void makeSound() {
        System.out.println("Dog barks");
    }
}

class Cat extends Animal {
    public void makeSound() {
        System.out.println("Cat meows");
    }
}

public class LateBindingExample {
    public static void main(String[] args) {
        Animal animal = new Animal();
        animal.makeSound(); // Calls the makeSound() method of Animal

        Animal dog = new Dog();
        dog.makeSound(); // Calls the makeSound() method of Dog

        Animal cat = new Cat();
        cat.makeSound(); // Calls the makeSound() method of Cat
    }
}
```

----

## **Define Dynamic Method Dispatch?**

The Dynamic method dispatch is a process where the method call is executed during the runtime. A reference variable is used to call
the super-class. This process is also known as Run-Time Polymorphism.     

```java
class Animal {
    public void makeSound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    public void makeSound() {
        System.out.println("Dog barks");
    }
}

class Cat extends Animal {
    public void makeSound() {
        System.out.println("Cat meows");
    }
}

public class LateBindingExample {
    public static void main(String[] args) {
        Animal animal = new Animal();
        animal.makeSound(); // Calls the makeSound() method of Animal

        Animal dog = new Dog();
        dog.makeSound(); // Calls the makeSound() method of Dog

        Animal cat = new Cat();
        cat.makeSound(); // Calls the makeSound() method of Cat
    }
}

```

----

## **Why is the delete function faster in the linked list than an array?**

Delete Function is faster in linked lists in Java as the user needs to make a minor update to the pointer value so that the node can point to the next successor in the list

----

## **Give a briefing on the life cycle of a thread?**

The life cycle of a thread includes five stages, as mentioned below.
- New Born State
- Runnable State
- Running State
- Blocked State
- Dead State

----

## **Explain the difference between >> and >>> operators?**

Although they look similar, there is a massive difference between both.

`>>` operator does the job of right shifting the sign bits
`>>>` operator is used in shifting out the zero-filled bits

----

## **Brief the life cycle of an applet?**

The life cycle of an applet involves the following.
- Initialization
- Start
- Stop
- Destroy
- Paint

----

## **Why are generics used in Java Programming?**

Compile-time type safety is provided by using generics. Compile-time type safety allows users to catch unnecessary invalid types at compile time. Generic methods
and classes help programmers specify a single method declaration, a set of related methods, or related types with an available class declaration. 

----

## **Explain the Externalizable interface?**

The Externalizable interface helps with control over the process of serialization. An "externalisable" interface incorporates readExternal and writeExternal methods.

----

## **What is the Daemon Thread?**

The Daemon thread can be defined as a thread with the least priority. This Daemon thread is designed to run in the background during the Garbage Collection in Java.
The setDaemon() method creates a Daemon thread in Java.

```java
public class Main {
    public static void main(String[] args) {
        Thread daemonThread = new Thread(new MyDaemonRunnable());
        daemonThread.setDaemon(true); // Set the thread as a daemon thread
        daemonThread.start();

        System.out.println("Main thread exiting...");
    }
}

class MyDaemonRunnable implements Runnable {
    public void run() {
        while (true) {
            System.out.println("Daemon thread running...");
            try {
                Thread.sleep(1000); // Sleep for 1 second
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
    }
}
```

----

## **Explain the term enumeration in Java?**

`Enumeration` or `enum` is an interface in Java. Enum allows the sequential access of the elements stored in a collection in Java.

```java
public class EnumerationExample {
    public static void main(String[] args) {
        DayOfWeek day = DayOfWeek.MONDAY;

        System.out.println("Today is " + day);

        if (day == DayOfWeek.SATURDAY || day == DayOfWeek.SUNDAY) {
            System.out.println("It's a weekend!");
        } else {
            System.out.println("It's a weekday.");
        }
    }
}

enum DayOfWeek {
    MONDAY,
    TUESDAY,
    WEDNESDAY,
    THURSDAY,
    FRIDAY,
    SATURDAY,
    SUNDAY
}
```

----

## **Why is Java is Dynamic?**

Java is designed to adapt to an evolving environment. Java programs include a large amount of runtime information that is used to resolve access to objects in real-time. 

----

## **Can you run a code before executing the main method?**

Yes, we can execute any code, even before the main method. We will be using a static block of code when creating the objects at the class's
load time. Any statements within this static block of code will get executed at once while loading the class, even before creating objects in the main method.

----

## **How many times is the finalize method called?**

The finalize method is called the Garbage collector. For every object, the Garbage Collector calls the finalize() method just for one time.


----

## **Can "this" and "super" keywords be used together?**

No, "this" and "super" keywords should be used in the first statement in the class constructor. The following code gives you a brief idea.

```java
public class Main {
    void baseClass() {
        // this(); // call to this must be first statement in constructor
        // super(); // call to super must be first statement in constructor
        System.out.println(" baseClass object is created");
    }
    public static void main(String []args){
        Main bclass = new Main();
    }
}
```

----

## **What is a JSP page?**

JSP is an abbreviation for Java Servlet Page. The JSP page consists of two types of text.
- Static Data 
- JSP elements

## **What is JDBC?**

JDBC is an abbreviation for Java Database Connector.

JDBC is an abstraction layer used to establish connectivity between an existing database and a Java application

----

## **Explain the various directives in JSP?**

Directives are instructions processed by JSP Engine. After the JSP page is compiled into a Servlet, Directives set page-level instructions, insert external files, and define customized tag libraries. Directives are defined using the symbols below:

start with `< %@` and then end with `% >`. 

The various types of directives are shown below:

__Include directive__
It includes a file and combines the content of the whole file with the currently active pages.

__Page directive__
Page Directive defines specific attributes in the JSP page, like the buffer and error page.

__Taglib__
Taglib declares a custom tag library, which is used on the page.

----

## **What are the observer and observable classes?**

Objects that inherit the "Observable class" take care of a list of "observers." 

When an Observable object gets upgraded, it calls the update() method of each of its observers. 

After that, it notifies all the observers that there is a change of state. 

The Observer interface gets implemented by objects that observe Observable objects.

```java
import java.util.Observable;
import java.util.Observer;

public class ObserverPatternExample {
    public static void main(String[] args) {
        // Create an observable object
        MyObservable observable = new MyObservable();

        // Create observer objects
        MyObserver observer1 = new MyObserver("Observer 1");
        MyObserver observer2 = new MyObserver("Observer 2");

        // Register the observers
        observable.addObserver(observer1);
        observable.addObserver(observer2);

        // Perform an update on the observable
        observable.performUpdate("Hello, observers!");

        // Remove observer1
        observable.deleteObserver(observer1);

        // Perform another update on the observable
        observable.performUpdate("Goodbye, observer1!");

        // Unregister all observers
        observable.deleteObservers();
    }
}

// Custom Observable class
class MyObservable extends Observable {
    public void performUpdate(Object data) {
        setChanged();
        notifyObservers(data);
    }
}

// Custom Observer class
class MyObserver implements Observer {
    private String name;

    public MyObserver(String name) {
        this.name = name;
    }

    public void update(Observable observable, Object data) {
        System.out.println(name + " received an update: " + data);
    }
}

// Output:
// Observer 1 received an update: Hello, observers!
// Observer 2 received an update: Hello, observers!
// Observer 2 received an update: Goodbye, observer1!
```

----

## **What is Session Management in Java?**

A session is essentially defined as the random conversation's dynamic state between the client and the server. The virtual communication channel
includes a string of responses and requests from both sides. The popular way of implementing session management is establishing a session ID in
the client's communicative discourse and the server.

----

## **Briefly explain the term Spring Framework?**

Spring is essentially defined as an application framework in Java and inversion of control containers for Java. The spring framework creates enterprise
applications in Java. Especially useful to keep in mind that the spring framework's central features are essentially conducive to any Java application.

----

## **How to handle exceptions in Spring MVC Framework?**

Spring MVC has two approaches for handling the exceptions:
- Exception handler method: In this kind of exception handling, the user will get the @ExceptionHandler annotation type used to annotate a method to handle exceptions.
- XML Configuration: The user can use the SimpleMappingExceptionResolver bean in Spring’s application file and map the exception.

----

## **What is JCA in Java?**

Java Cryptography Architecture gives a platform and provides architecture and application programming interfaces that enable decryption and encryption. 
Developers use Java Cryptography Architecture to combine the application with the security applications. Java Cryptography Architecture helps in implementing third party security rules and regulations. 
Java Cryptography Architecture uses the hash table, encryption message digest, etc. to implement the security.

----

## **Explain JPA in Java?**

The Java Persistence API enables us to create the persistence layer for desktop and web applications. Java Persistence deals in the following:
- Java Persistence API
- Query Language
- Java Persistence Criteria API
- Object Mapping Metadata

----

## **Explain the different authentications in Java Servlets?**

*Authentication options are available in Servlets:*
There are four different options for authentication in servlet:

*Basic Authentication:* 
Usernames and passwords are given by the client to authenticate the user.

*Form-based authentication:* 
In this, the login form is made by the programmer by using HTML.

*Digest Authentication:* 
It is similar to basic authentication, but the passwords are encrypted using the Hash formula. Hash Formula makes digest more secure.

*Client certificate Authentication:*
It requires that each client accessing the resource has a certificate that it sends to authenticate itself. Client Authentication requires the SSL protocol.

----

## **Explain FailFast iterator and FailSafe iterator along with examples for each?**

FailFast iterators and FailSafe iterators are used in Java Collections. 

FailFast iterators do not allow changes or modifications to the Java Collections, which means they fail when the latest element is added to the collection or an existing element gets removed from the collection.
The FailFast iterators tend to fail and throw an exception called ConcurrentModificationException.

Ex: ArrayList, HashMap

Whereas, on the other hand, FailSafe iterators allow changes or modifications to be done on the Java Collections. It is possible, as the FailSafe iterators usually operate on the cloned copy of the collection. Hence, they do not throw any specific exception.

Ex: CopyOnWriteArrayList

----

## **How do we reverse a string?**

The string can be reversed by using the following program.

```java
public class Main {

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

// Expected Output:
// Actual Word: Simplilearn, Word after reversing nraelilpmiS
```

----

## **Write a program to find the square root of a number?**

The Square root of a number can be found by using the following program.

```java
import java.util.Scanner;

public class Main {
    public static void main(String args[]) {
        try (Scanner sc = new Scanner(System.in)) {
            System.out.println("Input a number to find square root: ");
            double square = sc.nextDouble();
            double squareRoot = Math.sqrt(square);
            System.out.printf("The square root is: %f ", squareRoot);
        }
    }
}

// Expected Output:
// Input a number to find square root: 
// 4
// The square root is: 2,000000 
```

----

## **Write a program that detects the duplicate characters in a string?**

The program that finds the duplicate elements in a string is written below:

```java
import java.util.HashMap;
import java.util.Map;
import java.util.Set;

public class Main {
    public static void main(String args[]) {
        printDuplicateCharacters("Java is so cool!");
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

// Output:
// List of duplicate characters in String 'Simplilearn.' 
// : 3 
// : 2 
// : 2 
// : 3
```

----

## **Write a Program to remove duplicates in an ArrayList?**

The following program can be implemented to remove duplicate elements in an ArrayList

```java
import java.util.ArrayList;
import java.util.LinkedHashSet;
import java.util.List;
import java.util.Set;

public class Main {

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

// Output:
// Your list of elements in ArrayList : [1, 2, 3, 4, 5, 6, 3, 4, 5, 6]
// list of original numbers without duplication: [1, 2, 3, 4, 5, 6]
```

----

## **Find the word count in a string using HashMap Collection?**

The following program can be used for word count:

```java
import java.util.HashMap;

public class WordCountExample {
    public static void main(String[] args) {
        String text = "The quick brown fox jumps over the lazy dog";
        
        HashMap<String, Integer> wordCountMap = new HashMap<>();
        
        // Split the string into words
        String[] words = text.split(" ");
        
        // Iterate over each word
        for (String word : words) {
            // Remove any non-alphabetic characters from the word
            word = word.replaceAll("[^a-zA-Z]", "").toLowerCase();
            
            // Check if the word exists in the map
            if (wordCountMap.containsKey(word)) {
                // If the word exists, increment its count
                int count = wordCountMap.get(word);
                wordCountMap.put(word, count + 1);
            } else {
                // If the word does not exist, add it to the map with count 1
                wordCountMap.put(word, 1);
            }
        }
        
        // Print the word count
        for (String word : wordCountMap.keySet()) {
            int count = wordCountMap.get(word);
            System.out.println(word + ": " + count);
        }
    }
}

// Expected Output:
// {Hello=1, Simplilearn=1, Welcome=1, to=1, World,=1}
```

----

## **Write a program to find the Second Highest number in an ArrayList?**

The following program can be used to find the second biggest number in an array list.

```java
import java.util.HashMap;

public class Main {

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

// Output:
// {Hello=1, Simplilearn=1, Welcome=1, to=1, World,=1}
```

----

## **What is the difference between System.out, System.err, and System.in?**

System.out and System.err represent the monitor by default and thus can be used to send data or results to the monitor. System.out is used
to display normal messages and results. System.eerr is used to display error messages. System.in represents InputStream object which by
default represents standard input device, i.e., keyboard.

----

## **Could you provide some implementation of a Dictionary having a large number of words?**

The simplest implementation that can be given is that of a List wherein one can place ordered words and perform a Binary search.
The other implementation with a better search performance is HashMap where the key is used as the first character of the word and the value as a LinkedList.

Up another level, there are HashMaps like:

```java
hashmap {
    a (key) -> hashmap (key-aa , value (hashmap(key-aaa,value)
    b (key) -> hashmap (key-ba , value (hashmap(key-baa,value)
    z (key) -> hashmap (key-za , value (hashmap(key-zaa,value)
}
```

Up to n levels where n is the average size of the word in the dictionary.

----

## **What do you understand by an instance variable and a local variable?**

Generally, instance variables are declared in a class but outside methods whereas a local variable is declared within the blocks of code.


```java
// Local Variable
class Main {
    public static void main(String[] args)
    {
        int var = 145;
        System.out.println("Local Variable: " + var);
    }
}


//Instance variable
class Main {
    public int value = 12;
    public static void main(String[] args)
    {
        Main va = new Main();
        System.out.println("My value is: " + va.value);
    }
}
```

----

## **Can the main method be overloaded?**

Yes, the main method can be overloaded as many times as we want. Nevertheless, JVM prefers to call the main method with the help of its predefined calling method. 

Example:


```java
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

    /*
    public static int main(double[] args){
        System.out.println("Overloaded Double array Main Method");
        // Missing return statement here
    }
    */

    public static void main(float args){
        System.out.println("Overloaded float Main Method");
    }
}
```

----

## **Comment on method overloading and overriding by citing relevant examples?**

Method overloading occurs during the compile time, whereas method overriding occurs during the run time. Static
binding is used during overloading, whereas dynamic binding is used during methods overriding.

```java
//Function overloading
class Podium {
    Podium(){};
    // function1
    void addPodium(int a, int b) {
        System.out.println(a + b);
    }

    // function2 is overloaded
    float addPodium(float a, float b, float c) {
        System.out.println(a + b + c);
        float res = a + b + c;
        System.out.println(res);
        return res;
    }
}

//Function overriding
class Parent {
    void show()
    {
        System.out.println("I am Parent");
    }
}

class Child extends Parent {
    // show() function is overwritten below
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
```

----

## **A single try block and multiple catch blocks can co-exist in a Java Program? Explain?**

One or more catch blocks can follow a try block. Each catch block must have a unique exception handler. So, if you want
to perform multiple tasks in response to various exceptions, use the Java multi-catch block.

----

## **Do final, finally and finalize keywords have the same function?**

No, final, finally and finalize keywords have different functionalities.
- Final is used to restrict classes, variables, or methods, the final keyword.
- Finally is used to execute the code written inside the block without handling any exceptions.
- Finalize is used to call the function of the implementation of cleaning the garbage collection of an object. 

----

## **When can you use the "super" keyword?**

Basically, the super keyword is used to refer to the parent class. When there are the same fields in
both parent and child classes, then one can use a super keyword to access data members of the parent class.

```java
class Vehicle {
    int maxSpeed = 120;
}

class Car extends Vehicle {
    int maxSpeed = 180;

    void display()
    {
        // print maxSpeed of base class Vehicle
        System.out.println("Maximum Speed: " + super.maxSpeed);
    }
}

class Main {
    public static void main(String[] args)
    {
        Car small = new Car();
        small.display();
    }
}
```

----

## **What are shallow copy and deep copy in Java?**

In the case of a shallow copy, primitive data types are copied, whereas in the case of a deep copy along with primitive data types the object references are also copied.

```java
import java.util.Arrays;

class Ex {
    private int[] data;
    // makes a shallow copy of values
    public Ex(int[] values) {
        data = values;
    }

    public void showData() {
        System.out.println( Arrays.toString(data) );
    }
}

class Main {
    public static void main(String[] args)
    {
        int[] newData = {1,2,3,4,5};
        Ex small = new Ex(newData);
        small.showData();
    }
}
```

```java
import java.util.Arrays;

// Code explaining deep copy
class Ex {
    private int[] data;

    // altered to make a deep copy of values
    public Ex(int[] values) {
        data = new int[values.length];
        for (int i = 0; i < data.length; i++) {
            data[i] = values[i];
        }
    }

    public void showData() {
        System.out.println(Arrays.toString(data));
    }
}

public class Main {
    public static void main(String[] args)
    {
        int[] newData = {1,2,3,4,5};
        Ex small = new Ex(newData);
        small.showData();
    }
}
```

----

## **Using relevant properties highlight the differences between interfaces and abstract classes?**

An abstract class can have a combination of both abstract and non-abstract methods,
whereas an interface has only abstract methods in it.

----

## **What are the different ways of thread usage?**

There are two ways to define and implement a thread in Java. They are by implementing the runnable interface and extending the thread class.

```java
// Extending the Thread class
class Main extends Thread{
    public void run(){
        System.out.println("Thread runs...");
    }

    public static void main(String args[]){
        Main ib = new Main();
        ib.start();
    }
}
```

```java
// Implementing the Runnable interface
class InterviewBitThreadExample implements Runnable {
    public void run(){
        System.out.println("Thread runs...");
    }

    public static void main(String args[]){
        Thread ib = new Thread(new InterviewBitThreadExample());
        ib.start();
    }
}
```

Implementing a thread using the method of Runnable interface is more preferred and advantageous as Java
does not have support for multiple inheritances of classes.

start() method is used for creating a separate call stack for the thread execution. Once the call stack
is created, JVM calls the run() method for executing the thread in that call stack.

----

## **What is the difference between the ‘throw' and ‘throws' keyword in Java?**

The throw keyword is often used to explicitly throw an exception. It can only throw one exception at a time whereas throws can be used to declare multiple exceptions.

----

## **Identify the output of the below Java program and Justify your answer?**

```java
class Main {
    public static void main(String args[]) {
        Scaler s = new Scaler(5);
    }
}

class IB{
    IB(){
        System.out.println(" Welcome to InterviewBit ");
    }
}

class Scaler extends IB{
    Scaler(){
        System.out.println(" Welcome to Scaler Academy ");
    }

    Scaler(int x){
        // both statements must be first in line
        // super();
        this();
        System.out.println(" Welcome to Scaler Academy 2");
    }
}
```

The above code will throw the compilation error. It is because the super() is used to call the parent class constructor. But there is the condition that super() must be the first statement in the block. Now in this case, if we replace this() with super() then also it will throw the compilation error. Because this() also has to be the first statement in the block. So in conclusion, we can say that we __cannot use this() and super() keywords in the same block__.

----

## **Java works as a “pass by value” or “pass by reference” phenomenon?**

Java works as a __pass by value__ phenomenon, because pass by reference needs the help of pointers. But there are no pointers in Java.

```java
public class PassByValueExample {
    public static void main(String[] args) {
        int number = 10;
        System.out.println("Before method call: " + number);
        
        // Call the method
        modifyNumber(number);
        
        System.out.println("After method call: " + number);
    }
    
    public static void modifyNumber(int value) {
        value = 20; // Modify the local copy of the value
        System.out.println("Inside method: " + value);
    }
}
```

----

## **How to not allow serialization of attributes of a class in Java?**

One approach to not allow serialization of attributes of a class in Java is by using writeObject() and readObject() methods in the subclass and throwing a not Serializable exception.

```java
// To prevent the serialization of specific attributes of a class in Java, you can use the transient keyword. When you declare a variable as transient,
// it indicates that the variable should not be serialized. Here's how you can use it:

import java.io.Serializable;

public class MyClass implements Serializable {
    private transient String sensitiveData;
    private int normalData;
    // Rest of the class code
}

// In this example, the sensitiveData attribute is marked as transient, while the normalData attribute is not. When an object of MyClass is serialized,
// the sensitiveData attribute will be excluded from the serialization process. Only the non-transient attributes will be serialized.

// It's important to note that the transient keyword only affects the serialization process. When an object is deserialized, the transien
// attributes will be initialized with their default values (e.g., null for reference types, 0 for numeric types) unless you explicitly provide custom deserialization logic.

// Keep in mind that the transient keyword should be used with caution and applied only to attributes that are not essential or should not be persisted during serialization?**
```

----

## **What are the default values assigned to variables and instances in Java?**

By default, for a __numerical value__ it is __0__, for the __boolean value__ it is __false__ and for __objects__ it is __NULL__.

----

## **What do you mean by data encapsulation?**

Data encapsulation, also known as data hiding, is a fundamental principle of object-oriented programming (OOP) that involves bundling data and methods (functions) that operate on that data into a single unit called an object. It is a mechanism that allows the internal representation and implementation details of an object to be hidden from other parts of the program.

The concept of data encapsulation provides several benefits:

*Data Protection:* Encapsulation helps protect the integrity of data by hiding the internal representation of an object. The data can only be accessed and modified through the defined public methods (getters and setters) of the object. This prevents direct manipulation or accidental modification of the object's internal state by external code, ensuring data consistency and preventing unauthorized access.

*Modularity:* Encapsulation promotes modularity in software design. By encapsulating data and related methods into objects, the code can be organized into separate units that can be developed, tested, and maintained independently. This allows for better code organization and promotes code reuse.

*Abstraction:* Encapsulation provides an abstraction layer, where the complex internal details of an object are hidden behind a simplified public interface. Users of the object don't need to know how the data is stored or how the methods are implemented. They only need to know how to interact with the object through its public methods.

*Code Flexibility:* Encapsulation allows the internal implementation of an object to be changed without affecting the external code that uses the object. By keeping the internal details hidden, the implementation can be modified or optimized as long as the public interface remains consistent. This provides flexibility in making changes to the codebase without impacting other parts of the program.

In Java, data encapsulation is achieved through the use of access modifiers (e.g., public, private, protected) to control the visibility of fields and methods, and by providing public getter and setter methods (also known as accessor and mutator methods) to access and modify the object's data. By encapsulating data within objects and exposing a controlled interface, Java supports the principles of encapsulation and facilitates secure, modular, and flexible software development.

----

## **Can you tell the difference between equals() method and equality operator (==) in Java?**

Equality operator (==) is used to check the equality condition between two variables. But the equals() method is used to check the equality condition between two objects.

----

## **How is an infinite loop declared in Java?**

An infinite loop can be declared in Java by breaking the logic in the instruction block.  For example,

```java
// In this example, the for loop has no initialization, condition, or increment statement. Without these components, the loop will continue indefinitely without any termination condition.
for (;;) {
    // Code to be executed repeatedly
}
```

```java
// In this example, the condition true is always true, so the loop will continue to execute indefinitely.
while (true) {
    // Code to be executed repeatedly
}
```

----

## **Briefly explain the concept of constructor overloading?**

The concept of constructor overloading refers to having multiple methods in a class with their name being the same as the class name.
The difference lies in the set of parameters passed to the functions.

```java
public class MyClass {
    private int value;

    // Constructor with no parameters
    public MyClass() {
        value = 0;
    }

    // Constructor with one parameter
    public MyClass(int initialValue) {
        value = initialValue;
    }

    // Constructor with two parameters
    public MyClass(int initialValue, boolean isPositive) {
        if (isPositive) {
            value = Math.abs(initialValue);
        } else {
            value = initialValue;
        }
    }
    // Rest of the class code
}
```

----

## **Explain the use of the final keyword in variable, method and class?**

In Java, one can apply the final keyword to a variable, methods, and class. With the help of the final keyword, the variable turns
out to be a constant, the method cannot be inherited and the class cannot be overridden.

----

## **Is it possible that the ‘finally' block will not be executed? If yes then list the case?**

Yes, there is a possibility that the ‘finally’ block cannot get executed. Here are some of the cases where the above situation occurs.

During the time of fatal errors such as memory exhaustion, memory access error, etc.
During the time of using System.exit()

----

## **Difference between static methods, static variables, and static classes in Java?**

A variable, method, or class can be made static by using the static keyword. A static class cannot be instantiated. When both objects
or instances of a class share the same variables, this is referred to as static variables. Static methods are simply methods that
refer to the class in which they are written.

----

## **What is the main objective of garbage collection?**

The main goal of using garbage collection is to free the heap memory by eliminating unnecessary objects.

----

## **Apart from the security aspect, what are the reasons behind making strings immutable in Java?**

Because of security, synchronization, concurrency, caching, and class loading, the String is immutable in Java. The reason for making string final would be to destroy its immutability and help stop others from trying to extend it. String objects are cached in the String pool, making them immutable.

----

## **Which of the below generates a compile-time error? State the reason?**

```java
class Main {
    public static void main(String args[]) {
        int[] n1 = new int[0];
        boolean[] n2 = new boolean[-200]; // Negative ArraySize Exceptions
        // double[] n3 = new double[2241423798]; // Integer number too large
        char[] ch = new char[20];
    }
}
```

We get a compile-time error in line 3. The error we will get in Line 3 is - the integer number too large. It is because the array requires size as an integer.  And Integer takes 4 Bytes in the memory. And the number (2241423798) is beyond the capacity of the integer. The maximum array size we can declare is - (2147483647).

Because the array requires the size in integer, none of the lines (1, 2, and 4) will give a compile-time error. The program will compile fine. But we get the runtime exception in line 2. The exception is - NegativeArraySizeException. 

Here what will happen is - At the time when JVM will allocate the required memory during runtime then it will find that the size is negative. And the array size can’t be negative. So the JVM will throw the exception.

----

## **How would you differentiate between a String, StringBuffer, and a StringBuilder?**

The string class is immutable but the other two are mutable in nature. StringBuffer is synchronous whereas the StringBuilder is asynchronous.
String uses string pool as memory storage whereas the other two use heap memory for storage purposes.

----

## **What is a Comparator in Java?**

A comparator is an interface, which is used to sort the objects. 

----

## **In Java, static as well as private method overriding is possible. Comment on the statement?**

In Java, you could indeed override a private or static method. If you create a similar method in a child class with the same return type and method arguments,
it will hide the super class method; this is known as method hiding. Similarly, you cannot override a private method in a subclass because it is not accessible from that.

----

## **What makes a HashSet different from a TreeSet?**

In a HashSet, the elements are unsorted and work faster than a Tree set.  It is implemented using a hash table.

1. *Ordering:* HashSet does not maintain any particular order of its elements. The order in which elements are stored and retrieved is not guaranteed. It uses the hash code of the elements to determine their storage locations, resulting in efficient element retrieval but without any specific order.
TreeSet, on the other hand, maintains the elements in sorted order. It uses a binary tree data structure (specifically, a self-balancing red-black tree) to store the elements in a sorted manner. This enables efficient element retrieval and also allows for operations like finding the minimum or maximum element or retrieving elements within a specified range.

2. *Sorting:* HashSet does not provide any inherent sorting capability. If you need sorted elements, you would need to manually sort them using other mechanisms.
TreeSet automatically maintains the elements in sorted order according to their natural ordering (if they implement the Comparable interface) or a custom comparator provided during TreeSet creation.

3. *Performance:* HashSet generally offers better performance for basic operations like adding, removing, and checking for the presence of an element (contains) because it relies on the hash code of elements for efficient storage and retrieval.
TreeSet has a slightly slower performance for basic operations compared to HashSet because it needs to maintain the sorted order of elements using a binary tree structure.

4. *Duplicates:* HashSet does not allow duplicate elements. If you try to add a duplicate element, it will not be stored in the set.
TreeSet also does not allow duplicates. It maintains a distinct set of elements based on their natural ordering or the custom comparator.

5. *Navigational Operations:* TreeSet provides additional navigational operations that are not available in HashSet. These operations include finding the first and last elements, finding elements less than or greater than a given element, and finding elements within a specific range.

----

## **Why is the character array preferred over string for storing confidential information?**

Because Strings are immutable, any change will result in the creation of a new String, whereas char[] allows you to set all of the elements to blank or
zero. So storing a password in a character array clearly reduces the security risk of password theft.

----

## **What are the differences between HashMap and HashTable in Java?**

HashMap
HashTable

1. Asynchronous in nature
1. Synchronous in nature

2. Not thread-safe
2. Thread safe

3. It allows one null key and null values
3. It doesn’t allow null keys and values.

----

## **What is the importance of reflection in Java?**

Reflection is a powerful feature in Java that allows a program to examine and modify its own structure, behavior, and data at runtime. It provides the ability to analyze and manipulate classes, interfaces, methods, fields, and constructors dynamically, without having prior knowledge of their specific details at compile-time. Here are some key aspects that highlight the importance of reflection in Java:

Dynamic Loading and Instantiation: Reflection enables dynamic loading and instantiation of classes at runtime. It allows you to load classes, create objects, and invoke methods dynamically based on runtime conditions or configuration. This provides flexibility and extensibility by allowing the program to work with classes and objects that are determined at runtime.

Introspection and Metadata: Reflection allows you to examine the structure and characteristics of classes, interfaces, methods, and fields. You can retrieve information about their names, types, modifiers, annotations, and more. This introspection capability is useful for building generic frameworks, tools, and libraries that need to operate on classes and objects based on their metadata.

Dynamic Method Invocation: Reflection allows you to invoke methods dynamically at runtime, even if you don't know the exact method signature at compile-time. This enables you to build flexible and extensible systems that can adapt to different method variations or configurations.

Access to Private Members: Reflection provides the ability to access and modify private members of classes, such as private fields and methods, that are not accessible through normal programmatic means. While this can be useful in certain scenarios, it should be used judiciously to respect encapsulation and maintain code integrity.

Framework Development: Reflection is extensively used in Java frameworks, such as dependency injection frameworks (e.g., Spring), object-relational mapping (ORM) frameworks (e.g., Hibernate), and testing frameworks (e.g., JUnit). These frameworks utilize reflection to provide powerful features like automatic wiring of dependencies, mapping objects to database tables, and executing test methods dynamically.

Code Generation and Dynamic Adaptation: Reflection enables code generation and dynamic adaptation of classes and objects. It allows you to create new classes, modify existing classes, or generate proxy classes dynamically. This can be useful in scenarios where you need to generate code dynamically or adapt the behavior of existing classes at runtime.

Although reflection is a powerful feature, it should be used judiciously as it can introduce complexity, impact performance, and bypass compile-time safety checks. It is generally recommended to use reflection sparingly and only when there is a legitimate need for runtime introspection, dynamic behavior, or interaction with external components that rely on reflection.

----

## **What are the different types of Thread Priorities in Java? And what is the default priority of a thread assigned by JVM?**

There are different types of thread properties in Java. They are MIN_PRIORITY, MAX_PRIORITY, and NORM_PRIORITY. By default, the thread is assigned NORM_PRIORITY.

----

## **What is the 'IS-A' relationship in OOPs Java?**

'IS-A' relationship is related to the Inheritance property of OOPs Java. It is a kind of parent-child relationship that is established between two classes.

We offer complete Job Guarantee and money-back if you don't secure a job within 6 months of graduation. Get interview ready with intense and comprehensive career mentoring sessions in our Full Stack Java Developer Program. Enroll TODAY!

```java
class Animal {
    // ...
}

class Dog extends Animal {
    // ...
}
```

In this example, Dog is a subclass of Animal. We can say that "Dog IS-A Animal." The Dog class inherits the attributes and behaviors defined in the Animal class, such as Animal's methods and fields. This allows us to treat a Dog object as an Animal object, which means we can use a Dog object wherever an Animal object is expected.

The "IS-A" relationship facilitates code reuse, polymorphism, and abstraction. It allows you to create specialized classes that inherit and extend the functionality of more general classes, promoting code organization, modularity, and flexibility in your Java programs.

### https://www.simplilearn.com/tutorials/java-tutorial/java-interview-questions

### https://www.edureka.co/blog/interview-questions/java-interview-questions

## **Why Java is not 100% Object-oriented?**

Java is not 100% Object-oriented because it makes use of eight primitive data types such as boolean, byte, char, int, float, double, long, short which are not objects.

----

## **What are wrapper classes in Java?**

Wrapper classes convert the Java primitives into the reference types (objects). Every primitive data type has a class dedicated to it. These are known as wrapper
classes because they “wrap” the primitive data type into an object of that class. Refer to the below image which displays different primitive type, wrapper class and constructor argument.

Wrapper classes in Java are classes that provide a way to use primitive data types as objects. In Java, primitive data types (such as int, double, boolean, etc.) are not considered objects and do not have methods or other features available to objects. However, there are situations where it is necessary to treat primitive data types as objects. Wrapper classes bridge this gap by providing a class representation for each primitive type.

Java provides a set of predefined wrapper classes for each primitive type:

Integer for int
Double for double
Boolean for boolean
Character for char
Byte for byte
Short for short
Long for long
Float for float

Wrapper classes offer several useful functionalities:

*Object Representation:* Wrapper classes allow primitive data types to be represented as objects. This enables them to be used in situations where objects are required, such as in collections (e.g., ArrayList) or when passing parameters to methods that expect objects.

*Conversion and Parsing:* Wrapper classes provide methods for converting between primitive types and their corresponding wrapper class objects. For example, Integer class provides methods like parseInt() to parse a string into an int.

*Methods and Utility Functions:* Wrapper classes provide useful methods and utility functions specific to each data type. These include mathematical operations, comparison methods, conversion methods, and more. For example, the Double class provides methods like doubleValue(), compareTo(), isNaN(), etc.

*Autoboxing and Unboxing:* Java also provides automatic conversion between primitive types and their corresponding wrapper classes through a process called autoboxing and unboxing. This allows you to assign primitive values to wrapper class variables and vice versa without explicit conversion.

Wrapper classes are particularly useful in scenarios where you need to treat primitive types as objects, such as when working with collections, Java generics, or when utilizing Java libraries that expect objects rather than primitive types.

----

## **What is the difference between Array list and vector in Java?**

| ArrayList	| Vector |
| ------- | -------- |
| Array List is not synchronized. | Vector is synchronized. |
| Array List is fast as it’s non-synchronized. | Vector is slow as it is thread safe. |
| If an element is inserted into the Array List, it increases its Array size by 50%. | Vector defaults to doubling size of its array. |
| Array List does not define the increment size. | Vector defines the increment size. |
| Array List can only use Iterator for traversing an Array List. | Vector can use both Enumeration and Iterator for traversing. |

----

## **What is the difference between equals() and == in Java?**

Equals() method is defined in Object class in Java and used for checking equality of two objects defined by business logic.

"==" or equality operator in Java is a binary operator provided by Java programming language and used to compare primitives and objects. public boolean
equals(Object o) is the method provided by the Object class. The default implementation uses == operator to compare two objects. For example: method can
be overridden like String class. equals() method is used to compare the values of two objects.

## **When can you use the super keyword?**

In Java, the super keyword is a reference variable that refers to an immediate parent class object.
When you create a subclass instance, you’re also creating an instance of the parent class, which is referenced to by the super reference variable.

The uses of the Java super Keyword are: 
- To refer to an immediate parent class instance variable, use super.
- The keyword super can be used to call the method of an immediate parent class.
- Super() can be used to call the constructor of the immediate parent class.

----

## **What makes a HashSet different from a TreeSet?**

| HashSet | TreeSet |
| -------- | -------- |
| It is implemented through a hash table. | TreeSet implements SortedSet Interface that uses trees for storing data. |
| It permits the null object. | It does not allow the null object. |
| It is faster than TreeSet especially for search, insert, and delete operations. | It is slower than HashSet for these operations. |
| It does not maintain elements in an ordered way. | The elements are maintained in a sorted order. |
| It uses equals() method to compare two objects. | It uses compareTo() method for comparing two objects. |
| It does not permit a heterogenous object. | It permits a heterogenous object. |

----

## **What are the differences between HashMap and HashTable in Java?**

| HashMap | Hashtable |
| --------- | --------- |
| It is non synchronized. | It cannot be shared between many threads without proper synchronization code. | It is synchronized. It is thread-safe and can be shared with many threads. |
| It permits one null key and multiple null values. | It does not permit any null key or value. |
| is a new class introduced in JDK 1.2. | It was present in earlier versions of java as well. |
| It is faster. | It is slower. |
| It is traversed through the iterator. | It is traversed through Enumerator and Iterator. |
| It uses fail fast iterator. | It uses an enumerator which is not fail fast. |
| It inherits AbstractMap class. | It inherits Dictionary class. |
 
----

## **What is the importance of reflection in Java?**

Reflection is a runtime API for inspecting and changing the behavior of methods, classes, and interfaces. Java Reflection is a powerful tool that can be really beneficial. Java Reflection allows you to analyze classes, interfaces, fields, and methods during runtime without knowing what they are called at compile time. Reflection can also be used to create new objects, call methods, and get/set field values. External, user-defined classes can be used by creating instances of extensibility objects with their fully-qualified names. Debuggers can also use reflection to examine private members of classes.

----

## **How to not allow serialization of attributes of a class in Java?**

The Non-Serialized attribute can be used to prevent member variables from being serialized.
You should also make an object that potentially contains security-sensitive data non-serializable if possible. Apply the Non-Serialized attribute to certain fields that store sensitive data if the object must be serialized. If you don’t exclude these fields from serialization, the data they store will be visible to any programs with serialization permission.

----

## **Can you call a constructor of a class inside another constructor?**

Yes, we can call a constructor of a class inside another constructor. This is also called as __constructor chaining__. Constructor chaining can be done in 2 ways-

Within the same class: For constructors in the same class, the this() keyword can be used.
From the base class: The super() keyword is used to call the constructor from the base class.
The constructor chaining follows the process of inheritance. The constructor of the sub class first calls the constructor of the super class. Due to this, the creation of sub class’s object starts with the initialization of the data members of the super class. The constructor chaining works similarly with any number of classes. Every constructor keeps calling the chain till the top of the chain.
 
```java
public class Person {
    private String name;
    private int age;

    public Person() {
        this("Unknown", 0); // Invokes the parameterized constructor with default values
    }

    public Person(String name) {
        this(name, 0); // Invokes the parameterized constructor with name and default age
    }

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    // Getters and setters

    public static void main(String[] args) {
        Person person1 = new Person(); // Invokes the default constructor
        System.out.println(person1.getName()); // Output: Unknown
        System.out.println(person1.getAge()); // Output: 0

        Person person2 = new Person("John"); // Invokes the constructor with name parameter
        System.out.println(person2.getName()); // Output: John
        System.out.println(person2.getAge()); // Output: 0

        Person person3 = new Person("Jane", 25); // Invokes the constructor with name and age parameters
        System.out.println(person3.getName()); // Output: Jane
        System.out.println(person3.getAge()); // Output: 25
    }
}
```

----

## **Contiguous memory locations are usually used for storing actual values in an array but not in ArrayList. Explain?**

An array generally contains elements of the primitive data types such as int, float, etc. In such cases, the array directly stores these elements at contiguous
memory locations. While an ArrayList does not contain primitive data types. An arrayList contains the reference of the objects at different memory locations instead
of the object itself. That is why the objects are not stored at contiguous memory locations.
 
----

## **How is the creation of a String using new() different from that of a literal?**

When we create a string using new(), a new object is created. Whereas, if we create a string using the string literal syntax, it may return an already existing object with the same name.

----

## **Why is synchronization necessary? Explain with the help of a relevant example?**

Java allows multiple threads to execute. They may be accessing the same variable or object. Synchronization helps to execute threads one after another.
It is important as it helps to execute all concurrent threads while being in sync. It prevents memory consistency errors due to access to shared memory. An example of synchronization code is-

```java
class Counter {
    private int count = 0;

    public void increment() {
        count++;
    }

    public int getCount() {
        return count;
    }
}

class IncrementerThread extends Thread {
    private Counter counter;

    public IncrementerThread(Counter counter) {
        this.counter = counter;
    }

    public void run() {
        for (int i = 0; i < 1000; i++) {
            counter.increment();
        }
    }
}

public class Main {
    public static void main(String[] args) throws InterruptedException {
        Counter counter = new Counter();

        IncrementerThread thread1 = new IncrementerThread(counter);
        IncrementerThread thread2 = new IncrementerThread(counter);

        thread1.start();
        thread2.start();

        thread1.join();
        thread2.join();

        System.out.println("Final count: " + counter.getCount());
    }
}
```
In this example, we have a Counter class with an increment() method that increments a shared count variable by 1. We create two IncrementerThread instances that both share the same Counter object. Each thread runs a loop to call the increment() method 1000 times.

Without synchronization, there is a possibility of a race condition. Since both threads access and modify the count variable concurrently, they may interfere with each other's operations and lead to inconsistent results. The final count may vary each time the program is executed.

To ensure proper synchronization and consistent results, we can apply synchronization mechanisms. One way is by using the synchronized keyword:

```java
public synchronized void increment() {
    count++;
}
```

With synchronization, only one thread can execute the increment() method at a time, and other threads will be blocked until the execution completes. This ensures that the count variable is properly updated without any interference, and the final count will always be the expected value of 2000 (1000 increments from each thread).

By applying synchronization in the appropriate sections of code, we can prevent data races, maintain data integrity, and ensure thread safety in multi-threaded environments. It allows for proper coordination and consistency when multiple threads access shared resources or perform critical operations.

----

## **Explain the term "Double Brace Initialization" in Java?**

Double Brace Initialization is a Java term that refers to the combination of two independent processes. There are two braces used in this. The first brace creates an anonymous inner class. The second brace is an initialization block. When these both are used together, it is known as Double Brace Initialization. The inner class has a reference to the enclosing outer class, generally using the ‘this’ pointer. It is used to do both creation and initialization in a single statement. It is generally used to initialize collections. It reduces the code and also makes it more readable.
 
----

## **Why is it said that the length() method of String class doesn’t return accurate results?**

The length() method of String class doesn’t return accurate results because it simply takes into account the number of characters within in the String.
In other words, code points outside of the BMP (Basic Multilingual Plane), that is, code points having a value of U+10000 or above, will be ignored.

The reason for this is historical. One of Java’s original goals was to consider all text as Unicode; yet, Unicode did not define code points outside of the
BMP at the time. It was too late to modify char by the time Unicode specified such code points.

----

## **What are the differences between Heap and Stack Memory in Java?**

The major difference between Heap and Stack memory are:

| Features | Stack | Heap |
| ------- | ------- | ------- |
| Memory | Stack memory is used only by one thread of execution. | Heap memory is used by all the parts of the application. |
| Access | Stack memory can’t be accessed by other threads. | Objects stored in the heap are globally accessible. |
| Memory | Management	Follows LIFO manner to free memory. | Memory management is based on the generation associated with each object. |
| Lifetime | Exists until the end of execution of the thread. | Heap memory lives from the start till the end of application execution. |
| Usage | Stack memory only contains local primitive and reference variables to objects in heap space. | Whenever an object is created, it’s always stored in the Heap space. |

----

## **Why pointers are not used in Java?**

Java doesn’t use pointers because they are unsafe and increases the complexity of the program. Since, Java is known for its simplicity of code, adding
the concept of pointers will be contradicting. Moreover, since JVM is responsible for implicit memory allocation, thus in order to avoid direct access
to memory by the user,  pointers are discouraged in Java.

----

## **Differentiate between the constructors and methods in Java?**

| Methods | Constructors |
| ---------- | ---------- |
| 1. Used to represent the behavior of an object | 1. Used to initialize the state of an object |
| 2. Must have a return type | 2. Do not have any return type |
| 3. Needs to be invoked explicitly | 3. Is invoked implicitly |
| 4. No default method is provided by the compiler | 4. A default constructor is provided by the compiler if the class has none |
| 5. Method name may or may not be same as class name | 5. Constructor name must always be the same as the class name |

----

## **What is a Map in Java?**

In Java, Map is an interface of Util package which maps unique keys to values. The Map interface is not a subset of the main Collection interface and thus it
behaves little different from the other collection types. Below are a few of the characteristics of Map interface: 

Map doesn’t contain duplicate keys.
Each key can map at max one value.

```java
import java.util.HashMap;
import java.util.Map;

public class Main {
    public static void main(String[] args) {
        Map<String, Integer> map = new HashMap<>();

        map.put("apple", 1);
        map.put("banana", 2);
        map.put("cherry", 3);
        map.put("apple", 4); // Trying to insert a duplicate key

        System.out.println(map);
    }
}
```

----

## **Can you override a private or static method in Java?**

You cannot override a private or static method in Java. If you create a similar method with the same return type and same method arguments in child class then
it will hide the superclass method; this is known as method hiding. Similarly, you cannot override a private method in subclass because it’s not accessible
there. What you can do is create another private method with the same name in the child class. Let’s take a look at the example below to understand it better.

```java
class Base {
    private static void display() {
        System.out.println("Static or class method from Base");
    }

    public void print() {
        System.out.println("Non-static or instance method from Base");
    }

    class Main extends Base {
        private static void display() {
            System.out.println("Static or class method from Derived");
        }

        public void print() {
            System.out.println("Non-static or instance method from Derived");
        }

        public class test {
            public void main(String args[]) {
                Base obj = new Main();
                obj.display();
                obj.print();
            }
        }
    }
}
```

----

## **What is multiple inheritance? Is it supported by Java?**

The problem with multiple inheritance is that if multiple parent classes have the same method name, then at runtime it becomes difficult for the compiler to decide which method to execute from the child class.

Therefore, Java doesn’t support multiple inheritance. The problem is commonly referred to as Diamond Problem.

----

## **What is a marker interface?**

n Java, a marker interface is an interface that does not declare any methods. It serves as a special type of interface that acts as a "marker" or a tag to indicate something about the classes that implement it. The presence of the marker interface on a class provides additional information to the compiler or runtime environment.

Marker interfaces in Java are typically used for:

Identifying Special Behaviors: Marker interfaces are often used to identify certain characteristics or behaviors of a class. By implementing a specific marker interface, a class indicates that it possesses a particular capability or feature.

Flagging or Categorizing Classes: Marker interfaces can be used to categorize classes into specific groups or categories. They can act as metadata to mark classes for specific processing or handling based on their classification.

Enabling Runtime Processing: The presence of a marker interface on a class can enable certain runtime processing or behavior. It allows the runtime environment to make decisions or apply special treatment based on the interface implementation.

Some examples of marker interfaces in Java include:

java.io.Serializable: The Serializable interface is a marker interface that indicates that a class can be serialized, allowing objects of that class to be converted into a stream of bytes for storage or transmission.

java.lang.Cloneable: The Cloneable interface is a marker interface that indicates that a class can be cloned, allowing objects of that class to be copied or cloned using the clone() method.

java.util.RandomAccess: The RandomAccess interface is a marker interface that indicates that a List implementation provides efficient random access to its elements, allowing constant-time access to any position.

Marker interfaces are simple and lightweight, providing a way to add extra information or behavior to classes without adding any method requirements. They rely on conventions and the presence of the interface itself to convey meaning or trigger specific behavior.

```java
// Marker interface
interface Printable {
}

// Class implementing the marker interface
class Book implements Printable {
    private String title;
    
    public Book(String title) {
        this.title = title;
    }
    
    public String getTitle() {
        return title;
    }
    
    // Other methods and fields...
}

public class MarkerInterfaceExample {
    public static void main(String[] args) {
        Book book1 = new Book("Java Programming");
        Book book2 = new Book("Design Patterns");
        
        // Check if the objects implement the Printable marker interface
        if (book1 instanceof Printable) {
            System.out.println(book1.getTitle() + " is printable");
        }
        
        if (book2 instanceof Printable) {
            System.out.println(book2.getTitle() + " is printable");
        }
    }
}
```

----

## **What is object cloning in Java?**

Object cloning in Java is the process of creating an exact copy of an object. It basically means the ability to create an object with a similar state as the original object. To achieve this, Java provides a method clone() to make use of this functionality. This method creates a new instance of the class of the current object and then initializes all its fields with the exact same contents of corresponding fields. To object clone(), the marker interface java.lang.Cloneable must be implemented to avoid any runtime exceptions. One thing you must note is Object clone() is a protected method, thus you need to override it.

```java
// Marker interface
interface MyMarkerInterface {
    // No methods declared
}

// Class implementing the marker interface
class MyClass implements MyMarkerInterface {
    // Class implementation
}

public class Main {
    public static void main(String[] args) {
        MyClass myObj = new MyClass();

        // Check if the object implements the marker interface
        if (myObj instanceof MyMarkerInterface) {
            System.out.println("MyClass object implements MyMarkerInterface");
        } else {
            System.out.println("MyClass object does not implement MyMarkerInterface");
        }
    }
}
```

----

## **What is a copy constructor in Java?**

Copy constructor is a member function that is used to initialize an object using another object of the same class. Though there is no need for copy constructor in Java since all objects are passed by reference. Moreover, Java does not even support automatic pass-by-value.

```java
class Person {
    private String name;
    private int age;

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    // Copy constructor
    public Person(Person other) {
        this.name = other.name;
        this.age = other.age;
    }

    public String getName() {
        return name;
    }

    public int getAge() {
        return age;
    }
}

public class Main {
    public static void main(String[] args) {
        Person person1 = new Person("John", 25);

        // Create a new object using the copy constructor
        Person person2 = new Person(person1);

        // Modify the original object
        person1.setName("Alice");
        person1.setAge(30);

        // Display the details of both objects
        System.out.println("Person 1 - Name: " + person1.getName() + ", Age: " + person1.getAge());
        System.out.println("Person 2 - Name: " + person2.getName() + ", Age: " + person2.getAge());
    }
}
```

----

## **What is Request Dispatcher?**

RequestDispatcher interface is used to forward the request to another resource that can be HTML, JSP or another servlet in same application.
We can also use this to include the content of another resource to the response.

There are two methods defined in this interface:
- 1.void forward()
- 1.void include()

In Java, the RequestDispatcher interface is part of the Java Servlet API and provides a way to forward or include HTTP requests and responses between server-side components. It allows servlets or JSP pages to collaborate and share processing tasks.

The RequestDispatcher can be obtained from the ServletRequest object using the getRequestDispatcher() method. It provides two main methods:

forward(ServletRequest request, ServletResponse response): This method forwards the request and response objects from the current servlet to another servlet or JSP page for further processing. The original servlet relinquishes control, and the target servlet or JSP page becomes responsible for generating the response.

include(ServletRequest request, ServletResponse response): This method includes the response of another servlet or JSP page in the current servlet's response. The processing of the current servlet continues after the included response is appended.

The RequestDispatcher allows components in a web application to collaborate and delegate processing tasks to each other. It is commonly used for:

Forwarding requests to other servlets or JSP pages for additional processing or generating the response.
Including the output of other servlets or JSP pages in the current response.
Implementing MVC (Model-View-Controller) architecture by dispatching requests to appropriate components for handling different aspects of the application.
Overall, the RequestDispatcher provides a mechanism for coordinating and sharing processing tasks within a web application, allowing different components to work together to handle HTTP requests and generate responses.

Example:

Suppose we have two servlets, Servlet1 and Servlet2, and we want to forward a request from Servlet1 to Servlet2 for further processing.

```java
// Serverlet1.java
import javax.servlet?*;
import javax.servlet.http?*;
import java.io.IOException;

public class Servlet1 extends HttpServlet {
    protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // Perform some processing
        // ...

        // Obtain the RequestDispatcher for Servlet2
        RequestDispatcher dispatcher = request.getRequestDispatcher("/servlet2");

        // Forward the request and response objects to Servlet2
        dispatcher.forward(request, response);
    }
}

```

```java
// Serverlet2.java
import javax.servlet?*;
import javax.servlet.http?*;
import java.io.IOException;
import java.io.PrintWriter;

public class Servlet2 extends HttpServlet {
    protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // Perform some processing
        // ...

        // Set the response content type
        response.setContentType("text/html");

        // Get the PrintWriter object to write the response
        PrintWriter out = response.getWriter();

        // Write the response content
        out.println("<h1>Servlet2 Response</h1>");
        out.println("<p>This is the response from Servlet2.</p>");

        // Close the PrintWriter
        out.close();
    }
}

```

In this example, when a request is made to Servlet1, it performs some processing and then obtains the RequestDispatcher object for Servlet2 using the getRequestDispatcher() method.

The forward() method of the RequestDispatcher is then called to forward the request and response objects to Servlet2 for further processing. This means that the control is transferred to Servlet2, and it becomes responsible for generating the response.

In Servlet2, we perform some processing and generate the response using the PrintWriter object. The response content includes an HTML heading and a paragraph. Finally, the response is sent back to the client.

Note that the URL pattern "/servlet2" is used as the argument to getRequestDispatcher(), which corresponds to the URL pattern mapped to Servlet2 in the servlet configuration.

By using the RequestDispatcher and the forward() method, we can forward the request and response between servlets or JSP pages in a web application, allowing them to collaborate and share processing tasks.

----

## **What are the differences between forward() method and sendRedirect() methods?**

| forward() method | SendRedirect() method |
| ---------------- | ---------------------- |
| forward() sends the same request to another resource. | sendRedirect() method sends new request always because it uses the URL bar of the browser. |
| forward() method works at server side. | sendRedirect() method works at client side. |
| forward() method works within the server only. | sendRedirect() method works within and outside the server. |

----

## **What is the life-cycle of a servlet?**

There are 5 stages in the lifecycle of a servlet:LifeCycleServlet - Java Interview Questions - Edureka
- Servlet is loaded
- Servlet is instantiated
- Servlet is initialized
- Service the request
- Servlet is destroyed

----

## **How do cookies work in Servlets?**

Cookies are text data sent by server to the client and it gets saved at the client local machine.
Servlet API provides cookies support through javax.servlet.http.Cookie class that implements Serializable and Cloneable interfaces.
HttpServletRequest getCookies() method is provided to get the array of Cookies from request, since there is no point of adding Cookie to request, there are no methods to set or add cookie to request.
Similarly HttpServletResponse addCookie(Cookie c) method is provided to attach cookie in response header, there are no getter methods for cookie.

----

## **What are the differences between ServletContext vs ServletConfig?**

The difference between ServletContext and ServletConfig in Servlets JSP is in below tabular format.

| ServletConfig	| ServletContext |
| -------------	| ------------- |
| Servlet config object represent single servlet | It represent whole web application running on particular JVM and common for all the servlet |
| Its like local parameter associated with particular servlet | Its like global parameter associated with whole application |
| It’s a name value pair defined inside the servlet section of web.xml file so it has servlet wide scope | ServletContext has application wide scope so define outside of servlet tag in web.xml file. |
| getServletConfig() method is used to get the config object| getServletContext() method is  used to get the context object. |
| for example shopping cart of a user is a specific to particular user so here we can use servlet config | To get the MIME type of a file or application session related information is stored using servlet context object.  |

----

## **What are the different methods of session management in servlets?**

Session is a conversational state between client and server and it can consists of multiple request and response between client and server. Since HTTP and Web Server both are stateless, the only way to maintain a session is when some unique information about the session (session id) is passed between server and client in every request and response.

Some of the common ways of session management in servlets are:
- User Authentication
- HTML Hidden Field
- Cookies
- URL Rewriting
- Session Management API

----

## **What is JDBC Driver?**

JDBC Driver is a software component that enables java application to interact with the database. There are 4 types of JDBC drivers:

JDBC-ODBC bridge driver
Native-API driver (partially java driver)
Network Protocol driver (fully java driver)
Thin driver (fully java driver)

----

## **What are the steps to connect to a database in java?**

Registering the driver class
Creating connection
Creating statement
Executing queries
Closing connection

----

## **What are the JDBC API components?**

The java.sql package contains interfaces and classes for JDBC API.

Interfaces:
- Connection
- Statement
- PreparedStatement
- ResultSet
- ResultSetMetaData
- DatabaseMetaData
- CallableStatement etc.
- Classes:
- DriverManager
- Blob
- Clob
- Types
- SQLException etc.

----

## **What is the role of JDBC DriverManager class?**

The DriverManager class manages the registered drivers. It can be used to register and unregister drivers. It provides factory method that returns the instance of Connection.

----

## **What is JDBC Connection interface?**

The Connection interface maintains a session with the database. It can be used for transaction management. It provides factory methods that returns the instance of Statement, PreparedStatement, CallableStatement and DatabaseMetaData.

ConnectionInterface - Java Interview Questions - Edureka
In case you are facing any challenges with these java interview questions, please comment on your problems in the section below.

----

## **What is the purpose of JDBC ResultSet interface?**

The ResultSet object represents a row of a table. It can be used to change the cursor pointer and get the information from the database.

----

## **What is JDBC ResultSetMetaData interface?**

The ResultSetMetaData interface returns the information of table such as total number of columns, column name, column type etc.

----

## **What is JDBC DatabaseMetaData interface?**

The DatabaseMetaData interface returns the information of the database such as username, driver name, driver version, number of tables, number of views etc.

----

## **What do you mean by batch processing in JDBC?**

Batch processing helps you to group related SQL statements into a batch and execute them instead of executing a single query. By using batch processing technique in JDBC, you can execute multiple queries which makes the performance faster.

----

## **What is the difference between execute, executeQuery, executeUpdate?**

Statement execute(String query) is used to execute any SQL query and it returns TRUE if the result is an ResultSet such as running Select queries. The output is FALSE when there is no ResultSet object such as running Insert or Update queries. We can use getResultSet() to get the ResultSet and getUpdateCount() method to retrieve the update count.

Statement executeQuery(String query) is used to execute Select queries and returns the ResultSet. ResultSet returned is never null even if there are no records matching the query. When executing select queries we should use executeQuery method so that if someone tries to execute insert/update statement it will throw java.sql.SQLException with message “executeQuery method can not be used for update”.

Statement executeUpdate(String query) is used to execute Insert/Update/Delete (DML) statements or DDL statements that returns nothing. The output is int and equals to the row count for SQL Data Manipulation Language (DML) statements. For DDL statements, the output is 0.

You should use execute() method only when you are not sure about the type of statement else use executeQuery or executeUpdate method.

----

## **What do you understand by JDBC Statements?**

JDBC statements are basically the statements which are used to send SQL commands to the database and retrieve data back from the database. Various methods like execute(), executeUpdate(), executeQuery, etc. are provided by JDBC to interact with the database.

JDBC supports 3 types of statements:

Statement: Used for general purpose access to the database and executes a static SQL query at runtime.
PreparedStatement: Used to provide input parameters to the query during execution.
CallableStatement: Used to access the database stored procedures and helps in accepting runtime parameters.
In case you are facing any challenges with these java interview questions, please comment your problems in the section below. Apart from this Java Interview Questions Blog, if you want to get trained from professionals on this technology, you can opt for a structured training from edureka!

----

## **What is Spring?**

Wikipedia defines the Spring framework as “an application framework and inversion of control container for the Java platform. The framework’s core features can be used by any Java application, but there are extensions for building web applications on top of the Java EE platform.” Spring is essentially a lightweight, integrated framework that can be used for developing enterprise applications in java.

----

## **What are the differences between constructor injection and setter injection?**

|No.	|  Constructor Injection	            |                     Setter Injection |
| -------- | ---------------------------- | -------------------------------------- |
|1	|  No Partial Injection	                       |          Partial Injection |
|2	|  Doesn’t override the setter property	       |          Overrides the constructor property if both are defined. |
|3	|  Creates a new instance if any modification occurs	|     Doesn’t create a new instance if you change the property value |
|4 	|  Better for too many properties	               |          Better for a few properties. |

----

## **What is autowiring in Spring? What are the autowiring modes?**

Autowiring enables the programmer to inject the bean automatically. We don’t need to write explicit injection logic. Let’s see the code to inject bean using dependency injection.

```java
<bean id="emp" class="com.javatpoint.Employee" autowire="byName" />  
```

The autowiring modes are given below:

| No. | Mode | Description |
| ----- | ----- | ------------ |
| 1 | no | this is the default mode, it means autowiring is not enabled. |
| 2 | byName | Injects the bean based on the property name. It uses setter method. |
| 3 | byType | Injects the bean based on the property type. It uses setter method. |
| 4 | constructor | It injects the bean using constructor |

----

## **How to handle exceptions in Spring MVC Framework?**

Spring MVC Framework provides the following ways to help us achieving robust exception handling.

__Controller Based:__
We can define exception handler methods in our controller classes. All we need is to annotate these methods with @ExceptionHandler annotation.

__Global Exception Handler:__
Exception Handling is a cross-cutting concern and Spring provides @ControllerAdvice annotation that we can use with any class to define our global exception handler.

__HandlerExceptionResolver implementation:__
For generic exceptions, most of the times we serve static pages. Spring Framework provides HandlerExceptionResolver interface that we can implement to create global exception handler. The reason behind this additional way to define global exception handler is that Spring framework also provides default implementation classes that we can define in our spring bean configuration file to get spring framework exception handling benefits.

----

## **What are some of the important Spring annotations which you have used?**

Some of the Spring annotations that I have used in my project are:

__@Controller__ – for controller classes in Spring MVC project.

__@RequestMapping__ – for configuring URI mapping in controller handler methods. This is a very important annotation, so you should go through Spring MVC RequestMapping Annotation Examples

__@ResponseBody__ – for sending Object as response, usually for sending XML or JSON data as response.

__@PathVariable__ – for mapping dynamic values from the URI to handler method arguments.

__@Autowired__ – for autowiring dependencies in spring beans.

__@Qualifier__ – with @Autowired annotation to avoid confusion when multiple instances of bean type is present.

__@Service__ – for service classes.

__@Scope__ – for configuring the scope of the spring bean.

__@Configuration, @ComponentScan and @Bean__ – for java based configurations.

AspectJ annotations for configuring aspects and advices , @Aspect, @Before, @After, @Around, @Pointcut, etc.

----

## **How to integrate Spring and Hibernate Frameworks?**

We can use Spring ORM module to integrate Spring and Hibernate frameworks if you are using Hibernate 3+ where SessionFactory provides current session, then
you should avoid using HibernateTemplate or HibernateDaoSupport classes and better to use DAO pattern with dependency injection for the integration.

Also, Spring ORM provides support for using Spring declarative transaction management, so you should utilize that rather than going for hibernate boiler-plate code for transaction management. 

Integrating Spring and Hibernate frameworks involves configuring and wiring them together to leverage the benefits of both frameworks. Here are the general steps to integrate Spring and Hibernate:

Set up the project:

Create a new Java project using your preferred build tool (e.g., Maven or Gradle).
Include the required dependencies for both Spring and Hibernate in your project's build file.
Configure the Spring container:

Create a Spring configuration file (e.g., applicationContext.xml) to define the Spring beans and their dependencies.
Configure the data source bean to establish the database connection. You can use Spring's built-in DriverManagerDataSource or other data source implementations.
Set up the Hibernate session factory bean by providing the data source and other required Hibernate properties.
Configure the transaction manager to manage database transactions. Spring provides various transaction manager implementations, such as DataSourceTransactionManager or HibernateTransactionManager.
Create Hibernate entity classes:

Create your entity classes that represent the database tables in your application.
Annotate the entity classes with Hibernate annotations or use XML mappings to define the object-relational mapping (ORM) metadata.
Define Hibernate DAO classes:

Create DAO (Data Access Object) classes that encapsulate the CRUD operations and interact with the database using Hibernate.
Inject the session factory bean into the DAO classes to obtain a Hibernate session for performing database operations.
Configure Spring to manage Hibernate DAOs:

Declare the DAO beans in the Spring configuration file, specifying their dependencies (e.g., session factory).
Enable Spring's component scanning or explicitly define the DAO beans in the configuration file.
Implement business logic:

Create service classes that contain the business logic of your application.
Inject the DAO beans into the service classes to perform database operations.
Leverage Spring's transaction management:

Annotate the service classes or specific methods with @Transactional to enable Spring's declarative transaction management.
Spring will handle transaction boundaries, commit/rollback, and other transaction-related operations.
Build and run the application:

Build the project using your build tool.
Deploy the application to a web server or run it in your preferred environment.
By following these steps, you can integrate Spring and Hibernate frameworks, allowing Spring to manage the Hibernate session factory, transactions, and dependency injection while leveraging Hibernate's ORM capabilities for data persistence.

```java
// Entity class
@Entity
@Table(name = "users")
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    private String name;

    // Getters and setters
}

// DAO class
@Repository
public class UserDaoImpl implements UserDao {
    @Autowired
    private SessionFactory sessionFactory;

    @Override
    public User getUserById(Long id) {
        Session session = sessionFactory.getCurrentSession();
        return session.get(User.class, id);
    }

    // Other database operations
}

// Service class
@Service
@Transactional
public class UserService {
    @Autowired
    private UserDao userDao;

    public User getUserById(Long id) {
        return userDao.getUserById(id);
    }

    // Other business logic methods
}

// Main class
public class MainApp {
    public static void main(String[] args) {
        ApplicationContext context = new ClassPathXmlApplicationContext("applicationContext.xml");
        UserService userService = context.getBean(UserService.class);

        // Use the service to interact with the database
        User user = userService.getUserById(1L);
        System.out.println(user.getName());

        // ...
    }
}
```

In this example, we have a User entity class annotated with Hibernate annotations. The UserDaoImpl class is a Hibernate DAO that uses the session factory to perform database operations. The UserService class is a service layer that injects the DAO and provides business logic methods.

The Spring configuration file applicationContext.xml defines the beans, including the data source, session factory, transaction manager, DAO, and service beans. The @Repository, @Service, and @Transactional annotations are used to enable Spring's component scanning and transaction management.

In the MainApp class, we obtain the UserService bean from the Spring context and use it to retrieve a user from the database.

Note that this example is a simplified representation to demonstrate the integration of Spring and Hibernate. In a real-world application, you may need to configure additional settings, handle exceptions, and implement more advanced features based on your specific requirements.

----

## **Name the types of transaction management that Spring supports?**

Two types of transaction management are supported by Spring. They are:

Programmatic transaction management: In this, the transaction is managed with the help of programming. It provides you extreme flexibility, but it is very difficult to maintain.
Declarative transaction management: In this, transaction management is separated from the business code. Only annotations or XML based configurations are used to manage the transactions.
Apart from these Core Java interview questions for experienced professionals, if you want to get trained by professionals on this technology, you can opt for a structured training from edureka!

Hibernate – Java Interview Questions for Experienced Professionals

----

## **What is Hibernate Framework?**

Object-relational mapping or ORM is the programming technique to map application domain model objects to the relational database tables. Hibernate is Java-based ORM tool
that provides a framework for mapping application domain objects to the relational database tables and vice versa.

Hibernate provides a reference implementation of Java Persistence API, that makes it a great choice as ORM tool with benefits of loose coupling. We can use the Hibernate
persistence API for CRUD operations. Hibernate framework provide option to map plain old java objects to traditional database tables with the use of JPA
annotations as well as XML based configuration.

Similarly, hibernate configurations are flexible and can be done from XML configuration file as well as programmatically.

----

## **Example of Hibernate Framework**

Certainly! Here's a simple example of using Hibernate in Java:

Set up the project:

1. Create a new Java project and set up the necessary build configuration. Add the required dependencies for Hibernate in your project's build file (e.g., Maven or Gradle). Create Hibernate entity class:

2. Create a Java class that represents a table in your database. Annotate the class and its attributes with Hibernate annotations to define the object-relational mapping (ORM) metadata.

```java
import javax.persistence?*;

@Entity
@Table(name = "employees")
public class Employee {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    @Column(name = "name")
    private String name;

    @Column(name = "age")
    private int age;

    // Getters and setters
}
```

3. Configure Hibernate: Create a Hibernate configuration file (e.g., hibernate.cfg.xml) to specify the database connection details and other Hibernate settings.

```xml
<!-- hibernate.cfg.xml -->
<hibernate-configuration>
    <session-factory>
        <property name="hibernate.connection.driver_class">com.mysql.jdbc.Driver</property>
        <property name="hibernate.connection.url">jdbc:mysql://localhost:3306/mydatabase</property>
        <property name="hibernate.connection.username">root</property>
        <property name="hibernate.connection.password">password</property>
        <property name="hibernate.dialect">org.hibernate.dialect.MySQLDialect</property>
        <property name="hibernate.hbm2ddl.auto">update</property>
        <property name="hibernate.show_sql">true</property>
    </session-factory>
</hibernate-configuration>
```

4. Perform CRUD operations: Use the Hibernate API to perform CRUD (Create, Read, Update, Delete) operations on the database.

```java
import org.hibernate?*;
import org.hibernate.cfg.Configuration;

public class MainApp {
    public static void main(String[] args) {
        // Create a Hibernate SessionFactory
        SessionFactory sessionFactory = new Configuration().configure("hibernate.cfg.xml").buildSessionFactory();

        // Create a new employee
        Employee employee = new Employee();
        employee.setName("John Doe");
        employee.setAge(30);

        // Open a new Hibernate session
        Session session = sessionFactory.openSession();

        // Begin a transaction
        Transaction transaction = session.beginTransaction();

        // Save the employee to the database
        session.save(employee);

        // Commit the transaction
        transaction.commit();

        // Close the session
        session.close();

        // Retrieve the employee from the database
        Session session2 = sessionFactory.openSession();
        Employee retrievedEmployee = session2.get(Employee.class, employee.getId());
        System.out.println("Retrieved Employee: " + retrievedEmployee.getName() + " (Age: " + retrievedEmployee.getAge() + ")");

        // Close the session
        session2.close();

        // Close the SessionFactory
        sessionFactory.close();
    }
}
```

In this example, we have an Employee class annotated with Hibernate annotations. We create an Employee object, set its attributes, and save it to the database using the Hibernate Session object.

The Hibernate configuration file hibernate.cfg.xml specifies the database connection details and other Hibernate settings, such as the JDBC driver, database URL, dialect, and more.

We create a Hibernate SessionFactory using the Configuration class and the configuration file. Then, we open a new Hibernate Session and begin a transaction. We save the Employee object to the database, commit the transaction, and close the session.

----

## **What are the important benefits of using Hibernate Framework?**

Some of the important benefits of using hibernate framework are:
- Hibernate eliminates all the boiler-plate code that comes with JDBC and takes care of managing resources, so we can focus on business logic.
- Hibernate framework provides support for XML as well as JPA annotations, that makes our code implementation independent.
- Hibernate provides a powerful query language (HQL) that is similar to SQL. However, HQL is fully object-oriented and understands concepts like inheritance, polymorphism, and association.
- Hibernate is an open source project from Red Hat Community and used worldwide. This makes it a better choice than others because learning curve is small and there are tons of online documentation and help is easily available in forums.
- Hibernate is easy to integrate with other Java EE frameworks, it’s so popular that Spring Framework provides built-in support for integrating hibernate with Spring applications.
- Hibernate supports lazy initialization using proxy objects and perform actual database queries only when it’s required.
- Hibernate cache helps us in getting better performance.
- For database vendor specific feature, hibernate is suitable because we can also execute native sql queries.

Overall Hibernate is the best choice in current market for ORM tool, it contains all the features that you will ever need in an ORM tool.

----

## **Explain Hibernate architecture?**

Hibernate has a layered architecture which helps the user to operate without having to know the underlying APIs. Hibernate makes use of the database and configuration data to provide persistence services (and persistent objects) to the application. It includes many objects such as persistent object, session factory, transaction factory, connection factory, session, transaction etc.HibernateArchitecture - Java Interview Questions - Edureka

The Hibernate architecture is categorized in four layers.
- Java application layer
- Hibernate framework layer
- Backhand API layer
- Database layer

----

## **What are the differences between get and load methods?**

The differences between get() and load() methods are given below.

| No. | get() | load() |
| --- | ------- | ------ |
| 1 | Returns null if object is not found. | Throws ObjectNotFoundException if an object is not found. |
| 2 | get() method always hit the database. | load() method doesn’t hit the database. |
| 3 | It returns a real object, not a proxy. | It returns a proxy object. |
| 4 | It should be used if you are not sure about the existence of instance. | It should be used if you are sure that the instance exists. |

----

## **What are the advantages of Hibernate over JDBC?**

Some of the important advantages of Hibernate framework over are:

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

----

## **What is JDBC?**

JDBC stands for Java Database Connectivity. It is a Java API that provides a standard way to interact with relational databases. JDBC enables Java applications to connect to a database, execute SQL queries, retrieve and manipulate data, and manage database transactions.

Here are some key features and concepts related to JDBC:

Database Connectivity: JDBC provides classes and interfaces to establish a connection with a database server. It supports various database vendors through database-specific JDBC drivers.

JDBC Drivers: JDBC drivers are responsible for translating the generic JDBC API calls into the database-specific protocol required to communicate with the database server. There are four types of JDBC drivers: Type 1 (JDBC-ODBC bridge driver), Type 2 (native-API driver), Type 3 (network-protocol driver), and Type 4 (pure Java driver).

Connection and Statement: Once the connection to the database is established, JDBC provides the Connection interface to manage the connection. The Statement interface is used to execute SQL statements, such as queries, updates, inserts, and deletes.

Result Sets: When executing a query, JDBC returns a ResultSet object that represents the result of the query. The ResultSet allows you to navigate through the rows and retrieve data from the query result.

Prepared Statements: JDBC supports prepared statements, which allow you to pre-compile SQL statements with placeholders for parameters. Prepared statements help improve performance and prevent SQL injection attacks by separating SQL code from the data values.

Transactions: JDBC provides transaction management capabilities through the Connection interface. You can start, commit, or rollback transactions to ensure the integrity and consistency of database operations.

JDBC is widely used in Java applications to interact with relational databases, ranging from small desktop applications to large-scale enterprise systems. It provides a standardized and portable way to work with databases, allowing Java developers to leverage the power and flexibility of relational databases in their applications.

Example:

```java
import java.sql?*;

public class JdbcExample {
    public static void main(String[] args) {
        String jdbcUrl = "jdbc:mysql://localhost:3306/mydatabase";
        String username = "root";
        String password = "password";

        try {
            // Step 1: Load the JDBC driver
            Class.forName("com.mysql.jdbc.Driver");

            // Step 2: Establish a connection to the database
            Connection connection = DriverManager.getConnection(jdbcUrl, username, password);

            // Step 3: Create a Statement object
            Statement statement = connection.createStatement();

            // Step 4: Execute a query
            String sqlQuery = "SELECT * FROM employees";
            ResultSet resultSet = statement.executeQuery(sqlQuery);

            // Step 5: Process the results
            while (resultSet.next()) {
                int id = resultSet.getInt("id");
                String name = resultSet.getString("name");
                int age = resultSet.getInt("age");
                System.out.println("ID: " + id + ", Name: " + name + ", Age: " + age);
            }

            // Step 6: Close the resources
            resultSet.close();
            statement.close();
            connection.close();
        } catch (ClassNotFoundException e) {
            e.printStackTrace();
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}
```
In this example, we are connecting to a MySQL database using the MySQL JDBC driver. Here's a breakdown of the steps:

Load the JDBC driver using Class.forName(). The driver class name may vary depending on the database vendor.

Establish a connection to the database using DriverManager.getConnection(). Provide the JDBC URL, username, and password specific to your database.

Create a Statement object using the Connection.createStatement() method.

Execute a query using the Statement.executeQuery() method. In this example, we are retrieving all records from the "employees" table.

Process the results using a ResultSet. Iterate over the rows using the ResultSet.next() method and retrieve the values using column names or indices.

Close the resources (ResultSet, Statement, and Connection) to free up system resources.

Note: Make sure to replace the JDBC URL, username, and password with your actual database details.

This example demonstrates the basic JDBC workflow for executing a query and retrieving the results. Keep in mind that error handling, resource management, and best practices may vary depending on the specific requirements and complexity of your application.

----

## **What are the life-cycle methods for a jsp?**

| Methods | Description |
| -------- | ---------- |
| public void jspInit() | It is invoked only once, same as init method of servlet. |
| public void _jspService(ServletRequest request,ServletResponse)throws ServletException,IOException | It is invoked at each request, same as service() method of servlet. |
| public void jspDestroy() | It is invoked only once, same as destroy() method of servlet. |

----

## **What are the JSP implicit objects?**

JSP provides 9 implicit objects by default. They are as follows:

| Nr | Object | Type |
| ---- | ----- | ----- |
| 1 | out | JspWriter |
| 2 | request | HttpServletRequest |
| 3 | response | HttpServletResponse |
| 4 | config | ServletConfig |
| 5 | session | HttpSession |
| 6 | application | ServletContext |
| 7 | pageContext |  PageContext |
| 8 | page | Object |
| 9 | exception | Throwable |

----

## **What are the differences between include directive and include action?**

| include directive | include action |
| ----------------- | -------------- |
| The include directive includes the content at page translation time. | The include action includes the content at request time. |
| The include directive includes the original content of the page so page size increases at runtime. | The include action doesn’t include the original content rather invokes the include() method of Vendor provided class. |
| It’s better for static pages. | It’s better for dynamic pages. |

----

## **How to disable caching on back button of the browser?**

```java
// <%
// response.setHeader(“Cache-Control”,”no-store”);
// response.setHeader(“Pragma”,”no-cache”);
// response.setHeader (“Expires”, “0”); //prevents caching at the proxy server
// %>   
```

----

## **What are the different tags provided in JSTL?**

There are 5 type of JSTL tags.
- core tags
- sql tags
- xml tags
- internationalization tags
- functions tags

----

## **How to disable session in JSP?**

```java
// <%@ page session=“false” %>   
```

----

## **How to delete a Cookie in a JSP?**

```java
Cookie mycook = new Cookie("name1","value1");
response.addCookie(mycook1);
Cookie killmycook = new Cookie("mycook1","value1");
killmycook . set MaxAge ( 0 );
killmycook . set Path ("/");
killmycook . addCookie ( killmycook 1 );
```

OR

```java
<%
    Cookie[] cookies = request.getCookies();
    if (cookies != null) {
        for (Cookie cookie : cookies) {
            if ("myCookieName".equals(cookie.getName())) {
                cookie.setMaxAge(0); // Set maximum age to 0 to delete the cookie
                response.addCookie(cookie); // Update the cookie in the response
                break;
            }
        }
    }
%>
```

In the above example, we first retrieve all the cookies using request.getCookies(). We iterate over the cookies and check if the cookie name matches the one we want to delete (in this case, "myCookieName"). If a match is found, we set the maximum age of the cookie to 0 using cookie.setMaxAge(0). Finally, we add the updated cookie to the response using response.addCookie(cookie).
By setting the maximum age to 0, the browser will remove the cookie from its storage during the next request/response cycle.


----

## **Explain the jspDestroy() method?**

jspDestry() method is invoked from javax.servlet.jsp.JspPage interface whenever a JSP page is about to be destroyed. Servlets destroy methods can be easily
overridden to perform cleanup, like when closing a database connection.

```java
<%@ page import="javax.servlet.jsp.JspException" %>

<%
public void jspDestroy() {
    // Cleanup tasks
    // Release database connections, close files, etc.
    try {
        // Release any resources here
    } catch (Exception e) {
        // Handle exceptions if necessary
    }
}
%>
```

----

## **How is JSP better than Servlet technology?**

JSP is a technology on the server’s side to make content generation simple. They are document-centric, whereas servlets are programs.
A Java server page can contain fragments of Java program, which execute and instantiate Java classes. However, they occur inside an
HTML template file. It provides the framework for the development of a Web Application.

----

## **Why should we not configure JSP standard tags in web.xml?**

We don’t need to configure JSP standard tags in web.xml because when container loads the web application and find TLD files, it automatically
configures them to be used directly in the application JSP pages. We just need to include it in the JSP page using taglib directive.

----

## **How will you use JSP EL in order to get the HTTP method name?**

Using pageContext JSP EL implicit object you can get the request object reference and make use of the dot operator to retrieve the HTTP method name
in the JSP page. The JSP EL code for this purpose will look like ${pageContext.request.method}.

In case you are facing any challenges with these java interview questions, please comment on your problems in the section below. Apart from this 
ava Interview Questions Blog, if you want to get trained from professionals on this technology, you can opt for structured training from edureka!

----

## **What is the difference between Error and Exception?**

An error is an irrecoverable condition occurring at runtime. Such as OutOfMemory error. These JVM errors you cannot repair them at runtime. Though error can be caught in the catch block but the execution of application will come to a halt and is not recoverable.

While exceptions are conditions that occur because of bad input or human error etc. e.g. FileNotFoundException will be thrown if the specified file does not exist. Or a NullPointerException will take place if you try using a null reference. In most of the cases it is possible to recover from an exception (probably by giving the user feedback for entering proper values etc.

----

## **How can you handle Java exceptions?**

There are five keywords used to handle exceptions in Java: 
- try
- catch
- finally
- throw
- throws

----

## **What are the differences between Checked Exception and Unchecked Exception?**

__Checked Exception__
The classes that extend Throwable class except RuntimeException and Error are known as checked exceptions. 
Checked exceptions are checked at compile-time.
Example: IOException, SQLException etc.

```java
import java.io.FileReader;
import java.io.IOException;

public class Main {
    public static void main(String[] args) {
        FileReader fileReader = null;
        try {
            // Open a file
            fileReader = new FileReader("myfile.txt");

            // Perform some operations on the file
            // ...

        } catch (IOException e) {
            // Handle the IOException
            System.out.println("An error occurred while reading the file: " + e.getMessage());
        } finally {
            // Close the file in the finally block to ensure it's always closed
            try {
                if (fileReader != null) {
                    fileReader.close();
                }
            } catch (IOException e) {
                // Handle the IOException while closing the file
                System.out.println("An error occurred while closing the file: " + e.getMessage());
            }
        }
    }
}
```

__Unchecked Exception__
The classes that extend RuntimeException are known as unchecked exceptions. 
Unchecked exceptions are not checked at compile-time.
Example: ArithmeticException, NullPointerException etc.

```java
public class DivisionExample {
    public static void main(String[] args) {
        int dividend = 10;
        int divisor = 0;

        try {
            int result = divide(dividend, divisor);
            System.out.println("Result: " + result);
        } catch (ArithmeticException e) {
            System.out.println("An error occurred: " + e.getMessage());
        }
    }

    public static int divide(int dividend, int divisor) {
        return dividend / divisor;
    }
}
```

----

## **Will the finally block get executed when the return statement is written at the end of try block and catch block as shown below?**

The finally block always gets executed even hen the return statement is written at the end of the try block and the catch block. It always executes , whether there is
an exception or not. There are only a few situations in which the finally block does not execute, such as VM crash, power failure, software crash, etc. If you don’t want
to execute the finally block, you need to call the System.exit() method explicitly in the finally block.

----

## **How does an exception propagate in the code?**

If an exception is not caught, it is thrown from the top of the stack and falls down the call stack to the previous procedure. If the exception isn’t caught there, it falls back to the previous function, and so on, until it’s caught or the call stack reaches the bottom. The term for this is Exception propagation.

----

## **Can you explain the Java thread lifecycle?**

The java thread lifecycle has the following states-

__New__ When a thread is created, and before the program starts the thread, it is in the new state. It is also referred to as a born thread.

__Runnable__ When a thread is started, it is in the Runnable state. In this state, the thread is executing its task.

__Waiting__ Sometimes, a thread goes to the waiting state, where it remains idle because another thread is executing. When the other thread has finished, the waiting thread again comes into the running state.

__Timed Waiting__ In timed waiting, the thread goes to waiting state. But, it remains in waiting state for only a specified interval of time after which it starts executing.It remains waiting either till the time interval ends or till the other thread has finished.

__Terminated__ A thread is said to be in this state once it terminates. It may be because the thread has completed its task or due to any other reason.

----

## **What purpose do the keywords final, finally, and finalize fulfill?**

__Final__

Final is used to apply restrictions on class, method, and variable. A final class can’t be inherited, final method can’t be overridden and final variable value can’t be changed. Let’s take a look at the example below to understand it better.

```java
class Main {
    public static void main(String args[]) {
        final int a = 10; // Final variable
        int a = 50; // Error as value can't be changed
    }
}
```

__Finally__

Finally is used to place important code, it will be executed whether the exception is handled or not. Let’s take a look at the example below to understand it better.

```java
class Main {
    public static void main(String args[]) {
        try {
            int x=100;
        }
        catch(Exception e) {
            System.out.println(e);
        }
        finally {
            System.out.println("finally block is executing");}
    }
}
```

__Finalize__

Finalize is used to perform clean up processing just before the object is garbage collected. Let’s take a look at the example below to understand it better.

```java
class Main {
    public void finalize() {
        System.out.println("Finalize is called");
    }
    public static void main(String args[])
    {
        Main f1=new Main();
        Main f2=new Main();
        f1=NULL;
        f2=NULL;
        System.gc();
    }
}
```

----

## **What are the differences between throw and throws?**

| throw keyword | throws keyword |
| -------------- | -------------- |
| Throw is used to explicitly throw an exception. | Throws is used to declare an exception. |
| Checked exceptions can not be propagated with throw only. | Checked exception can be propagated with throws. |
| Throw is followed by an instance. | Throws is followed by class. |
| Throw is used within the method. | Throws is used with the method signature. |
| You cannot throw multiple exception | You can declare multiple exception e.g. public void method()throws IOException,SQLException. |

----

## **What is exception hierarchy in java?**

The hierarchy is as follows:

Throwable is a parent class of all Exception classes. There are two types of Exceptions: Checked exceptions and UncheckedExceptions or RunTimeExceptions. Both type of exceptions extends Exception class whereas errors are further classified into Virtual Machine error and Assertion error.

ExceptionHierarchy - Java Interview Questions - Edureka

----

## **How to create a custom Exception?**

To create you own exception extend the Exception class or any of its subclasses.

```java
class New1Exception extends Exception { } // this will create Checked Exception
class NewException extends IOException { } // this will create Checked exception
class NewException extends NullPonterExcpetion { } // this will create UnChecked exception
```

----

## **What are the important methods of Java Exception Class?**

Exception and all of it’s subclasses doesn’t provide any specific methods and all of the methods are defined in the base class Throwable.

__String getMessage()__ – This method returns the message String of Throwable and the message can be provided while creating the exception through it’s constructor.

__String getLocalizedMessage()__ – This method is provided so that subclasses can override it to provide locale specific message to the calling program. Throwable class implementation of this method simply use __getMessage()__ - method to return the exception message.

__Synchronized Throwable getCause()__ – This method returns the cause of the exception or null id the cause is unknown.

__String toString()__ – This method returns the information about Throwable in String format, the returned String contains the name of Throwable class and localized message.

__void printStackTrace()__ – This method prints the stack trace information to the standard error stream, this method is overloaded and we can pass PrintStream or PrintWriter as an argument to write the stack trace information to the file or stream.

----

## **What are the differences between processes and threads?**

| Process | Thread |
| -------- | -------- |
| Definition | An executing instance of a program is called a process. A thread is a subset of the process. |
| Communication | Processes must use inter-process communication to communicate with sibling processes. Threads can directly communicate with other threads of its process. |
| Control | Processes can only exercise control over child processes. Threads can exercise considerable control over threads of the same process. |
| Changes | Any change in the parent process does not affect child processes. Any change in the main thread may affect the behavior of the other threads of the process. |
| Memory | Run in separate memory spaces.	Run in shared memory spaces. |
| Controlled by	Process | Is controlled by the operating system. Threads are controlled by programmer in a program. |
| Dependence | Processes are independent. Threads are dependent. |

----

## **What is a finally block? Is there a case when finally will not execute?**

Finally block is a block which always executes a set of statements. It is always associated with a try block regardless of any exception that occurs or not. 
Yes, finally will not be executed if the program exits either by calling System.exit() or by causing a fatal error that causes the process to abort.

----

## **What is synchronization?**

Synchronization refers to multi-threading. A synchronized block of code can be executed by only one thread at a time. As Java supports execution of multiple threads, two or more threads may access the same fields or objects. Synchronization is a process which keeps all concurrent threads in execution to be in sync. Synchronization avoids memory consistency errors caused due to inconsistent view of shared memory. When a method is declared as synchronized the thread holds the monitor for that method’s object. If another thread is executing the synchronized method the thread is blocked until that thread releases the monitor. 

----

## **Can we write multiple catch blocks under single try block?**

Yes we can have multiple catch blocks under single try block but the approach should be from specific to general. Let’s understand this with a programmatic example.

```java
public class MultipleCatchExample {
    public static void main(String[] args) {
        try {
            int[] numbers = {1, 2, 3};
            int index = 4;
            int result = numbers[index];
            System.out.println("Result: " + result);
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Array index out of bounds: " + e.getMessage());
        } catch (ArithmeticException e) {
            System.out.println("Arithmetic exception occurred: " + e.getMessage());
        } catch (Exception e) {
            System.out.println("An exception occurred: " + e.getMessage());
        }
    }
}
```

----

## **What are the important methods of Java Exception Class?**

Methods are defined in the base class Throwable. Some of the important methods of Java exception class are stated below. 

String getMessage() – This method returns the message String about the exception. The message can be provided through its constructor.

public StackTraceElement[] getStackTrace() – This method returns an array containing each element on the stack trace. The element at index 0 represents the top of the call stack whereas the last element in the array represents the method at the bottom of the call stack.

Synchronized Throwable getCause() – This method returns the cause of the exception or null id as represented by a Throwable object.

String toString() – This method returns the information in String format. The returned String contains the name of Throwable class and localized message.

void printStackTrace() – This method prints the stack trace information to the standard error stream. 

----

## **What is OutOfMemoryError in Java?**

OutOfMemoryError is the subclass of java.lang.Error which generally occurs when our JVM runs out of memory.

----

## **What is a Thread?**

A thread is the smallest piece of programmed instructions which can be executed independently by a scheduler. In Java, all the programs will have at least one thread which is known as the main thread. This main thread is created by the JVM when the program starts its execution. The main thread is used to invoke the main() of the program.

----

## **What are the two ways to create a thread?**

In Java, threads can be created in the following two ways:- 

By implementing the Runnable interface.
By extending the Thread

----

## **What are the different types of garbage collectors in Java?**

Garbage collection in Java a program which helps in implicit memory management. Since in Java, using the new keyword you can create objects dynamically, which once created will consume some memory. Once the job is done and there are no more references left to the object, Java using garbage collection destroys the object and relieves the memory occupied by it. Java provides four types of garbage collectors:

Serial Garbage Collector
Parallel Garbage Collector
CMS Garbage Collector
G1 Garbage Collector

### https://www.edureka.co/blog/interview-questions/java-interview-questions/

### https://www.interviewbit.com/java-interview-questions/

## **Can you tell the difference between equals() method and equality operator (==) in Java?**

We are already aware of the (==) equals operator. That we have used this to compare the equality of the values. But when we talk about the terms of object-oriented programming, we deal with the values in the form of objects. And this object may contain multiple types of data. So using the (==) operator does not work in this case. So we need to go with the .equals() method.

Both [(==) and .equals()] primary functionalities are to compare the values, but the secondary functionality is different. 

So in order to understand this better, let’s consider this with the example -

```java
String str1 = "InterviewBit";
String str2 = "InterviewBit";
```

System.out.println(str1 == str2);
This code will print true. We know that both strings are equals so it will print true. But here (==) Operators don’t compare each character in this case. It compares the memory location. And because the string uses the constant pool for storing the values in the memory, both str1 and str2 are stored at the same memory location. See the detailed Explanation in Question no 73: Link.

Now, if we modify the program a little bit with -

```java
String str1 = new String("InterviewBit");
String str2 = "InterviewBit";
System.out.println(str1 == str2);
```

Then in this case, it will print false. Because here no longer the constant pool concepts are used. Here, new memory is allocated. So here the memory address is different, therefore ( == ) Operator returns false. But the twist is that the values are the same in both strings. So how to compare the values? Here the .equals() method is used.

.equals() method compares the values and returns the result accordingly.  If we modify the above code with - 

```java
System.out.println(str1.equals(str2));
```

Then it returns true.

| equals() | == |
| ------ | ---- |
| This is a method defined in the Object class. | It is a binary operator in Java. |
| The .equals() Method is present in the Object class, so we can override our custom .equals() method in the custom class, for objects comparison. | It cannot be modified. They always compare the HashCode. |
| This method is used for checking the equality of contents between two objects as per the specified business logic. | This operator is used for comparing addresses (or references), i.e checks if both the objects are pointing to the same memory location. |

Note: In the cases where the equals method is not overridden in a class, then the class uses the default implementation of the equals method that is closest to the parent class.
Object class is considered as the parent class of all the java classes. The implementation of the equals method in the Object class uses the == operator to compare two objects. This default implementation can be overridden as per the business logic.

----

## **Can the static methods be overloaded?**

Yes! There can be two or more static methods in a class with the same name but differing input parameters.

----

## **Why is the main method static in Java?**

The main method is always static because static members are those methods that belong to the classes, not to an individual object. So if the main method will not be static then for every object, It is available. And that is not acceptable by JVM. JVM calls the main method based on the class name itself. Not by creating the object.

Because there must be only 1 main method in the java program as the execution starts from the main method. So for this reason the main method is static. 

----

## **Can the static methods be overridden?**

No! Declaration of static methods having the same signature can be done in the subclass but run time polymorphism can not take place in such cases.
Overriding or dynamic polymorphism occurs during the runtime, but the static methods are loaded and looked up at the compile time statically. Hence, these methods cant be overridden.

----

## **Difference between static methods, static variables, and static classes in java?**

Static Methods and Static variables are those methods and variables that belong to the class of the java program, not to the object of the class. This gets memory where the class is loaded. And these can directly be called with the help of class names.
For example - We have used mathematical functions in the java program like - max(), min(), sqrt(), pow(), etc. And if we notice that, then we will find that we call it directly with the class name. Like - Math.max(), Math.min(), etc. So that is a static method.  And Similarly static variables we have used like (length) for the array to get the length. So that is the static method.
Static classes - A class in the java program cannot be static except if it is the inner class. If it is an inner static class, then it exactly works like other static members of the class.

----

## **What is the main objective of garbage collection?**

The main objective of this process is to free up the memory space occupied by the unnecessary and unreachable objects during the Java program execution by deleting those unreachable objects.
This ensures that the memory resource is used efficiently, but it provides no guarantee that there would be sufficient memory for the program execution.

----

## **What is a ClassLoader?**

Java Classloader is the program that belongs to JRE (Java Runtime Environment). The task of ClassLoader is to load the required classes and interfaces to the JVM when required. 
Example- To get input from the console, we require the scanner class. And the Scanner class is loaded by the ClassLoader.

----

## **What part of memory - Stack or Heap - is cleaned in garbage collection process?**

Heap.

----

## **Apart from the security aspect, what are the reasons behind making strings immutable in Java?**

A String is made immutable due to the following reasons:

String Pool: Designers of Java were aware of the fact that String data type is going to be majorly used by the programmers and developers. Thus, they wanted optimization from the beginning. They came up with the notion of using the String pool (a storage area in Java heap) to store the String literals. They intended to decrease the temporary String object with the help of sharing. An immutable class is needed to facilitate sharing. The sharing of the mutable structures between two unknown parties is not possible. Thus, immutable Java String helps in executing the concept of String Pool.

Multithreading: The safety of threads regarding the String objects is an important aspect in Java. No external synchronization is required if the String objects are immutable. Thus, a cleaner code can be written for sharing the String objects across different threads. The complex process of concurrency is facilitated by this method.
Collections: In the case of Hashtables and HashMaps, keys are String objects. If the String objects are not immutable, then it can get modified during the period when it resides in the HashMaps. Consequently, the retrieval of the desired data is not possible. Such changing states pose a lot of risks. Therefore, it is quite safe to make the string immutable.

----

## **Which of the below generates a compile-time error? State the reason?**

```java
int[] n1 = new int[0];
boolean[] n2 = new boolean[-200];
double[] n3 = new double[2241423798]; // true, integer number too large
char[] ch = new char[20];
```

We get a compile-time error in line 3. The error we will get in Line 3 is - integer number too large. It is because the array requires size as an integer. And Integer takes 4 Bytes in the memory. And the number (2241423798) is beyond the capacity of the integer. The maximum array size we can declare is - (2147483647).

Because the array requires the size in integer, none of the lines (1, 2, and 4) will give a compile-time error. The program will compile fine. But we get the runtime exception in line 2. The exception is - NegativeArraySizeException. 

Here what will happen is - At the time when JVM will allocate the required memory during runtime then it will find that the size is negative. And the array size can’t be negative. So the JVM will throw the exception.

----

## **Is this program giving a compile-time error? If Yes then state the reason and number of errors it will give. If not then state the reason?**

```java
abstract final class IB{
    public abstract void printMessage();
 }
 class ScalarAcademy extends IB{
    public void printMessage(){
        System.out.println("Welcome to Scalar Academy By InterviewBit");
    }
 }
 
class ScalarTopics extends ScalarAcademy{
    public void printMessage(){
                System.out.println("Welcome to Scalar Topics By Scalar Academy");
            }
 }

public class Main{
    public static void main(String[] args) {
        IB ib = new ScalarTopics();
        ib.printMessage();
    }
}

// Output:
// [Illegal Combination of modifiers: abstract and final] at line 1.
// [Cannot inherit from final ‘InterviewBit’] at line 4.
```

----

## **What is a Comparator in java?**

Consider the example where we have an ArrayList of employees like( EId, Ename, Salary), etc. Now if we want to sort this list of employees based on the names of employees. Then that is not possible to sort using the Collections.sort() method. We need to provide something to the sort() function depending on what values we have to perform sorting. Then in that case a comparator is used.

Comparator is the interface in java that contains the compare method. And by overloading the compare method, we can define that on what basis we need to compare the values. 

```java
import java.util.ArrayList;
import java.util.Collections;
import java.util.Comparator;
import java.util.List;

class Student {
    private String name;
    private int age;

    public Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }

    public int getAge() {
        return age;
    }

    @Override
    public String toString() {
        return "Student{" +
                "name='" + name + '\'' +
                ", age=" + age +
                '}';
    }
}

class AgeComparator implements Comparator<Student> {
    @Override
    public int compare(Student s1, Student s2) {
        return Integer.compare(s1.getAge(), s2.getAge());
    }
}

public class ComparatorExample {
    public static void main(String[] args) {
        List<Student> students = new ArrayList<>();
        students.add(new Student("Alice", 20));
        students.add(new Student("Bob", 18));
        students.add(new Student("Charlie", 22));

        System.out.println("Before sorting:");
        for (Student student : students) {
            System.out.println(student);
        }

        Collections.sort(students, new AgeComparator());

        System.out.println("\nAfter sorting by age:");
        for (Student student : students) {
            System.out.println(student);
        }
    }
}
```

----

## **In Java, static as well as private method overriding is possible. Comment on the statement?**

The statement in the context is completely False. The static methods have no relevance with the objects, and these methods are of the class level. In the case of a child class, a static method with a method signature exactly like that of the parent class can exist without even throwing any compilation error.

The phenomenon mentioned here is popularly known as method hiding, and overriding is certainly not possible. Private method overriding is unimaginable because the visibility of the private method is restricted to the parent class only. As a result, only hiding can be facilitated and not overriding.

----

## **What is the importance of reflection in Java?**

The term reflection is used for describing the inspection capability of a code on other code either of itself or of its system and modify it during runtime.
Consider an example where we have an object of unknown type and we have a method ‘fooBar()’ which we need to call on the object. The static typing system of Java doesn't allow this method invocation unless the type of the object is known beforehand. This can be achieved using reflection which allows the code to scan the object and identify if it has any method called “fooBar()” and only then call the method if needed.

```java
Method methodOfFoo = fooObject.getClass().getMethod("fooBar", null);
methodOfFoo.invoke(fooObject, null);
```

*Using reflection has its own cons:*

*Speed* — Method invocations due to reflection are about three times slower than the direct method calls.
*Type safety* — When a method is invoked via its reference wrongly using reflection, invocation fails at runtime as it is not detected at compile/load time.
*Traceability* — Whenever a reflective method fails, it is very difficult to find the root cause of this failure due to a huge stack trace. One has to deep dive into the invoke() and proxy() method logs to identify the root cause. Hence, it is advisable to follow solutions that don't involve reflection and use this method as a last resort.

Example:

```java
import java.lang.reflect.Field;
import java.lang.reflect.Method;

class MyClass {
    private int privateField;

    public void publicMethod() {
        System.out.println("Inside publicMethod");
    }

    private void privateMethod() {
        System.out.println("Inside privateMethod");
    }
}

public class ReflectionExample {
    public static void main(String[] args) throws NoSuchFieldException, NoSuchMethodException {
        MyClass obj = new MyClass();

        // Get the class object
        Class<?> cls = obj.getClass();

        // Accessing fields using reflection
        Field privateField = cls.getDeclaredField("privateField");
        System.out.println("Field name: " + privateField.getName());

        // Accessing methods using reflection
        Method publicMethod = cls.getMethod("publicMethod");
        System.out.println("Method name: " + publicMethod.getName());

        Method privateMethod = cls.getDeclaredMethod("privateMethod");
        System.out.println("Method name: " + privateMethod.getName());
    }
}
```

In the above example, we have a class MyClass with a private field privateField and two methods: publicMethod and privateMethod.

In the ReflectionExample class, we create an instance of MyClass and then obtain its class object using the getClass() method.

Using reflection, we can access the private field and methods of the class. We use the getDeclaredField() method to access the private field privateField and getMethod() to access the public method publicMethod.

To access the private method privateMethod, we use getDeclaredMethod() instead, as it allows us to access private methods.

Finally, we print the names of the field and methods obtained through reflection.

Reflection provides a powerful mechanism to examine and manipulate the properties and behavior of classes at runtime. It allows you to access private members, invoke methods dynamically, and perform other advanced operations. However, it should be used judiciously, as it can introduce complexity and impact performance if used improperly.

----

## **What are the different types of Thread Priorities in Java? And what is the default priority of a thread assigned by JVM?**

__There are a total of 3 different types of priority available in Java.__
- MIN_PRIORITY: It has an integer value assigned with 1.
- MAX_PRIORITY: It has an integer value assigned with 10.
- NORM_PRIORITY: It has an integer value assigned with 5.

In Java, Thread with MAX_PRIORITY gets the first chance to execute. But the default priority for any thread is NORM_PRIORITY assigned by JVM. 

```java
public class ThreadPriorityExample {
    public static void main(String[] args) {
        Thread thread1 = new MyThread("Thread 1", Thread.MIN_PRIORITY);
        Thread thread2 = new MyThread("Thread 2", Thread.NORM_PRIORITY);
        Thread thread3 = new MyThread("Thread 3", Thread.MAX_PRIORITY);

        thread1.start();
        thread2.start();
        thread3.start();
    }
}

class MyThread extends Thread {
    public MyThread(String name, int priority) {
        super(name);
        setPriority(priority);
    }

    @Override
    public void run() {
        System.out.println(getName() + " started.");
        for (int i = 0; i < 5; i++) {
            System.out.println(getName() + ": " + i);
        }
        System.out.println(getName() + " finished.");
    }
}
```

----

## **What is the difference between the program and the process?**

A program can be defined as a line of code written in order to accomplish a particular task.
Whereas the process can be defined as the programs which are under execution. 

A program doesn't execute directly by the CPU. First, the resources are allocated to the program and when it is ready for execution then it is a process.

----

## **What are the differences between constructor and method of a class in Java?**

| Constructor | Method |
| --------- | ------- |
| Constructor is used for initializing the object state. | Method is used for exposing the object's behavior. |
| Constructor has no return type. | Method should have a return type. Even if it does not return anything, return type is void. |
| Constructor gets invoked implicitly. | Method has to be invoked on the object explicitly. |

If the constructor is not defined, then a default constructor is provided by the java compiler.	If a method is not defined, then the compiler does not provide it.
The constructor name should be equal to the class name.	The name of the method can have any name or have a class name too.
A constructor cannot be marked as final because whenever a class is inherited, the constructors are not inherited. Hence, marking it final doesn't make sense. Java throws compilation error saying - modifier final not allowed here	A method can be defined as final but it cannot be overridden in its subclasses.
Final variable instantiations are possible inside a constructor and the scope of this applies to the whole class and its objects.	A final variable if initialised inside a method ensures that the variable cant be changed only within the scope of that method.

----

## **Identify the output of the below java program and Justify your answer?**

```java
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
```

The above code will throw the compilation error. It is because the super() is used to call the parent class constructor. But there is the condition that super() must be the first statement in the block. Now in this case, if we replace this() with super() then also it will throw the compilation error. Because this() also has to be the first statement in the block. So in conclusion, we can say that we cannot use this() and super() keywords in the same block.

----

## **Java works as “pass by value” or “pass by reference” phenomenon?**

Java always works as a “pass by value”. There is nothing called a “pass by reference” in Java. However, when the object is passed in any method, the address of the value is passed due to the nature of object handling in Java. When an object is passed, a copy of the reference is created by Java and that is passed to the method. The objects point to the same memory location. 2 cases might happen inside the method:

Case 1: When the object is pointed to another location: In this case, the changes made to that object do not get reflected the original object before it was passed to the method as the reference points to another location.
For example:

```java
class IBT{
    int num;
    IBT(int x){
        num = x;
    }
    IBT(){
        num = 0;
    }
}

class Driver {
    public static void main(String[] args)
    {
        // create a reference
        IBT ibTestObj = new IBT(20);
        // Pass the reference to updateObject Method
        updateObject(ibTestObj);
        // After the updateObject is executed, check for the value of num in the object.
        System.out.println(ibTestObj.num);
    }
    public static void updateObject(IBT ibObj)
    {
        // Point the object to new reference
        ibObj = new IBT();
        // Update the value
        ibObj.num = 50;
    }
}

// Output:
// 20
```

Case 2: When object references are not modified: In this case, since we have the copy of reference the main object pointing to the same memory location, any changes in the content of the object get reflected in the original object.
For example:

```java
class IBTest{
    int num;
    IBTest(int x){
        num = x;
    }
    IBTest(){
        num = 0;
    }
}
class Main{
    public static void main(String[] args)
    {
        //create a reference
        IBTest ibTestObj = new IBTest(20);
        //Pass the reference to updateObject Method
        updateObject(ibTestObj);
        //After the updateObject is executed, check for the value of num in the object.
        System.out.println(ibTestObj.num);
    }
    public static void updateObject(IBTest ibObj)
    {
        // no changes are made to point the ibObj to new location
        // Update the value of num
        ibObj.num = 50;
    }
}

// Output:
// 50
```

----

## **How to not allow serialization of attributes of a class in Java?**

In order to achieve this, the attribute can be declared along with the usage of transient keyword as shown below:

```java
public class Main {
    private transient String someInfo;
    private String name;
    private int id;
    // :
    // Getters setters
    // :
} 
```

In the above example, all the fields except someInfo can be serialized.

----

## **What happens if the static modifier is not included in the main method signature in Java?**

There wouldn't be any compilation error. But then the program is run, since the JVM cant map the main method signature, the code throws “NoSuchMethodError” error at the runtime.

----

## **Consider the below program, identify the output, and also state the reason for that?**

```java
public class Main{
    public static void main(String[] args) {
        System.out.println(" Hello. Main Method. ");
    }
    public static void main(int[] args) {
        System.out.println(" Hello. Main Method2. ");
    }
}

// Output
// Hello. Main Method.
```

The output of the above program will be Hello. Main Method. This is because JVM will always call the main method based on the definition it
already has. Doesn't matter how many main methods we overload it will only execute one main method based on its declaration in JVM.

----

## **Can we make the main() thread a daemon thread?**

In java multithreading, the main() threads are always non-daemon threads. And there is no way we can change the nature of the non-daemon thread to the daemon thread.

----

## **What happens if there are multiple main methods inside one class in Java?**

The program can't compile as the compiler says that the method has been already defined inside the class.

----

## **What do you understand by Object Cloning and how do you achieve it in Java?**

It is the process of creating an exact copy of any object. In order to support this, a java class has to implement the Cloneable interface of java.lang package and override the clone() method provided by the Object class the syntax of which is:

```java
// Implement the Cloneable interface
class MyClass implements Cloneable {
    private int value;

    public MyClass(int value) {
        this.value = value;
    }

    public int getValue() {
        return value;
    }

    public void setValue(int value) {
        this.value = value;
    }

    // Override the clone method
    @Override
    protected Object clone() throws CloneNotSupportedException {
        return super.clone();
    }
}

public class Main {
    public static void main(String[] args) {
        // Create an object
        MyClass original = new MyClass(10);

        try {
            // Clone the object
            MyClass cloned = (MyClass) original.clone();

            // Modify the value in the cloned object
            cloned.setValue(20);

            // Output the values of the original and cloned objects
            System.out.println("Original value: " + original.getValue());
            System.out.println("Cloned value: " + cloned.getValue());
        } catch (CloneNotSupportedException e) {
            e.printStackTrace();
        }
    }
}

```

In the above example, we have the MyClass class that implements the Cloneable interface. The class has a value field and getter/setter methods.

To enable cloning, we override the clone method from the Object class. In the main method, we create an original object of MyClass. Then, we clone the object using the clone method and cast it to MyClass.

We modify the value of the cloned object and output the values of the original and cloned objects. The output will show that modifying the cloned object does not affect the original object.

----

## **How does an exception propagate in the code?**

When an exception occurs, first it searches to locate the matching catch block. In case, the matching catch block is located, then that block would be executed. Else, the exception propagates through the method call stack and goes into the caller method where the process of matching the catch block is performed. This propagation happens until the matching catch block is found. If the match is not found, then the program gets terminated in the main method.

----

## **How do exceptions affect the program if it doesn't handle them?**

Exceptions are runtime errors. Suppose we are making an android application with java. And it all works fine but there is an exceptional case when the application tries to get the file from storage and the file doesn’t exist (This is the case of exception in java). And if this case is not handled properly then the application will crash. This will be a bad experience for users.  This is the type of error that cannot be controlled by the programmer. But programmers can take some steps to avoid this so that the application won’t crash. The proper action can be taken at this step.

If exceptions are not handled in a Java program, they can have several effects:

Program Termination: Unhandled exceptions can cause the program to terminate abruptly. When an exception occurs and is not caught or handled, it propagates up the call stack until it reaches the top-level of the program. At this point, if the exception is not caught, the program terminates, and an error message or stack trace is displayed.

Incomplete Operations: If an exception occurs during the execution of a specific operation or task, and the exception is not handled, the operation may not complete successfully. This can leave the program in an inconsistent state or with incomplete results.

Resource Leaks: If an exception occurs while working with resources like files, database connections, or network sockets, and the exception is not properly handled or cleaned up, it can result in resource leaks. Unclosed resources can lead to memory leaks or prevent other parts of the program from accessing those resources.

Unexpected Behavior: Unhandled exceptions can lead to unexpected behavior in the program. It can cause the program to produce incorrect results, crash, or behave unpredictably.

Debugging Difficulties: If exceptions are not handled, it becomes harder to identify and debug the cause of the problem. Without proper exception handling, error messages or stack traces may not be logged or displayed, making it challenging to trace the root cause of the issue.

It is essential to handle exceptions appropriately in a Java program to ensure proper error handling, graceful program termination, resource cleanup, and to maintain expected program behavior.

----

## **Is it mandatory for a catch block to be followed after a try block?**

No, it is not necessary for a catch block to be present after a try block. - A try block should be followed either by a catch block or by a finally block. If the exceptions likelihood is more, then they should be declared using the throws clause of the method.

----

## **Will the finally block get executed when the return statement is written at the end of try block and catch block as shown below?**

```java
class SomeClass {
    public int someMethod(int i){
        try{
            return 1;
        }catch(Exception e){
            return 999;
        }finally{
            System.out.println("Gets executed!");
        }
    }
}

class Main {
    public static void main(String[] args)
    {
        SomeClass someObj = new SomeClass();
        someObj.someMethod(2);
    }
}

// Answer
// Yes, finally block will be executed irrespective of the exception or not. The only case where finally block is not executed is when it encounters ‘System.exit()’ method anywhere in try/catch block.
```

----

## **Can you call a constructor of a class inside the another constructor?**

Yes, the concept can be termed as constructor chaining and can be achieved using this().

```java
class Person {
    private String name;
    private int age;

    // Constructor with name and age parameters
    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    // Constructor with only name parameter, which sets the age to a default value of 0
    public Person(String name) {
        this(name, 0);
    }
}

public class Main {
    public static void main(String[] args)
    {
        Person newP = new Person("John", 45);
    }
}
```

----

## **Contiguous memory locations are usually used for storing actual values in an array but not in ArrayList. Explain?**

In the case of ArrayList, data storing in the form of primitive data types (like int, float, etc.) is not possible. The data members/objects present in the ArrayList have references to the objects which are located at various sites in the memory. Thus, storing of actual objects or non-primitive data types (like Integer, Double, etc.) takes place in various memory locations.

However, the same does not apply to the arrays. Object or primitive type values can be stored in arrays in contiguous memory locations, hence every element does not require any reference to the next element.

----

## **How does the size of ArrayList grow dynamically? And also state how it is implemented internally?**

__ArrayList is implemented in such a way that it can grow dynamically. We don't need to specify the size of ArrayList. For adding the values in it, the methodology it uses is__

1. Consider initially that there are 2 elements in the ArrayList. [2, 3].
2. If we need to add the element into this. Then internally what will happen is-
    1. ArrayList will allocate the new ArrayList of Size (current size + half of the current size). And add the old elements into the new. Old - [2, 3],    New - [2, 3, null].
    2. Then the new value will be inserted into it. [2, 3, 4, null]. And for the next time, the extra space will be available for the value to be inserted.
3. This process continues and the time taken to perform all of these is considered as the amortized constant time. 

__This is how the ArrayList grows dynamically. And when we delete any entry from the ArrayList then the following steps are performed__

1. It searches for the element index in the array. Searching takes some time. Typically it’s O(n) because it needs to search for the element in the entire array.
2. After searching the element, it needs to shift the element from the right side to fill the index.

So this is how the elements are deleted from the ArrayList internally. Similarly, the search operations are also implemented internally as defined in removing elements from the list (searching for elements to delete).

```java
import java.util.ArrayList;

public class ArrayListExample {
    public static void main(String[] args) {
        // Create an ArrayList of integers
        ArrayList<Integer> numbers = new ArrayList<>();

        // Add elements to the ArrayList
        numbers.add(10);
        numbers.add(20);
        numbers.add(30);

        // Get the size of the ArrayList
        int size = numbers.size();
        System.out.println("Size of ArrayList: " + size);

        // Access elements by index
        int firstElement = numbers.get(0);
        System.out.println("First element: " + firstElement);

        // Modify an element
        numbers.set(1, 25);

        // Remove an element
        numbers.remove(2);

        // Iterate over the ArrayList
        System.out.println("Elements in ArrayList:");
        for (int number : numbers) {
            System.out.println(number);
        }

        // Check if the ArrayList contains a specific element
        boolean contains = numbers.contains(10);
        System.out.println("Contains 10? " + contains);

        // Clear the ArrayList
        numbers.clear();

        // Check if the ArrayList is empty
        boolean isEmpty = numbers.isEmpty();
        System.out.println("Is ArrayList empty? " + isEmpty);
    }
}
```

----

## **Although inheritance is a popular OOPs concept, it is less advantageous than composition. Explain?**

Inheritance lags behind composition in the following scenarios:

Multiple-inheritance is not possible in Java. Classes can only extend from one superclass. In cases where multiple functionalities are required, for example - to read and write information into the file, the pattern of composition is preferred. The writer, as well as reader functionalities, can be made use of by considering them as the private members.
Composition assists in attaining high flexibility and prevents breaking of encapsulation.
Unit testing is possible with composition and not inheritance. When a developer wants to test a class composing a different class, then Mock Object can be created for signifying the composed class to facilitate testing. This technique is not possible with the help of inheritance as the derived class cannot be tested without the help of the superclass in inheritance.
The loosely coupled nature of composition is preferable over the tightly coupled nature of inheritance.
Let’s take an example:

```java
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

// In the above example, inheritance is followed. Now, some modifications
// are done to the Top class like this:
public class Top {
    public int start() {
        return 0;
    }
    public void stop() {
    }
}

// If the new implementation of the Top class is followed, a compile-time error is bound to occur in the Bottom class. Incompatible return type is there
// for the Top.stop() function. Changes have to be made to either the Top or the Bottom class to ensure compatibility. However, the composition technique
// can be utilized to solve the given problem:
class Bottom {
    Top par = new Top();
    public int stop() {
        par.start();
        par.stop();
        return 0;
    }
} 
```

----

## **What are Composition and Aggregation? State the difference?**

Composition, and Aggregation help to build (Has - A - Relationship) between classes and objects. But both are not the same in the end. Let’s understand with the help of an example. 

Consider the University as a class that has some departments in it. So the university will be the container object. And departments in it will contain objects. Now in this case, if the container object destroys then the contained objects will also get destroyed automatically.  So here we can say that there is a strong association between the objects. So this Strong Association is called Composition.
Now consider one more example. Suppose we have a class department and there are several professors' objects there in the department. Now if the department class is destroyed then the professor's object will become free to bind with other objects. Because container objects (Department) only hold the references of contained objects (Professor’s). So here is the weak association between the objects. And this weak association is called Aggregation.

----

## **How is the creation of a String using new() different from that of a literal?**

When a String is formed as a literal with the assistance of an assignment operator, it makes its way into the String constant pool so that String Interning can take place. This same object in the heap will be referenced by a different String if the content is the same for both of them.

```java
// new()
String str1 = new String("Hello");
```

```java
// literal
String str2 = "Hello";
```

----

## **Question**

The checking() function will return true as the same content is referenced by both the variables.

Conversely, when a String formation takes place with the help of a new() operator, interning does not take place. The object gets created in the heap memory even if the same content object is present.

```java
class Checker {
    public boolean checking() {
        String first = new String("InterviewBit");
        String second = new String("InterviewBit");
        if (first == second)
            return true;
        else
            return false;
    }
}

public class Main{
    public static void main(String[] args){
        Checker nChecker = new Checker();
        nChecker.checking();
    }
}
```

The checking() function will return false as the same content is not referenced by both the variables.

----

## **How is the 'new' operator different from the ‘newInstance()’ operator in java?**

Both new and newInstance() operators are used to creating objects.

The difference is- that when we already know the class name for which we have to create the object then we use a new operator. But suppose we don’t know the class name for which we need to create the object, Or we get the class name from the command line argument, or the database, or the file. Then in that case we use the 'newInstance()' operator.

The 'newInstance()' keyword throws an exception that we need to handle. It is because there are chances that the class definition doesn’t exist, and we get the class name from runtime. So it will throw an exception.

----

## **Is exceeding the memory limit possible in a program despite having a garbage collector?**

Yes, it is possible for the program to go out of memory in spite of the presence of a garbage collector. Garbage collection assists in recognizing and eliminating those objects which are not required in the program anymore, in order to free up the resources used by them.

In a program, if an object is unreachable, then the execution of garbage collection takes place with respect to that object. If the amount of memory required for creating a new object is not sufficient, then memory is released for those objects which are no longer in the scope with the help of a garbage collector. The memory limit is exceeded for the program when the memory released is not enough for creating new objects.

Moreover, exhaustion of the heap memory takes place if objects are created in such a manner that they remain in the scope and consume memory. The developer should make sure to dereference the object after its work is accomplished. Although the garbage collector endeavors its level best to reclaim memory as much as possible, memory limits can still be exceeded.

Let’s take a look at the following example:

```java
import java.util.LinkedList;
import java.util.List;

public class Main{
    public static void main(String[] args){
        List<String> example = new LinkedList<String>();
        while(true){
            example.add(new String("Memory Limit Exceeded"));
        }
    }
}
```

----

## **Why is synchronization necessary? Explain with the help of a relevant example?**

Concurrent execution of different processes is made possible by synchronization. When a particular resource is shared between many threads, situations may arise in which multiple threads require the same shared resource.

Synchronization assists in resolving the issue and the resource is shared by a single thread at a time. Let’s take an example to understand it more clearly. For example, you have a URL and you have to find out the number of requests made to it. Two simultaneous requests can make the count erratic.

No synchronization:

```java
class Counting {
    private int increase_counter;
    public int increase() {
        increase_counter = increase_counter + 1;
        return increase_counter;
    }
}

public class Main {
    public static void main(String[] args) {
        Counting newCounting = new Counting();
        newCounting.increase();
    }
}
```

If a thread Thread1 views the count as 10, it will be increased by 1 to 11. Simultaneously, if another thread Thread2 views the count as 10, it will be increased by 1 to 11. Thus, inconsistency in count values takes place because the expected final value is 12 but the actual final value we get will be 11.

Now, the function increase() is made synchronized so that simultaneous accessing cannot take place.

With synchronization:

```java
class Counting {
    private int increase_counter;
    public synchronized int increase() {
        increase_counter = increase_counter + 1;
        return increase_counter;
    }
}

public class Main {
    public static void main(String[] args) {
        Counting newCounting = new Counting();
        newCounting.increase();
    }
}
```

If a thread Thread1 views the count as 10, it will be increased by 1 to 11, then the thread Thread2 will view the count as 11, it will be increased by 1 to 12. Thus, consistency in count values takes place.

----

## **In the given code below, what is the significance of ... ?**

Ability to provide ... is a feature called varargs (variable arguments) which was introduced as part of Java 5.
The function having ... in the above example indicates that it can receive multiple arguments of the datatype String.
For example, the fooBarMethod can be called in multiple ways and we can still have one method to process the data as shown below:

```java
class FooBar {
    public void fooBarMethod(String... variables){
        System.out.println("fooBarMethod");
    }
}

class Main {
    public void myMethod(String... variables){
        for(String variable : variables){
            FooBar NewFooBar = new FooBar();
            NewFooBar.fooBarMethod("foo", "bar");
            NewFooBar.fooBarMethod("foo", "bar", "boo");
            NewFooBar.fooBarMethod(new String[]{"foo", "var", "boo"});
        }
    }
}
```

More explanation:

__1. Variable Arguments (Varargs):__

The ... notation allows you to pass a variable number of arguments of the same type to a method. This provides flexibility and convenience when you need to handle methods with a varying number of arguments.

```java
public void printNumbers(int... numbers) {
    for (int num : numbers) {
        System.out.println(num);
    }
}

// Usage
// printNumbers(1, 2, 3); // Prints: 1 2 3
// printNumbers(10, 20); // Prints: 10 20
// printNumbers(); // No arguments, prints nothing
```

__2. Array Initialization:__

The ... notation can also be used during array initialization to create an array with an unspecified number of elements.

```
int[] numbers = {1, 2, 3, ...};
```

----

## **What will be the output of the below java program and define the steps of Execution of the java program with the help of the below code?**

```java
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

// Output:
// Static Block 1. Value of j = 0
// Static method. 
// Static Block 2. Value of j = 10
// Instance Block 1. Value of i = 0
// Instance Block 2. Value of i = 5
// Instance method. 
```

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

## **Define System.out.println()?**

System.out.println() is used to print the message on the console.

System - It is a class present in java.lang package.

out - is the static variable of type PrintStream class present in the System class.

println() - is the method present in the PrintStream class.

So if we justify the statement, then we can say that if we want to print anything on the console then we need to call the println() method that was present in PrintStream class. And we can call this using the output object that is present in the System class.

----

## **Can you explain the Java thread lifecycle?**

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

## **What could be the tradeoff between the usage of an unordered array versus the usage of an ordered array?**

The main advantage of having an ordered array is the reduced search time complexity of O(log n) whereas the time complexity in an unordered array is O(n).
The main drawback of the ordered array is its increased insertion time which is O(n) due to the fact that its element has to reordered to maintain the order of array during every insertion whereas the time complexity in the unordered array is only O(1).
Considering the above 2 key points and depending on what kind of scenario a developer requires, the appropriate data structure can be used for implementation.

----

## **Is it possible to import the same class or package twice in Java and what happens to it during runtime?**

It is possible to import a class or package more than once, however, it is redundant because the JVM internally loads the package or class only once.

----

## **In case a package has subpackages, will it suffice to import only the main package? E.g. does importing of com.myMainPackage?* also import com.myMainPackage.mySubPackage?*?**

This is a big NO. We need to understand that the importing of the sub-packages of a package needs to be done explicitly. Importing the parent package only results in the import of the classes within it and not the contents of its child/sub-packages.

----

## **Will the finally block be executed if the code System.exit(0) is written at the end of try block?**

NO. The control of the program post System.exit(0) is immediately gone and the program gets terminated which is why the finally block never gets executed.

----

## **What do you understand by marker interfaces in Java?**

Marker interfaces, also known as tagging interfaces are those interfaces that have no methods and constants defined in them. They are there for helping the compiler and JVM to get run time-related information regarding the objects.

----

## **Explain the term "Double Brace Initialisation" in Java?**

This is a convenient means of initializing any collections in Java. Consider the below example.

```java
import java.util.HashSet;
import java.util.Set;

class Main {
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

// Output:
// [set3, set2, set1]
```

In the above example, we see that the stringSets were initialized by using double braces.

The first brace does the task of creating an anonymous inner class that has the capability of accessing the parent class’s behavior. In our example, we are creating the subclass of HashSet so that it can use the add() method of HashSet.
The second braces do the task of initializing the instances.
Care should be taken while initializing through this method as the method involves the creation of anonymous inner classes which can cause problems during the garbage collection or serialization processes and may also result in memory leaks.

----

## **Why is it said that the length() method of String class doesn't return accurate results?**

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

## **What is the output of the below code and why?**

```java
public class Main{
    public static void main(String[] args)
    {
        System.out.println('b' + 'i' + 't');
    }
}

// Output:
// 319
```

“bit” would have been the result printed if the letters were used in double-quotes (or the string literals). But the question has the character literals (single quotes) being used which is why concatenation wouldn't occur. The corresponding ASCII values of each character would be added and the result of that sum would be printed.
The ASCII values of ‘b’, ‘i’, ‘t’ are:

```java
'b' = 98
'i' = 105
't' = 116
98 + 105 + 116 = 319

// Output:
// 319
```

----

## **What are the possible ways of making object eligible for garbage collection (GC) in Java?**

__First Approach: Set the object references to null once the object creation purpose is served.__

```java
public class Main {
    public static void main (String [] args){
        String s1 = "Some String";
        // s1 referencing String object - not yet eligible for GC
        s1 = null; // now s1 is eligible for GC
    }
}
```

__Second Approach: Point the reference variable to another object. Doing this, the object which the reference variable was referencing before becomes eligible for GC.__

```java
public class Main {
    public static void main(String [] args){
        String s1 = "To Garbage Collect";
        String s2 = "Another Object";
        System.out.println(s1); // s1 is not yet eligible for GC
        s1 = s2; // Point s1 to other object pointed by s2
        /* Here, the string object having the content  "To Garbage Collect" is not referred by any reference variable. Therefore, it is eligible for GC */
    }
}
```

__Third Approach: Island of Isolation Approach: When 2 reference variables pointing to instances of the same class, and these variables refer to only each other and the objects pointed by these 2 variables don't have any other references, then it is said to have formed an “Island of Isolation” and these 2 objects are eligible for GC.__

```java
public class IBGarbageCollect {
   IBGarbageCollect ib;    
   public static void main(String [] str) {
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
```

----

## **In the below Java Program, how many objects are eligible for garbage collection?**

```java
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
```

In the above program, a total of 7 objects will be eligible for garbage collection. Let’s visually understand what's happening in the code.

In the above figure on line 3, we can see that on each array index we are declaring a new array so the reference will be of that new array on all the 3 indexes. So the old array will be pointed to by none. So these three are eligible for garbage collection. And on line 4, we are creating a new array object on the older reference. So that will point to a new array and older multidimensional objects will become eligible for garbage collection.

----

## **What is the best way to inject dependency? Also, state the reason?**

There is no boundation for using a particular dependency injection. But the recommended approach is - 

Setters are mostly recommended for optional dependencies injection, and constructor arguments are recommended for mandatory ones. This is because constructor injection enables the injection of values into immutable fields and enables reading them more easily.

```java
public class UserService {
    private UserRepository userRepository;

    public UserService(UserRepository userRepository) {
        this.userRepository = userRepository;
    }

    // Rest of the UserService implementation
}
```

In the above example, the UserService class has a dependency on the UserRepository class, which is passed through the constructor. The dependency is explicitly declared, and the class relies on the caller to provide an instance of UserRepository during object creation.

By using constructor injection, you can achieve better decoupling, testability, and maintainability in your code. Other forms of dependency injection, such as setter injection or field injection, have their use cases but can introduce more ambiguity and potential issues compared to constructor injection.

----

## **How we can set the spring bean scope. And what supported scopes does it have?**

A scope can be set by an annotation such as the @Scope annotation or the "scope" attribute in an XML configuration file.

Spring Bean supports the following five scopes:
- Singleton
- Prototype
- Request
- Session
- Global-session

----

## **What are the different categories of Java Design patterns?**

Java Design patterns are categorized into the following different types. And those are also further categorized as 

Structural patterns:

- Adapter

```java
// Adaptee class with incompatible interface
class LegacyRectangle {
    public void display(int x1, int y1, int x2, int y2) {
        System.out.println("LegacyRectangle: display(x1=" + x1 + ", y1=" + y1 + ", x2=" + x2 + ", y2=" + y2 + ")");
    }
}

// Target interface
interface Shape {
    void draw(int x1, int y1, int x2, int y2);
}

// Adapter class
class RectangleAdapter implements Shape {
    private LegacyRectangle legacyRectangle;

    public RectangleAdapter(LegacyRectangle legacyRectangle) {
        this.legacyRectangle = legacyRectangle;
    }

    @Override
    public void draw(int x1, int y1, int x2, int y2) {
        legacyRectangle.display(x1, y1, x2, y2);
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create the LegacyRectangle object
        LegacyRectangle legacyRectangle = new LegacyRectangle();

        // Create the RectangleAdapter object and pass the LegacyRectangle to it
        RectangleAdapter adapter = new RectangleAdapter(legacyRectangle);

        // Use the adapter to call the draw method
        adapter.draw(10, 20, 30, 40);
    }
}
```

- Bridge

```java
// Abstraction
abstract class Shape {
    protected Color color;

    public Shape(Color color) {
        this.color = color;
    }

    public abstract void draw();
}

// Concrete Abstraction
class Circle extends Shape {
    private int radius;

    public Circle(int radius, Color color) {
        super(color);
        this.radius = radius;
    }

    @Override
    public void draw() {
        System.out.println("Drawing Circle with radius " + radius);
        color.applyColor();
    }
}

class Square extends Shape {
    private int sideLength;

    public Square(int sideLength, Color color) {
        super(color);
        this.sideLength = sideLength;
    }

    @Override
    public void draw() {
        System.out.println("Drawing Square with side length " + sideLength);
        color.applyColor();
    }
}

// Implementor
interface Color {
    void applyColor();
}

// Concrete Implementors
class RedColor implements Color {
    @Override
    public void applyColor() {
        System.out.println("Applying red color");
    }
}

class BlueColor implements Color {
    @Override
    public void applyColor() {
        System.out.println("Applying blue color");
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        Shape circle = new Circle(5, new RedColor());
        circle.draw();

        Shape square = new Square(10, new BlueColor());
        square.draw();
    }
}
```

- Filter

```java
import java.util.ArrayList;
import java.util.List;

// Product class
class Product {
    private String name;
    private String category;
    private double price;

    public Product(String name, String category, double price) {
        this.name = name;
        this.category = category;
        this.price = price;
    }

    public String getName() {
        return name;
    }

    public String getCategory() {
        return category;
    }

    public double getPrice() {
        return price;
    }
}

// Filter interface
interface Filter {
    List<Product> filter(List<Product> products);
}

// Concrete filters
class CategoryFilter implements Filter {
    private String category;

    public CategoryFilter(String category) {
        this.category = category;
    }

    @Override
    public List<Product> filter(List<Product> products) {
        List<Product> filteredProducts = new ArrayList<>();
        for (Product product : products) {
            if (product.getCategory().equalsIgnoreCase(category)) {
                filteredProducts.add(product);
            }
        }
        return filteredProducts;
    }
}

class PriceFilter implements Filter {
    private double minPrice;
    private double maxPrice;

    public PriceFilter(double minPrice, double maxPrice) {
        this.minPrice = minPrice;
        this.maxPrice = maxPrice;
    }

    @Override
    public List<Product> filter(List<Product> products) {
        List<Product> filteredProducts = new ArrayList<>();
        for (Product product : products) {
            if (product.getPrice() >= minPrice && product.getPrice() <= maxPrice) {
                filteredProducts.add(product);
            }
        }
        return filteredProducts;
    }
}

// Product catalog
class ProductCatalog {
    private List<Product> products;

    public ProductCatalog(List<Product> products) {
        this.products = products;
    }

    public List<Product> filterProducts(Filter filter) {
        return filter.filter(products);
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create a list of products
        List<Product> products = new ArrayList<>();
        products.add(new Product("iPhone", "Electronics", 1000.0));
        products.add(new Product("Shirt", "Clothing", 25.0));
        products.add(new Product("TV", "Electronics", 800.0));
        products.add(new Product("Jeans", "Clothing", 50.0));

        // Create a product catalog
        ProductCatalog catalog = new ProductCatalog(products);

        // Apply filters
        Filter categoryFilter = new CategoryFilter("Electronics");
        List<Product> electronicsProducts = catalog.filterProducts(categoryFilter);
        System.out.println("Electronics products:");
        for (Product product : electronicsProducts) {
            System.out.println(product.getName());
        }

        Filter priceFilter = new PriceFilter(30.0, 1000.0);
        List<Product> affordableProducts = catalog.filterProducts(priceFilter);
        System.out.println("Affordable products:");
        for (Product product : affordableProducts) {
            System.out.println(product.getName());
        }
    }
}
```

- Composite

```java
import java.util.ArrayList;
import java.util.List;

// Component interface
interface Component {
    void render();
}

// Leaf class
class Leaf implements Component {
    private String name;

    public Leaf(String name) {
        this.name = name;
    }

    @Override
    public void render() {
        System.out.println("Rendering Leaf: " + name);
    }
}

// Composite class
class Composite implements Component {
    private String name;
    private List<Component> children;

    public Composite(String name) {
        this.name = name;
        this.children = new ArrayList<>();
    }

    public void add(Component component) {
        children.add(component);
    }

    public void remove(Component component) {
        children.remove(component);
    }

    @Override
    public void render() {
        System.out.println("Rendering Composite: " + name);
        for (Component component : children) {
            component.render();
        }
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create leaf components
        Component leaf1 = new Leaf("Leaf 1");
        Component leaf2 = new Leaf("Leaf 2");
        Component leaf3 = new Leaf("Leaf 3");

        // Create composite components
        Composite composite1 = new Composite("Composite 1");
        Composite composite2 = new Composite("Composite 2");

        // Add leaf components to composite1
        composite1.add(leaf1);
        composite1.add(leaf2);

        // Add leaf and composite components to composite2
        composite2.add(leaf3);
        composite2.add(composite1);

        // Render the composite components
        composite2.render();
    }
}
```

- Decorator

```java
// Component interface
interface Pizza {
    String getDescription();
    double getCost();
}

// Concrete component
class PlainPizza implements Pizza {
    @Override
    public String getDescription() {
        return "Plain pizza";
    }

    @Override
    public double getCost() {
        return 5.0;
    }
}

// Decorator abstract class
abstract class PizzaDecorator implements Pizza {
    protected Pizza pizza;

    public PizzaDecorator(Pizza pizza) {
        this.pizza = pizza;
    }

    @Override
    public String getDescription() {
        return pizza.getDescription();
    }

    @Override
    public double getCost() {
        return pizza.getCost();
    }
}

// Concrete decorator classes
class CheeseDecorator extends PizzaDecorator {
    public CheeseDecorator(Pizza pizza) {
        super(pizza);
    }

    @Override
    public String getDescription() {
        return super.getDescription() + ", Cheese";
    }

    @Override
    public double getCost() {
        return super.getCost() + 2.0;
    }
}

class TomatoDecorator extends PizzaDecorator {
    public TomatoDecorator(Pizza pizza) {
        super(pizza);
    }

    @Override
    public String getDescription() {
        return super.getDescription() + ", Tomato";
    }

    @Override
    public double getCost() {
        return super.getCost() + 1.5;
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create a plain pizza
        Pizza pizza = new PlainPizza();
        System.out.println("Plain Pizza:");
        System.out.println("Description: " + pizza.getDescription());
        System.out.println("Cost: $" + pizza.getCost());

        // Decorate the plain pizza with cheese
        pizza = new CheeseDecorator(pizza);
        System.out.println("\nCheese Decorated Pizza:");
        System.out.println("Description: " + pizza.getDescription());
        System.out.println("Cost: $" + pizza.getCost());

        // Decorate the cheese pizza with tomato
        pizza = new TomatoDecorator(pizza);
        System.out.println("\nTomato Decorated Pizza:");
        System.out.println("Description: " + pizza.getDescription());
        System.out.println("Cost: $" + pizza.getCost());
    }
}
```

- Facade

```java
// Complex subsystem classes
class OrderValidation {
    public boolean validateOrder(int orderId) {
        // Perform order validation logic
        System.out.println("Validating order: " + orderId);
        return true;
    }
}

class PaymentProcessing {
    public void processPayment(int orderId) {
        // Perform payment processing logic
        System.out.println("Processing payment for order: " + orderId);
    }
}

class InventoryManagement {
    public void updateInventory(int orderId) {
        // Perform inventory update logic
        System.out.println("Updating inventory for order: " + orderId);
    }
}

// Facade class
class OrderProcessingFacade {
    private OrderValidation orderValidation;
    private PaymentProcessing paymentProcessing;
    private InventoryManagement inventoryManagement;

    public OrderProcessingFacade() {
        this.orderValidation = new OrderValidation();
        this.paymentProcessing = new PaymentProcessing();
        this.inventoryManagement = new InventoryManagement();
    }

    public void processOrder(int orderId) {
        boolean isOrderValid = orderValidation.validateOrder(orderId);
        if (isOrderValid) {
            paymentProcessing.processPayment(orderId);
            inventoryManagement.updateInventory(orderId);
            System.out.println("Order processed successfully.");
        } else {
            System.out.println("Order validation failed. Unable to process order.");
        }
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        OrderProcessingFacade facade = new OrderProcessingFacade();
        int orderId = 12345;
        facade.processOrder(orderId);
    }
}
```

- Flyweight

```java
import java.util.HashMap;
import java.util.Map;

// Flyweight interface
interface Shape {
    void draw();
}

// Concrete flyweight class
class Circle implements Shape {
    private String color;
    private int x;
    private int y;
    private int radius;

    public Circle(String color) {
        this.color = color;
    }

    public void setX(int x) {
        this.x = x;
    }

    public void setY(int y) {
        this.y = y;
    }

    public void setRadius(int radius) {
        this.radius = radius;
    }

    @Override
    public void draw() {
        System.out.println("Drawing a circle with color: " + color +
                ", x: " + x + ", y: " + y + ", radius: " + radius);
    }
}

// Flyweight factory class
class ShapeFactory {
    private static final Map<String, Shape> circleMap = new HashMap<>();

    public static Shape getCircle(String color) {
        Shape circle = circleMap.get(color);

        if (circle == null) {
            circle = new Circle(color);
            circleMap.put(color, circle);
            System.out.println("Creating a new circle of color: " + color);
        }

        return circle;
    }
}

// Client code
public class Main {
    private static final String[] colors = {"Red", "Blue", "Green", "Yellow", "Black"};

    public static void main(String[] args) {
        for (int i = 0; i < 10; i++) {
            Circle circle = (Circle) ShapeFactory.getCircle(getRandomColor());
            circle.setX(getRandomX());
            circle.setY(getRandomY());
            circle.setRadius(10);
            circle.draw();
        }
    }

    private static String getRandomColor() {
        return colors[(int) (Math.random() * colors.length)];
    }

    private static int getRandomX() {
        return (int) (Math.random() * 100);
    }

    private static int getRandomY() {
        return (int) (Math.random() * 100);
    }
}
```

- Proxy

```java
// Subject interface
interface Image {
    void display();
}

// RealSubject class
class RealImage implements Image {
    private String filename;

    public RealImage(String filename) {
        this.filename = filename;
        loadFromDisk();
    }

    private void loadFromDisk() {
        System.out.println("Loading image: " + filename);
    }

    @Override
    public void display() {
        System.out.println("Displaying image: " + filename);
    }
}

// Proxy class
class ImageProxy implements Image {
    private String filename;
    private RealImage realImage;

    public ImageProxy(String filename) {
        this.filename = filename;
    }

    @Override
    public void display() {
        if (realImage == null) {
            realImage = new RealImage(filename);
        }
        realImage.display();
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        Image image1 = new ImageProxy("image1.jpg");
        Image image2 = new ImageProxy("image2.jpg");

        // Image1 is loaded and displayed
        image1.display();

        // Image2 is only loaded when displayed
        image2.display();
    }
}
```

Behavioral patterns:

- Interpreter

```java
// Abstract Expression
interface Expression {
    boolean interpret(String context);
}

// Terminal Expression
class TerminalExpression implements Expression {
    private String data;

    public TerminalExpression(String data) {
        this.data = data;
    }

    @Override
    public boolean interpret(String context) {
        return context.contains(data);
    }
}

// Non-Terminal Expression
class AndExpression implements Expression {
    private Expression expression1;
    private Expression expression2;

    public AndExpression(Expression expression1, Expression expression2) {
        this.expression1 = expression1;
        this.expression2 = expression2;
    }

    @Override
    public boolean interpret(String context) {
        return expression1.interpret(context) && expression2.interpret(context);
    }
}

// Non-Terminal Expression
class OrExpression implements Expression {
    private Expression expression1;
    private Expression expression2;

    public OrExpression(Expression expression1, Expression expression2) {
        this.expression1 = expression1;
        this.expression2 = expression2;
    }

    @Override
    public boolean interpret(String context) {
        return expression1.interpret(context) || expression2.interpret(context);
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        Expression person1 = new TerminalExpression("John");
        Expression person2 = new TerminalExpression("Jane");

        // Rule: John and Jane are colleagues
        Expression isColleague = new AndExpression(person1, person2);

        // Rule: John or Jane is a manager
        Expression isManager = new OrExpression(person1, person2);

        String context1 = "John is a colleague";
        String context2 = "Jane is a manager";
        String context3 = "John and Jane are colleagues and managers";

        System.out.println(context1 + " - Colleague? " + isColleague.interpret(context1));
        System.out.println(context2 + " - Manager? " + isManager.interpret(context2));
        System.out.println(context3 + " - Colleague or Manager? " + isColleague.interpret(context3)
                + " or " + isManager.interpret(context3));
    }
}
```

- Template method/pattern

```java
// Abstract class defining the template method
abstract class AbstractClass {
    // Template method
    public void templateMethod() {
        step1();
        step2();
        step3();
    }

    // Concrete implementation of step 1
    public void step1() {
        System.out.println("AbstractClass: Step 1");
    }

    // Abstract methods to be implemented by subclasses
    public abstract void step2();

    public abstract void step3();
}

// Concrete class implementing the template method
class ConcreteClass extends AbstractClass {
    @Override
    public void step2() {
        System.out.println("ConcreteClass: Step 2");
    }

    @Override
    public void step3() {
        System.out.println("ConcreteClass: Step 3");
    }
}

// Another concrete class implementing the template method
class AnotherConcreteClass extends AbstractClass {
    @Override
    public void step2() {
        System.out.println("AnotherConcreteClass: Step 2");
    }

    @Override
    public void step3() {
        System.out.println("AnotherConcreteClass: Step 3");
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        AbstractClass abstractClass = new ConcreteClass();
        abstractClass.templateMethod();

        System.out.println();

        abstractClass = new AnotherConcreteClass();
        abstractClass.templateMethod();
    }
}
```

- Chain of responsibility

```java
// Request class
class Request {
    private String type;
    private String content;

    public Request(String type, String content) {
        this.type = type;
        this.content = content;
    }

    public String getType() {
        return type;
    }

    public String getContent() {
        return content;
    }
}

// Handler interface
interface Handler {
    void setNextHandler(Handler handler);

    void handleRequest(Request request);
}

// Concrete handler
class ConcreteHandler implements Handler {
    private Handler nextHandler;

    @Override
    public void setNextHandler(Handler handler) {
        nextHandler = handler;
    }

    @Override
    public void handleRequest(Request request) {
        if (request.getType().equals("Type1")) {
            System.out.println("ConcreteHandler: Handling Type1 request");
            // Handle the request
        } else if (nextHandler != null) {
            nextHandler.handleRequest(request);
        } else {
            System.out.println("ConcreteHandler: Unable to handle the request");
        }
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        Handler handler1 = new ConcreteHandler();
        Handler handler2 = new ConcreteHandler();

        handler1.setNextHandler(handler2);

        // Create a request
        Request request = new Request("Type1", "Request content");

        // Send the request to the first handler
        handler1.handleRequest(request);
    }
}
```

- Command pattern

```java
// Command interface
interface Command {
    void execute();
}

// Receiver class
class Light {
    public void turnOn() {
        System.out.println("Light is on");
    }

    public void turnOff() {
        System.out.println("Light is off");
    }
}

// Concrete commands
class TurnOnCommand implements Command {
    private Light light;

    public TurnOnCommand(Light light) {
        this.light = light;
    }

    @Override
    public void execute() {
        light.turnOn();
    }
}

class TurnOffCommand implements Command {
    private Light light;

    public TurnOffCommand(Light light) {
        this.light = light;
    }

    @Override
    public void execute() {
        light.turnOff();
    }
}

// Invoker class
class RemoteControl {
    private Command command;

    public void setCommand(Command command) {
        this.command = command;
    }

    public void pressButton() {
        command.execute();
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create the receiver
        Light light = new Light();

        // Create the commands
        Command turnOnCommand = new TurnOnCommand(light);
        Command turnOffCommand = new TurnOffCommand(light);

        // Create the invoker
        RemoteControl remoteControl = new RemoteControl();

        // Set the commands for the invoker
        remoteControl.setCommand(turnOnCommand);
        remoteControl.pressButton();

        remoteControl.setCommand(turnOffCommand);
        remoteControl.pressButton();
    }
}
```

- Iterator pattern

```java
import java.util.ArrayList;
import java.util.Iterator;
import java.util.List;

// Aggregate interface
interface Aggregate {
    Iterator<String> createIterator();
}

// Concrete Aggregate class
class ConcreteAggregate implements Aggregate {
    private List<String> items;

    public ConcreteAggregate() {
        items = new ArrayList<>();
    }

    public void addItem(String item) {
        items.add(item);
    }

    @Override
    public Iterator<String> createIterator() {
        return new ConcreteIterator(items);
    }
}

// Iterator interface
interface Iterator<T> {
    boolean hasNext();

    T next();
}

// Concrete Iterator class
class ConcreteIterator implements Iterator<String> {
    private List<String> items;
    private int position;

    public ConcreteIterator(List<String> items) {
        this.items = items;
        position = 0;
    }

    @Override
    public boolean hasNext() {
        return position < items.size();
    }

    @Override
    public String next() {
        return items.get(position++);
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        Aggregate aggregate = new ConcreteAggregate();
        aggregate.addItem("Item 1");
        aggregate.addItem("Item 2");
        aggregate.addItem("Item 3");

        Iterator<String> iterator = aggregate.createIterator();
        while (iterator.hasNext()) {
            String item = iterator.next();
            System.out.println(item);
        }
    }
}
```

- Strategy pattern

```java
// Strategy interface
interface PaymentStrategy {
    void pay(int amount);
}

// Concrete strategies
class CreditCardPaymentStrategy implements PaymentStrategy {
    private String cardNumber;
    private String expirationDate;
    private String cvv;

    public CreditCardPaymentStrategy(String cardNumber, String expirationDate, String cvv) {
        this.cardNumber = cardNumber;
        this.expirationDate = expirationDate;
        this.cvv = cvv;
    }

    @Override
    public void pay(int amount) {
        System.out.println("Paid $" + amount + " using Credit Card");
        // Additional logic for credit card payment
    }
}

class PayPalPaymentStrategy implements PaymentStrategy {
    private String email;
    private String password;

    public PayPalPaymentStrategy(String email, String password) {
        this.email = email;
        this.password = password;
    }

    @Override
    public void pay(int amount) {
        System.out.println("Paid $" + amount + " using PayPal");
        // Additional logic for PayPal payment
    }
}

// Context class
class ShoppingCart {
    private PaymentStrategy paymentStrategy;

    public void setPaymentStrategy(PaymentStrategy paymentStrategy) {
        this.paymentStrategy = paymentStrategy;
    }

    public void checkout(int amount) {
        paymentStrategy.pay(amount);
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        ShoppingCart cart = new ShoppingCart();

        // Set payment strategy to credit card
        PaymentStrategy creditCardStrategy = new CreditCardPaymentStrategy("1234567890123456", "12/2025", "123");
        cart.setPaymentStrategy(creditCardStrategy);
        cart.checkout(100);

        System.out.println();

        // Set payment strategy to PayPal
        PaymentStrategy payPalStrategy = new PayPalPaymentStrategy("example@example.com", "password");
        cart.setPaymentStrategy(payPalStrategy);
        cart.checkout(200);
    }
}
```

- Visitor pattern

```java
// Element interface
interface Element {
    void accept(Visitor visitor);
}

// Concrete Element classes
class ConcreteElementA implements Element {
    @Override
    public void accept(Visitor visitor) {
        visitor.visit(this);
    }

    public String operationA() {
        return "ConcreteElementA operation";
    }
}

class ConcreteElementB implements Element {
    @Override
    public void accept(Visitor visitor) {
        visitor.visit(this);
    }

    public String operationB() {
        return "ConcreteElementB operation";
    }
}

// Visitor interface
interface Visitor {
    void visit(ConcreteElementA elementA);

    void visit(ConcreteElementB elementB);
}

// Concrete Visitor class
class ConcreteVisitor implements Visitor {
    @Override
    public void visit(ConcreteElementA elementA) {
        System.out.println("Visitor is visiting " + elementA.operationA());
    }

    @Override
    public void visit(ConcreteElementB elementB) {
        System.out.println("Visitor is visiting " + elementB.operationB());
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        Element[] elements = { new ConcreteElementA(), new ConcreteElementB() };

        Visitor visitor = new ConcreteVisitor();

        for (Element element : elements) {
            element.accept(visitor);
        }
    }
}
```

J2EE patterns:

- MVC Pattern

```java
// Model
class User {
    private String name;
    private String email;

    public User(String name, String email) {
        this.name = name;
        this.email = email;
    }

    public String getName() {
        return name;
    }

    public String getEmail() {
        return email;
    }
}

// View
class UserView {
    public void displayUserDetails(String name, String email) {
        System.out.println("User Details:");
        System.out.println("Name: " + name);
        System.out.println("Email: " + email);
    }
}

// Controller
class UserController {
    private User model;
    private UserView view;

    public UserController(User model, UserView view) {
        this.model = model;
        this.view = view;
    }

    public void updateView() {
        view.displayUserDetails(model.getName(), model.getEmail());
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create the model
        User user = new User("John Doe", "johndoe@example.com");

        // Create the view
        UserView userView = new UserView();

        // Create the controller
        UserController userController = new UserController(user, userView);

        // Update and display the view
        userController.updateView();
    }
}
```

- Data Access Object pattern

```java
// Model
class User {
    private String username;
    private String password;

    public User(String username, String password) {
        this.username = username;
        this.password = password;
    }

    public String getUsername() {
        return username;
    }

    public String getPassword() {
        return password;
    }
}

// Data Access Object (DAO) interface
interface UserDao {
    void addUser(User user);
    User getUser(String username);
    void updateUser(User user);
    void deleteUser(User user);
}

// Concrete DAO implementation
class UserDaoImpl implements UserDao {
    private List<User> userList;

    public UserDaoImpl() {
        userList = new ArrayList<>();
    }

    @Override
    public void addUser(User user) {
        userList.add(user);
        System.out.println("User added successfully");
    }

    @Override
    public User getUser(String username) {
        for (User user : userList) {
            if (user.getUsername().equals(username)) {
                return user;
            }
        }
        return null;
    }

    @Override
    public void updateUser(User user) {
        for (User existingUser : userList) {
            if (existingUser.getUsername().equals(user.getUsername())) {
                existingUser.setPassword(user.getPassword());
                System.out.println("User updated successfully");
                return;
            }
        }
        System.out.println("User not found");
    }

    @Override
    public void deleteUser(User user) {
        userList.remove(user);
        System.out.println("User deleted successfully");
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        UserDao userDao = new UserDaoImpl();

        // Add a new user
        User user1 = new User("john", "password123");
        userDao.addUser(user1);

        // Get a user by username
        User fetchedUser = userDao.getUser("john");
        System.out.println("Fetched User: " + fetchedUser.getUsername() + ", " + fetchedUser.getPassword());

        // Update user password
        User updatedUser = new User("john", "newpassword");
        userDao.updateUser(updatedUser);

        // Delete user
        userDao.deleteUser(updatedUser);
    }
}
```

- Front controller pattern

```java
// Front Controller
class FrontController {
    private Dispatcher dispatcher;

    public FrontController() {
        dispatcher = new Dispatcher();
    }

    private boolean isAuthenticUser() {
        // Check if the user is authenticated
        // In a real application, you would implement proper authentication logic here
        System.out.println("User is authenticated.");
        return true;
    }

    private void trackRequest(String request) {
        // Log the user's request
        System.out.println("Tracking request: " + request);
    }

    public void dispatchRequest(String request) {
        // Log and track the request
        trackRequest(request);

        // Check if the user is authenticated
        if (isAuthenticUser()) {
            // Dispatch the request to the appropriate handler
            dispatcher.dispatch(request);
        }
    }
}

// Dispatcher
class Dispatcher {
    private HomeView homeView;
    private AboutView aboutView;

    public Dispatcher() {
        homeView = new HomeView();
        aboutView = new AboutView();
    }

    public void dispatch(String request) {
        if (request.equalsIgnoreCase("HOME")) {
            homeView.show();
        } else if (request.equalsIgnoreCase("ABOUT")) {
            aboutView.show();
        } else {
            System.out.println("Invalid request.");
        }
    }
}

// Views
class HomeView {
    public void show() {
        System.out.println("Displaying Home Page");
    }
}

class AboutView {
    public void show() {
        System.out.println("Displaying About Page");
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create the front controller
        FrontController frontController = new FrontController();

        // Simulate user requests
        frontController.dispatchRequest("HOME");
        frontController.dispatchRequest("ABOUT");
        frontController.dispatchRequest("CONTACT");
    }
}
```

- Intercepting filter pattern

```java
// Filter interface
interface Filter {
    void execute(String request);
}

// Concrete filters
class AuthenticationFilter implements Filter {
    @Override
    public void execute(String request) {
        System.out.println("Authenticating request: " + request);
    }
}

class LoggingFilter implements Filter {
    @Override
    public void execute(String request) {
        System.out.println("Logging request: " + request);
    }
}

class RateLimitFilter implements Filter {
    @Override
    public void execute(String request) {
        System.out.println("Applying rate limit to request: " + request);
    }
}

// Target
class Target {
    public void execute(String request) {
        System.out.println("Executing request: " + request);
    }
}

// Filter chain
class FilterChain {
    private List<Filter> filters = new ArrayList<>();
    private Target target;

    public void addFilter(Filter filter) {
        filters.add(filter);
    }

    public void setTarget(Target target) {
        this.target = target;
    }

    public void execute(String request) {
        for (Filter filter : filters) {
            filter.execute(request);
        }
        target.execute(request);
    }
}

// Filter manager
class FilterManager {
    private FilterChain filterChain;

    public FilterManager(Target target) {
        filterChain = new FilterChain();
        filterChain.setTarget(target);
    }

    public void addFilter(Filter filter) {
        filterChain.addFilter(filter);
    }

    public void filterRequest(String request) {
        filterChain.execute(request);
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create the target
        Target target = new Target();

        // Create the filter manager
        FilterManager filterManager = new FilterManager(target);

        // Add filters to the filter manager
        filterManager.addFilter(new AuthenticationFilter());
        filterManager.addFilter(new LoggingFilter());
        filterManager.addFilter(new RateLimitFilter());

        // Execute the request through the filter manager
        filterManager.filterRequest("GET /api/data");
    }
}
```

- Transfer object pattern

```java
// Transfer Object
class UserTO {
    private String username;
    private String email;

    public UserTO(String username, String email) {
        this.username = username;
        this.email = email;
    }

    public String getUsername() {
        return username;
    }

    public String getEmail() {
        return email;
    }
}

// Business Service
class UserService {
    public UserTO getUserById(int userId) {
        // Simulate fetching user data from a database
        // Here, we create a dummy user for demonstration purposes
        String username = "John Doe";
        String email = "john.doe@example.com";

        // Create and return the transfer object
        return new UserTO(username, email);
    }

    public void updateUser(UserTO user) {
        // Simulate updating user data in a database
        System.out.println("Updating user: " + user.getUsername());
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create an instance of the business service
        UserService userService = new UserService();

        // Retrieve user data using the transfer object
        UserTO user = userService.getUserById(123);

        // Modify the user data
        user.setEmail("new-email@example.com");

        // Update the user data using the transfer object
        userService.updateUser(user);
    }
}
```

Creational patterns:

- Factory method/Template

```java
// Product interface
interface Product {
    void operation();
}

// Concrete products
class ConcreteProductA implements Product {
    @Override
    public void operation() {
        System.out.println("Operation in Product A");
    }
}

class ConcreteProductB implements Product {
    @Override
    public void operation() {
        System.out.println("Operation in Product B");
    }
}

// Creator interface
interface Creator {
    Product createProduct();
}

// Concrete creators
class ConcreteCreatorA implements Creator {
    @Override
    public Product createProduct() {
        return new ConcreteProductA();
    }
}

class ConcreteCreatorB implements Creator {
    @Override
    public Product createProduct() {
        return new ConcreteProductB();
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create a concrete creator
        Creator creatorA = new ConcreteCreatorA();

        // Use the creator to create a product
        Product productA = creatorA.createProduct();
        productA.operation();

        // Create a different concrete creator
        Creator creatorB = new ConcreteCreatorB();

        // Use the different creator to create a different product
        Product productB = creatorB.createProduct();
        productB.operation();
    }
}
```

- Abstract Factory

```java
// Abstract Product A
interface ProductA {
    void operationA();
}

// Concrete Product A1
class ConcreteProductA1 implements ProductA {
    @Override
    public void operationA() {
        System.out.println("Operation A in Product A1");
    }
}

// Concrete Product A2
class ConcreteProductA2 implements ProductA {
    @Override
    public void operationA() {
        System.out.println("Operation A in Product A2");
    }
}

// Abstract Product B
interface ProductB {
    void operationB();
}

// Concrete Product B1
class ConcreteProductB1 implements ProductB {
    @Override
    public void operationB() {
        System.out.println("Operation B in Product B1");
    }
}

// Concrete Product B2
class ConcreteProductB2 implements ProductB {
    @Override
    public void operationB() {
        System.out.println("Operation B in Product B2");
    }
}

// Abstract Factory
interface AbstractFactory {
    ProductA createProductA();
    ProductB createProductB();
}

// Concrete Factory 1
class ConcreteFactory1 implements AbstractFactory {
    @Override
    public ProductA createProductA() {
        return new ConcreteProductA1();
    }

    @Override
    public ProductB createProductB() {
        return new ConcreteProductB1();
    }
}

// Concrete Factory 2
class ConcreteFactory2 implements AbstractFactory {
    @Override
    public ProductA createProductA() {
        return new ConcreteProductA2();
    }

    @Override
    public ProductB createProductB() {
        return new ConcreteProductB2();
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create a concrete factory
        AbstractFactory factory1 = new ConcreteFactory1();

        // Use the factory to create products
        ProductA productA1 = factory1.createProductA();
        productA1.operationA();

        ProductB productB1 = factory1.createProductB();
        productB1.operationB();

        // Create a different concrete factory
        AbstractFactory factory2 = new ConcreteFactory2();

        // Use the different factory to create different products
        ProductA productA2 = factory2.createProductA();
        productA2.operationA();

        ProductB productB2 = factory2.createProductB();
        productB2.operationB();
    }
}
```

- Builder

```java
// Product class
class Product {
    private String property1;
    private String property2;
    private String property3;

    public void setProperty1(String property1) {
        this.property1 = property1;
    }

    public void setProperty2(String property2) {
        this.property2 = property2;
    }

    public void setProperty3(String property3) {
        this.property3 = property3;
    }

    public void display() {
        System.out.println("Property 1: " + property1);
        System.out.println("Property 2: " + property2);
        System.out.println("Property 3: " + property3);
    }
}

// Builder interface
interface Builder {
    void buildProperty1(String property1);
    void buildProperty2(String property2);
    void buildProperty3(String property3);
    Product getResult();
}

// Concrete builder
class ConcreteBuilder implements Builder {
    private Product product = new Product();

    @Override
    public void buildProperty1(String property1) {
        product.setProperty1(property1);
    }

    @Override
    public void buildProperty2(String property2) {
        product.setProperty2(property2);
    }

    @Override
    public void buildProperty3(String property3) {
        product.setProperty3(property3);
    }

    @Override
    public Product getResult() {
        return product;
    }
}

// Director class
class Director {
    public Product construct(Builder builder) {
        builder.buildProperty1("Value 1");
        builder.buildProperty2("Value 2");
        builder.buildProperty3("Value 3");
        return builder.getResult();
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        Director director = new Director();
        Builder builder = new ConcreteBuilder();

        Product product = director.construct(builder);
        product.display();
    }
}
```

- Prototype

```java
// Prototype interface
interface Prototype {
    Prototype clone();
}

// Concrete prototype
class ConcretePrototype implements Prototype {
    private String property;

    public ConcretePrototype(String property) {
        this.property = property;
    }

    public void setProperty(String property) {
        this.property = property;
    }

    public String getProperty() {
        return property;
    }

    @Override
    public Prototype clone() {
        return new ConcretePrototype(property);
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Create a prototype object
        ConcretePrototype prototype = new ConcretePrototype("Initial Property");

        // Clone the prototype
        ConcretePrototype clone = (ConcretePrototype) prototype.clone();

        // Modify the property of the clone
        clone.setProperty("Modified Property");

        // Output the properties of the prototype and clone
        System.out.println("Prototype Property: " + prototype.getProperty());
        System.out.println("Clone Property: " + clone.getProperty());
    }
}
```

- Singleton

```java
// Singleton class
class Singleton {
    private static Singleton instance;

    // Private constructor to prevent direct instantiation
    private Singleton() {
    }

    // Public method to access the singleton instance
    public static Singleton getInstance() {
        if (instance == null) {
            // Create a new instance if it doesn't exist
            instance = new Singleton();
        }
        return instance;
    }

    // Other methods of the singleton class
    public void showMessage() {
        System.out.println("Hello, I am a singleton object!");
    }
}

// Client code
public class Main {
    public static void main(String[] args) {
        // Get the singleton instance
        Singleton singleton = Singleton.getInstance();

        // Use the singleton object
        singleton.showMessage();
    }
}
```

----

## **What is a Memory Leak? Discuss some common causes of it?**

The Java Garbage Collector (GC) typically removes unused objects when they are no longer required, but when they are still referenced, the unused objects cannot be removed. So this causes the memory leak problem. Example - Consider a linked list like the structure below -

In the above image, there are unused objects that are not referenced. But then also Garbage collection will not free it. Because it is referencing some existing referenced object. So this can be the situation of memory leak.

Some common causes of Memory leaks are - 

When there are Unbounded caches.
Excessive page swapping is done by the operating system.
Improper written custom data structures.
Inserting into a collection object without first deleting it.
etc.

```java
public class GarbageCollectorExample {
    public static void main(String[] args) {
        // Create objects
        MyClass obj1 = new MyClass();
        MyClass obj2 = new MyClass();
        MyClass obj3 = new MyClass();

        // Set references to null
        obj1 = null;
        obj2 = null;

        // Trigger garbage collection
        System.gc();

        // Other program logic...
    }
}

class MyClass {
    // Constructor
    public MyClass() {
        System.out.println("Creating object: " + this);
    }

    // Finalizer
    @Override
    protected void finalize() throws Throwable {
        System.out.println("Finalizing object: " + this);
        super.finalize();
    }
}
```

----

## **Assume a thread has a lock on it, calling the sleep() method on that thread will release the lock?**

A thread that has a lock won't be released even after it calls sleep(). Despite the thread sleeping for a specified period of time, the lock will not be released.

----

## **Check if a given string is palindrome using recursion?**

```java
/*
* Java program to check if a given inputted string is palindrome or not using recursion.
*/
import java.util?*;
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
```

----

## **Write a Java Program to print Fibonacci Series using Recursion?**

```java
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
```

In the above code, we are printing the base 2 Fibonacci values 0 and 1. And then based on the length of Fibonacci to be printed, we are using the helper function to print that.

----

## **Write a Java program to check if the two strings are anagrams?**

The main idea is to validate the length of strings and then if found equal, convert the string to char array and then sort the arrays and check if both are equal.

```java
import java.util.Arrays;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);

        //Input from two strings
        System.out.print("First String: ");
        String string1 = s.nextLine();
        System.out.print("Second String: ");
        String string2 = s.nextLine();

        // check for the length
        if (string1.length() == string2.length()) {
            // convert strings to char array
            char[] characterArray1 = string1.toCharArray();
            char[] characterArray2 = string2.toCharArray();
            // sort the arrays
            Arrays.sort(characterArray1);
            Arrays.sort(characterArray2);
            // check for equality, if found equal then anagram, else not an anagram
            boolean isAnagram = Arrays.equals(characterArray1, characterArray2);
            System.out.println("Anagram: " + isAnagram);
        }
    }
}
```

----

## **Write a Java Program to find the factorial of a given number?**

```java
class FindFactorial {
    public void findFactorial() {
        int num = 10;
        long factorialResult = 1l;
        for(int i = 1; i <= num; ++i)
        {
            factorialResult *= i;
        }
        System.out.println("Factorial: "+factorialResult);
    }
}

public class Main {
    public static void main(String[] args) {
        FindFactorial nFindFactorial = new FindFactorial();
        nFindFactorial.findFactorial();

    }
}
```

----

## **Given an array of non-duplicating numbers from 1 to n where one number is missing, write an efficient java program to find that missing number?**

Idea is to find the sum of n natural numbers using the formula and then finding the sum of numbers in the given array. Subtracting these two sums results
in the number that is the actual missing number. This results in O(n) time complexity and O(1) space complexity.

```java
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
```

----

## **Write a Java Program to check if any number is a magic number or not. A number is said to be a magic number if after doing sum of digits in each step and inturn doing sum of digits of that sum, the ultimate result (when there is only one digit left) is 1?**

Example, consider the number:

```java
// Step 1: 163 => 1+6+3 = 10
// Step 2: 10 => 1+0 = 1 => Hence 163 is a magic number

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
```

----

## **Write a Java program to create and throw custom exceptions?**

```java
class Main {
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
```

We have created the exception class named with CustomException and called the base exception constructor with the error message that we want to print.
And to avoid handling exceptions in the main method, we have used the throws keyword in the method declaration.

----

## **Write a Java program to reverse a string?**

```java
class Main{
    public static void main(String[] args){
        // Input String
        String str = "Welcome to InterviewBit";

        // Pointers.
        int i = 0, j = str.length()-1;

        // Result character array to store the reversed string.
        char[] revString = new char[j+1];

        // Looping and reversing the string.
        while(i < j){
            revString[j] = str.charAt(i);
            revString[i] = str.charAt(j);
            i++;
            j--;
        }
        // Printing the reversed String.
        System.out.println("Reversed String = " + String.valueOf(revString));
    }
}
```

In the above code, we are storing the last character from the string to the first and the first value to the last in the output character array. And doing the same thing in the loop for the remaining 2nd to n-1 characters. This is how the string will be reversed.

----

## **Write a Java program to rotate arrays 90 degree clockwise by taking matrices from user input?**

```java
import java.util.Scanner;

public class Main
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

        // Rotation

        // Transpose
        for(int i = 0; i < no; i++){
            for(int j = i; j < no; j++){
                int temp = a[i][j];
                a[i][j] = a[j][i];
                a[j][i] = temp;
            }
        }

        // Reverse Each row
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
```

In the above code, for rotating the matrix to  90 degrees we are first transposing the matrix so the row becomes the column. And after that, we are reversing each row in the matrix. So this is how the matrix got rotated.

----

## **Write a java program to check if any number given as input is the sum of 2 prime numbers?**

Example :

Input - 18

Output - 

18 = 13 + 5
18 = 11 + 7

```java
public class Main
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
```

In the above code, for any number n, we find all the 2 pairs of numbers that are added together resulting in n. And each checking number if it is prime. If it is prime then we are printing that.

----

## **Write a Java program for solving the Tower of Hanoi Problem?**

```java
public class Main
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
```

In the above code we are first moving the n-1 disk from Tower A to Tower B, then moving that nth disk from Tower A to Tower C, and finally, the remaining n-1 disk from Tower B to Tower C. And we are doing this recursively for the n-1 disk.

----

## **Implement Binary Search in Java using recursion?**

```java
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
```

In the above code, we are finding the middle element each time and checking if the element is in the middle or not.
If it is not, then we check on which side from the middle it exists. And Recursively searching on the particular subarray.
So this way we are reducing the search space by 2 every time. So the search time is very low.

### https://www.interviewbit.com/java-interview-questions/

### https://www.digitalocean.com/community/tutorials/java-programming-interview-questions

## **How do you reverse a string in Java?**

There is no reverse() utility method in the String class. However, you can create a character array from the string and then iterate it from the end to the start. You can append the characters to a string builder and finally return the reversed string.

The following example code shows one way to reverse a string:

```java
public class Main {
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
```

Bonus points for adding null check in the method and using StringBuilder for appending the characters. Note that the indexing in Java starts from 0, so you need to start at chars.length - 1 in the for loop.

----

## **How do you swap two numbers without using a third variable in Java?**

Swapping numbers without using a third variable is a three-step process that’s better visualized in code:

b = b + a; // now b is sum of both the numbers
a = b - a; // b - a = (b + a) - a = b (a is swapped)
b = b - a; // (b + a) - b = a (b is swapped)
The following example code shows one way to implement the number swap method:

```java
public class Main {

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
```

The output shows that the integer values are swapped:
a is 10 and b is 20
After swapping, a is 20 and b is 10

----

## **Write a Java program to check if a vowel is present in a string?**

The following example code shows how to use a regular expression to check whether the string contains vowels:

```java
public class Main {

    public static void main(String[] args)
    {
        System.out.println(stringContainsVowels("Hello")); // true
        System.out.println(stringContainsVowels("TV")); // false
    }

    public static boolean stringContainsVowels(String input)
    {
        return input.toLowerCase().matches("?*[aeiou]?*");
    }
}

// Output:
// true
// false
```

----

## **Write a Java program to check if the given number is a prime number?**

You can write a program to divide the given number n, by a number from 2 to n/2 and check the remainder. If the remainder is 0, then it’s not a prime number. The following example code shows one way to check if a given number is a Prime number:

```java
// Prime number check
public class Main {

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
```

Although this program works, it’s not very memory and time-efficient. Consider that, for a given number N, if there is a prime number M between 2 to √N (square root of N) that evenly divides it, then N is not a prime number.

----

## **Write a Java program to print a Fibonacci sequence using recursion?**

A Fibonacci sequence is one in which each number is the sum of the two previous numbers. In this example, the sequence begins with 0 and 1. The following example code shows how to use a for loop to print a Fibonacci sequence:

```java
public class Main {
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

// Output
// 0, 1, 1, 2, 3, 5, 8, 13, 21, 34,
```

You can also use recursion to print a Fibonacci sequence, because the Fibonacci number is generated by adding the previous two numbers in the sequence:

F(N) = F(N-1) + F(N-2)

The following example class shows how to use recursion to calculate a Fibonacci sequence that is 10 numbers long:

```java
public class Main {
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

// Output
// A Fibonacci sequence of 10 numbers: 0 1 1 2 3 5 8 13 21 34
```

----

## **How do you check if a list of integers contains only odd numbers in Java?**

You can use a for loop and check whether each element is odd:

```java
public static boolean onlyOddNumbers(List<Integer> list) {
	for (int i : list) {
		if (i % 2 == 0)
			return false;
	}

	return true;
}

// If the list is large, you can use parallel stream for faster processing, as shown in the following example code:
public static boolean onlyOddNumbers(List<Integer> list) {
	return list
			.parallelStream() // parallel stream for faster processing
			.anyMatch(x -> x % 2 != 0); // return as soon as any elements match the condition
}
```

To learn more about the math behind determining if an integer is odd, refer to the Modulo operation on Wikipedia.

----

## **How do you check whether a string is a palindrome in Java?**
	
A palindrome string is the same string backwards or forwards. To check for a palindrome, you can reverse the input string and check if the result is equal to the input. The following example code shows how to use the String charAt(int index) method to check for palindrome strings:

```java
class Checkers {
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
}

public class Main{
    public static void main(String[] args) {
        Checkers newCheckers = new Checkers();
        newCheckers.checkPalindromeString("This is an input string");
    }
}
```

----

## **How do you remove spaces from a string in Java?**

The following example code shows one way to remove spaces from a string using with the Character.isWhitespace() method:

```java
class Cleaner {
    String removeWhiteSpaces(String input) {
        StringBuilder output = new StringBuilder();

        char[] charArray = input.toCharArray();

        for (char c : charArray) {
            if (!Character.isWhitespace(c))
                output.append(c);
        }

        return output.toString();
    }
}

public class Main{
    public static void main(String[] args) {
        Cleaner newCleaner = new Cleaner();
        newCleaner.removeWhiteSpaces("This is an input string");
    }
}
```

Learn more about removing spaces and other characters from a string in Java.

----

## **How do you remove leading and trailing spaces from a string in Java?**

The String class contains two methods to remove leading and trailing whitespaces: trim() and strip(). The strip() method was added to the String class in Java 11. The strip() method uses the Character.isWhitespace() method to check if the character is a whitespace. This method uses Unicode code points, while the trim() method identifies any character with a codepoint value less than or equal to U+0020 as a whitespace character.

The strip() method is the recommended way to remove whitespaces because it uses the Unicode standard. The following example code shows how to use the strip() method to remove whitespaces:

```java
public class Main{
    public static void main(String[] args) {
        String s = "  abc  def\t";
        s = s.strip();
        System.out.println(s);
    }
}
```

----

## **How do you sort an array in Java?**

The Arrays utility class has many overloaded sort() methods to sort primitive and to object arrays. If you are sorting a primitive array in the natural order, then you can use the Arrays.sort() method, as shown in the following example:

```java
import java.util.Arrays;

public class Main{
    public static void main(String[] args) {
        int[] array = {1, 2, 3, -1, -2, 4};
        Arrays.sort(array);
        System.out.println(Arrays.toString(array));
    }
}
```

However, if you want to sort an array of objects, then the object must implement the Comparable interface. If you want to specify the sorting criteria, then you can pass the Comparator for the sorting logic. Learn more about Comparable and Comparator in Java.

----

## **How do you create a deadlock scenario programmatically in Java?**

Deadlock is a scenario in a multi-threaded Java environment where two or more threads are blocked forever. The deadlock situation arises with at two or more threads. The following example code creates a deadlock scenario:

```java
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

public class Main {

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

// Output:
// t1 acquiring lock on java.lang.Object@418b535d
// t1 acquired lock on java.lang.Object@418b535d
```

All three threads will be able to acquire a lock on the first object. However, they are using shared resources and are started in such a way that they will keep on waiting indefinitely to acquire the lock on the second object. You can use the Java thread dump to detect the deadlocks. Learn more about deadlock in Java.

----

## **How can you find the factorial of an integer in Java?**

The factorial of an integer is calculated by multiplying all the numbers from 1 to the given number:

F(n) = F(1)*F(2)...F(n-1)*F(n)
The following example code shows how to use recursion to find the factorial of an integer:

```java
public class Main {
    public static long factorial(long n) {
        if (n == 1)
            return 1;
        else
            return (n * factorial(n - 1));
    }

    public static void main(String[] args) throws InterruptedException {
        factorial(4);
    }
}
```

----

## **How do you implement a binary search in Java?**
	
The array elements must be sorted to implement binary search. The binary search algorithm is based on the following conditions:

If the key is less than the middle element, then you now need to search only in the first half of the array.
If the key is greater than the middle element, then you need to search only in the second half of the array.
If the key is equal to the middle element in the array, then the search ends.
Finally, if the key is not found in the whole array, then it should return -1. This indicates that the element is not present.
The following example code implements a binary search:

```java
public class Main {
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

    public static void main(String[] args) throws InterruptedException {
        binarySearch(new int[]{1, 2, 3, 4, 5, 6, 7, 8}, 4, 8, 2);
    }
}
```

----

## **Write a Java program that illustrates merge sort?**

Merge sort is one of the most efficient sorting algorithms. It works on the principle of “divide and conquer”. It is based on the idea of breaking down a list into several sub-lists until each sub-list consists of a single element, and then merging those sub-lists in a manner that results in a sorted list. The following example code shows one way to use merge sort:

```java
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
```

----

## **Can you create a pyramid of characters in Java?**

Pattern programs are a very popular interview topic. This type of question is used to understand the logical thinking abilities of the interviewee. Refer to Pyramid Pattern Programs in Java for examples of different ways to create pyramid patterns.

----

## **Write Java program that checks if two arrays contain the same elements?**

To check if two arrays contain the same elements, you need to first create a set of elements from both the arrays, and then compare the elements in these sets to find if there is an element that is not present in both sets. The following example code shows how to check if two arrays only contain common elements:

import java.util.Arrays;
import java.util.HashSet;
import java.util.Set;

```java
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

// Output
// true
// false
```

----

## **How do you get the sum of all elements in an integer array in Java?**

You can use a for loop to iterate over the array elements and add them to get the final sum:

```java
public class Main {
    public static void main(String[] args) throws InterruptedException {
        int[] array = { 1, 2, 3, 4, 5 };

        int sum = 0;

        for (int i : array)
            sum += i;

        System.out.println(sum);
    }
}

// Output:
// 15
```

----

## **How do you find the second largest number in an array in Java?**

There are many ways to solve this problem. You can sort the array in natural ascending order and take the second last value. However, sorting is an expensive operation. You can also use two variables to find the second largest value in a single iteration, as shown in the following example:

```java
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
```

----

## **How do you shuffle an array in Java?**

The following example code shows how to use the Random class to generate random index numbers and shuffle the elements:


```java
import java.util.Random;

public class Main {
    public static void main(String[] args) throws InterruptedException {
        int[] array = { 1, 2, 3, 4, 5, 6, 7 };

        Random rand = new Random();

        for (int i = 0; i < array.length; i++) {
            int randomIndexToSwap = rand.nextInt(array.length);
            int temp = array[randomIndexToSwap];
            array[randomIndexToSwap] = array[i];
            array[i] = temp;
        }
    }
}
```

```java
System.out.println(Arrays.toString(array));
```

You can run the shuffling code inside another for loop to shuffle multiple rounds.

----

## **How can you find a string in a text file in Java?**

The following example code shows how to use the Scanner class to read the file contents line by line and then use the String contains() method to check if the string is present in the file:

```java
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
```

Note that the example code assumes that the string that you’re searching for in the file doesn’t contain newline characters.

----

## **How do you print a date in specific format in Java?**

The following example code shows how to use the SimpleDateFormat class to format the date string:

```java
import java.text.SimpleDateFormat;
import java.util.Date;

public class Main {
    public static void main(String[] args) throws InterruptedException {
        String pattern = "MM-dd-yyyy";
        SimpleDateFormat simpleDateFormat = new SimpleDateFormat(pattern);

        String date = simpleDateFormat.format(new Date());
        System.out.println(date); // 06-23-2020
    }
}
```

Lear more about the Java SimpleDateFormat.

----

## **How do you merge two lists in Java?**

The following example code shows how to use the addAll() method to merge multiple lists in Java:

```java
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
```

----

## **How do you remove all occurrences of a given character from an input string in Java?**

The String class doesn’t have a method to remove characters. The following example code shows how to use the replace() method to create a new string without the given character:

```java
public class Main {
    public static void main(String[] args) throws InterruptedException {
        String str1 = "abcdABCDabcdABCD";
        str1 = str1.replace("a", "");
        System.out.println(str1); 
    }
}

// Output:
// bcdABCDbcdABCD
```

String is immutable in Java. All the string manipulation methods return a new string, which is why you need to assign it to another variable. Learn more about removing characters from a string in Java.

----

## **How do you get distinct characters and their count in a string in Java?**

You can create the character array from the string. Then iterate over it and create a HashMap with the character as key and their count as value. The following example code shows how to extract and count the characters of a string:

```java
import java.util.HashMap;
import java.util.Map;

public class Main {
    public static void main(String[] args) throws InterruptedException {
        String str1 = "abcdABCDabcd";

        char[] chars = str1.toCharArray();

        Map<Character, Integer> charsCount = new HashMap<>();

        for (char c : chars) {
            if (charsCount.containsKey(c)) {
                charsCount.put(c, charsCount.get(c) + 1);
            } else {
                charsCount.put(c, 1);
            }
        }
        System.out.println(charsCount); // {a=2, A=1, b=2, B=1, c=2, C=1, d=2, D=1}
    }
}

// Output:
// {a=2, A=1, b=2, B=1, c=2, C=1, d=2, D=1}
```

----

## **Can you prove that a String object in Java is immutable programmatically?**

The following example code shows how to prove that a String object is immutable and the comments in the code explain each step:

```java
import java.util.HashMap;
import java.util.Map;

public class Main {
    public static void main(String[] args) throws InterruptedException {
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
    }
}

// Output:
// true
// false
// Java
```

----

## **Can you write some code to showcase inheritance in Java?**

The following example code shows how to use the extends keyword to create a subclass of the class Animal. The new class Cat inherits the variable from the Animal class and adds more code that only belongs to the Cat class.

```java
class Animal {
    String color;
}

class Cat extends Animal {
    void meow() {
        System.out.println("Meow");
    }
}
public class Main {
    public static void main(String[] args) throws InterruptedException {
        Cat Amy = new Cat();
        Amy.meow();
    }
}
```

----

## **How do you show a diamond problem with multiple inheritance in Java?**

The diamond problem occurs when a class inherits from multiple classes and ambiguity occurs when it’s unclear which method to execute from
which class. Java doesn’t allow extending multiple classes to avoid the diamond problem illustrated by the following example:

```java
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
```

----

## **How do you illustrate a try catch example in Java?**

The following example code shows an example of try-catch:

```java
import java.io.FileInputStream;
import java.io.FileNotFoundException;

public class Main {

    // From Java 7 onwards, you can also catch multiple exceptions in a single catch block,
    // as shown in the following example. It’s useful when you have the same code in all the catch blocks.
    public static void foo(int x) throws IllegalArgumentException, NullPointerException {
        System.out.print(x);
    }

    public static void main(String[] args) throws InterruptedException {

        try {
            FileInputStream fis = new FileInputStream("test.txt");
        } catch(FileNotFoundException e) {
            e.printStackTrace();
        }

        try {
            foo(10);
        } catch (IllegalArgumentException | NullPointerException e) {
            System.out.println(e.getMessage());
        }
    }
}
```

----

## **Write a Java program to show a NullPointerException?**

If you are calling a function on null, it will throw a NullPointerException, as shown in the following example code:

```java
public class Main {
    static void printString(String s, int count) {
        for (int i = 0; i < count; i++) {
            System.out.println(s.toUpperCase()); // Exception in thread "main" java.lang.NullPointerException
        }
    }

    // static void printString(String s, int count) {
    //     if (s == null) return;
    //     for (int i = 0; i < count; i++) {
    //         System.out.println(s.toUpperCase());
    //     }
    // }

    public static void main(String[] args) throws InterruptedException {
        printString(null, 3);
    }
}
```

You can also throw IllegalArgumentException based on the project requirements.

----

## **How do you create a record in Java?**

Records was added as a standard feature in Java 16. Records enable you to create a POJO class with minimal code. Records automatically generates hashCode(), equals(), getter methods, and toString() method code for the class. Records are final and implicitly extend the java.lang.Record class. The following example code shows one way to cerate a record:

```java
import java.util.Map;

public class Main {
    public record EmpRecord(int id, String name, long salary, Map<String, String> addresses) {
        
    }
    
    public static void main(String[] args) {
        String textBlock = """
		Hi
		Hello
		Yes""";
    }
}
```

Learn more about records in Java. For details about POJO, refer to Plain old Java object on Wikipedia.

----

## **How do you create text blocks in Java?**

Java 15 added the text blocks feature. You can create multiline strings using text blocks. The multiline string has to be written inside of a pair of triple-double quotes, as shown in the following example:

```java
public class Main {
    public static void main(String[] args) {
        String textBlock = """
		Hi
		Hello
		Yes""";
    }
}
```

It’s the same as creating a string, such as Hi\\nHello\\nYes.

----

## **Show an example of switch expressions and multi-label case statements in Java?**

The switch expressions were added as a standard feature in Java 14. The following examples show switch expressions as well as multi-label case statements:

```java
import java.util.Map;

public class Main {
    public static void main(String[] args) {
        int choice = 2;

        int x = switch (choice) {
            case 1, 2, 3:
                yield choice;
            default:
                yield -1;
        };

        System.out.println("x = " + x); // x = 2

        // You can also use lambda expressions in switch expressions.
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
    }
}

// Output:
// x = 2
// TTS
```

----

## **How do you compile and run a Java class from the command line?**

This example refers to the following Java file:

```java
public class Main {
    public static void main(String args[]) {
        System.out.println("Hi");
    }
}

// Output:
// Hi
```

You can compile it using the following command in your terminal:

```cmd
javac Test.java
```

To run the class, use the following command in your terminal:

```cmd
java Test
```

For the recent releases, the java command will also compile the program if the class file is not present. If the class is in a package, such as com.example, then it should be inside the folder com/example. The command to compile and run is:

```cmd
java com/example/Test.java
```

If your class requires some additional JARs to compile and run, you can use the java -cp option. For example:

```cmd
java -cp .:~/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar  com/example/Test.java
```

----

## **How do you create an enum in Java?**

The following example code shows how to create a basic enum:

```java
public enum ThreadStates {
	START,
	RUNNING,
	WAITING,
	DEAD;
}
```

ThreadStates is the enum with fixed constants fields START, RUNNING, WAITING, and DEAD. All enums implicitly extend the java.lang.Enum class and implement the Serializable and Comparable interfaces. Enum can have methods also. Learn more about enums in Java.

----

## **How do you use the forEach() method in Java?**

The forEach() method provides a shortcut to perform an action on all the elements of an iterable. The following example code shows how to iterate over the list elements and print them:

```java
import java.util.ArrayList;
import java.util.Iterator;
import java.util.List;

public class Main {
    public static void main(String args[]) {
        List<String> list = new ArrayList<>();
        Iterator<String> it = list.iterator();
        while (it.hasNext()) {
            System.out.println(it.next());
        }

        // You can use the forEach() method with a lambda expression to reduce the code size, as shown in the following example code:
        List<String> list1 = new ArrayList<>();
        list1.forEach(System.out::print);
    }
}
```

----

## **How do you write an interface with default and static method?**

Java 8 introduced default and static methods in interfaces. This bridged the gap between interfaces and abstract classes. The following example code shows one way to write an interface with the default and static method:

```java
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
```

----

## **How do you create a functional interface?**

An interface with exactly one abstract method is called a functional interface. The major benefit of functional interfaces is that you can use lambda expressions to instantiate them and avoid using bulky anonymous class implementation. The @FunctionalInterface annotation indicates a functional interface, as shown in the following example code:

```java
@FunctionalInterface
interface Foo {
	void test();
}
```

----

## **Show an example of using lambda expressions in Java?**

Runnable is an excellent example of a functional interface. You can use lambda expressions to create a runnable, as shown in the following example code:

```java
Runnable r1 = () -> System.out.println("My Runnable");
```

----

## **Show examples of overloading and overriding in Java?**

When a class has two or more methods with the same name, they are called overloaded methods. The following example code shows as overloaded method called print:

```java
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

// When a superclass method is also implemented in the child class, it’s called overriding. The following example code shows how to annotate the printname() method that’s implemented in both classes:
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
```

----

## **Guess the Output**

Test yourself by guessing the output of the following code snippets.

```java
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
```

----

## **Find 5 mistakes in the following code snippet**

```java
public class Main {
    public static void main(String[] args) {
        String s = args[10];
        System.out.println("Argument 10: " + s);
    }
}

// Output:
// 1. Return type is not need in class
// 2. AMpersend missing in line with String s = "abc";
// 3. mainmethod must be public of course
// 4. 
```

### https://www.digitalocean.com/community/tutorials/java-programming-interview-questions

### https://javahungry.blogspot.com/2020/05/entry-level-interview-questions.html

## **What are the main features of Java?**

a.  Java is an Object-Oriented programming language
b.  Simple
c.  Distributed
d.  Java support Multithread
e.  Java is a Platform independent programming language
f.  Java is more secured than other languages
g.  Portable
h.  Robust

----

## **What is an Array?**

The collection of similar data types is known as Array. You can find it in detail here.

----

## **Is it possible to declare an Array without Array size?**

It is not possible to declare an Array without Array size. If you try to do so then you will get compile-time error.

----

## **What do you understand by the term Object-Oriented Programming language?**

The object-oriented programming language is a language that uses objects in programming.

----

## **What are the basic principles of the OOPs concept?**

a. Abstraction
b. Polymorphism
c. Encapsulation
d. Inheritance

----

## **What is the abstraction in java?**

Abstraction means hiding the detailed information from the user. Abstraction can be achieved by interfaces and abstract classes.

----

## **What do you mean by inheritance in java?**

Inheritance is the main feature of java. Inheritance means java class or interface can inherit the properties and behavior from another class or interface. Inheritance can be gained by implementing interfaces or extending classes. You can find it in detail here.

----

## **What do you mean by the Object in java?**

The object is the instance of a class. A class contains the basic properties and behavior of a real-world object. We can instantiate this class with a new keyword to make an object.
For example, Animal.java has a class named Animal. Animal animal = new Animal() is an object or instance of this class.

----

## **What is a constructor?**

Java provides the facility to declare a special member of the class with the same name, no return type, and with zero or many parameters is called a constructor.

----

## **What is polymorphism in java?**

Poly means many and Morph means forms of a method or constructor or operator. So finally, Polymorphism means many forms of the same method or constructor or operators. You can find it in detail here.

----

## **What do you mean by the method overloading?**

The method with the same name but the number of arguments are different is called method overloading. Methods return type should be the same for all methods. You can find it in detail here.

----

## **What do you mean by the method overriding in java?**

You can find the details about method overriding here.

----

## **Does java support multiple inheritance?**

Java classes do not support multiple inheritance but can gain multiple inheritance by using the interfaces.

----

## **Describe constructor vs method?**

The constructor is the special member of the class with the same name as the class and no return type. But the method is the ordinary member of a class used to describe the behavior of some object or class.

----

## **Is it possible to overload the main() method?**

Yes, the main method can be overloaded. But we should declare original one like public static void main(String args[]){} because JVM will look for this when starting execution.

----

## **What is the difference between String, StringBuilder and StringBuffer?**

You can find the answer in detail here.

----

## **What is the difference between Collection and Collections?**

The difference between Collection and Collections you can find it in detail here.

----

## **What is multithreaded programming?**

Multithreaded means multiple threads will run to execute the task simultaneously.  It's important in the programming world. The operating system is an example of a multithreaded system.

```java
public class MultithreadedExample {
    public static void main(String[] args) {
        MyThread thread1 = new MyThread("Thread 1");
        MyThread thread2 = new MyThread("Thread 2");
        MyThread thread3 = new MyThread("Thread 3");
        
        thread1.start();
        thread2.start();
        thread3.start();
        
        try {
            thread1.join();
            thread2.join();
            thread3.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        System.out.println("All threads have completed!");
    }
}

class MyThread extends Thread {
    private String name;
    
    public MyThread(String name) {
        this.name = name;
    }
    
    @Override
    public void run() {
        System.out.println("Thread " + name + " is running...");
        
        for (int i = 1; i <= 5; i++) {
            System.out.println("Thread " + name + " is counting: " + i);
            
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
        
        System.out.println("Thread " + name + " has completed!");
    }
}
```

----

## **What is the difference between Error and Exception?**

Error is generated by the environment at runtime. The exception is generated by the application intentionally or mistakenly. An exception can be checked or unchecked,
but the error is only unchecked. You can find the difference between Error and Exception here.

----

## **Difference between static and non-static methods?**

Static methods belong to a class but non-static methods belong to an object. You don’t need to instantiate a class to access the static methods, but you have to instantiate
the class to get access to non-static methods.

----

## **Difference between method overloading and method overriding?**

You can find the difference between method overloading and method overriding here.

----

## **What are the different ways to create threads in java?**

There are two ways to create threads in java. Ways are listed below:
a. Implement Runnable interface
b. By extending Thread class

----

## **What is the synchronization in java?**

Synchronization is a technique to control access of a method with multiple threads at the same time. If we declare a method synchronized, then only one thread can use this method at a time. This is basically used for Thread safety. You can find it in detail here.

```java
class Counter {
    private int count;

    public synchronized void increment() {
        count++;
    }

    public synchronized int getCount() {
        return count;
    }
}

class IncrementThread extends Thread {
    private Counter counter;

    public IncrementThread(Counter counter) {
        this.counter = counter;
    }

    @Override
    public void run() {
        for (int i = 0; i < 1000; i++) {
            counter.increment();
        }
    }
}

public class SynchronizationExample {
    public static void main(String[] args) throws InterruptedException {
        Counter counter = new Counter();

        IncrementThread thread1 = new IncrementThread(counter);
        IncrementThread thread2 = new IncrementThread(counter);

        thread1.start();
        thread2.start();

        thread1.join();
        thread2.join();

        System.out.println("Counter value: " + counter.getCount());
    }
}
```

In this example, we have a Counter class that contains a count variable. The increment() method is marked as synchronized, which means only one thread can execute that method at a time. The getCount() method is also marked as synchronized for consistency, even though it doesn't modify any shared state.

We create two IncrementThread instances, each working on the same Counter object. The run() method of each thread calls the increment() method of the Counter object 1000 times.

In the main method, we start both threads and then wait for them to complete using the join() method. Finally, we print the value of the counter.

Due to synchronization, even though the increment() method is called concurrently by multiple threads, the shared count variable is incremented correctly and the final output will always be 2000 (1000 increments from each thread). Without synchronization, there would be a chance of data corruption or inconsistent results.

----

## **What is the use of the final keyword?**

We cannot change the value of a final variable. We are not able to inherit a final class and cannot override a final method.

----

## **What is the garbage collection of java?**

To clean the object from memory which has no reference is called garbage collection. It’s an important feature of java. Java automatically clears the objects from memory. We don’t need to clean the object manually from memory.

```java
public class GarbageCollectionExample {
    public static void main(String[] args) {
        // Create objects
        MyClass obj1 = new MyClass();
        MyClass obj2 = new MyClass();
        
        // Assign obj2 to obj1
        obj1 = obj2;
        
        // Set obj2 to null
        obj2 = null;
        
        // Request garbage collection
        System.gc();
    }
}

class MyClass {
    // Constructor
    public MyClass() {
        System.out.println("Creating an object");
    }
    
    // Finalize method
    @Override
    protected void finalize() throws Throwable {
        System.out.println("Finalizing an object");
    }
}
```

----

## **What is the cloning in java?**

Java cloning means create an exact copy of an object. Shallow or Deep cloning is used in java to clone a java object. The clone() method is used to clone an object.
You can find the difference between Shallow and Deep cloning here.

```java
class Person implements Cloneable {
    private String name;
    private int age;

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }

    public int getAge() {
        return age;
    }

    @Override
    public Object clone() throws CloneNotSupportedException {
        return super.clone();
    }
}

public class CloningExample {
    public static void main(String[] args) {
        try {
            // Create an object
            Person person1 = new Person("John", 30);

            // Clone the object
            Person person2 = (Person) person1.clone();

            // Verify the clone
            System.out.println("Original: " + person1.getName() + " - " + person1.getAge());
            System.out.println("Clone: " + person2.getName() + " - " + person2.getAge());

            // Modify the clone
            person2.setName("Alice");
            person2.setAge(25);

            // Verify the changes
            System.out.println("Original: " + person1.getName() + " - " + person1.getAge());
            System.out.println("Clone: " + person2.getName() + " - " + person2.getAge());
        } catch (CloneNotSupportedException e) {
            e.printStackTrace();
        }
    }
}

// Output:
// Original: John - 30
// Clone: John - 30
// Original: John - 30
// Clone: Alice - 25

```

In this example, we have a Person class that implements the Cloneable interface. The Person class has a name and an age as its attributes.

Inside the Person class, we override the clone() method inherited from the Object class. We call the super.clone() method to perform a shallow copy of the object. This method creates a new instance of the Person class and copies the values of the attributes.

In the main method, we create an instance of the Person class (person1). We then clone this object using the clone() method and store the clone in another variable (person2).

We verify that the cloning process worked correctly by printing the attributes of both the original object and the clone.

Next, we modify the attributes of the clone (person2). We print the attributes again to demonstrate that the modifications made to the clone do not affect the original object.

----

## **What is JVM?**

Java virtual machine is called JVM. JVM compiles and interprets the java code. JVM manages the garbage collection mechanism and other things efficiently. JVM manages objects in heap memory.

----

## **What are the difference between final, finally and finalize in java?**

The keyword final is used to make a class, variable, or methods final. Final classes cannot be inherited, variables value cannot be changed, and methods cannot be overridden.
The keyword finally used in the exception handler to clear some post-task after the execution of try or catch block.
The finalize keyword used to clean up some tasks before the object is removed from memory. The finalize method mainly used in garbage collection.
You can find it in detail here.

----

## **What is the difference between float and double datatypes?**

You can find the answer in detail here.

----

## **Is it possible to override the overloaded method in java?**

Yes, in java it is possible to override the overloaded method.

That's all for today. Please mention in comments in case you have any questions related to top 30 entry level interview questions and answers.

### https://javahungry.blogspot.com/2020/05/entry-level-interview-questions.html

### https://www.interviewbit.com/j2ee-interview-questions/

## **What is J2EE?**

J2EE or Java Enterprise Edition is a Java-based platform that is a combination of services protocols and APIs (Application Programming Interfaces) that provides capabilities to develop multi-tier, secure, stable and fast enterprise-level applications. J2EE provides web, enterprise, web service and various other specifications for developing enterprise-level web applications.

----

## **What are the main advantages of J2EE?**

Following are the advantages of the J2EE platform:

*Support for Web Services:* J2EE provides a platform to develop and deploy web services. The JAX-RPC (Java API for XML based Remote Procedure Call) helps developers develop SOAP-based portable and interoperable web services, clients and endpoints.

*Faster Time to Market:* J2EE uses the concept of containers for simplifying the development. This helps in business logic separation from lifecycle management and resources which aids developers to focus on business logic than on the infrastructure. For instance, the EJB (Enterprise JavaBeans) container takes care of threading, distributed communication, transaction management, scaling etc and provides a necessary abstraction to the developers.

*Compatibility:* J2EE platform follows the principle of “Write Once, Run Anywhere”. It provides comprehensive standards and APIs that ensures compatibility among different application vendors resulting in the portability of applications.

*Simplified connectivity:* J2EE helps in easier applications connectivity which allows utilizing the capabilities of different devices. It also provides JMS (Java Message Service) to integrate diverse applications in asynchronous and loosely coupled ways. It also provides CORBA (Common Object Request Broker Architecture) support for linking systems tightly via remote calls.
Due to all the above benefits packed in one technology, it helps the developers to reduce the TCO (Total Cost of Ownership) and also focus more on actual business logic implementation.

----

## **What are some of the technologies provided by the J2EE platform?**

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

----

## **What are the various components of J2EE application architecture?**

J2EE is made up of 3 main components (tiers) - Client tier, Middle tier, Enterprise data tier as shown in the below image:


Client Tier: This tier has programs and applications which interact with the user and they are generally located in different machines from the server. Here, different inputs are taken from the user and these requests are forwarded to the server for processing and the response will be sent back to the client.

Middle Tier: This tier comprises of Web components and EJB containers. The web components are either servlet or JSP pages that process the request and generate the response. At the time of the application’s assembly, the client’s static HTML codes, programs and applets along with the server’s components are bundled within the web components. The EJB components are present for processing inputs from the user which are sent to the Enterprise Bean that is running in the business tier.

Enterprise Data Tier: This tier includes database servers, resource planning systems and various other data sources that are located on a separate machine which are accessed by different components by the business tier. Technologies like JPA, JDBC, Java transaction API, Java Connector Architecture etc are used in this tier.

----

## **How is JDK different from JIT?**

JDK (Java Development Kit) is a cross-platformed software development environment offering various collections of libraries and tools required for developing Java applications and applets. It also consists of JRE that provides tools and libraries which aids in byte code execution. JDK is needed for writing and running programs in Java. Whereas JIT stands for Just In Time Compiler which is a module inside JVM (which is inside JRE). JIT compiler is used for compiling some parts of byte code having similar functionality at the same time to machine code for optimising the compilation time and performance.

----

## **How are PATH and CLASSPATH different from each other in terms of J2EE?**

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

## **What do you understand by build file?**

A build file is used for automating various steps involved in software development. Along with this, the build file also specifies libraries and their versions that need to be included. It also includes the type of optimizations required for the project. Whenever the project size increases, build provides a standard way to build the project.

----

## **Why do we have JDBC and JNDI in J2EE? How are they different from each other?**

JDBC or Java Database Connectivity provides guidelines and APIs for connecting databases from different vendors like MySQL, Oracle, PostgreSQL etc for getting data. JNDI (Java Naming and Directory Interface) helps in providing logical structure to retrieve a resource from the database, EJB beans, messaging queues etc without knowing the actual host address or port. A resource can be registered with JNDI and then those registered application components can be accessed using the JNDI name.

----

## **What is an EJB? How can you use it in J2EE?**

EJB or Enterprise Java Beans is one of the most important parts of the J2EE platform that helps to develop enterprise-level multi-tiered applications and deploy them by keeping in mind performance, scalability and robustness. EJBs can be used when we want to achieve the following:

Clustering: For deploying the application in a cluster environment, EJBs can be used to achieve high availability and fault tolerance.
Concurrency without using Threads: EJBs can be used to achieve concurrency without using actual threads since they are instantiated using the object pool and are available in the EJB container. This helps in achieving performance without involving complexities around Threads.

Transaction management: EJBs can be used for achieving transaction management for databases by using annotations provided by EJB.
Database Connection Pool: EJB can access connection pools defined in the J2EE server. The connection pools help in achieving abstraction of database connectivity and operations.
Security: EJBs use JAAS (Java Authentication and Authorization Service) to develop secure applications. EJB methods can be authenticated and authorised with only configuration changes.
Scheduler Service: EJBs can be used in the Timer Service which enables task implementation for further execution or repetitive execution.

----

## **What are the J2EE applets? Why can we use it?**

Applets are J2EE client components that are written in Java and are executed in a web browser or a variety of other devices which supports the applet programming model. They are used for providing interactive features to web apps and help in providing small, portable embedded Java programs in HTML pages which will be run automatically when we view the pages.

```java
import java.applet.Applet;
import java.awt.Graphics;

public class MyJ2EEApplet extends Applet {

    public void init() {
        // Initialization code goes here
    }

    public void start() {
        // Start code goes here
    }

    public void stop() {
        // Stop code goes here
    }

    public void destroy() {
        // Cleanup code goes here
    }

    public void paint(Graphics g) {
        // Drawing code goes here
        g.drawString("Welcome to J2EE Applet", 50, 50);
    }
}
```

----

## **What is the architecture model of Struts?**

Strut is a combination of JSP, Java Servlets, messages and custom tags that together form an application development framework for developing enterprise-level applications. It is based on MVC (Model-View-Controller) architecture.


Model: This component defines the internal system state. It can either be a Java Beans cluster or a single bean depending on the application architecture.
View: Struts make use of JSP technology for designing views of enterprise-level applications.
Controller: It is a servlet and is used for managing user actions that process requests and respond to them.

----

## **What do you understand by ORM?**

ORM stands for Object-Relational Mapping that transforms objects of Java class to tables in relational databases and vice versa using metadata describing the mapping between the database and the objects. 

This is represented as shown in the below image:

Consider an example where we have an Employee class having employeeId, firstName, lastName, contactNo as attributes. Consider we also have an Employee table that has ID, FNAME, LNAME and CONTACT_NO as columns. If we want to send data from our Java application and save it in the database, we cannot do it straightforwardly by simply saving the Java objects in the database directly. We need some sort of a mapper that maps the Java objects to the records that are compatible to be saved in the database table. This is where ORM comes into the picture. ORM helps in this transformation while writing data to the database as described in the below image:


The database records cannot be directly consumed by the Java applications as Java only deals with objects. ORM again plays a major role in the transformation of database records to Java objects.

----

## **What constitutes web components?**

Java Servlets and Java Server Pages (JSP) components together constitute web components.


__Java Servlets dynamically process requests and responses:__

```java
import javax.servlet?*;
import javax.servlet.http?*;
import java.io.IOException;

public class MyServlet extends HttpServlet {
  
    @Override
    public void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // Set the response content type
        response.setContentType("text/html");

        // Get the PrintWriter object to write the response
        PrintWriter out = response.getWriter();

        // Write the HTML content to the response
        out.println("<html>");
        out.println("<head>");
        out.println("<title>My Servlet</title>");
        out.println("</head>");
        out.println("<body>");
        out.println("<h1>Hello, Servlet!</h1>");
        out.println("</body>");
        out.println("</html>");
    }
}
```

__JSP pages are used for executing servlets that allow a natural approach to creating static content.__

```java
import javax.servlet?*;
import javax.servlet.http?*;
import java.io.IOException;

public class MyServlet extends HttpServlet {
  
    @Override
    public void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // Set the response content type
        response.setContentType("text/html");

        // Get the PrintWriter object to write the response
        PrintWriter out = response.getWriter();

        // Write the HTML content to the response
        out.println("<html>");
        out.println("<head>");
        out.println("<title>My Servlet</title>");
        out.println("</head>");
        out.println("<body>");
        out.println("<h1>Hello, Servlet!</h1>");
        out.println("</body>");
        out.println("</html>");
    }
}
```

----

## **What do you understand by JSF?**

JSF stands for Java Server Faces which is a web framework that is intended for simplifying the development process for user interfaces. It is a standardized display technology for Java-based web applications. It is based on MVC (Model-View-Controller) pattern and provides reusable UI components.

An example:

First, create a JSF page named "example.xhtml" with the following code:

```java
<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml"
      xmlns:h="http://java.sun.com/jsf/html">
<head>
    <title>JSF Example</title>
</head>
<body>
    <h1>Welcome to JSF!</h1>
    <h:form>
        <h:inputText value="#{helloBean.name}" />
        <h:commandButton value="Say Hello" action="#{helloBean.sayHello}" />
    </h:form>
    <h2>#{helloBean.greeting}</h2>
</body>
</html>
```

In this example, the JSF page contains HTML code along with JSF components defined using the "h" namespace. We have an input text field and a command button that triggers the "sayHello" method in the managed bean. The result is displayed using the #{helloBean.greeting} expression.

Next, create a managed bean class named "HelloBean.java" with the following code:

```java
import javax.faces.bean.ManagedBean;
import javax.faces.bean.RequestScoped;

@ManagedBean
@RequestScoped
public class HelloBean {

    private String name;
    private String greeting;

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getGreeting() {
        return greeting;
    }

    public void setGreeting(String greeting) {
        this.greeting = greeting;
    }

    public void sayHello() {
        greeting = "Hello, " + name + "!";
    }
}
```

In this example, the managed bean class is annotated with @ManagedBean to indicate that it is a managed bean. The @RequestScoped annotation specifies the scope of the bean. The class has a name property that is bound to the input text field in the JSF page using the value attribute. The greeting property holds the greeting message. The sayHello method is invoked when the command button is clicked, and it sets the greeting message based on the entered name.

Finally, you need to configure your JSF application in the "faces-config.xml" file:

```java
<?xml version="1.0" encoding="UTF-8"?>
<faces-config xmlns="http://java.sun.com/xml/ns/javaee"
              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
              xsi:schemaLocation="http://java.sun.com/xml/ns/javaee http://java.sun.com/xml/ns/javaee/web-facesconfig_2_0.xsd"
              version="2.0">
    <managed-bean>
        <managed-bean-name>helloBean</managed-bean-name>
        <managed-bean-class>HelloBean</managed-bean-class>
        <managed-bean-scope>request</managed-bean-scope>
    </managed-bean>
</faces-config>
```

In this configuration file, we define the managed bean with its name, class, and scope.

Now, you can deploy and run your JSF application on a compatible server, and the "example.xhtml" page will be rendered with the form and functionality to enter a name and display a greeting message when the button is clicked.

----

## **What factors should a J2EE application possess for operating in a global economy?**

Following are the factors that a J2EE application should possess to operate globally:

Financial Considerations: Each country has its taxes, restrictions and tariffs depending on the government. All these factors should be considered while developing the J2EE application.
Language Requirements: An application developed should support regional languages of the country for wider user coverage.
Legal Differences: Every government has their custom laws, privacy laws and requirements for each country. An application developed should abide by all the rules of the land.

----

## **What are the differences between JVM vs JIT vs JDK vs JRE?**

JVM	JIT	JDK	JRE
Java Virtual Machine: Introduced for managing system memory and also to provide a portable execution environment for Java applications.	Just in Time Compilation: This is a part of JVM and was developed for improving JVM performance.	 Java Development Kit: JDK is a cross-platformed software development environment offering various collections of libraries and tools required for developing Java applications and applets.	Java Runtime Environment: JRE is part of JDK that consists of JVM, core classes and support libraries. It is used for providing a runtime environment for running Java programs.
Used for compiling byte code to machine code completely.	This is used for compiling only reusable byte code to machine code.	JDK is essential for writing and running programs in Java.	JRE is a subset of JDK and is like a container that consists of JVM, supporting libraries and other files. It doesn't have development tools such as compilers and debuggers.
This is used for providing platform independence.	This is used for improving the performance of JVM.	JDK is used for developing Java programs as it provides libraries and compiler tools as well as JRE for running the code.	JRE is not suitable for development. It is used for running Java Programs as it provides runtime environments and tools for supporting execution.
J2EE Interview Questions for Experienced

----

## **What are the design goals of J2EE architecture?**

The design goals of J2EE architecture are as follows:

__Service Availability:__ To ensure that the application is available 24*7 to achieve required business goals.
__Data Connectivity:__ The connection between a J2EE application and legacy systems should remain compatible enough for ensuring business functions.
__Ease of Accessibility:__ The user should be able to connect to applications using any device and from anywhere.
__User Interaction:__ The user interaction should be seamless and should be able to connect to different devices like desktops, mobiles, laptops etc.
__Abstraction and Flexibility:__ The developer should focus on business logic and the configuration details should be handled by the server.

----

## **What do you understand by Connectors? Can you describe the Connector Architecture?**

Connectors are used for providing standard extension mechanisms to provide connectivity to different enterprise information systems. A connector architecture consists
of resource adapters and system-level contracts, both of which are specific to enterprise information systems. The resource adapters are plugged into the container.
The connector architecture defines certain contracts which a resource adapter must support for plugging into J2EE applications like security, transaction, resource management etc.

----

## **What do you understand by JRMP?**

JRMP stands for __Java Remote Method Protocol__ which is used for Remote Method Invocation (RMI) for passing Java objects as arguments. It is an underlying protocol used by RMI for marshalling objects as a stream during object serialization for transferring objects from one JVM to other.

----

## **What happens if the database connected to the Java application via connection pool suddenly goes down?**

Since the Java application uses a connection pool, it has active connections that would get disconnected if the database goes down. When the queries are executed to retrieve or modify data, then we will get a Socket exception.

----

## **How is 32-bit JVM different from 64-bit JVM?**

64-bit JVM is used in 64-bit operating systems whereas 32-bit JVM is used for 32-bit operating systems. In 64-bit JVM, we can specify more heap size memory up to 100G when compared to the 4G limit of 32-bit JVM. Java applications take more memory while running in 64-bit JVM when compared to running the same application in 32-bit JVM. This is because of the increased size of the Ordinary Object Pointer. However, this can be bypassed by making use of the -XXCompressedOOP option of the JVM for telling to use 32-bit pointers. Additionally, 64-bit JVM uses 12 bytes object header size and a maximum of 8 bytes of internal references whereas the 32-bit JVM uses 8 bytes headers and a maximum of 4 bytes of internal references.

----

## **How is a webserver different from an application server?**

| Web Server | Application Server |
| ------------- | ------------ |
| Web servers are computer programs that accept requests and returns responses based on that. | Application servers are used for installing, operating and hosting associated applications and services. |
| It constitutes the web container. | It constitutes both a web container and an EJB container. |
| These are useful for getting static content for the applications. | These are useful for getting dynamic content. |
| This consumes and utilizes fewer resources. | It makes use of more resources. |
| Provide an environment for running web applications. | Provide an environment for running enterprise applications. |
| Web servers don’t support multithreading. | Multithreading is supported in application servers. |
| This server makes use of HTML and HTTP protocols. | The application server has GUI (Graphical User Interface) and also supports HTTP, RPC/RMI protocols. |
	
----	

## **What is the purpose of heap dumps and how do you analyze a heap dump?**

Heap dumps consist of a snapshot of all live objects on Java heap memory that are used by running Java applications. Detailed information for each object like type, class name, address, size and references to other objects can be obtained in the heap dump. Various tools help in analyzing heap dumps in Java. For instance, JDK itself provides jhat tool for analysing heap dump. Heap dumps are also used for analysing memory leaks which is a phenomenon that occurs when there are objects that are not used by the application anymore and the garbage collection is not able to free that memory as they are still shown as referenced objects.

__Following are the causes that result in memory leaks:__
- Continuously instantiating objects without releasing them.
- Unclosed connection objects (such as connections to the database) post the required operation.
- Static variables holding on to references of objects.
- Adding objects in HashMap without overriding hashCode() equals() method. If these methods are not included, then the hashmap will continuously grow without ignoring the duplicates.
- Unbounded caches.
- Listener methods that are uninvoked.

Due to this, the application keeps consuming more and more memory and eventually this leads to OutOfMemory Errors and can ultimately crash the application. We can make use of the Eclipse Memory Analyzer or jvisualVM tool for analysing heap dump to identify memory leaks.

----

## **How can we take a heap dump of a Java process?**

There are multiple ways for taking heap dump of Java process. Tools like jCmd, jVisualVM, jmap are available for this purpose. For example, if we are using jmap, then heap dump can be taken by running the below command:

```cmd
$ jmap -dump:live, file=/path/of/heap_dump.hprof  PID
```

This heap dump contains live objects that are stored in heap_dump.hprof file. Process ID (PID) of the Java process is needed to get the dump that can be obtained by using ps or grep commands.

----

## **How is J2EE different from Spring?**

| J2EE | Spring |
| ----- | ------- |
| J2EE is a standard or specification defined by Sun/Oracle which is used for web development. | Spring is a framework used for designing templates for an application. |
| J2EE has an Oracle-based license. | Spring is an open-source framework. |
| J2EE is based on a 3D framework- Logical Tiers, Client Tiers, and Presentation Tiers. | Spring is based on layered architecture having many modules that are made on top of the core container. |
| J2EE makes use of high-level object-oriented languages like Java. | Spring doesn’t have a specific programming model. |
| J2EE is faster. | Spring is slower than J2EE. |
| Makes use of JTA API with execution. | Spring provides a layer of abstraction to help JTA execution merchants. |

----

## **What are EAR, WAR, and JAR?**

EAR stands for Enterprise Archive file and it consists of web, EJB and client components all compressed and packed into a file called .ear file. EAR files allow us to deploy different modules onto the application server simultaneously.

WAR stands for Web Archive file and consists of all web components packed and compressed in a .war file. This file allows testing and deploying web applications easily in a single request.

JAR stands for Java Archive file. It consists of all libraries and class files that constitute APIs. These are packed and compressed in a file called the .jar file. These are used for deploying the entire application including classes and resources in a single request.

----

## **What do you know about Hibernate?**

Hibernate is an Object Relational Mapper framework in Java that provides a layer of abstraction for retrieving or modifying data in the database. It handles all the implementations internally and the developer need not worry about how the connections to the databases are made, how the data translation from Java application to Database and vice versa happens. Hibernate supports powerful object-oriented concepts like inheritance, association, polymorphism, compositions, collections that help in making queries using the Java approach by using HQL (Hibernate Query Language).

----

## **What are deployment descriptors used for?**

Servlets are server-side components that aid in developing powerful server-side applications. Ther are servers that are platform-independent and follow various protocols as per the application design. The most commonly used protocol is the HTTP protocol. In Java, we can create servlets by implementing the Servlet interface that has 3 lifecycle methods - init, service and destroy - and we can use the below classes for implementing servlets:

```java
javax.servlet.http.HttpServletRequest
javax.servlet.http.HttpServletResponse
javax.servlet.http.HttpSession.
```

----

## **Can you describe the phases of the servlet lifecycle?**

The below image describes the different phases of the servlet lifecycle:

There are five phases, are as follows:

__Classloading phase:__ The first step is to load the servlet class file (.class extension) by the web container.

__Instantiation phase:__ Next step is to instantiate the servlet by calling the default constructor.

__Initialize phase:__ In this phase, the init() method of the servlet is run where the servlet configuration will be assigned to the servlet. This is a lifecycle method provided by the Servlet interface which is run only once in the servlet lifetime.

__Request Handling phase:__ Here, the servlets provide services to different requests by making use of the service() method of the Servlet interface.

__Removal phase:__ In this phase, the destroy() lifecycle method of the Servlet interface will be called that is used for clearing the configuration and closing resources before servlet destruction. Post this, the garbage collection will take place.

----

## **How does a servlet application work?**

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

## **What do you understand by Java Message Service (JMS)?**

JMS is a Java-based API that is like a gateway to the message-oriented middleware like SonicMQ, IBM MQSeries etc. It provides a mechanism for sending and receiving messages by making use of the publishing/subscribe (1 message multiple receivers) model or point-to-point (1 message 1 receiver) paradigm from one client to another. 

The following image describes how 2 clients can communicate with each other utilizing JMS providers.

__Conclusion:__
J2EE defines standards and specifications for various components such as e-mailing, database connectivity, security, XML parsing, CORBA communication etc that help in developing complex, reliable, secure and distributed servlets and applications that follow the client-server model. It provides various API interfaces that act as standards between different vendor adapters and J2EE components. This ensures that the application components are not dependent on vendor codes. Due to this, J2EE has been very popular among Java developers in the field of software development.

----

## **Which of the following exception is thrown when the initialization of servlet fails?**

- RemoteException
- ServletException (true)
- SocketException
- IOException

----

## **Which of the following option is not a J2EE client?**

- JSP (true)
- Web Applications
- Applets
- Java Web Start clients

----

## **What is the directory path where the classes should be present for the application’s Classloader?**

- /root/lib/classes/
- /WEB-INF/lib/classes/
- /WEB-INF/classes/ (true)
- /root/classes/

----

## **What lifecycle method is called for the first time and only once by a servlet?**

- start()
- run()
- initialize()
- init() (true)

----

## **What is the scope of the response object?**

- page
- session
- response (true, local scope)
- request

----

## **Which of the below files have the EJB modules of the application?**

- .zip
- .jar (true)
- .war
- .ear

----

## **Which tier provides internal functionality to J2EE apps?**

- Enterprise Interface System Tier
- Presentation Tier
- Enterprise Java Beans Tier
- Web Tier

----

## **When is the destroy method of a filter called?**

- Only once at the end of the filter lifecycle
- After the doFilter method is executed
- Only once at the beginning of the filter lifecycle
- never called

----

## **Which of the following option is responsible for optimising byte codes to machine code?**

- JVM (true)
- JDK
- JRE
- JIT

----

## **Which of the following bean type is defined without client view interfaces?**

- Stateful Session bean
- Stateless Session bean (true)
- Message Driven Bean
- BMP Entity bean

### https://www.interviewbit.com/j2ee-interview-questions/

### https://www.softwaretestinghelp.com/j2ee-interview-questions-answers/

----

## **What are the components of J2EE applications?**

The components of J2EE applications include:

__Client-tier components:__ Run-on the client machine.
__Web tier components:__ Run-on the J2EE server.
__Business tier components:__ Run-on the J2EE server.
__Enterprise Information System software (EIS software):__ Runs on the EIS server.

----

## **What are the J2EE client types?**

J2EE client types are
- Applets
- Application clients
- Java Web Start enabled clients, by Java Web Start technology.
- Wireless clients, based on the Mobile Information Device Profile (MIDP) technology.

----

## **What is a J2EE container?**

The interface between a component and the low-level platform with specific functionality that supports the component is called a container. The application server maintains control and provides relevant services through an interface or framework calls as a container.

----

## **What are defined as web components?**

Java Servlets and Java server pages technology components are identified as web components. Servlets dynamically receive requests and make responses. JSP server pages also behave as Java Servlets but facilitate to create more static content.

----

## **Describe the MVC on struts?**

MVC stands for Model View Controller. Each section in the Model View Controller can be described as follows:

Model: Model represents the internal state of the system as a set of single or many Java Beans.
View: Most often the view is constructed using Java Server Pages (JSP) technology.
Controller: The controller is the process that focuses on receiving client requests and produce the next level of a user interface according to the request. The primary component of the controller in the framework is the “ActionServlet” servlet class.

----

## **Define JSF?**

JSF stands for Java Server Faces. It is the user interface (UI) designing framework for Java Web application developments. There is a set of reusable UI components associated with JSF. Also, JSF has based on Model-View-Controller (MVC) design concepts and patterns. The automated data saving process from form to server and display at the client side is also handled by JSF.

----

## **What is Hashtable?**

Hashtable is a collection synchronized object. It allows null value but not the duplicate values. Hashtable is like a HashMap.

----

## **Define Hibernate?**

Hibernate is an open-source object-relational mapping and query service which facilitates writing Hibernate Query Language (HQL) scripts instead of Structured Query Language (SQL) scripts.

It is a fast and easy process than writing native SQL. Hibernate has more powerful object-oriented contents like associations, inheritance, and polymorphism. Also, it has powerful compositions and collections. Hibernate allows making queries using a Java-based approach.

----

## **What are the identified limitation of hibernate?**

Slower in action: In execution of HQL queries take more time than it executes directly.
Only composite key support is available and it prevents advanced query options.
No shared value type references are available.

----

## **What are the identified advantages of hibernate?**

Advantages are:

Database and vendor independence application.
Standard Object-relational mapping support.
Domain object mapping for a relational database.
Better performance than Java Database Connectivity.
Java Persistence API based applications.

----

## **Describe ORM?**E

Object-Relational mapping (ORM) can be described as follows:

The mapped objects in a Java class to the tables of the relational database using metadata describes the database and object mapping. The working method is to transform data from one representation to another.

----

## **What are the advantages of Object-Relational Mapping (ORM)?**

Advantages are:

Productivity: Reduced time for data access coding with the help of automatic code creation base on the defined data model.
Maintainability: All code generated from ORM are well tested. Only the developer is required to create the correct functionality
Performance: The code generated from ORM completely manages the data access needs of the application. No need to create any data access code. Also, the code is optimized to speed up the data access process.
Vendor independence: The code generated from ORM does not depend on the vendor. This is to increase the portability of the application.

----

## **What is the use of method save()?**

In hibernate, this method is used to stores an object into the database. There is a check for duplicate records before inserting it.

----

## **What is the use of method saveorupdate()?**

In hibernate, method saveorupdate() is used to update an object using the identifier. When the value for the identifier is NULL then the method is directed to call save().

----

## **What is the difference between load() and get()?**

When the object is not available in either cache or database, the load() method throws an exception. No null values are returned from the load() method.

```java
import org.hibernate.Session;
import org.hibernate.SessionFactory;
import org.hibernate.cfg.Configuration;
import com.example.entity.Employee;

public class Main {
    public static void main(String[] args) {
        // Create a Hibernate SessionFactory
        SessionFactory sessionFactory = new Configuration()
                .configure("hibernate.cfg.xml")
                .addAnnotatedClass(Employee.class)
                .buildSessionFactory();

        // Open a Hibernate session
        Session session = sessionFactory.getCurrentSession();

        try {
            // Begin a transaction
            session.beginTransaction();

            // Load an Employee object from the database
            Employee employee = session.load(Employee.class, 1L);

            // Access the properties of the loaded Employee object
            System.out.println("Employee ID: " + employee.getId());
            System.out.println("Employee Name: " + employee.getName());
            System.out.println("Employee Salary: " + employee.getSalary());

            // Commit the transaction
            session.getTransaction().commit();
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            // Close the session and release resources
            session.close();
            sessionFactory.close();
        }
    }
}
```

When the object is not available in either cache or database, get() returns null.

```java
import org.hibernate.Session;
import org.hibernate.SessionFactory;
import org.hibernate.cfg.Configuration;
import com.example.entity.Employee;

public class Main {
    public static void main(String[] args) {
        // Create a Hibernate SessionFactory
        SessionFactory sessionFactory = new Configuration()
                .configure("hibernate.cfg.xml")
                .addAnnotatedClass(Employee.class)
                .buildSessionFactory();

        // Open a Hibernate session
        Session session = sessionFactory.getCurrentSession();

        try {
            // Begin a transaction
            session.beginTransaction();

            // Get an Employee object from the database
            Employee employee = session.get(Employee.class, 1L);

            // Access the properties of the retrieved Employee object
            System.out.println("Employee ID: " + employee.getId());
            System.out.println("Employee Name: " + employee.getName());
            System.out.println("Employee Salary: " + employee.getSalary());

            // Commit the transaction
            session.getTransaction().commit();
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            // Close the session and release resources
            session.close();
            sessionFactory.close();
        }
    }
}
```

----

## **What is meant by connection pooling?**

Connection pooling is a mechanism to re-use the existing connections. The pooling mechanism maintains a number of already created object connections and when there is a demand, the mechanism directly uses the existing connection without creating a new one.

Example

1. Add the Apache Commons DBCP dependency to your project. You can include it in your Maven project by adding the following dependency to your pom.xml file:

```xml
<dependency>
    <groupId>org.apache.commons</groupId>
    <artifactId>commons-dbcp2</artifactId>
    <version>2.9.0</version>
</dependency>
```

2. Create a DataSource object that represents the connection pool configuration. This can be done using the BasicDataSource class provided by DBCP:

```java
import org.apache.commons.dbcp2.BasicDataSource;

public class ConnectionPool {
    private static final String DB_URL = "jdbc:mysql://localhost:3306/mydb";
    private static final String DB_USERNAME = "username";
    private static final String DB_PASSWORD = "password";

    private static BasicDataSource dataSource;

    static {
        dataSource = new BasicDataSource();
        dataSource.setUrl(DB_URL);
        dataSource.setUsername(DB_USERNAME);
        dataSource.setPassword(DB_PASSWORD);
    }

    public static BasicDataSource getDataSource() {
        return dataSource;
    }
}
```

3. Use the connection pool to obtain database connections whenever needed:

```java
import java.sql.Connection;
import java.sql.PreparedStatement;
import java.sql.ResultSet;
import java.sql.SQLException;
import org.apache.commons.dbcp2.BasicDataSource;

public class Main {
    public static void main(String[] args) {
        BasicDataSource dataSource = ConnectionPool.getDataSource();

        try (Connection connection = dataSource.getConnection()) {
            // Use the connection for database operations
            PreparedStatement statement = connection.prepareStatement("SELECT * FROM employees");
            ResultSet resultSet = statement.executeQuery();
            
            while (resultSet.next()) {
                // Process the result set
                int employeeId = resultSet.getInt("id");
                String employeeName = resultSet.getString("name");
                double employeeSalary = resultSet.getDouble("salary");
                
                System.out.println("Employee ID: " + employeeId);
                System.out.println("Employee Name: " + employeeName);
                System.out.println("Employee Salary: " + employeeSalary);
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}
```

In this example, we create a BasicDataSource object that represents the connection pool configuration. The DB_URL, DB_USERNAME, and DB_PASSWORD constants specify the database connection details. We then use the dataSource.getConnection() method to obtain a connection from the pool.

With connection pooling, the connections are managed by the pool and are automatically returned to the pool when the Connection object is closed. This allows for efficient reuse of connections and reduces the overhead of creating new connections for each database operation.

Note that connection pooling libraries like Apache Commons DBCP offer additional configuration options for controlling the size of the connection pool, maximum connection limits, and other advanced features.

----

## **Define the Collection types in Hibernate?**

One-to-many reference is defined as a collection. There are five main collection types associated with J2EE. They are: Set type, List type, Array type, Map type, Bag type

----

## **Define a thin client?**

A program interface that does not have any operations like database queries, complex business rules or any connection to the third-party application is called a thin client.

```java
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.io.PrintWriter;
import java.net.Socket;

public class ThinClient {
    public static void main(String[] args) {
        try {
            // Establish a connection with the server
            Socket socket = new Socket("localhost", 8080);

            // Create input and output streams for communication
            BufferedReader input = new BufferedReader(new InputStreamReader(socket.getInputStream()));
            PrintWriter output = new PrintWriter(socket.getOutputStream(), true);

            // Send a request to the server
            output.println("GET /api/data HTTP/1.1");
            output.println("Host: localhost");
            output.println();

            // Receive and display the response from the server
            String response;
            while ((response = input.readLine()) != null) {
                System.out.println(response);
            }

            // Close the connection
            socket.close();
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

In this example, the thin client establishes a socket connection with a server (assumed to be running on localhost at port 8080). It then creates input and output streams to send and receive data to and from the server.

The client sends an HTTP GET request to the server by writing the request headers to the output stream. In this case, it sends a simple GET request to retrieve data from an API endpoint.

After sending the request, the client reads the response from the server line by line using the input stream and displays it on the console.

Finally, the client closes the socket connection.

Note that this example assumes a basic understanding of socket programming and HTTP communication. The server-side implementation for handling the client request and providing the desired response is not included here, as it would depend on the specific server application or API being used.

----

## **Describe the file types *.ear, * .jar and *.war?**

*.jar files – Property file containing libraries, resources, and accessories are included with the *.jar file extension.
*.war files – The files that are required for the development of web application (HTML, java scripts, JSP) are included with a *.war file extension.
*.ear files – The files for Enterprise Java Beans modules for the application are saved as *.ear files.

----

## **How spring is related to J2EE?**

Spring is an open-source application that reduces the complexity of enterprise application development. Spring is based on an inversion of control or dependency injection design patterns.

----

## **What are the advantages of using spring for application development?**

Plain Old Java Object (POJO) based development facilitates to re-use existing components.
Possible to reduce development cost by improving the productivity of the application development.
Improve the testability of application with dependency injection.
Improve maintainability with reduced code coupling.
No need to have an application server and works on enterprise service.

----

## **Discuss the benefit of the Spring Framework?**

Benefits are as follows:

Possibility to organize middle-tier objects in an efficient way.
Easy initialization for properties.
Easily testable components.
Lightweight container.
Possibilities to use configuration management service of spring in any runtime environment with whatever architectural layer.

----

## **Describe servlet?**

The Server-side component that provides a powerful mechanism to create server-side programs is called a servlet. There are servlets available with a design for various protocols. Servlet is also server and platform-independent. The most commonly used protocol for the servlet is Hypertext Transfer Protocol (HTTP). Also, a servlet is a pure java object.

----

## **Describe the phases of the servlet lifecycle?**

The phases of servlet lifecycle are:

Classloading phase – Web container loads the servlet class file (*.class).
Instantiation phase – By calling default no-arg constructor, the servlet class gets Instantiated.
Initialize phase – The method Init () called in this phase in only one time of the lifetime of a servlet. Servlet configuration is assigned to the servlet.
Request Handling phase – In this phase, only servlets spends most of the time. Servlet provides the services to various requests by calling Service ().
Removal phase – The destroy () function is called before servlet destruction. Garbage collection occurs later.

----

## **What are the different types of JSP tags?**

There are 4 different types of tags associated with JSP. They are mentioned below:
- Directives
- Declarations
- Scriptlets
- Expressions

----

## **Describe the action form?**

A Java bean that is associated with single or multiple action mapping is called an action form. Action form objects are automatically populated at the server end when data has been entered from the client side through a user interface (UI).

Session states of a web application are maintained by action forms.

----

## **Describe the Secure Socket Layer (SSL)?**

The technology that is used to communicate between the web server and the web browser is called Secure Socket Layer (SSL). More specifically, SSL is a protocol that describes how algorithms are to be used in encryption.

The technology establishes an encrypted link between two parties and this link is allowed to secure transmission of sensitive information such as login credentials, credit/debit card information and social security numbers.

----

## **What is id URL?**

URL stands for __Uniform Resource Locator__ and it is the textual reference writing standard to an arbitrary piece of data in the World Wide Web (www). The general structure of the URL is as follows:

```cmd
protocol://host/local info
```

protocol – Protocol is for fetching the object (example: HTTP, FTP)
host – Internet name of the targeted host.
local info – String is passed to the protocol handler on the remote host. In many cases, it is a file name with an extension.

----

## **What is URN?**

URN stands for the Uniform Resource Name. It is a unique identifier that identifies an entity. But the information on where the entity is located is not available.

----

## **What are the steps associated with the servlet life cycle?**

The following steps are associated with the servlet life cycle:
1. Loading of the servlet class.
2. Instantiation of Servlet.
3. Execution of the init method.
4. Request handling phase. In this phase, service methods are called.
5. Removal from the service phase. In this phase, the destroy method is called.

----

## **Is Servlet is pure java object or not?**

Yes, Servlet is a pure java object.

----

## **What is EJB?**

EJB stands for Enterprise Java Beans. It is the server-side component that executes in EJB container and encapsulates the business logic for the enterprise application.

----

## **What are the system services of the EJB container?**

EJB Container provides the following system services:
- Persistence
- Security
- Transaction
- Connection pooling
- Component lifecycle management
- Threading

----

## **What are the design principles for EJB?**

Design principle includes:

The behavior of the EJB application is specified by interfaces.
EJB applications are loosely coupled and tired.
Implementation is hidden from the client-side.
The EJB container supports the application developer.
The API to the application is in session tier.
The API to the data sources is in the entity tier.

----

## **What are the advantages of EJB components?**

Advantages are:

There is support for the integration of components from different vendors.
Possibility to authorize the EJB component’s detailed knowledge of the environment.
Possibility to assemble applications from separate component sources.
Interaction with its clients is entirely specified in terms of Java interfaces.
Portability support.
It does not maintain resources.

----

## **What are the Basic and subtypes of Enterprise Java Beans (EJB)?**

Two main types and subtypes of EJB are as follows:

Session Beans
Stateful session beans
Stateless session beans
Entity Beans
Bean Managed Persistence (BMP)
Container-Managed Persistence (CMP)
Message Driven Beans

----

## **What is the description of the expression element?**

Answer: The expressions used for writing dynamic content back to the client browser are called expression elements.

----

## **What are the two types of comments supported by JSP?**

Two types of comments supported by JSP are:
- HTML comment
- JSP comment

----

## **What is called the JSP directive?**

JSP directive is the mechanism to provide metadata information to web containers about the JSP file. In the translation and compilation phases of the JSP life cycle, this Metadata is used by the web container.

----

## **What are the different types of JSP directive?**

There are 3 different types of JSP directives available. These are:
- Page directive
- Include directive
- Taglib directive

### https://www.softwaretestinghelp.com/j2ee-interview-questions-answers

# tps://www.javatpoint.com/j2ee-interview-questions

----

## **hat do you understand by J2EE?**

J2EE stands for Java 2 Enterprise Edition. The functionality of J2EE is developing and deploying multi-tier web-based enterprise applications. The J2EE platform is the combination of a set of services, application programming interfaces (APIs), and protocols. The J2EE platform adds the capabilities required to provide a complete, stable, secure, and fast Java platform at the enterprise level.

----

## **What do you mean by J2EE Module?**

A J2EE module is a software unit that consists of one or more J2EE components for the same container type with one deployment descriptor of that type. Modules can be easily deployed or assembled into J2EE applications.

----

## **What are the four types of J2EE modules?**
- Application Client Module
- WEB Module
- Enterprise JavaBeans Module
- Resource Adapter Module

----

## **What does the application client module contain?**

Application client module contains the following:
- Class files
- Client deployment descriptor
- It is packaged as JAR files with a .jar extension.

----

## **What does the web module contain?**

The web module contains the following:
- JSP (Java Server Pages) files
- Class files for servlets
- Web deployment descriptor
- GIF (Graphics Interchange Format) and HTML (Hypertext Markup Language) files
These modules are packaged as JAR files with a .war (Web Archive) extension.

----

## **What does Enterprise JavaBeans module contain?**

The Enterprise JavaBeans (EJB) module contains the following:
- Class files for enterprise beans
- An EJB deployment descriptor
- These modules are packaged as JAR files with a .jar extension.

----

## **What does resource adapt module contain?**

The resource adapter module contains the following:
- Java interfaces
- Classes
- Native libraries
- Other documentation
- Resource Adapter deployment descriptor
These modules are packaged as JAR files with a .rar (Resource Adapter Archive) extension.

----

## **What are the main components of the J2EE application?**

A J2EE component is assembled into a J2EE application with its related classes and files. It can also communicate with other components. The J2EE defines the following main components:
- Application clients components.
- Java Servlet and JavaServer Pages technology components.
- Business Components (Enterprise JavaBeans).
- Resource adaptor components.

----

## **What is considered as a web component?**

Java Servlet and Java Server Pages technology components are considered as web components. Servlets are based on Java programming language which dynamically receives requests and generates responses. Java Server pages execute as servlets and allow a more natural approach to creating static content.

----

## **What are the types of J2EE clients?**

- Applets
- Application clients
- Java Web Start-enabled clients
- Wireless clients

----

## **What do you understand by a word applet?**

An applet is a J2EE component that typically executes in a web browser. It can also be executed in a variety of other applications or devices that support the applet programming model.

----

## **What is the container?**

A container is the runtime support of a system level entity. Containers provide components with features such as lifecycle management, security, deployment, and threading.

----

## **What is an "applet container"?**

A container that provides support for the applet programming model is known as "applet container."


----

## **What do you understand by a thin client?**

A thin client is a light-weight interface to the application that does not support operations like query database, execute complex business rules, or connect to legacy applications.

----

## **What is JavaServer Faces (JSF)?**

JavaServer Faces is a user interface (UI) designing framework which is used for Java-based web applications. JavaServer Faces provides a set of reusable UI components- a standard for web applications. JSF is based on the MVC design pattern. It automatically saves the form data to the server and populates the form dates when display on the client side.

1. Create a new Java project in your preferred IDE.

2. Add the JSF library to your project's classpath. The specific steps may vary depending on your IDE.

3. Create a new JavaServer Faces Managed Bean called "HelloBean.java" in your project's source folder:

```java
import javax.faces.bean.ManagedBean;
import javax.faces.bean.RequestScoped;

@ManagedBean
@RequestScoped
public class HelloBean {
    private String name;
    private String message;

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getMessage() {
        return message;
    }

    public void sayHello() {
        message = "Hello, " + name + "!";
    }
}
```

4. Create a JSF XHTML file called "hello.xhtml" in the web content folder of your project:

```html
<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml"
      xmlns:h="http://java.sun.com/jsf/html"
      xmlns:f="http://java.sun.com/jsf/core">
<head>
    <title>Hello JSF</title>
</head>
<body>
    <h:form>
        <h:inputText value="#{helloBean.name}" />
        <h:commandButton value="Say Hello" action="#{helloBean.sayHello}" />
    </h:form>

    <h:outputText value="#{helloBean.message}" rendered="#{not empty helloBean.message}" />
</body>
</html>
```

5. Configure the JSF servlet mapping in the web.xml file:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<web-app version="3.0" xmlns="http://java.sun.com/xml/ns/javaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://java.sun.com/xml/ns/javaee http://java.sun.com/xml/ns/javaee/web-app_3_0.xsd">
    <display-name>JSFExample</display-name>

    <servlet>
        <servlet-name>FacesServlet</servlet-name>
        <servlet-class>javax.faces.webapp.FacesServlet</servlet-class>
        <load-on-startup>1</load-on-startup>
    </servlet>

    <servlet-mapping>
        <servlet-name>FacesServlet</servlet-name>
        <url-pattern>*.xhtml</url-pattern>
    </servlet-mapping>
</web-app>
```

6. Run the application on a servlet container (e.g., Apache Tomcat).
7. Access the application using the following URL: http://localhost:8080/your-project-name/hello.xhtml.

----

## **What is an EJB platform?**

EJB stands for The Enterprise JavaBeans. EJB platform manages functions such as transaction and state management, resource pooling, multithreading, and simple searches while you concentrate on writing business logic.

----

## **What do you mean by the deployment descriptor?**

A deployment descriptor is based on XML (Extensible Markup Language) that supports .xml extension. It is used to describe a component's deployment settings. A J2EE application and its module, both have its deployment descriptor.

----

## **Define the Struts in the J2EE framework?**

Struts is an application development framework based on MVC (Model-View-Controller) architecture. It is a combination of Java Servlets, JSP, Custom tags, and messages. It is used to design applications for large enterprises. It can be described as:

*Model*
The model defines the internal state of a system. It can be either single or a cluster of Java Beans based on app architecture.

*View*
JSP technology is used to design a view of any enterprise application.

*Controller*
A controller is used to manage the actions of users. It processes the client request and responds based on the request. The main component in the framework is a servlet of class ActionServlet. This servlet is configured by defining a set of ActionMappings.

----

## **Define Hashtable in J2EE?**

Hashtable is similar to HashMap except that Hashtable is synchronized. Hashtable is a cluster of synchronized objects where null values and duplicate values are not allowed.

----

## **Define Hibernate and HQL?**

Hibernate is an object-relational mapping and query service. In hibernate, we can write HQL (Hibernate Query Language) scripts instead of SQL, which saves lots of time and effort. Hibernate provides a more powerful association, inheritance, polymorphism, composition, and collections. We can process queries easily into the database using the Java objects. Hibernate also allows us to express queries using Java-based criteria.

----

## **What are the limitations of Hibernate?**

Following are some limitations of hibernate:
- Slower execution of queries.
- Only HQL support is available for composite keys.
- No shared references are available to the value type.

----

## **What are the major benefits of hibernate?**

Following are some major benefits of hibernate:
- Hibernate is independent of database and vendor so it is the portable framework.
- Domain objects can be mapped to the relational database.
- JPA support for standard ORM.
- Better database connectivity in Hibernate when compared to JDBC.

----

## **Define ORM and its working in J2EE?**

ORM refers to Object-Relational mapping. It is the object in a Java class which is mapped into the tables of a relational database using the metadata that describes the mapping between the objects and database. It transforms the data from one representation to another.

----

## **What is authorization?**

An authorization is a process by which access to a method or resource is determined. It relies on the determination of whether the principal associated with a request through authentication is in a given security role. A security role can be explained as a logical grouping of users defined by the person who assembles the application. A deployer maps the security roles to security identities. Security identities may be principles or groups in the operational environment.

----

## **Define authorization constraint?**

An authorization rule which determines who is permitted to access Web resource collection is known as authorization constraint.

----

## **How will you explain save() and saveorupdate() methods in hibernate?**

The *Save()* method in hibernate is used to store an object in the database. It creates a new entry if the record doesn't exist.

The *Saveorupdate()* method in hibernate is used for updating the object using the identifier. If the identifier is unavailable, this method calls save(). If the identifier is available, it will call the update method.

----

## **How will you explain load() and get() methods?**

__Load()__: If an object is missing in the Cache or database, Load() method will throw an exception. Load() method never returns null.

__Get()__: If an object is missing in the Cache or database, Get() method returns a null value, not the exception.

----

## **What is a web container in J2EE?**

An interface between a component and the low-level platform with defined functionality that is designed to support the component is defined as the web container in J2EE.

----

## **What is the concept of connection pooling?**

Connection pooling is a simple concept which is popular to reuse existing connections. It means that if object connections are already well-defined and connected, then they can be reused whenever there is a requirement instead of generating a new one.

----

## **What do you understand by the servlet?**

Servlet is a server-side component which provides full functionalities to create a server-side program. There are different servlets available with a specific design for a variety of protocols. The most popular type of protocol for the servlet is HTTP.Servlets, which use the classes in the java packages javax.servlet, javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse, javax.servlet.http.HttpSession;. All servlets must include the Servlet interface, which defines life-cycle methods.

----

## **Give some advantages of ORM (object-relational mapping)?**

__Productivity__
The automatic code is generated to reduce the overall data access time based on the data model defined.

__Performance__
The complete requirements of an application are managed by the automated code generated by the ORM, which means that there is no need for any extra code, and the overall data access process is made faster and optimized.

__Vendor Independent__
The generated code is independent of the vendor, which increases the overall portability of an application.
Maintainability
The code is well tested and generated by the ORM, and only a developer can understand the code perfectly.

----

## **Tell about the core interfaces of the hibernate framework?**

__Session Interface__

In Java, the HttpSession interface is a part of the Java Servlet API and provides a way to store information about a user session on the server-side. It allows you to maintain stateful information across multiple HTTP requests and responses.

Here's an example that demonstrates the usage of HttpSession:

```java
import javax.servlet.ServletException;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import javax.servlet.http.HttpSession;
import java.io.IOException;

public class SessionExampleServlet extends HttpServlet {

    protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
        // Get the HttpSession object associated with the request
        HttpSession session = request.getSession();

        // Store a value in the session
        session.setAttribute("username", "JohnDoe");

        // Retrieve the value from the session
        String username = (String) session.getAttribute("username");

        response.getWriter().println("Username from session: " + username);
    }
}

```


__SessionFactory Interface__

In Java, the SessionFactory interface is part of the Hibernate framework, which is an Object-Relational Mapping (ORM) tool. The SessionFactory is responsible for creating and managing Hibernate Session objects, which are used to interact with the database.

Here's an example that demonstrates the usage of the SessionFactory interface:

```java
import org.hibernate.Session;
import org.hibernate.SessionFactory;
import org.hibernate.cfg.Configuration;

public class HibernateExample {

    public static void main(String[] args) {
        // Create the Hibernate configuration
        Configuration configuration = new Configuration();
        configuration.configure("hibernate.cfg.xml");

        // Build the SessionFactory
        SessionFactory sessionFactory = configuration.buildSessionFactory();

        // Open a new session
        Session session = sessionFactory.openSession();

        // Perform database operations using the session
        // ...

        // Close the session and the SessionFactory
        session.close();
        sessionFactory.close();
    }
}
```

__Configuration Interface__

In Java, the Configuration interface is part of the Hibernate framework and is used to configure Hibernate and specify various settings for the persistence layer. It allows you to customize Hibernate's behavior and define the mappings between Java classes and database tables.

Here's an example that demonstrates the usage of the Configuration interface:

```java
import org.hibernate.Session;
import org.hibernate.SessionFactory;
import org.hibernate.cfg.Configuration;

public class HibernateExample {

    public static void main(String[] args) {
        // Create the Hibernate configuration
        Configuration configuration = new Configuration();
        configuration.configure("hibernate.cfg.xml");

        // Build the SessionFactory
        SessionFactory sessionFactory = configuration.buildSessionFactory();

        // Open a new session
        Session session = sessionFactory.openSession();

        // Perform database operations using the session
        // ...

        // Close the session and the SessionFactory
        session.close();
        sessionFactory.close();
    }
}
```

In this example, we create and use a Configuration object to configure Hibernate. Here's a breakdown of the code:

Configuration configuration = new Configuration();: We create a new Configuration object, which is used to configure Hibernate.

configuration.configure("hibernate.cfg.xml");: We load the configuration from a specific XML file. In this example, the file is named hibernate.cfg.xml. The configuration file typically includes properties like database connection details, Hibernate dialect, mapping files, etc.

SessionFactory sessionFactory = configuration.buildSessionFactory();: We build the SessionFactory using the configuration. This step creates the SessionFactory object based on the provided configuration. The SessionFactory is an expensive object to create and should typically be created once during the application's startup.

Session session = sessionFactory.openSession();: We open a new Session from the SessionFactory. The Session represents a single unit of work with the database and provides methods for querying, inserting, updating, and deleting entities.

Perform database operations using the Session: Once you have a Session, you can use it to perform database operations, such as querying data, saving new entities, updating existing entities, or deleting records.

session.close();: After you are done with the Session, you should close it to release resources and ensure proper cleanup.

sessionFactory.close();: Finally, you should close the SessionFactory when you are done using it, typically during the application shutdown.

The Configuration interface allows you to set up and customize Hibernate's behavior by specifying properties and mappings. It serves as a central point to configure Hibernate before building the SessionFactory and starting database interactions with the help of Session objects.

__Transaction Interface__

In Java, the Transaction interface is part of the Java Persistence API (JPA) and is used to manage transactions in a database environment. It provides methods to control the transaction boundaries, commit or roll back the transaction, and set other transaction-related properties.

The Transaction interface is typically obtained from the EntityManager object, which represents the persistence context and is responsible for managing entities and database operations.

Here's an example that demonstrates the usage of the Transaction interface:

```java
import javax.persistence.EntityManager;
import javax.persistence.EntityManagerFactory;
import javax.persistence.EntityTransaction;
import javax.persistence.Persistence;

public class JpaExample {

    public static void main(String[] args) {
        // Create the EntityManagerFactory
        EntityManagerFactory emf = Persistence.createEntityManagerFactory("myPersistenceUnit");

        // Create the EntityManager
        EntityManager em = emf.createEntityManager();

        // Get the EntityTransaction
        EntityTransaction transaction = em.getTransaction();

        try {
            // Begin the transaction
            transaction.begin();

            // Perform database operations using the EntityManager
            // ...

            // Commit the transaction
            transaction.commit();
        } catch (Exception e) {
            // Roll back the transaction in case of an exception
            if (transaction.isActive()) {
                transaction.rollback();
            }
        } finally {
            // Close the EntityManager
            em.close();
        }

        // Close the EntityManagerFactory
        emf.close();
    }
}
```

In this example, we obtain a Transaction object from the EntityManager. Here's a breakdown of the code:

EntityManagerFactory emf = Persistence.createEntityManagerFactory("myPersistenceUnit");: We create an EntityManagerFactory using a persistence unit name. The persistence unit is defined in the persistence.xml file, which specifies the database connection details and other JPA configurations.

EntityManager em = emf.createEntityManager();: We create an EntityManager from the EntityManagerFactory. The EntityManager represents the persistence context and is used to perform database operations and manage entities.

EntityTransaction transaction = em.getTransaction();: We obtain the Transaction object from the EntityManager. The Transaction interface allows us to manage the transaction boundaries and perform commit or rollback operations.

transaction.begin();: We begin the transaction by calling the begin() method. This marks the starting point of the transaction.

Perform database operations using the EntityManager: Within the try block, you can perform various database operations using the EntityManager, such as querying data, saving new entities, updating existing entities, or deleting records.

transaction.commit();: If all the database operations within the transaction are successful, we commit the transaction using the commit() method. This saves the changes to the database permanently.

Catch exceptions and roll back the transaction: If an exception occurs during the transaction, we catch the exception, roll back the transaction using the rollback() method, and handle any necessary error handling or logging.

em.close();: Finally, we close the EntityManager to release resources and ensure proper cleanup.

emf.close();: We close the EntityManagerFactory when we are done using it, typically during the application shutdown.

The Transaction interface allows you to control the boundaries of a transaction, perform commit or rollback operations, and handle any exceptions or errors that occur during the transaction. It ensures that database operations are executed atomically and consistently.

__Query and Criteria Interface__

In Java, the Query and Criteria interfaces are part of the Java Persistence API (JPA) and provide different approaches to perform database queries.

Query Interface:
The Query interface allows you to create and execute dynamic queries against the database. It provides methods to define the query structure, set parameters, and retrieve the results.

Here's an example that demonstrates the usage of the Query interface:

```java
import javax.persistence.EntityManager;
import javax.persistence.EntityManagerFactory;
import javax.persistence.Persistence;
import javax.persistence.Query;
import java.util.List;

public class JpaQueryExample {

    public static void main(String[] args) {
        // Create the EntityManagerFactory
        EntityManagerFactory emf = Persistence.createEntityManagerFactory("myPersistenceUnit");

        // Create the EntityManager
        EntityManager em = emf.createEntityManager();

        try {
            // Create and execute the query
            String jpql = "SELECT e FROM Employee e WHERE e.department = :dept";
            Query query = em.createQuery(jpql);
            query.setParameter("dept", "IT");

            List<Employee> resultList = query.getResultList();

            // Process the query results
            for (Employee employee : resultList) {
                System.out.println(employee.getName());
            }
        } finally {
            // Close the EntityManager
            em.close();
        }

        // Close the EntityManagerFactory
        emf.close();
    }
}
```


In Java, the Query and Criteria interfaces are part of the Java Persistence API (JPA) and provide different approaches to perform database queries.

Query Interface:
The Query interface allows you to create and execute dynamic queries against the database. It provides methods to define the query structure, set parameters, and retrieve the results.
Here's an example that demonstrates the usage of the Query interface:

java
Copy code
import javax.persistence.EntityManager;
import javax.persistence.EntityManagerFactory;
import javax.persistence.Persistence;
import javax.persistence.Query;
import java.util.List;

public class JpaQueryExample {

    public static void main(String[] args) {
        // Create the EntityManagerFactory
        EntityManagerFactory emf = Persistence.createEntityManagerFactory("myPersistenceUnit");

        // Create the EntityManager
        EntityManager em = emf.createEntityManager();

        try {
            // Create and execute the query
            String jpql = "SELECT e FROM Employee e WHERE e.department = :dept";
            Query query = em.createQuery(jpql);
            query.setParameter("dept", "IT");

            List<Employee> resultList = query.getResultList();

            // Process the query results
            for (Employee employee : resultList) {
                System.out.println(employee.getName());
            }
        } finally {
            // Close the EntityManager
            em.close();
        }

        // Close the EntityManagerFactory
        emf.close();
    }
}
In this example, we use the Query interface to execute a JPQL (Java Persistence Query Language) query. Here's a breakdown of the code:

String jpql = "SELECT e FROM Employee e WHERE e.department = :dept";: We define a JPQL query string. In this example, we select employees from the "Employee" entity where the department is specified as a parameter.

Query query = em.createQuery(jpql);: We create a Query object by passing the JPQL query string to the createQuery() method of the EntityManager.

query.setParameter("dept", "IT");: We set the value of the named parameter ":dept" to "IT" using the setParameter() method.

List<Employee> resultList = query.getResultList();: We execute the query and retrieve the results as a list of Employee objects using the getResultList() method.

Process the query results: We iterate over the list of Employee objects and perform the necessary operations.

Criteria Interface:
The Criteria interface provides a type-safe and object-oriented way to construct queries dynamically. It allows you to define query criteria using a fluent API without writing any SQL or JPQL statements directly.

Here's an example that demonstrates the usage of the Criteria interface:

```java
import javax.persistence.EntityManager;
import javax.persistence.EntityManagerFactory;
import javax.persistence.Persistence;
import javax.persistence.criteria.CriteriaBuilder;
import javax.persistence.criteria.CriteriaQuery;
import javax.persistence.criteria.Predicate;
import javax.persistence.criteria.Root;
import java.util.List;

public class JpaCriteriaExample {

    public static void main(String[] args) {
        // Create the EntityManagerFactory
        EntityManagerFactory emf = Persistence.createEntityManagerFactory("myPersistenceUnit");

        // Create the EntityManager
        EntityManager em = emf.createEntityManager();

        try {
            // Create CriteriaBuilder and CriteriaQuery
            CriteriaBuilder criteriaBuilder = em.getCriteriaBuilder();
            CriteriaQuery<Employee> criteriaQuery = criteriaBuilder.createQuery(Employee.class);
            Root<Employee> root = criteriaQuery.from(Employee.class);

            // Define query criteria
            Predicate departmentPredicate = criteriaBuilder.equal(root.get("department"), "IT");
            Predicate salaryPredicate = criteriaBuilder.greaterThan(root.get("salary"), 50000);
            criteriaQuery.where(criteriaBuilder.and(departmentPredicate, salaryPredicate));

            // Execute the query
            List<Employee> resultList = em.createQuery(criteriaQuery).getResultList();

            // Process the query results
            for (Employee employee : resultList) {
                System.out.println(employee.getName());
            }
        } finally {
            // Close the EntityManager
            em.close();
        }

        // Close the EntityManagerFactory
        emf.close();
    }
}
```

In this example, we use the Criteria interface to construct a dynamic query. Here's a breakdown of the code:

CriteriaBuilder criteriaBuilder = em.getCriteriaBuilder();: We obtain a CriteriaBuilder instance from the EntityManager.

CriteriaQuery<Employee> criteriaQuery = criteriaBuilder.createQuery(Employee.class);: We create a CriteriaQuery object, specifying the result type as Employee.

Root<Employee> root = criteriaQuery.from(Employee.class);: We create a Root object that represents the entity type on which the query is based. In this case, we use the Employee entity.

Predicate departmentPredicate = criteriaBuilder.equal(root.get("department"), "IT");: We create a predicate to specify the department criterion, comparing the "department" attribute of the Employee entity with the value "IT".

Predicate salaryPredicate = criteriaBuilder.greaterThan(root.get("salary"), 50000);: We create a predicate to specify the salary criterion, checking if the "salary" attribute of the Employee entity is greater than 50000.

criteriaQuery.where(criteriaBuilder.and(departmentPredicate, salaryPredicate));: We combine the predicates using the and() method of the CriteriaBuilder to define the overall query criteria.

List<Employee> resultList = em.createQuery(criteriaQuery).getResultList();: We execute the query by passing the CriteriaQuery object to the createQuery() method of the EntityManager and retrieve the results as a list of Employee objects.

Process the query results: We iterate over the list of Employee objects and perform the necessary operations.

Both the Query and Criteria interfaces provide different approaches to construct and execute dynamic queries in JPA. The choice between them depends on the specific requirements and coding preferences of your application.

----

## **What is B2b?**

B2b indicates to business-to-business.

----

## **What is the file extension used for hibernate mapping file and hibernate configuration file?**

For hibernate mapping, the file name should be like filename.hbm.xml.

For hibernate configuration, the file name should be like hibernate.cfg.xml.

----

## **Define a way to add Hibernate mapping file in hibernate configuration file?**

It can be easily performed by:

```java
<mapping resource="filename.hbm.xml"/>  
```

----

## **What are the main components of multi-tier architecture?**

The main components of multi-tier architecture are:

Presentation Tier
The front-end component existing in this tier is used to display the presentation.

Resource Tier
The back-end component existing in this tier is used to communicate with the database.

Business Tier
The component existing in this tier is used to provide business logic for the system.

----

## **Explain JTA, JNDI, and JMS?**

JTA represents JAVA Transaction API, which is used for coordinating and managing transactions across the enterprise information system.

JNDI represents Java Naming Directory Interface, which is used for accessing data from directory services.

JMS represents the Java Messaging Service, which is used for receiving and sending messages through messaging systems.

----

## **Explain the J2EE tiers?**

J2EE has the following tiers:

*Client Tier*
It indicates to the browser from which request is processed to the server. The interfaces that are available in this tier are HTML browser, Java application, an applet, or a non-java application.


*Middle Tier*
It comprises of a presentation tier and integration tier. The UI (User Interface) is created in the presentation tier using JavaServer Pages. The business logic is written inside the business tier with the help of Enterprise Java Bean. The objects of the database are created in the integration tier.

*Backend*
It constitutes the Enterprise Information System (EIS) which is used to store the data.

----

## **Describe the EAR, WAR, and JAR?**

EAR stands for Enterprise Archive file. It consists of the components of the web, EJB, and client. All the components of the EAR are packed in a compressed file with the extension .ear.

WAR stands for a Web Archive file. It consists of all the components related to the web application. All the components are packed in a compressed file with the extension .war.

JAR stands for Java Archive file. It consists of all the class files and library files, which constitute an API (Application Programming Interface). All the components are packed in a compressed file with the extension .jar.

Each type of file (.ear, .war, and .jar) is processed uniquely by application servers, servlet containers, EJB containers, etc.

----

## **What do you understand by Spring?**

Spring is a light-weight open source framework for developing enterprise applications. It resolves the complexity of enterprise application development and provides easy development for the J2EE. It was initially written by Rod Johnson. It was released under the Apache 2.0 license in June 2003.

----

## **What are the different modules used in Spring?**

There are mainly seven core modules in spring:

The Core container module
Object/Relational mapping module
DAO module
Application context module
Aspect Oriented Programming
Web module
MVC module

----

## **What is action mapping?**

In action mapping, a user specifies action class for a particular URL, i.e., path and different target view, which means, forwards on to which request-response is forwarded. The ActionMapping defines the information that the ActionServlet knows about the mapping of a particular request to an instance of a specific Action class. The mapping is transferred to the execute() method of the Action class, enabling access to this information directly.

----

## **What do you understand by ActionForm?**

ActionForm is a Java bean which may associate one or more ActionMappings. A java bean changes to FormBean when a user extends a class org.apache.struts.action.ActionForm. ActionForm object is generally populated on the server side automatically, and the client enters data from UI. ActionForm manages the session state for a web application.

----

## **What is backing bean?**

A backing bean is a JavaBeans component which corresponds to JavaServer Pages that includes JavaServer Faces components. The backing bean describes the properties for the components on the page and methods which perform processing for the component.

This processing may include event handling, validation, and processing associated with navigation.

----

## **What is the build file?**

A build file is an XML file that consists of one or more asant targets. A target is a set of tasks that a user wants to get executed. When starting asant, a user can select which target is to be executed. If there is no target, then the default target of the project is executed.

----

## **What do you understand by business logic?**

Business logic is the code that includes the functionality of an application. In the EJB (Enterprise JavaBeans) architecture, this logic is implemented by the methods of an enterprise bean.

----

## **How will you explain CDATA?**

A CDATA is a predefined XML tag for the character data, which means "don't interpret these characters," it is similar to parsed character data (PCDATA), in which the standard rules of XML syntax apply. CDATA sections are used to show examples of XML syntax.

----

## **What do you mean by the Component Contract?**

The contract between the J2EE component and its container is known as the component contract. This type of contract includes:

Life-cycle management of the component
An interface which is used by instance to obtain various information and services from its container
List of services that every container must provide for its components.

----

## **What do you understand by Connector? Explain Connector Architecture?**

A connector is a standard extension mechanism for containers, which provides connectivity to enterprise information systems. It is specific to an enterprise information system and contains a resource adapter and application development tools for enterprise information system connectivity. The resource adapter is plugged into a container through its support for system-level contracts, defined in the Connector architecture.

An architecture for the integration of J2EE products with enterprise information systems is known as the connector architecture. A connector architecture consists of:

A resource adapter which is given by an enterprise information system vendor
A J2EE product that allows this resource adapter to plug in.
Connector architecture also defines a set of contracts which a resource adapter must support to plug into a J2EE product (e.g., transactions, security, and resource management).

### https://www.javatpoint.com/j2ee-interview-questions

### https://www.interviewkickstart.com/interview-questions/java-and-j2ee-interview-questions

----

## **What’s the difference between JVM Spec, JVM Runtime, and JVM Implementation?**

JVM spec is simply the specification of JVM. JVM implementation is the actual implementation of JVM by vendors. Meanwhile, JVM runtime is a running program supporting Java specified programs.

----

## **What is JIT?**

The Just-in-Time compiler improves the performance of Java apps by combining platform-neutral bytecode to the native machine code during run time.

----

## **What are JRE and JDK?**

JDK is a kit providing an environment to execute and develop the Java program. On the other hand, JRE is a kit that provides an environment to run (not develop) the Java program.

----

## **Define Locale?**

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

## **Define HQL?**

HQL (Hibernate Query Language) is an object-oriented query language. Unlike SQL, which works on tables and columns, HQL works on persistent objects and properties. HQL is a superset of Java Persistence Query Language (JPQL). This means that all JPQL queries are valid HQL queries, but all HQL queries are not JPQL queries

----

## **What is a Java thin client?**

Thin client is a lightweight client. A thin client connects to the cluster through a standard socket connection without becoming a part of the cluster topology. Thin client does not hold any data and is not used for computing calculations. It performs all operations through the standard node​.

----

## **What does URN mean?**

URN is an abbreviation for Uniform Resource Name. It is a unique identifier that identifies an entity. 

----

## **What are the uses of Spring?**

Spring is an open-source application development framework for enterprise Java. It is one of the most widely used frameworks for Java. Developers use Spring to develop high-performing, testable, and reusable code

----

## **What are the different phases that fall under the life cycle of a servlet?**

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

## **What are the different components in the multi-tier architecture?**

The presentation tier, Resource tier, and Business tier are the components of multi-tier architecture.

----

## **What are the different modules in Spring?**

The list of spring modules is
- Aspect-oriented programming
- DAO module
- O/R mapping module
- Core container module
- Web module
- Application context module.

----

## **What is a servlet?**

A servlet is a server-side component that provides development mechanisms for server-side programs. It makes use of classes available under a Java package.

----

## **Define the various phases in the life cycle of a servlet?**

The different phases are:
- Servlet instantiation
- Servlet class loading
- The init method
- Removal from the service
- Request handling

----

## **Define JMS, JNDI, and JTA?**

*JNDI*: It is Java Naming Directory Interface. It helps access information from the directory services.

*JMS*: It is a Java Messaging Service. It is responsible for receiving and sending messages through various messaging systems.

*JTA*: It is a Java Transaction API. It coordinates and manages the transaction in an enterprise information system.

----

## **What is connection pooling?**

Connection pooling is a practice generally used to extract already existing connections. These connections can be used instead of generating new connections.

----

## **Define hibernate proxy?**

It is an object proxy that includes the process of retrieving the objects until and unless you require them.

----

## **How will you create a SessionFactory?**

Configuration cfg = new Configuration(); cfg.addResource("dir/hibernate.hbm.xml"); cfg.setProperties( System.getProperties() ); SessionFactory sessions = cfg.buildSessionFactory();

----

## **Mention the collection types in hibernate?**

List, array, map, bag, set are the collection types in hibernate.

----

## **Mention the JSP tag types?**

JSP tags are divided into four categories:
- Declarations
- Directives
- Expressions
- Scriptlets

----

## **What is the minimum eligibility to become a Java developer?**

Becoming a Java developer requires a Bachelor’s degree in Computer Science or any related field. However, experience is equally important to appear for Java and J2EE interview questions.

----

## **Are Java and J2EE the same?**

Before appearing for Java and J2EE interview questions, you should have a common understanding of the difference between both these programming languages. J2EE is just an extension of Java SE, which is based on the Java programming language.
In simple words, J2EE is a part of Java featuring a powerful library set.

----

## **What are the four types of J2EE modules?**

The four types of J2EE modules are Application Client Module, WEB Module, Enterprise JavaBeans Module, and Resource Adapter Module.

----

## **What is J2EE?**

J2EE stands for Java 2 Platform, Enterprise Edition. The J2EE platform is used to create multi-tier, web-based applications by utilizing a set of protocols and application programming interfaces (APIs).

### https://www.interviewkickstart.com/interview-questions/java-and-j2ee-interview-questions

### https://career.guru99.com/top-50-j2ee-interview-questions

----

## **What is J2EE?**

J2EE means Java 2 Enterprise Edition. The functionality of J2EE is developing multitier web-based applications. The J2EE platform is consists of a set of services, application programming interfaces (APIs), and protocols.

----

## **What are the four components of J2EE application?**

Application clients components.
Servlet and JSP technology are web components.
Business components (JavaBeans).
Resource adapter components

----

## **What are types of J2EE clients?**

Applets
Application clients
Java Web Start-enabled clients, by Java Web Start technology.
Wireless clients, based on MIDP technology.
The video player is currently playing an ad. You can skip the ad in 5 sec with a mouse or keyboard

----

## **What is considered as a web component?**

Java Servlet and Java Server Pages technology components are web components. Servlets are Java programming language that dynamically receives requests and makes responses. JSP pages execute as servlets but allow a more natural approach to creating static content.

----

## **What is JSF?**

JavaServer Faces (JSF) is a user interface (UI) designing framework for Java web applications. JSF provides a set of reusable UI components, a standard for web applications. JSF is based on MVC design pattern. It automatically saves the form data to the server and populates the form date when display on the client side.

----

## **Define Hash table**
HashTable is just like Hash Map, Collection having a key(Unique), value pairs. Hashtable is a collection Synchronized object. It does not allow duplicate values or null values.

----

## **What is Hibernate?**

Hibernate is an open source object-relational mapping and query service. In hibernate we can write HQL instead of SQL which save developers to spend more time on writing the native SQL.

Hibernate has a more powerful association, inheritance, polymorphism, composition, and collections. It is a beautiful approach for persisting into the database using the Java objects. Hibernate also allows you to express queries using Java-based criteria.

----

## **What is the limitation of hibernate?**

Slower in executing the queries than queries are used directly.
Only query language support for composite keys.
No shared references to value types.

----

## **What are the advantages of hibernate?**

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

## **Difference between save and saveorupdate**

save() – This method in Hibernate is used to stores an object in the database. It inserts an entry if the record doesn’t exist, otherwise not.
saveorupdate () -This method in the hibernate is used for updating the object using identifier. If the identifier is missing this method calls save(). If the identifier exists, it will call update method.

----

## **Difference between load and get method?**

load() can’t find the object from cache or database, an exception is thrown, and the load() method never returns null.
get() method returns null if the object can’t be found. The load() method may return a proxy instead of a real persistent instance get() never returns a proxy.

----

## **How to invoke a stored procedure in hibernate?**

{ ? = call thisISTheProcedure() }

To invoke a stored procedure in Hibernate, you can use the org.hibernate.procedure.ProcedureCall interface. Here's an example of how to invoke a stored procedure using Hibernate:

```java
import org.hibernate.Session;
import org.hibernate.SessionFactory;
import org.hibernate.cfg.Configuration;
import org.hibernate.procedure.ProcedureCall;
import org.hibernate.procedure.ProcedureOutputs;

public class HibernateStoredProcedureExample {

    public static void main(String[] args) {
        // Create the Hibernate configuration
        Configuration configuration = new Configuration();
        configuration.configure("hibernate.cfg.xml");

        // Build the SessionFactory
        SessionFactory sessionFactory = configuration.buildSessionFactory();

        // Open a new session
        Session session = sessionFactory.openSession();

        try {
            // Create a ProcedureCall instance for the stored procedure
            ProcedureCall procedureCall = session.createStoredProcedureCall("your_stored_procedure_name");

            // Bind input parameters if necessary
            procedureCall.registerParameter("param1", String.class, ParameterMode.IN).bindValue("value1");
            procedureCall.registerParameter("param2", Integer.class, ParameterMode.IN).bindValue(123);

            // Execute the stored procedure
            ProcedureOutputs procedureOutputs = procedureCall.getOutputs();

            // Process the procedure outputs if necessary
            // ...

        } finally {
            // Close the session and the SessionFactory
            session.close();
            sessionFactory.close();
        }
    }
}
```

In this example, we invoke a stored procedure using Hibernate's ProcedureCall interface. Here's a breakdown of the code:

ProcedureCall procedureCall = session.createStoredProcedureCall("your_stored_procedure_name");: We create a ProcedureCall instance by calling the createStoredProcedureCall() method on the Hibernate Session. Replace "your_stored_procedure_name" with the name of your stored procedure.

procedureCall.registerParameter("param1", String.class, ParameterMode.IN).bindValue("value1");: If your stored procedure has input parameters, you can bind them using the registerParameter() method. Provide the parameter name, its Java type, and the parameter mode (IN, OUT, or INOUT). You can then set the parameter value using the bindValue() method.

ProcedureOutputs procedureOutputs = procedureCall.getOutputs();: We execute the stored procedure by calling the getOutputs() method on the ProcedureCall. This will execute the stored procedure and retrieve the outputs.

Process the procedure outputs if necessary: You can use the ProcedureOutputs object to access the outputs of the stored procedure and process them according to your requirements.

Make sure to configure your Hibernate mapping files or annotations properly to map the stored procedure and its parameters. Additionally, ensure that your database and the JDBC driver support stored procedures. The specific configuration may vary depending on your Hibernate version, database, and ORM setup.

----

## **What are the benefits of ORM?**

Productivity
Maintainability
Performance
Vendor independence

----

## **What are the Core interfaces of Hibernate framework?**

Session Interface
SessionFactory Interface
Configuration Interface
Transaction Interface
Query and Criteria Interface

----

## **What is the file extension used for hibernate mapping file?**

The name of the file should be like this: `filename.hbm.xml`

----

## **What is the file name of hibernate configuration file?**

The name of the file should be like this: `hibernate.cfg.xml`

----

## **How Hibernate is database independent explain?**

Only changing the full property full database can be replaced.

```xml
<property name="hibernate.dialect">org.hibernate.dialect.Oracle9Dialect</property> and
<property name="hibernate.connection.driver_class">oracle.jdbc.driver.OracleDriver</property>
```

----

## **How to add Hibernate mapping file in hibernate configuration file?**

```java
By <mapping resource="filename.hbm.xml"/>
```

----

## **Define connection pooling?**

Connection pooling is a mechanism reuse the connection which contains the number of already created object connection. So whenever it is necessary for an object, this mechanism is used to get objects without creating it.

----

## **What is the Hibernate proxy?**

An object proxy is just a way to avoid retrieving an object until you need it. Hibernate 2 does not proxy objects by default.

----

## **What do you create a SessionFactory?**

Configuration cfg = new Configuration(); cfg.addResource("dir/hibernate.hbm.xml"); cfg.setProperties( System.getProperties() ); SessionFactory sessions = cfg.buildSessionFactory();

----

## **What is HQL?**

HQL stands for Hibernate Query Language. Hibernate allows to the user to express queries in its portable SQL extension, and this is called as HQL. It also allows the user to express in native SQL.

----

## **What are the Collection types in Hibernate?**

Set, List, Array, Map, Bag are collection type in Hibernate.

----

## **What is a thin client?**

A thin client is a program interface to the application that does not have any operations like the query of databases, execute complex business rules, or connect to legacy applications.

----

## **Differentiate between .ear,  .jar and .war files?**

.jar files: These files are with the .jar extension. The .jar files contain the libraries, resources and accessories files like property files.
.war files: These files are with the .war extension. The .war file contains JSP, HTML, javascript and other files necessary for the development of web applications.
.ear files: The .ear file contains the EJB modules of the application.

----

## **What is the JSP tag?**

In JSP tags can be divided into four different types.

Directives
Declarations
Scriplets
Expressions

----

## **How to access web.xml init parameters from JSP page?**

For example, if you have:

```xml
<context-param> <param-name>Id</param-name> <param-value>this is the value</param-value></context-param>
```

You can access this parameter

```xml
<h:outputText value="#{initParam['Id']}"/>
```

----

## **What are JSP Directives?**

1.page Directives `<%@page language=”java” %>`
2. include Directives: `<%@ include file=”/header.jsp” %>`
3. taglib Directives `<%@ taglib uri=”tlds/taglib.tld” prefix=”html” %>`

----

## **What is the EAR file?**

An EAR file is a JAR file with an .ear extension. A J2EE application with all of its modules is delivered in an EAR file.

----

## **What will happen when you compile and run the following code?**

```java
public class Main
{
    public static void main(String argv[])
    {
        int array[]=new int[]{1,2,3};
        System.out.println(array [1]);
    }
}

// Output:
// 2
```

----

## **What are Struts?**

Struts framework is a Model-View-Controller(MVC) architecture for designing large-scale applications. It is a combination of Java Servlets, JSP, Custom tags, and message. Struts help you to create an extensible development environment for your application, based on published standards and proven design patterns. Model in many applications represents the internal state of the system as a set of one or more JavaBeans.The View is most often constructed using JavaServer Pages (JSP) technology.The Controller is focused on receiving requests from the client and producing the next phase of the user interface to an appropriate View component. The primary component of the Controller in the framework is a servlet of class ActionServlet. This servlet is configured by defining a set of ActionMappings.

Sure! Here's a simple example of a Struts application in Java:

Create a new Java project in your preferred IDE.

Add the necessary Struts dependencies to your project. You can use a build tool like Maven or Gradle, or manually download the JAR files and add them to your project's classpath. The core Struts library and its dependencies include:

struts-core.jar
struts-taglib.jar
struts-tiles.jar (optional, for tile-based layouts)
Create a struts.xml configuration file in the src directory of your project. This file will define the mapping between URLs, actions, and result pages. Here's a sample struts.xml configuration:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE struts PUBLIC "-//Apache Software Foundation//DTD Struts Configuration 2.3//EN" "http://struts.apache.org/dtds/struts-2.3.dtd">
<struts>
  <package name="default" namespace="/" extends="struts-default">
    <action name="hello" class="com.example.HelloAction">
      <result>/hello.jsp</result>
    </action>
  </package>
</struts>
```

Create a Java class called HelloAction in the com.example package. This class will define the logic for handling the "hello" action. Here's an example:

```java
package com.example;

import com.opensymphony.xwork2.ActionSupport;

public class HelloAction extends ActionSupport {
    private String message;

    public String execute() {
        message = "Hello, Struts!";
        return SUCCESS;
    }

    public String getMessage() {
        return message;
    }
}
```

Create a JSP file called hello.jsp in the WebContent directory. This file will display the message from the action class. Here's an example:

```html
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
<head>
    <title>Hello Struts</title>
</head>
<body>
    <h1>${message}</h1>
</body>
</html>
```

Configure your web application deployment descriptor (web.xml) in the WEB-INF directory. Add the following servlet mapping to route requests to Struts:

```xml
<servlet>
    <servlet-name>struts2</servlet-name>
    <servlet-class>org.apache.struts2.dispatcher.ng.servlet.StrutsServlet</servlet-class>
    <init-param>
        <param-name>config</param-name>
        <param-value>/WEB-INF/struts.xml</param-value>
    </init-param>
    <load-on-startup>1</load-on-startup>
</servlet>

<servlet-mapping>
    <servlet-name>struts2</servlet-name>
    <url-pattern>/*</url-pattern>
</servlet-mapping>
```

Deploy your application to a web server (e.g., Tomcat) and access the following URL in your browser: http://localhost:8080/your-app-context/hello. You should see the "Hello, Struts!" message displayed on the page.

This example demonstrates the basic structure of a Struts application, where requests are mapped to actions defined in the struts.xml configuration file. The actions handle the request and forward the user to a result page, such as a JSP.

----

## **What is ActionErrors?**

ActionErrors object that encapsulates any validation errors that have been found. If no errors are found, return null or an ActionErrors object with no recorded error messages.The default implementation attempts to forward to the HTTP version of this method. Holding request parameters  mapping and request  and returns set of validation errors, if validation failed; an empty set or null

```java
import com.opensymphony.xwork2.ActionSupport;

public class MyAction extends ActionSupport {
    private String username;
    private String password;

    public String execute() {
        // Validate the username and password
        if (username == null || username.isEmpty()) {
            addActionError("Username is required");
        }
        if (password == null || password.isEmpty()) {
            addActionError("Password is required");
        }

        // Handle any errors
        if (hasErrors()) {
            return INPUT;
        }

        // Process the login logic
        // ...

        return SUCCESS;
    }

    // Getters and setters for username and password

    public String getUsername() {
        return username;
    }

    public void setUsername(String username) {
        this.username = username;
    }

    public String getPassword() {
        return password;
    }

    public void setPassword(String password) {
        this.password = password;
    }
}
```

----

## **What is ActionForm?**

ActionForm is a Java bean that associates one or more ActionMappings. A java bean become FormBean when extend org.apache.struts.action.ActionForm class. ActionForm object is automatically populated on the server side which data has been entered by the client from UI. ActionForm maintains the session state for a web application.


In Struts 1.x, the ActionForm class is used to encapsulate and validate the user input from HTML forms. Here's an example of how to create and use an ActionForm in a Java class:

Create a Java class that extends org.apache.struts.action.ActionForm:

```java
import org.apache.struts.action.ActionForm;

public class LoginForm extends ActionForm {
    private String username;
    private String password;

    // Default constructor
    public LoginForm() {
    }

    // Getters and setters for the form fields
    public String getUsername() {
        return username;
    }

    public void setUsername(String username) {
        this.username = username;
    }

    public String getPassword() {
        return password;
    }

    public void setPassword(String password) {
        this.password = password;
    }

    // Additional validation or business logic methods
    // ...
}
```

In this example, the LoginForm class extends ActionForm and defines two fields: username and password. It also provides the corresponding getters and setters for these fields.

Configure the ActionForm in your struts-config.xml file:

```xml
<struts-config>
    <form-beans>
        <form-bean name="loginForm" type="com.example.LoginForm" />
    </form-beans>
    <action-mappings>
        <action path="/login" type="com.example.LoginAction" name="loginForm" scope="request">
            <forward name="success" path="/success.jsp" />
            <forward name="failure" path="/failure.jsp" />
        </action>
    </action-mappings>
</struts-config>
```

In this example, we define a form bean with the name "loginForm" and the corresponding class "com.example.LoginForm".

Create an action class to handle the form submission and process the input:

```java
import org.apache.struts.action.Action;
import org.apache.struts.action.ActionForm;
import org.apache.struts.action.ActionForward;
import org.apache.struts.action.ActionMapping;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

public class LoginAction extends Action {
    public ActionForward execute(ActionMapping mapping, ActionForm form, HttpServletRequest request, HttpServletResponse response) throws Exception {
        LoginForm loginForm = (LoginForm) form;

        // Get the username and password from the form
        String username = loginForm.getUsername();
        String password = loginForm.getPassword();

        // Perform validation or business logic
        if (username.equals("admin") && password.equals("password")) {
            return mapping.findForward("success");
        } else {
            return mapping.findForward("failure");
        }
    }
}
```

In this example, the LoginAction class extends Action and overrides the execute() method. Inside the method, we cast the ActionForm parameter to our specific LoginForm class and retrieve the username and password from the form.

We can perform validation or business logic on the form data and return an appropriate ActionForward. In this case, if the username is "admin" and the password is "password", we return the "success" forward, which will redirect the user to the success.jsp page. Otherwise, we return the "failure" forward, redirecting the user to the failure.jsp page.

Create the JSP files for success and failure pages (success.jsp and failure.jsp) in the appropriate location.
Note that this example is specific to Struts 1.x. Struts 2.x uses a different approach for handling forms.

----

## **What is action mapping?**

In action mapping, we specify action class for particular URL ie path and different target view ie forwards on to which request response will be forwarded.The ActionMapping represents the information that the ActionServlet knows about the mapping of a particular request to an instance of a particular Action class. The mapping is passed to the execute() method of the Action class, enabling access to this information directly.

Sure! In Struts 1.x, the ActionMapping class is used to map a URL pattern to an action class. Here's an example of how to define and use an action mapping in a Java class:

Configure the action mapping in your struts-config.xml file:

```xml
<struts-config>
    <action-mappings>
        <action path="/hello" type="com.example.HelloAction" name="helloForm" scope="request" validate="true">
            <forward name="success" path="/success.jsp" />
        </action>
    </action-mappings>
</struts-config>
```

In this example, we define an action mapping for the URL pattern "/hello". The type attribute specifies the fully qualified class name of the action class that will handle this URL pattern. The name attribute specifies the form bean name associated with this action. The scope attribute indicates the scope in which the form bean should be stored (e.g., request, session). The validate attribute specifies whether to perform form validation. The forward element defines the result forward for a successful execution of the action.

Create an action class to handle the action mapping:

```java
import org.apache.struts.action.Action;
import org.apache.struts.action.ActionForm;
import org.apache.struts.action.ActionForward;
import org.apache.struts.action.ActionMapping;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

public class HelloAction extends Action {
    public ActionForward execute(ActionMapping mapping, ActionForm form, HttpServletRequest request, HttpServletResponse response) throws Exception {
        // Perform any necessary logic or processing

        return mapping.findForward("success");
    }
}
```

In this example, the HelloAction class extends Action and overrides the execute() method. Inside the method, you can perform any necessary logic or processing for the action. The ActionMapping parameter provides access to the configuration defined in struts-config.xml. In this case, we simply return the "success" forward defined in the action mapping.

Create the JSP file for the success page (success.jsp) in the appropriate location.
When a user accesses the URL pattern "/hello" in the application, Struts will look for the corresponding action mapping defined in struts-config.xml. It will then instantiate the associated action class (HelloAction in this example) and call its execute() method. The action class can perform any necessary logic or processing and return the appropriate forward, which will determine the next page to display.

Note that this example is specific to Struts 1.x. Struts 2.x uses a different approach for action mappings.

----

## **What is the MVC on struts?**

MVC stands Model-View-Controller.

Model: Model in many applications represent the internal state of the system as a set of one or more JavaBeans.

View: The View is most often constructed using JavaServer Pages (JSP) technology.

Controller: The Controller is focused on receiving requests from the client and producing the next phase of the user interface to an appropriate View component. The primary component of the Controller in the framework is a servlet of class ActionServlet. This servlet is configured by defining a set of ActionMappings.

----

## **What are different modules in spring?**

There are seven core modules in spring
- The Core container module
- O/R mapping module (Object/Relational)
- DAO module
- Application context module
- Aspect Oriented Programming
- Web module
- MVC module

----

## **What is Bean Factory, have you used XMLBean factory?**

XmlBeanFactory is one of the implementation of bean Factory org.springframework.beans.factory.xml.XmlBeanFactory is used to creat bean instance defined in our xml file. BeanFactory factory = new XmlBeanFactory(new FileInputStream("beans.xml")); Or ClassPathResource resorce = new ClassPathResource("beans.xml"); XmlBeanFactory factory = new XmlBeanFactory(resorce);

----

## **What is Spring?**

Spring is a lightweight open source framework for the development of enterprise application that resolves the complexity of enterprise application development is also providing a cohesive framework for J2EE application development which is primarily based on IOC (inversion of control) or DI (dependency injection) design pattern.

----

## **What is the functionality of ActionServlet and RequestProcessor?**

Receiving the HttpServletRequest
Populating JavaBean from the request parameters
Displaying response on the web page Issues
Content type issues handling
Provide extension points

----

## **ActionServlet, RequestProcessor, and Action classes are the components of ..?**

Controller

----

## **What is default scope in Spring?**

Singleton.

----

## **What are advantages of Spring usage?**

Pojo based programming enables reuse component.
Improve productivity and subsequently reduce development cost.
Dependency Injection can be used to improve testability.
Spring required enterprise services without a need for the expensive application server.
It reduces coupling in code and improves maintainability.

----

## **What are the Benefits Spring Framework?**

Lightweight container
Spring can effectively organize your middle tier objects
Initialization of properties is easy. No need to read from a properties file
application code is much easier to unit test
Objects are created Lazily, Singleton – configuration
Spring’s configuration management services can be used in any architectural layer, in whatever runtime environment

----

## **Lifecycle interfaces in spring?**

1) InitializingBean <bean id="expInitBean" init-method="init"/> public class ExpBean { public void init() { // do some initialization code } } OR <bean id=" expInitBean "/> public class ExpBean implements InitializingBean { public void afterPropertiesSet() { // do some initialization code } } 2) DisposableBean <bean id="expInitBean" destroy-method="cleanup"/> public class ExpBean { public void cleanup() { // do some destruction code (like releasing pooled connections) } } OR <bean id="expInitBean"/> public class ExpBean implements DisposableBean { public void destroy() { // do some destruction code (like releasing pooled connections) } }

----

## **How to Create Object without using the keyword "new" in java?**

Without new, the Factory methods are used to create objects for a class. For example
Calender c=Calender.getInstance();
Here Calender is a class, and the method getInstance() is a Factory method which can create an object for Calendar class.

----

## **What is a servlet?**

Servlets is a server-side component that provides a powerful mechanism for developing server side programs. Servlets is a server, as well as platform-independent and Servlets, are designed for various protocols. Most commonly used HTTP protocols. Servlets use the classes in the java packages javax.servlet, javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse, javax.servlet.http.HttpSession;. All servlets must implement the Servlet interface, which defines life-cycle methods.

----

## **Servlet is pure java object or not?**

Yes, pure java object.

----

## **What are the phases of the servlet life cycle?**

The life cycle of a servlet consists of the following phases:

Servlet class loading
Servlet instantiation
 the init method
Request handling (call the service method)
Removal from service (call the destroy method)

### https://career.guru99.com/top-50-j2ee-interview-questions

### https://www.simplilearn.com/j2ee-interview-questions-answers-article

## **What is J2EE?**

J2EE, or Java Enterprise Edition, is a Java-based platform that combines services protocols with APIs (Application Programming Interfaces), giving users the ability to create enterprise-level applications that are multi-tiered, safe, stable, and quick. J2EE offers a variety of specifications for creating enterprise-level online applications, including web, enterprise, web service, and others.

----

## **What are the benefits of J2EE?**

Given below are the benefits of J2EE:

Faster time to market: J2EE employs the idea of containers to make development simpler. This supports the separation of business logic from lifecycle management and resources, allowing developers to concentrate more on the business logic than the infrastructure. The EJB (Enterprise JavaBeans) container, for example, handles threading, distributed communication, transaction management, scaling, etc. and offers the developers the necessary abstraction.
Support for Web Series: A platform for creating and deploying web services is offered by J2EE. The Java API for XML-based Remote Procedure Call, or JAX-RPC, assists programmers in creating SOAP-based web services, clients, and endpoints that are portable and interoperable.
Compatibility: The "Write Once, Run Anywhere" guiding philosophy is used by the J2EE platform. It offers thorough standards and APIs that guarantee interoperability between various application providers and, as a result, the portability of programmes.
Simplified Connectivity: J2EE facilitates applications' connectivity, enabling the use of various devices' capabilities. Additionally, it offers JMS (Java Message Service) for asynchronous, loosely linked application integration. Additionally, it offers support for CORBA (Common Object Request Broker Architecture), which enables close system integration through remote calls.

----

## **Name various components of J2EE application architecture?**

J2EE is made up of 3 main components (tiers) - Client tier, Middle tier, Enterprise data tier:

Client Tier: Programs and apps in this tier typically run on machines other than the server and interact with users. Different user inputs are taken in this instance, and the requests are submitted to the server for processing before being returned to the client with the result.
Middle Tier: Web components and EJB containers make up this tier. The web components that process the request and produce the response are either servlet or JSP pages. Static HTML codes, programmes, and applets from the client are packed with the server's components when the application is put together, along with the web components. The Enterprise Bean, which is running on the business tier, needs the EJB components to handle input from the user.
Enterprise Data Tier: Database servers, resource management programmes, and several other data sources are included in this tier and are accessible by various business tier components via a separate workstation. This tier makes use of technologies like JPA, JDBC, Java transaction API, Java Connector Architecture, etc.

----

## **What are the different technologies provided to the J2EE platform?**

Given below are the important technologies provided to J2EE platform:

*Java Server Pages (JSP)*: Delivering XML and HTML documents makes use of this. In addition to these, we may use other sorts of data using OutputStream.
*Java API for XML Based RPC (JAX-RPC)*: This is used to create web applications and clients that employ Remote Procedure Calls and XML.
*Java Servlets*: The request-response approach can be used to access applications hosted by servers, which are extended by classes known as servlets.
*Enterprise Java Beans*: This is a server-side component that provides runtime environment, security, servlet lifecycle management, transaction management, and other services in order to encapsulate the business logic of the application.
*J2EE Deployment API*: It offers specifications for web services deployment.
*J2EE Connector Architecture*: This establishes a common framework for linking J2EE platforms with other EIS (Enterprise Information Systems), including mainframe operations, database systems, and many legacy applications written in other languages.
*J2EE Authorization Contract for Containers*: This is used to specify security agreements between application servers and authorization policy modules.
*Java Management Extensions (JMX)*: They are used to provide tools for managing and monitoring networks, objects, devices, and applications.
*Java API for XML Registries*: This gives users a consistent API to access several XML Registries, enabling the infrastructure needed to create and deploy web services.
*Java Message Service (JMS)*: This messaging standard enables distributed, loosely coupled, asynchronous, and reliable communication across various J2EE components so that they can create, send, receive, and read messages.
*Java Transaction API (JTA)*: This is used to specify the Java standard interfaces for managers and transaction systems.
*Java Naming and Directory Interface (JNDI)*: For Java-based applications, this API offers name and directory functionality.
*JDBC Data Access API*: This offers APIs for obtaining data from several data sources, including relational databases, flat files, and spreadsheets.
*Common Object Request Broker Architecture (CORBA)*: In order to facilitate system communication implemented on many platforms, this standard for establishing Object Management Groups is provided.

----

## **How is JDK different from JIT?**

A cross-platform software development environment called JDK (Java Development Kit) provides diverse collections of libraries and tools needed to create Java programmes and applets. It also includes JRE, which offers tools and libraries that support the execution of byte code. JDK is required for creating and executing Java programmes. while JIT refers to the Just In Time Compiler, a module found inside the JVM (which is inside JRE). For the purpose of reducing compilation time and improving speed, JIT compilers are used to compile some portions of byte code that perform similarly to machine code simultaneously.

----

## **What do you understand by build file?**

A build file is used to automate numerous software development processes. The build file additionally specifies the versions of libraries that must be included in addition to this. The kinds of optimizations needed for the project are also included. When the project size grows, build offers a standardized method for building the project.

----

## **How are CLASSPATH and PATH different from each other in terms of J2EE?**

Key environmental variables utilized by Java systems include PATH and CLASSPATH.

Whether Java is installed on the system or not has no bearing on PATH, a system-level variable. While JVM uses CLASSPATH, which is entirely Java-specific, to load the classes needed by running Java programmes.
The JDK binaries or native libraries like java.exe are referenced by the PATH variable. In contrast, the CLASSPATH variable directs users to Java binaries, such as bytecode-filled JAR files.

----

## **How is a multi tier client server architectural model advantageous?**

The tiers that make up a multi-tier client-server architectural model all communicate with one another. The three-tier application paradigm shown below shows how the client/presentation, business logic, and database tiers interact with one another to handle requests and provide responses:

The user interface and business logic can both be altered independently.
Each tier may be individually coded or designed. Java or Python, for instance, can be used to code the intermediate tier, while Angular or React can be used to code the client tier, etc.
Between the components, abstraction is introduced. As an illustration, the client tier can access data without being aware of the origin of the response, the server infrastructure in the backend, etc.
Instead of needing to create a new connection for each user, the database may feature pooled connections that allow users to share data.

----

## **Why do we have JNDI and JDBC in J2EE?**

JDBC, or Java Database Connectivity, offers instructions and APIs for establishing connections to databases from many vendors, including MySQL, Oracle, PostgreSQL, etc., in order to obtain data. Without knowing the precise host address or port, JNDI (Java Naming and Directory Interface) assists in creating a logical framework to access a resource from the database, EJB beans, messaging queues, etc. After registering a resource with JNDI, application components can subsequently be accessed by using the JNDI name.

----

## **What are the J2EE aplets? Why can we use it?**

Applets are Java-based J2EE client components that run in a web browser or on a number of other platforms that support the applet development model. They assist in providing small, portable embedded Java programmes in HTML pages that will be run automatically when we browse the pages and are used to provide interactive capabilities to online apps.

----

## **What is EJB? How can you use it in J2EE?**

One of the most crucial components of the J2EE platform, EJB, or Enterprise Java Beans, enables the creation and deployment of enterprise-level multi-tiered applications while keeping performance, scalability, and robustness in mind. When we wish to accomplish the following, we can utilize EJBs:

Clustering: EJBs can be utilized for the application's deployment in a cluster environment to provide high availability and fault tolerance.
Concurrency without using Threads: Due to the fact that EJBs are available in the EJB container and are instantiated using the object pool, concurrency can be achieved without the usage of actual threads. This aids in achieving performance without engaging Threads-related complexity.
Full Stack Web Developer Course
To become an expert in MEAN StackVIEW COURSEFull Stack Web Developer Course

----

## **What is the architecture model of Struts?**

Strut is an application development framework for creating enterprise-level applications that combines JSP, Java Servlets, messages, and custom tags. MVC (Model-View-Controller) architecture is the foundation of it.

View: JSP technology is used by Struts to develop views for enterprise-level applications.
Model: The internal system state is defined by this component. Depending on the architecture of the application, it could either be a Java Beans cluster or a single bean.
Controller:It manages user actions that process requests and give answers to them. It is a servlet.

----

## **What is ORM?**

By leveraging metadata that describes the relationship between the database and the objects, object-relational mapping, or ORM, converts Java class objects to tables in relational databases and vice versa.

----

## **What constitutes web components?**

Web components are made up of Java Servlets and Java Server Pages (JSP) elements. Java Servlets process requests and responses on the fly. Servlets that enable a natural method to create static content are executed through JSP pages.

----

## **What is EJB platform?**

The Enterprise JavaBeans are referred to as EJBs. While you focus on building business logic, the EJB platform handles tasks like transaction and state management, resource pooling, multithreading, and simple searches.

----

## **What is JSF?**

JSF, or Java Server Faces, is a web framework designed to make the creation of user interfaces more straightforward. It is a common display solution for web applications with a Java foundation. It offers reusable UI components and is built on the MVC (Model-View-Controller) pattern.

----

## **What factors should a J2EE application possess for operating in a global economy?**

The following are the factors that a J2EE application possess for operating in a global economy:

Language Requirements: For a wider user base, a programme should support the national language as well as regional ones.
Financial Consideration: Depending on the government, every nation has its own taxes, regulations, and tariffs. When creating a J2EE application, all of these elements should be taken into account.
Legal Differences: Every government has its own set of customary laws, privacy laws, and demands for every nation. A designed application must abide by all applicable laws.

----

## **What are Connectors? Describe the Connector Architecture?**

Connectors are used to offer connectivity to various enterprise information systems through standard extension protocols. Resource adapters and system-level contracts, both of which are unique to enterprise information systems, make up a connector architecture. Plugging the resource adapters into the container. For a resource adapter to be plugged into J2EE applications, it must satisfy certain contracts that the connector architecture prescribes, such as security, transaction, resource management, etc.

----

## **What are the design goals of J2EE architecture?**

The following are the design goals of J2EE architecture:

User Interaction: The user experience should be smooth and connect to a variety of devices, including computers, mobile phones, laptops, etc.
Data Connectivity: A J2EE application's link to legacy systems needs to be stable enough to support business operations.
Service Availability: To guarantee that the application is accessible around-the-clock in order to meet necessary business objectives.
Ease of Accessibility: Applications should be accessible to users from any location and on any device.
Abstraction and Flexibility: The server should handle the configuration details while the developer should concentrate on the business logic.
New Course: Full Stack Development for Beginners
Learn Git Command, Angular, NodeJS, Maven & MoreENROLL NOWNew Course: Full Stack Development for Beginners

----

## **What is JRMP?**

JRMP, or Java Remote Method Protocol, is a tool used for Remote Method Invocation (RMI), which allows Java objects to be passed as arguments. When moving items from one JVM to another using object serialization, RMI uses this underlying protocol to marshal objects as a stream.

----

## **How is 32-bit JVM different from 64-bit JVM?**

In contrast to 32-bit operating systems, 64-bit operating systems use the 64-bit JVM. As opposed to the 4G limit of 32-bit JVM, we can select higher heap size memory in 64-bit JVM up to 100G. When running in a 64-bit JVM, Java programmes consume more memory than when running in a 32-bit JVM. The Ordinary Object Pointer's larger size is to blame for this. However, this can be avoided by instructing the JVM to utilize 32-bit pointers by using the -XXCompressedOOP option. In contrast to the 32-bit JVM, which utilizes 8-byte headers and a maximum of 4-byte internal references, the 64-bit JVM employs 12-byte object headers and a maximum of 8-byte internal references.

----

## **What is the purpose of heap dumps and how do you analyze a heap dump?**

Heap dumps are a snapshot of all active objects being used by active Java programmes on the Java heap memory. The heap dump contains comprehensive information for each item, including type, class name, address, size, and relationships to other objects. Numerous tools are useful when examining Java heap dumps. For instance, JDK itself offers the jhat tool for heap dump analysis. Heap dumps are also used for memory leak analysis. Memory leaks are a phenomenon that happens when there are objects that are no longer needed by the application but are still represented as referenced objects by the garbage collection, making it impossible to free that memory. Following are the causes that result in memory leaks:

Constantly creating new instances of objects without relinquishing them.
Open connection objects, such as database connections, post the necessary operation.
Static variables preserving object references.
Adding objects to a hashmap without modifying the equals() method of the hash code. If these techniques are left out, the hashmap will continue to expand while taking duplicates into account.
Infinite caches.
Techniques that are uninvoked by listeners.
As a result, the application keeps using more and more memory, which finally causes OutOfMemory Errors and can cause the application to crash. To find memory leaks in heap dumps, we can analyze the data using the visualVM for Eclipse Memory Analyzer tools.

----

## **What are EAR, WAR, and JAR?**

Enterprise Archive File, or EAR, is a compressed and packaged file that contains client, EJB, and web components. Its extension is.ear. We can deploy many modules simultaneously to the application server using EAR files.

The term "WAR" refers to a file that contains all web components that have been compressed and packaged together. This file makes it simple to test and deploy web apps with just one request.

Java Archive file is referred to as a JAR. It includes all of the class files and libraries that make up APIs. The.jar file contains these compressed and packaged together. These are employed for the single-request deployment of the full application, including classes and resources.

----

## **What is Spring?**

A lightweight open source framework for creating enterprise apps is called Spring. It solves the enterprise application development complexity and offers simple J2EE development. Rod Johnson was the author of the original draught. In June 2003, it was made available under the Apache 2.0 license.

----

## **What is Hibernate?**

Hibernate is a Java-based Object Relational Mapper technology that offers an abstraction layer for accessing or changing database data. The developer should not worry about how the connections to the databases are formed, how the data translation from Java application to Database and vice versa occurs because it handles all implementations inside. Strong object-oriented concepts supported by Hibernate include inheritance, association, polymorphism, compositions, and collections that aid in query creation when using the Java method and HQL (Hibernate Query Language).

----

## **Can you describe the phases of the servlet life cycle?**

Given below are the five phases:

Classloading phases: The web container must first load the servlet class file with the.class extension.
Instantiation phases: The servlet must then be instantiated by executing the default function Object.
Initialize phases: This stage involves running the servlet's init() method, where the servlet configuration will be given to it. This is a lifecycle method offered by the Servlet interface that is only executed once during the lifetime of the servlet.
Request handling: By utilizing the service() function of the Servlet interface, the servlets in this instance deliver services to various requests.
Remove phases: The Servlet interface destroy() lifecycle method, which is used to clear the configuration and close resources before servlet destruction, will be called during this phase. The waste will then be picked up after this.

----

## **What are different modules used in Spring?**

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

## **What is a backing bean?**

Backing beans are JavaBeans components that relate to JavaServer Pages and contain JavaServer Faces components. The backing bean outlines the characteristics for the page components as well as the methods that process them. Event handling, validation, and navigational processing are a few examples of this processing.

----

## **What is the build file?**

An XML file with one or more asant targets is referred to as a build file. A target is a list of assignments that a user hopes to complete. A user can specify which target should be executed when asant is started. If there isn't a target, the project's default target is carried out.

----

## **Explain business logic?**

The code that contains an application's functionality is known as business logic. This logic is implemented in the EJB (Enterprise JavaBeans) architecture by the enterprise bean's methods.

### https://www.simplilearn.com/j2ee-interview-questions-answers-article

### https://engineeringinterviewquestions.com/java-swing-interview-questions-and-answers
### https://engineeringinterviewquestions.com/java-swing-interview-questions-and-answers

### http://www.a2zinterviews.com/java-questions/swing-questions

## **What are differences between Swing and AWT?**

 	There is couple of differences between swing and AWT.
AWT component are considered to be heavyweight while Swing component are lightweights.
Swing has plug gable look and feel.
AWT is platform dependent same GUI will look different platform while Swing is developed in Java and is platform dependent.

----

## **Why Swing components are called lightweight component?**
 	
AWT component are associated with native screen resource and called heavyweight component.
While Swing components is uses the screen resource of an ancestor instead of having their own and that's why called lightweight or lighter component.

----

## **What is the difference between a scrollbar and a scrollpane?**
 	
A Scrollbar is just a component, but not a container.
A Scrolpane is a container.
A Scrollpane handles its own events and performs its own scrolling.

----

## **What is a container in a GUI?**

A container contains and arranges other components (including other container) through the use of layout managers, which use specific layout policies to determine where components should go as a function of the size of the container.

----

## **What is Event Driven Thread (EDT) is Swing?**
 	
Event Driven Thread or EDT is a special thread in Swing and AWT. Event Driven Thread is used to draw graphics and listen for events in Swing.
You will get a bonus point if you able to highlight that time consuming operations like connecting to database, opening a file or connecting to network should not be done on EDT thread because it could lead to freezing GUI because of blocking and time consuming nature of these operations instead they should be done on separate thread and EDT can just be used o spawn those thread on a button click or mouse click.

----

## **What is a layout manager and what are different types of layout managers available in Java Swing?**

A layout manager is an object that is used to organize components in a container.
FlowLayout: The elements of a Flow Layout are organized in a top to bottom, left to right fashion.
Border Layout: The elements of a BorderLayout are organized at the borders(North, South East and West) and the center of a container.
Card Layout: The elements of a CardLayout are stacked, on top of the other, like a deck of cards.
Grid Layout: The elements of a GridLayout are of equal size and laid out using the square of a grid.
Grid Bag Layout: The elements of a GridBagLayout are organized according to a grid. However, the elements may be different sizes and may occupy more than one row or column of the grid. In addition, the rows and columns may have different sizes.

----

## **What is the difference between a Window and a Frame?**

The Frame extends Window to define a main application window that can have a menu bar.

----

## **What is the difference between the paint() and repaint() methods?**
 	
The paint() method supports painting via a Graphics object.
The repaint() method is used to cause paint() to be invoked by the AWT painting thread.

----

## **Does Swing is thread safe?**
 	
Since Swing components are not thread safe it means you cannot update these components in any thread other than Event Driven Thread.
If you do so you will get unexpected behavior.
Some time interviewer will also ask what are thread safe methods in swing which can be safely called from any thread only few like repaint() and revalidate().

----

## **What are peerless components?**

The peerless components are called light weight components.

----

## **What advantage do Java's layout managers provide over traditional windowing systems?**
 	
Java uses layout managers to lay out components in a consistent manner across all windowing platforms.
Since Java's layout managers aren't tied to absolute sizing and positioning, they are able to accommodate platform specific differences among windowing systems.

----

## **Which package has light weight component?**
 	
javax.Swing package contains light weight components.
All components in Swing, except JApplet, JDialog, JFrame and JWindow are lightweight components.

----

## **What is the difference between the Font and FontMetrics classes?**

The FontMetrics class is used to define implementation specific properties, such as ascent and descent of a Font object.

----

## **What is the difference between the Font and FontMetrics classes?**

The FontMetrics class is used to define implementation specific properties, such as ascent and descent of a Font object.

----

## **How can a GUI component handle its own events?**

A component can handle its own events by implementing the required event listener interface and adding itself as its own event listener.

----

## **Why swing is not thread safe?**
 	
The Swing API was designed to be powerful, flexible and easy of use.
In particular, we wanted to make it easy for programmers to build new Swing components, whether from scratch or by extending components that we provide.
For this reason, we do not require Swing components to support access from multiple threads.
Instead, we make it easy to send requests to a component so that the requests run on a single thread.

----

## **Name Container classes?**
 	
Window
Frame
Dialog
File Dialog
Panel
Applet or ScrollPane

----

## **What method is used to specify a container's layout?**
 	
The setLayout() method is used to specify a container's layout.
For example, setLayout(new Flow Layout()); will be set the layout as Flow Layout.

----

## **Which containers use a Flow Layout as their default layout?**

The Panel and Applet classes use the Flow Layout as their default layout.

----

## **Name Components subclasses that support painting?**
 	
The Canvas
Frame
Panel and
Applet classes support painting

----

## **What is the preferred size of a component?**

The preferred size of a component is the minimum component size that will allow the component to display normally.

----

## **Which container method is used to cause a container to be laid out and redisplayed?**

validate()

----

## **Name the containers which use Border Layouts as their default layout?**
	
Window
Frame and
Dialog classes

----

## **What do heavy weight components mean?**
 	
Heavy weight components like Abstract Window Toolkit (AWT) depend on the local windowing toolkit.
For example, java.awt. Button is a heavy weight component.

----

## **What is the purpose of the enableEvents() method?**
 	
The enableEvents() method is used to enable an event for a particular component.
Normally, an event is enabled when a listener is added to an object for a particular event.
The enableEvents() method is used by objects that handle events by overriding their event dispatch methods.

----

## **What is swing?**

Swing is a comprehensive set of user interface components whose look and feel can be defined at runtime. Swing is a set of classes that provide more powerful and flexible components that are possible with the AWT.

----

## **Explain the JTable and TableDateModel interface in Swing?**
 	
JTable is one of the powerful features given by Swing. This class, present in the swing.table package, shows the data in the form of tables, in a much better way. We can also select an entire column or row at a time.
JTable (TableDataaModel) is the constructor for a JTable.
The method addColumn (JTableColumn) appends a column to the end of the JTable's array of columns and JTableHeader's getTableHeader () method gives a Header to the table.
The TableDataModel interface specifies the interface for objects that provides data for cells in a JTable. We can have an object of this interface by creating an object of JTableDataModelAdapter after overriding the methods.

----

## **How different is Swing from AWT?**
 
In addition to familiar components, such as buttons, check boxes, labels, etc. Swing supplies several exciting additions, including tabbed panes, scroll panes, trees, and tables. Even familiar components, such as buttons, have more capabilities in Swing. For example, a button may have both an image and a text string associated with it. Also, the image can be changed as the state of the button changes.
Unlike AWT components, Swing components are not implemented by platform-specific code. Instead, they are written entirely in Java and, therefore, are platform-independent.
Swing components can be treated as lightweight components. One of the most important features of Swing components is their pluggable look and feel design, which increases the reliability and consistency of applications and applets deployed across platforms.

----

## **How do you classify Swing Components?**

Swing components are classified under the following headings:
Top level containers – The containers at the top of any swing component hierarchy are:
Applet
Dialog
Frame
General purpose containers – The intermediate containers are
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

## **What is MVC?**

Model-View-Controller (MVC) is a well known object oriented design for GUI components. The architecture of swing components is based on MVC design. When a GUI component is developed using MVC architecture, it is divided into three parts:
Model-An object that defines the component's state
View-The visual screen representation of component.
Controller-An object that controls a component in such a way that it responds to user input.
The model part of an MVC-based component provides information that can be used to specify the component's value, provided the component has any value properties, e.g. the min and max values of a slider control are stored in the component's model part.
The Controller part modifies information maintained by the component's model part in response to input from the user.
The View part manages the way in which the object is drawn on the screen.

----

## **What is the main difference between Dialog and Frame?**
 	
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
 	
### http://www.a2zinterviews.com/java-questions/swing-questions

### https://quescol.com/interview-preparation/core-java-coding-questions

## **Write a program to reverse an integer in Java?**

```java
import org.apache.struts.action.Action;
import org.apache.struts.action.ActionForm;
import org.apache.struts.action.ActionForward;
import org.apache.struts.action.ActionMapping;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

public class HelloAction extends Action {
    public ActionForward execute(ActionMapping mapping, ActionForm form, HttpServletRequest request, HttpServletResponse response) throws Exception {
        // Perform any necessary logic or processing

        return mapping.findForward("success");
    }
}
```

----

## **Write a program in Java to check whether an integer is Armstrong number or not?**

```java
public class ArmstrongNumber {
    public static void main(String[] args) {
        int number = 153;
        boolean isArmstrong = isArmstrongNumber(number);

        if (isArmstrong) {
            System.out.println(number + " is an Armstrong number.");
        } else {
            System.out.println(number + " is not an Armstrong number.");
        }
    }

    public static boolean isArmstrongNumber(int number) {
        int originalNumber = number;
        int result = 0;
        int digits = countDigits(number);

        while (number != 0) {
            int digit = number % 10;
            result += Math.pow(digit, digits);
            number /= 10;
        }

        return result == originalNumber;
    }

    public static int countDigits(int number) {
        int count = 0;

        while (number != 0) {
            number /= 10;
            count++;
        }

        return count;
    }
}
```

----

## **Write a program in Java to check given number is prime or not?**

```java
public class PrimeNumber {
    public static void main(String[] args) {
        int number = 29;
        boolean isPrime = isPrimeNumber(number);

        if (isPrime) {
            System.out.println(number + " is a prime number.");
        } else {
            System.out.println(number + " is not a prime number.");
        }
    }

    public static boolean isPrimeNumber(int number) {
        if (number <= 1) {
            return false;
        }

        for (int i = 2; i <= Math.sqrt(number); i++) {
            if (number % i == 0) {
                return false;
            }
        }

        return true;
    }
}
```

----

## **Write a program in Java to print the Fibonacci series using iteration?**

```java
public class FibonacciSeries {
    public static void main(String[] args) {
        int n = 10; // Number of Fibonacci numbers to print

        System.out.println("Fibonacci Series:");
        printFibonacciSeries(n);
    }

    public static void printFibonacciSeries(int n) {
        int first = 0;
        int second = 1;

        for (int i = 0; i < n; i++) {
            System.out.print(first + " ");

            int next = first + second;
            first = second;
            second = next;
        }
    }
}
```

----

## **Write a program in Java to print the Fibonacci series using recursion?**

```java
public class FibonacciSeries {
    public static void main(String[] args) {
        int n = 10; // Number of Fibonacci numbers to print

        System.out.println("Fibonacci Series:");
        for (int i = 0; i < n; i++) {
            System.out.print(fibonacci(i) + " ");
        }
    }

    public static int fibonacci(int n) {
        if (n <= 1) {
            return n;
        } else {
            return fibonacci(n - 1) + fibonacci(n - 2);
        }
    }
}
```

----

## **Write a program in Java to check whether a number is Palindrome or not using iteration?**

```java
public class PalindromeNumber {
    public static void main(String[] args) {
        int number = 12321;
        
        if (isPalindrome(number)) {
            System.out.println(number + " is a palindrome number.");
        } else {
            System.out.println(number + " is not a palindrome number.");
        }
    }

    public static boolean isPalindrome(int number) {
        int originalNumber = number;
        int reversedNumber = 0;

        while (number != 0) {
            int digit = number % 10;
            reversedNumber = reversedNumber * 10 + digit;
            number /= 10;
        }

        return originalNumber == reversedNumber;
    }
}
```

----

## **Write a program in Java to check whether a number is Palindrome or not using recursion?**

```java
public class PalindromeNumber {
    public static void main(String[] args) {
        int number = 12321;
        
        if (isPalindrome(number)) {
            System.out.println(number + " is a palindrome number.");
        } else {
            System.out.println(number + " is not a palindrome number.");
        }
    }

    public static boolean isPalindrome(int number) {
        int originalNumber = number;
        int reversedNumber = reverseNumber(number);

        return originalNumber == reversedNumber;
    }

    public static int reverseNumber(int number) {
        if (number < 10) {
            return number;
        }

        int lastDigit = number % 10;
        int remainingDigits = number / 10;
        int reversedNumber = reverseNumber(remainingDigits);

        return concatenateDigits(reversedNumber, lastDigit);
    }

    public static int concatenateDigits(int number, int digit) {
        int placeValue = 1;
        int temp = number;

        while (temp >= 10) {
            temp /= 10;
            placeValue *= 10;
        }

        return (number * 10) + (digit * placeValue);
    }
}
```

----

## **Write a program in Java to find greatest among three integers?**

```java
public class GreatestNumber {
    public static void main(String[] args) {
        int num1 = 10;
        int num2 = 20;
        int num3 = 15;

        int greatest = findGreatestNumber(num1, num2, num3);

        System.out.println("The greatest number among " + num1 + ", " + num2 + ", and " + num3 + " is: " + greatest);
    }

    public static int findGreatestNumber(int num1, int num2, int num3) {
        int greatest = num1;

        if (num2 > greatest) {
            greatest = num2;
        }

        if (num3 > greatest) {
            greatest = num3;
        }

        return greatest;
    }
}
```

----

## **Write a program in Java to find sum of digits of a number using recursion?**

```java
public class SumOfDigits {
    public static void main(String[] args) {
        int number = 12345;
        int sum = sumOfDigits(number);

        System.out.println("Sum of digits of " + number + " is: " + sum);
    }

    public static int sumOfDigits(int number) {
        if (number == 0) {
            return 0;
        } else {
            return number % 10 + sumOfDigits(number / 10);
        }
    }
}
```

----

## **Write a program in Java to swap two numbers without using third variable?**

```java
public class SwapNumbers {
    public static void main(String[] args) {
        int num1 = 10;
        int num2 = 20;

        System.out.println("Before swapping:");
        System.out.println("num1 = " + num1);
        System.out.println("num2 = " + num2);

        swapNumbers(num1, num2);

        System.out.println("After swapping:");
        System.out.println("num1 = " + num1);
        System.out.println("num2 = " + num2);
    }

    public static void swapNumbers(int num1, int num2) {
        num1 = num1 + num2;
        num2 = num1 - num2;
        num1 = num1 - num2;
    }
}
```

----

## **Write a program in Java to swap two numbers using third variable?**

```java
public class SwapNumbers {
    public static void main(String[] args) {
        int num1 = 10;
        int num2 = 20;

        System.out.println("Before swapping:");
        System.out.println("num1 = " + num1);
        System.out.println("num2 = " + num2);

        swapNumbers(num1, num2);

        System.out.println("After swapping:");
        System.out.println("num1 = " + num1);
        System.out.println("num2 = " + num2);
    }

    public static void swapNumbers(int num1, int num2) {
        int temp = num1;
        num1 = num2;
        num2 = temp;
    }
}
```

----

## **Write a program in Java to find prime factors of a given integer?**

```java
public class PrimeFactors {
    public static void main(String[] args) {
        int number = 84;

        System.out.println("Prime factors of " + number + ":");
        findPrimeFactors(number);
    }

    public static void findPrimeFactors(int number) {
        for (int i = 2; i <= number; i++) {
            if (number % i == 0) {
                boolean isPrime = true;
                for (int j = 2; j < i; j++) {
                    if (i % j == 0) {
                        isPrime = false;
                        break;
                    }
                }
                if (isPrime) {
                    System.out.println(i);
                }
            }
        }
    }
}
```

----

## **Write a program in Java to add two integer without using arithmetic operator?**

```java
public class AddWithoutOperator {
    public static void main(String[] args) {
        int num1 = 15;
        int num2 = 27;

        int sum = addWithoutOperator(num1, num2);

        System.out.println("Sum of " + num1 + " and " + num2 + " is: " + sum);
    }

    public static int addWithoutOperator(int num1, int num2) {
        while (num2 != 0) {
            int carry = num1 & num2;
            num1 = num1 ^ num2;
            num2 = carry << 1;
        }

        return num1;
    }
}
```

----

## **Write a program in Java to find given number is perfect or not?**

```java
public class PerfectNumber {
    public static void main(String[] args) {
        int number = 28;

        if (isPerfectNumber(number)) {
            System.out.println(number + " is a perfect number.");
        } else {
            System.out.println(number + " is not a perfect number.");
        }
    }

    public static boolean isPerfectNumber(int number) {
        int sum = 0;

        for (int i = 1; i <= number / 2; i++) {
            if (number % i == 0) {
                sum += i;
            }
        }

        return sum == number;
    }
}
```

----

## **Java Program to Calculate the Average of Integer Array?**

```java
public class AverageOfArray {
    public static void main(String[] args) {
        int[] numbers = {5, 10, 15, 20, 25};

        double average = calculateAverage(numbers);

        System.out.println("Average: " + average);
    }

    public static double calculateAverage(int[] array) {
        int sum = 0;

        for (int number : array) {
            sum += number;
        }

        return (double) sum / array.length;
    }
}
```

----

## **Java Program to calculate the Average of number taken from user?**

```java
import java.util.Scanner;

public class AverageOfNumbers {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the number of elements: ");
        int n = scanner.nextInt();

        int[] numbers = new int[n];

        System.out.println("Enter the elements:");
        for (int i = 0; i < n; i++) {
            numbers[i] = scanner.nextInt();
        }

        double average = calculateAverage(numbers);

        System.out.println("Average: " + average);

        scanner.close();
    }

    public static double calculateAverage(int[] array) {
        int sum = 0;

        for (int number : array) {
            sum += number;
        }

        return (double) sum / array.length;
    }
}
```

----

## **Java Program to calculate factorial using iterative method?**

```java
public class Factorial {
    public static void main(String[] args) {
        int number = 5;

        long factorial = calculateFactorial(number);

        System.out.println("Factorial of " + number + " is: " + factorial);
    }

    public static long calculateFactorial(int number) {
        long factorial = 1;

        for (int i = 1; i <= number; i++) {
            factorial *= i;
        }

        return factorial;
    }
}
```

----

## **Java Program to calculate factorial using recursion?**

```java
public class Factorial {
    public static void main(String[] args) {
        int number = 5;

        long factorial = calculateFactorial(number);

        System.out.println("Factorial of " + number + " is: " + factorial);
    }

    public static long calculateFactorial(int number) {
        if (number == 0) {
            return 1;
        } else {
            return number * calculateFactorial(number - 1);
        }
    }
}
```

----

## **Java Program to check a given number is even or odd?**

```java
public class EvenOdd {
    public static void main(String[] args) {
        int number = 7;

        if (isEven(number)) {
            System.out.println(number + " is an even number.");
        } else {
            System.out.println(number + " is an odd number.");
        }
    }

    public static boolean isEven(int number) {
        return number % 2 == 0;
    }
}
```

----

## **Java program to print first n Prime Number with explanation?**

```java
public class PrimeNumbers {
    public static void main(String[] args) {
        int n = 10; // Number of prime numbers to print
        int count = 0; // Counter for prime numbers
        int number = 2; // Starting number to check for primality

        System.out.println("First " + n + " prime numbers:");

        // Iterate until the desired number of prime numbers are found
        while (count < n) {
            if (isPrime(number)) {
                System.out.print(number + " ");
                count++;
            }
            number++;
        }
    }

    // Method to check whether a number is prime or not
    public static boolean isPrime(int number) {
        if (number <= 1) {
            return false;
        }

        // Check divisibility from 2 to square root of the number
        for (int i = 2; i * i <= number; i++) {
            if (number % i == 0) {
                return false; // Number is divisible, hence not prime
            }
        }

        return true; // Number is prime
    }
}
```

----

## **Java Program to print Prime Number in a given range?**

```java
public class PrimeNumbersInRange {
    public static void main(String[] args) {
        int start = 10; // Starting number of the range
        int end = 50; // Ending number of the range

        System.out.println("Prime numbers between " + start + " and " + end + ":");
        printPrimeNumbersInRange(start, end);
    }

    public static void printPrimeNumbersInRange(int start, int end) {
        for (int number = start; number <= end; number++) {
            if (isPrime(number)) {
                System.out.print(number + " ");
            }
        }
    }

    public static boolean isPrime(int number) {
        if (number <= 1) {
            return false;
        }

        for (int i = 2; i * i <= number; i++) {
            if (number % i == 0) {
                return false;
            }
        }

        return true;
    }
}
```

----

## **Java Program to find Smallest number among three?**

```java
public class SmallestNumber {
    public static void main(String[] args) {
        int num1 = 10;
        int num2 = 5;
        int num3 = 8;

        int smallest = findSmallestNumber(num1, num2, num3);

        System.out.println("The smallest number is: " + smallest);
    }

    public static int findSmallestNumber(int num1, int num2, int num3) {
        int smallest = num1;

        if (num2 < smallest) {
            smallest = num2;
        }

        if (num3 < smallest) {
            smallest = num3;
        }

        return smallest;
    }
}
```

----

## **Java program to calculate the power using the POW method?**

```java
public class PowerCalculation {
    public static void main(String[] args) {
        double base = 2.5;
        double exponent = 3.0;

        double result = Math.pow(base, exponent);

        System.out.println(base + " raised to the power of " + exponent + " is: " + result);
    }
}
```

----

## **Java Program to calculate the power without using POW function?**

```java
public class PowerCalculation {
    public static void main(String[] args) {
        double base = 2.5;
        int exponent = 3;

        double result = calculatePower(base, exponent);

        System.out.println(base + " raised to the power of " + exponent + " is: " + result);
    }

    public static double calculatePower(double base, int exponent) {
        double result = 1.0;

        if (exponent >= 0) {
            for (int i = 1; i <= exponent; i++) {
                result *= base;
            }
        } else {
            // Negative exponent
            for (int i = 1; i <= Math.abs(exponent); i++) {
                result /= base;
            }
        }

        return result;
    }
}
```

----

## **Java Program to calculate the square of a given number?**

```java
public class SquareCalculation {
    public static void main(String[] args) {
        int number = 5;

        int square = calculateSquare(number);

        System.out.println("The square of " + number + " is: " + square);
    }

    public static int calculateSquare(int number) {
        return number * number;
    }
}
```

----

## **Java Program to calculate the cube of a given number?**

```java
public class CubeCalculation {
    public static void main(String[] args) {
        int number = 3;

        int cube = calculateCube(number);

        System.out.println("The cube of " + number + " is: " + cube);
    }

    public static int calculateCube(int number) {
        return number * number * number;
    }
}
```

----

## **Java Program to calculate the square root of a given number?**

```java
public class SquareRootCalculation {
    public static void main(String[] args) {
        double number = 25;

        double squareRoot = calculateSquareRoot(number);

        System.out.println("The square root of " + number + " is: " + squareRoot);
    }

    public static double calculateSquareRoot(double number) {
        return Math.sqrt(number);
    }
}
```

----

## **Java program to calculate LCM of given two numbers?**

```java
public class LCMCalculation {
    public static void main(String[] args) {
        int number1 = 12;
        int number2 = 18;

        int lcm = calculateLCM(number1, number2);

        System.out.println("The LCM of " + number1 + " and " + number2 + " is: " + lcm);
    }

    public static int calculateLCM(int number1, int number2) {
        int max = Math.max(number1, number2);
        int lcm = max;

        while (true) {
            if (lcm % number1 == 0 && lcm % number2 == 0) {
                break;
            }
            lcm += max;
        }

        return lcm;
    }
}
```

----

## **Java Program to find GCD or HCF of two numbers?**

```java
public class GCDHCF {
    public static void main(String[] args) {
        int number1 = 24;
        int number2 = 36;

        int gcd = calculateGCD(number1, number2);

        System.out.println("The GCD of " + number1 + " and " + number2 + " is: " + gcd);
    }

    public static int calculateGCD(int number1, int number2) {
        while (number2 != 0) {
            int temp = number2;
            number2 = number1 % number2;
            number1 = temp;
        }

        return number1;
    }
}
```

----

## **Java Program to find GCD of two numbers using recursion?**

```java
public class GCDRecursion {
    public static void main(String[] args) {
        int number1 = 24;
        int number2 = 36;

        int gcd = calculateGCD(number1, number2);

        System.out.println("The GCD of " + number1 + " and " + number2 + " is: " + gcd);
    }

    public static int calculateGCD(int number1, int number2) {
        if (number2 == 0) {
            return number1;
        }

        return calculateGCD(number2, number1 % number2);
    }
}
```

----

## **Java Program to check the given year is a leap year or not?**

```java
public class LeapYear {
    public static void main(String[] args) {
        int year = 2024;

        boolean isLeapYear = checkLeapYear(year);

        if (isLeapYear) {
            System.out.println(year + " is a leap year.");
        } else {
            System.out.println(year + " is not a leap year.");
        }
    }

    public static boolean checkLeapYear(int year) {
        if (year % 4 == 0) {
            if (year % 100 == 0) {
                if (year % 400 == 0) {
                    return true;  // Divisible by 400, so it is a leap year
                }
                return false;  // Divisible by 100 but not by 400, so it is not a leap year
            }
            return true;  // Divisible by 4 but not by 100, so it is a leap year
        }
        return false;  // Not divisible by 4, so it is not a leap year
    }
}
```

----

## **Java Program to convert Celsius to Fahrenheit?**

```java
public class CelsiusToFahrenheit {
    public static void main(String[] args) {
        double celsius = 25.0;
        double fahrenheit = convertCelsiusToFahrenheit(celsius);

        System.out.println(celsius + " degrees Celsius is equal to " + fahrenheit + " degrees Fahrenheit.");
    }

    public static double convertCelsiusToFahrenheit(double celsius) {
        double fahrenheit = (celsius * 9 / 5) + 32;
        return fahrenheit;
    }
}
```

----

## **Java Program to convert Fahrenheit to Celsius?**

```java
public class FahrenheitToCelsius {
    public static void main(String[] args) {
        double fahrenheit = 77.0;
        double celsius = convertFahrenheitToCelsius(fahrenheit);

        System.out.println(fahrenheit + " degrees Fahrenheit is equal to " + celsius + " degrees Celsius.");
    }

    public static double convertFahrenheitToCelsius(double fahrenheit) {
        double celsius = (fahrenheit - 32) * 5 / 9;
        return celsius;
    }
}
```

----

## **Java program to calculate Simple Interest with explanation?**

```java
public class SimpleInterestCalculation {
    public static void main(String[] args) {
        double principal = 1000.0;
        double rate = 5.0;
        double time = 2.0;

        double simpleInterest = calculateSimpleInterest(principal, rate, time);

        System.out.println("Principal: $" + principal);
        System.out.println("Rate of Interest: " + rate + "%");
        System.out.println("Time: " + time + " years");
        System.out.println("Simple Interest: $" + simpleInterest);
    }

    public static double calculateSimpleInterest(double principal, double rate, double time) {
        double interest = (principal * rate * time) / 100;
        return interest;
    }
}
```

----

## **Java Coding Questions on String**

```java
public class SimpleInterestCalculation {
    public static void main(String[] args) {
        double principal = 1000.0;
        double rate = 5.0;
        double time = 2.0;

        double simpleInterest = calculateSimpleInterest(principal, rate, time);

        System.out.println("Principal: $" + principal);
        System.out.println("Rate of Interest: " + rate + "%");
        System.out.println("Time: " + time + " years");
        System.out.println("Simple Interest: $" + simpleInterest);
    }

    public static double calculateSimpleInterest(double principal, double rate, double time) {
        double interest = (principal * rate * time) / 100;
        return interest;
    }
}
```

----

## **Write a method in Java which will remove any given character from a String?**

```java
public class StringCharacterRemoval {
    public static void main(String[] args) {
        String str = "Hello, World!";
        char charToRemove = 'l';

        String result = removeCharacter(str, charToRemove);

        System.out.println("Original string: " + str);
        System.out.println("Modified string: " + result);
    }

    public static String removeCharacter(String str, char charToRemove) {
        StringBuilder builder = new StringBuilder();

        for (int i = 0; i < str.length(); i++) {
            char currentChar = str.charAt(i);

            if (currentChar != charToRemove) {
                builder.append(currentChar);
            }
        }

        return builder.toString();
    }
}
```

----

## **Write a program in Java to count occurrence of a given character in a String?**

```java
public class CharacterCount {
    public static void main(String[] args) {
        String str = "Hello, World!";
        char target = 'l';

        int count = countOccurrences(str, target);

        System.out.println("The character '" + target + "' occurs " + count + " times in the string.");
    }

    public static int countOccurrences(String str, char target) {
        int count = 0;

        for (int i = 0; i < str.length(); i++) {
            if (str.charAt(i) == target) {
                count++;
            }
        }

        return count;
    }
}
```

----

## **Write a program in Java to check if two String are Anagram?**

```java
import java.util.Arrays;

public class AnagramCheck {
    public static void main(String[] args) {
        String str1 = "listen";
        String str2 = "silent";

        boolean isAnagram = checkAnagram(str1, str2);

        if (isAnagram) {
            System.out.println(str1 + " and " + str2 + " are anagrams.");
        } else {
            System.out.println(str1 + " and " + str2 + " are not anagrams.");
        }
    }

    public static boolean checkAnagram(String str1, String str2) {
        // Remove spaces and convert to lowercase for case-insensitive comparison
        str1 = str1.replaceAll("\\s", "").toLowerCase();
        str2 = str2.replaceAll("\\s", "").toLowerCase();

        // Check if the lengths of the strings are equal
        if (str1.length() != str2.length()) {
            return false;
        }

        // Convert strings to character arrays and sort them
        char[] charArray1 = str1.toCharArray();
        char[] charArray2 = str2.toCharArray();
        Arrays.sort(charArray1);
        Arrays.sort(charArray2);

        // Compare the sorted character arrays
        return Arrays.equals(charArray1, charArray2);
    }
}
```

----

## **Write a program in Java to check a String is palindrome or not?**

```java
public class PalindromeCheck {
    public static void main(String[] args) {
        String str = "madam";

        boolean isPalindrome = checkPalindrome(str);

        if (isPalindrome) {
            System.out.println(str + " is a palindrome.");
        } else {
            System.out.println(str + " is not a palindrome.");
        }
    }

    public static boolean checkPalindrome(String str) {
        int length = str.length();

        for (int i = 0; i < length / 2; i++) {
            if (str.charAt(i) != str.charAt(length - 1 - i)) {
                return false;
            }
        }

        return true;
    }
}
```

----

## **Java program to check given character is vowel or consonant?**

```java
public class VowelConsonantCheck {
    public static void main(String[] args) {
        char ch = 'a';

        if (isVowel(ch)) {
            System.out.println(ch + " is a vowel.");
        } else {
            System.out.println(ch + " is a consonant.");
        }
    }

    public static boolean isVowel(char ch) {
        ch = Character.toLowerCase(ch);

        if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') {
            return true;
        }

        return false;
    }
}
```

----

## **Java program to check given character is digit or not?**

```java
public class DigitCheck {
    public static void main(String[] args) {
        char ch = '7';

        if (isDigit(ch)) {
            System.out.println(ch + " is a digit.");
        } else {
            System.out.println(ch + " is not a digit.");
        }
    }

    public static boolean isDigit(char ch) {
        return Character.isDigit(ch);
    }
}
```

----

## **Java program to replace the string space with a given character?**

```java
public class ReplaceSpaces {
    public static void main(String[] args) {
        String str = "Hello World";
        char replacementChar = '-';

        String replacedString = replaceSpaces(str, replacementChar);

        System.out.println("Original string: " + str);
        System.out.println("Replaced string: " + replacedString);
    }

    public static String replaceSpaces(String str, char replacementChar) {
        StringBuilder replaced = new StringBuilder();

        for (int i = 0; i < str.length(); i++) {
            if (str.charAt(i) == ' ') {
                replaced.append(replacementChar);
            } else {
                replaced.append(str.charAt(i));
            }
        }

        return replaced.toString();
    }
}
```

----

## **Java program to convert lowercase char to uppercase of string?**

```java
public class ConvertToLowercase {
    public static void main(String[] args) {
        String str = "Hello, World!";

        String convertedString = convertToLowercase(str);

        System.out.println("Original string: " + str);
        System.out.println("Converted string: " + convertedString);
    }

    public static String convertToLowercase(String str) {
        StringBuilder converted = new StringBuilder();

        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);

            if (Character.isLowerCase(ch)) {
                ch = Character.toUpperCase(ch);
            }

            converted.append(ch);
        }

        return converted.toString();
    }
}
```

----

## **Java program to convert lowercase vowel to uppercase in string?**

```java
public class ConvertLowercaseVowels {
    public static void main(String[] args) {
        String str = "Hello, World!";

        String convertedString = convertLowercaseVowels(str);

        System.out.println("Original string: " + str);
        System.out.println("Converted string: " + convertedString);
    }

    public static String convertLowercaseVowels(String str) {
        StringBuilder converted = new StringBuilder();

        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);

            if (isLowercaseVowel(ch)) {
                ch = Character.toUpperCase(ch);
            }

            converted.append(ch);
        }

        return converted.toString();
    }

    public static boolean isLowercaseVowel(char ch) {
        ch = Character.toLowerCase(ch);

        return ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u';
    }
}
```

----

## **Java program to delete vowels in a given string?**

```java
public class DeleteVowels {
    public static void main(String[] args) {
        String str = "Hello, World!";

        String deletedVowelsString = deleteVowels(str);

        System.out.println("Original string: " + str);
        System.out.println("String after deleting vowels: " + deletedVowelsString);
    }

    public static String deleteVowels(String str) {
        StringBuilder deletedVowels = new StringBuilder();

        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);

            if (!isVowel(ch)) {
                deletedVowels.append(ch);
            }
        }

        return deletedVowels.toString();
    }

    public static boolean isVowel(char ch) {
        ch = Character.toLowerCase(ch);

        return ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u';
    }
}
```

----

## **Java program to count Occurrence Of Vowels & Consonants in a String?**

```java
public class CountVowelsConsonants {
    public static void main(String[] args) {
        String str = "Hello, World!";
        
        int vowelCount = countVowels(str);
        int consonantCount = countConsonants(str);
        
        System.out.println("Original string: " + str);
        System.out.println("Vowel count: " + vowelCount);
        System.out.println("Consonant count: " + consonantCount);
    }
    
    public static int countVowels(String str) {
        int count = 0;
        str = str.toLowerCase();
        
        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);
            
            if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') {
                count++;
            }
        }
        
        return count;
    }
    
    public static int countConsonants(String str) {
        int count = 0;
        str = str.toLowerCase();
        
        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);
            
            if (ch >= 'a' && ch <= 'z' && !isVowel(ch)) {
                count++;
            }
        }
        
        return count;
    }
    
    public static boolean isVowel(char ch) {
        return ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u';
    }
}
```

----

## **Java program to print the highest frequency character in a String?**

```java
import java.util.HashMap;
import java.util.Map;

public class HighestFrequencyCharacter {
    public static void main(String[] args) {
        String str = "Hello, World!";
        char highestFreqChar = getHighestFrequencyChar(str);

        System.out.println("Original string: " + str);
        System.out.println("Highest frequency character: " + highestFreqChar);
    }

    public static char getHighestFrequencyChar(String str) {
        Map<Character, Integer> charFrequencyMap = new HashMap<>();

        // Calculate the frequency of each character in the string
        for (char ch : str.toCharArray()) {
            if (Character.isLetter(ch)) {
                ch = Character.toLowerCase(ch);
                charFrequencyMap.put(ch, charFrequencyMap.getOrDefault(ch, 0) + 1);
            }
        }

        char highestFreqChar = ' ';
        int highestFrequency = 0;

        // Find the character with the highest frequency
        for (Map.Entry<Character, Integer> entry : charFrequencyMap.entrySet()) {
            if (entry.getValue() > highestFrequency) {
                highestFreqChar = entry.getKey();
                highestFrequency = entry.getValue();
            }
        }

        return highestFreqChar;
    }
}
```

----

## **Java program to Replace First Occurrence Of Vowel With ‘-‘ in String?**

```java
public class ReplaceFirstVowel {
    public static void main(String[] args) {
        String str = "Hello, World!";
        String replacedString = replaceFirstVowel(str);

        System.out.println("Original string: " + str);
        System.out.println("String after replacing first vowel: " + replacedString);
    }

    public static String replaceFirstVowel(String str) {
        StringBuilder replaced = new StringBuilder();

        boolean foundVowel = false;

        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);

            if (!foundVowel && isVowel(ch)) {
                replaced.append('-');
                foundVowel = true;
            } else {
                replaced.append(ch);
            }
        }

        return replaced.toString();
    }

    public static boolean isVowel(char ch) {
        ch = Character.toLowerCase(ch);

        return ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u';
    }
}
```

----

## **Java program to count alphabets, digits and special characters?**

```java
public class CountCharacters {
    public static void main(String[] args) {
        String str = "Hello,123!";

        int alphabetCount = countAlphabets(str);
        int digitCount = countDigits(str);
        int specialCharCount = countSpecialCharacters(str);

        System.out.println("Original string: " + str);
        System.out.println("Alphabet count: " + alphabetCount);
        System.out.println("Digit count: " + digitCount);
        System.out.println("Special character count: " + specialCharCount);
    }

    public static int countAlphabets(String str) {
        int count = 0;

        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);

            if (Character.isLetter(ch)) {
                count++;
            }
        }

        return count;
    }

    public static int countDigits(String str) {
        int count = 0;

        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);

            if (Character.isDigit(ch)) {
                count++;
            }
        }

        return count;
    }

    public static int countSpecialCharacters(String str) {
        int count = 0;

        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);

            if (!Character.isLetter(ch) && !Character.isDigit(ch)) {
                count++;
            }
        }

        return count;
    }
}
```

----

## **Java program to remove blank space from string?**

```java
public class RemoveSpaces {
    public static void main(String[] args) {
        String str = "  Hello,   World!  ";
        String trimmedString = removeSpaces(str);

        System.out.println("Original string: " + str);
        System.out.println("String after removing spaces: " + trimmedString);
    }

    public static String removeSpaces(String str) {
        return str.replaceAll("\\s+", "");
    }
}
```

----

## **Java program to Concatenate two strings?**

```java
public class ConcatenateStrings {
    public static void main(String[] args) {
        String str1 = "Hello";
        String str2 = "World";

        String concatenatedString = concatenateStrings(str1, str2);

        System.out.println("String 1: " + str1);
        System.out.println("String 2: " + str2);
        System.out.println("Concatenated string: " + concatenatedString);
    }

    public static String concatenateStrings(String str1, String str2) {
        return str1 + str2;
    }
}
```

----

## **Java Program to remove repeated character from string?**

```java
import java.util.LinkedHashSet;

public class RemoveRepeatedCharacters {
    public static void main(String[] args) {
        String str = "Hello, World!";
        String withoutRepeatedChars = removeRepeatedCharacters(str);

        System.out.println("Original string: " + str);
        System.out.println("String after removing repeated characters: " + withoutRepeatedChars);
    }

    public static String removeRepeatedCharacters(String str) {
        LinkedHashSet<Character> uniqueChars = new LinkedHashSet<>();

        for (int i = 0; i < str.length(); i++) {
            uniqueChars.add(str.charAt(i));
        }

        StringBuilder result = new StringBuilder();
        for (Character ch : uniqueChars) {
            result.append(ch);
        }

        return result.toString();
    }
}
```

----

## **Java program to calculate sum of integers in string?**

```java
public class SumOfIntegersInString {
    public static void main(String[] args) {
        String str = "I have 5 apples and 3 oranges.";
        int sum = calculateSumOfIntegers(str);

        System.out.println("Original string: " + str);
        System.out.println("Sum of integers in the string: " + sum);
    }

    public static int calculateSumOfIntegers(String str) {
        int sum = 0;
        StringBuilder currentNumber = new StringBuilder();

        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);

            if (Character.isDigit(ch)) {
                currentNumber.append(ch);
            } else {
                if (currentNumber.length() > 0) {
                    sum += Integer.parseInt(currentNumber.toString());
                    currentNumber.setLength(0);
                }
            }
        }

        if (currentNumber.length() > 0) {
            sum += Integer.parseInt(currentNumber.toString());
        }

        return sum;
    }
}
```

----

## **Java program to print all non repeating character in string?**

```java
import java.util.LinkedHashMap;
import java.util.Map;

public class NonRepeatingCharacters {
    public static void main(String[] args) {
        String str = "Hello, World!";
        String nonRepeatingChars = findNonRepeatingCharacters(str);

        System.out.println("Original string: " + str);
        System.out.println("Non-repeating characters: " + nonRepeatingChars);
    }

    public static String findNonRepeatingCharacters(String str) {
        Map<Character, Integer> charCountMap = new LinkedHashMap<>();

        // Count the occurrence of each character
        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);
            charCountMap.put(ch, charCountMap.getOrDefault(ch, 0) + 1);
        }

        StringBuilder result = new StringBuilder();
        // Append non-repeating characters to the result string
        for (Map.Entry<Character, Integer> entry : charCountMap.entrySet()) {
            if (entry.getValue() == 1) {
                result.append(entry.getKey());
            }
        }

        return result.toString();
    }
}
```

----

## **Java Program to sort characters of string in Ascending Order?**

```java
import java.util.Arrays;

public class SortCharacters {
    public static void main(String[] args) {
        String str = "hello world";
        String sortedString = sortCharacters(str);

        System.out.println("Original string: " + str);
        System.out.println("String after sorting characters in ascending order: " + sortedString);
    }

    public static String sortCharacters(String str) {
        // Convert the string to a character array
        char[] charArray = str.toCharArray();

        // Sort the character array in ascending order
        Arrays.sort(charArray);

        // Convert the sorted character array back to a string
        return new String(charArray);
    }
}
```

----

## **Java Program to sort character of string in descending order?**

```java
import java.util.Arrays;
import java.util.Collections;

public class SortCharactersDescending {
    public static void main(String[] args) {
        String str = "hello world";
        String sortedString = sortCharactersDescending(str);

        System.out.println("Original string: " + str);
        System.out.println("String after sorting characters in descending order: " + sortedString);
    }

    public static String sortCharactersDescending(String str) {
        // Convert the string to a character array
        Character[] charArray = new Character[str.length()];
        for (int i = 0; i < str.length(); i++) {
            charArray[i] = str.charAt(i);
        }

        // Sort the character array in descending order
        Arrays.sort(charArray, Collections.reverseOrder());

        // Convert the sorted character array back to a string
        StringBuilder sortedString = new StringBuilder(charArray.length);
        for (Character ch : charArray) {
            sortedString.append(ch);
        }

        return sortedString.toString();
    }
}
```

----

## **Write a program in Java for, In array 1-100 numbers are stored, one number is missing how do you find it?**

```java
public class FindMissingNumber {
    public static void main(String[] args) {
        // Create the array with 99 elements (missing one number)
        int[] array = new int[99];
        for (int i = 0; i < array.length; i++) {
            array[i] = i + 1;
        }

        // Choose a random number from 1 to 100 and remove it from the array
        int missingNumber = (int) (Math.random() * 100) + 1;
        for (int i = 0; i < array.length; i++) {
            if (array[i] == missingNumber) {
                array[i] = 0;
                break;
            }
        }

        // Find the missing number
        int missing = findMissingNumber(array);
        System.out.println("Missing number: " + missing);
    }

    public static int findMissingNumber(int[] array) {
        int expectedSum = 0;
        int actualSum = 0;

        // Calculate the sum of all numbers from 1 to 100
        for (int i = 1; i <= 100; i++) {
            expectedSum += i;
        }

        // Calculate the sum of the given array
        for (int num : array) {
            actualSum += num;
        }

        // Find the missing number
        return expectedSum - actualSum;
    }
}
```

----

## **Write a program in Java for, In a array 1-100 multiple numbers are duplicates, how do you find it?**

```java
public class FindMissingNumber {
    public static void main(String[] args) {
        // Create the array with 99 elements (missing one number)
        int[] array = new int[99];
        for (int i = 0; i < array.length; i++) {
            array[i] = i + 1;
        }

        // Choose a random number from 1 to 100 and remove it from the array
        int missingNumber = (int) (Math.random() * 100) + 1;
        for (int i = 0; i < array.length; i++) {
            if (array[i] == missingNumber) {
                array[i] = 0;
                break;
            }
        }

        // Find the missing number
        int missing = findMissingNumber(array);
        System.out.println("Missing number: " + missing);
    }

    public static int findMissingNumber(int[] array) {
        int expectedSum = 0;
        int actualSum = 0;

        // Calculate the sum of all numbers from 1 to 100
        for (int i = 1; i <= 100; i++) {
            expectedSum += i;
        }

        // Calculate the sum of the given array
        for (int num : array) {
            actualSum += num;
        }

        // Find the missing number
        return expectedSum - actualSum;
    }
}
```

----

## **Write a program in Java for, How to find all pairs in array of integers whose sum is equal to given number?**

```java
import java.util.Arrays;

public class FindPairs {
    public static void main(String[] args) {
        int[] array = {2, 4, 6, 8, 9, 3, 5};
        int targetSum = 10;

        System.out.println("Pairs with sum " + targetSum + ":");
        findPairs(array, targetSum);
    }

    public static void findPairs(int[] array, int targetSum) {
        Arrays.sort(array); // Sort the array in ascending order

        int left = 0;
        int right = array.length - 1;

        while (left < right) {
            int currentSum = array[left] + array[right];
            if (currentSum == targetSum) {
                System.out.println(array[left] + ", " + array[right]);
                left++;
                right--;
            } else if (currentSum < targetSum) {
                left++;
            } else {
                right--;
            }
        }
    }
}
```

----

## **Write a program in Java for, In a array 1-100 exactly one number is duplicate how do you find it?**

```java
public class FindDuplicateNumber {
    public static void main(String[] args) {
        // Create the array with duplicate number
        int[] array = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 20, 21, 22, 23, 24, 25};

        // Find the duplicate number
        int duplicate = findDuplicateNumber(array);
        System.out.println("Duplicate number: " + duplicate);
    }

    public static int findDuplicateNumber(int[] array) {
        int expectedSum = 0;
        int actualSum = 0;

        // Calculate the sum of numbers from 1 to 100
        for (int i = 1; i <= 100; i++) {
            expectedSum += i;
        }

        // Calculate the sum of the given array
        for (int num : array) {
            actualSum += num;
        }

        // The difference between the expected sum and actual sum is the duplicate number
        return actualSum - expectedSum;
    }
}
```

----

## **Write a program in Java for, Given two arrays 1,2,3,4,5 and 2,3,1,0,5 find which number is not present in the second array?**

```java
import java.util.HashSet;

public class FindMissingNumber {
    public static void main(String[] args) {
        int[] array1 = {1, 2, 3, 4, 5};
        int[] array2 = {2, 3, 1, 0, 5};

        int missingNumber = findMissingNumber(array1, array2);
        System.out.println("Missing number: " + missingNumber);
    }

    public static int findMissingNumber(int[] array1, int[] array2) {
        HashSet<Integer> set = new HashSet<>();

        // Add all elements of array2 to the set
        for (int num : array2) {
            set.add(num);
        }

        // Iterate over array1 to find the missing number
        for (int num : array1) {
            if (!set.contains(num)) {
                return num;
            }
        }

        return -1; // Return -1 if no missing number is found
    }
}
```

----

## **Write a program in Java for, How to compare two array is equal in size or not?**

```java
public class CompareArrays {
    public static void main(String[] args) {
        int[] array1 = {1, 2, 3, 4, 5};
        int[] array2 = {2, 3, 1, 0, 5};
        int[] array3 = {1, 2, 3, 4, 5, 6};

        boolean equalSize1 = compareArraySize(array1, array2);
        System.out.println("Array1 and Array2 are equal in size: " + equalSize1);

        boolean equalSize2 = compareArraySize(array1, array3);
        System.out.println("Array1 and Array3 are equal in size: " + equalSize2);
    }

    public static boolean compareArraySize(int[] array1, int[] array2) {
        return array1.length == array2.length;
    }
}
```

----

## **Write a program in Java to find largest and smallest number in array?**

```java
public class FindMinMax {
    public static void main(String[] args) {
        int[] array = {5, 8, 2, 10, 3, 1};

        int largest = findLargestNumber(array);
        int smallest = findSmallestNumber(array);

        System.out.println("Largest number: " + largest);
        System.out.println("Smallest number: " + smallest);
    }

    public static int findLargestNumber(int[] array) {
        int largest = Integer.MIN_VALUE;

        for (int num : array) {
            if (num > largest) {
                largest = num;
            }
        }

        return largest;
    }

    public static int findSmallestNumber(int[] array) {
        int smallest = Integer.MAX_VALUE;

        for (int num : array) {
            if (num < smallest) {
                smallest = num;
            }
        }

        return smallest;
    }
}
```

----

## **Write a program in Java to find second highest number in an integer array?**

```java
public class FindSecondHighest {
    public static void main(String[] args) {
        int[] array = {5, 8, 2, 10, 3, 1};

        int secondHighest = findSecondHighestNumber(array);

        System.out.println("Second highest number: " + secondHighest);
    }

    public static int findSecondHighestNumber(int[] array) {
        int highest = Integer.MIN_VALUE;
        int secondHighest = Integer.MIN_VALUE;

        for (int num : array) {
            if (num > highest) {
                secondHighest = highest;
                highest = num;
            } else if (num > secondHighest && num < highest) {
                secondHighest = num;
            }
        }

        return secondHighest;
    }
}
```

----

## **Write a program in Java to find top two maximum number in array?**

```java
public class FindTopTwoMax {
    public static void main(String[] args) {
        int[] array = {5, 8, 2, 10, 3, 1};

        int[] topTwoMax = findTopTwoMaximumNumbers(array);

        System.out.println("Top two maximum numbers: " + topTwoMax[0] + " and " + topTwoMax[1]);
    }

    public static int[] findTopTwoMaximumNumbers(int[] array) {
        int max1 = Integer.MIN_VALUE;
        int max2 = Integer.MIN_VALUE;

        for (int num : array) {
            if (num > max1) {
                max2 = max1;
                max1 = num;
            } else if (num > max2 && num != max1) {
                max2 = num;
            }
        }

        int[] result = {max1, max2};
        return result;
    }
}
```

----

## **Java program to print array in reverse Order?**

```java
public class ReverseArray {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5};

        System.out.println("Original Array:");
        printArray(array);

        System.out.println("\nArray in Reverse Order:");
        printArrayInReverse(array);
    }

    public static void printArray(int[] array) {
        for (int num : array) {
            System.out.print(num + " ");
        }
    }

    public static void printArrayInReverse(int[] array) {
        for (int i = array.length - 1; i >= 0; i--) {
            System.out.print(array[i] + " ");
        }
    }
}
```

----

## **Java program to reverse array without using second array?**

```java
public class ReverseArray {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5};

        System.out.println("Original Array:");
        printArray(array);

        System.out.println("\nArray in Reverse Order:");
        reverseArray(array);

        System.out.println("\nReversed Array:");
        printArray(array);
    }

    public static void printArray(int[] array) {
        for (int num : array) {
            System.out.print(num + " ");
        }
    }

    public static void reverseArray(int[] array) {
        int start = 0;
        int end = array.length - 1;

        while (start < end) {
            int temp = array[start];
            array[start] = array[end];
            array[end] = temp;
            start++;
            end--;
        }
    }
}
```

----

## **Java Program to calculate length of an array?**

```java
public class ArrayLength {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5};

        int length = calculateArrayLength(array);

        System.out.println("Length of the array: " + length);
    }

    public static int calculateArrayLength(int[] array) {
        return array.length;
    }
}
```

----

## **Java program to insert an element at end of an Array?**

```java
public class InsertAtEnd {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5};
        int elementToInsert = 6;

        System.out.println("Original Array:");
        printArray(array);

        int[] newArray = insertAtEnd(array, elementToInsert);

        System.out.println("\nArray after inserting element at the end:");
        printArray(newArray);
    }

    public static void printArray(int[] array) {
        for (int num : array) {
            System.out.print(num + " ");
        }
    }

    public static int[] insertAtEnd(int[] array, int element) {
        int[] newArray = new int[array.length + 1];

        for (int i = 0; i < array.length; i++) {
            newArray[i] = array[i];
        }

        newArray[newArray.length - 1] = element;

        return newArray;
    }
}
```

----

## **Java program to insert element at a given location in Array?**

```java
public class InsertAtLocation {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5};
        int elementToInsert = 10;
        int insertIndex = 2;

        System.out.println("Original Array:");
        printArray(array);

        int[] newArray = insertAtLocation(array, elementToInsert, insertIndex);

        System.out.println("\nArray after inserting element at index " + insertIndex + ":");
        printArray(newArray);
    }

    public static void printArray(int[] array) {
        for (int num : array) {
            System.out.print(num + " ");
        }
    }

    public static int[] insertAtLocation(int[] array, int element, int index) {
        int[] newArray = new int[array.length + 1];

        for (int i = 0; i < index; i++) {
            newArray[i] = array[i];
        }

        newArray[index] = element;

        for (int i = index + 1; i < newArray.length; i++) {
            newArray[i] = array[i - 1];
        }

        return newArray;
    }
}
```

----

## **Java Program to delete element at end of Array?**

```java
public class DeleteAtEnd {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5};

        System.out.println("Original Array:");
        printArray(array);

        int[] newArray = deleteAtEnd(array);

        System.out.println("\nArray after deleting element from the end:");
        printArray(newArray);
    }

    public static void printArray(int[] array) {
        for (int num : array) {
            System.out.print(num + " ");
        }
    }

    public static int[] deleteAtEnd(int[] array) {
        int[] newArray = new int[array.length - 1];

        for (int i = 0; i < newArray.length; i++) {
            newArray[i] = array[i];
        }

        return newArray;
    }
}
```

----

## **Java Program to delete given element from Array?**

```java
public class DeleteElementFromArray {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5};
        int elementToDelete = 3;

        System.out.println("Original Array:");
        printArray(array);

        int[] newArray = deleteElement(array, elementToDelete);

        System.out.println("\nArray after deleting " + elementToDelete + ":");
        printArray(newArray);
    }

    public static void printArray(int[] array) {
        for (int num : array) {
            System.out.print(num + " ");
        }
    }

    public static int[] deleteElement(int[] array, int element) {
        int indexToDelete = -1;

        // Find the index of the element to delete
        for (int i = 0; i < array.length; i++) {
            if (array[i] == element) {
                indexToDelete = i;
                break;
            }
        }

        if (indexToDelete == -1) {
            // Element not found, return the original array
            return array;
        }

        int[] newArray = new int[array.length - 1];
        int newIndex = 0;

        // Copy elements to the new array, except the one to be deleted
        for (int i = 0; i < array.length; i++) {
            if (i != indexToDelete) {
                newArray[newIndex] = array[i];
                newIndex++;
            }
        }

        return newArray;
    }
}
```

----

## **Java Program to delete element from array at given index?**

```java

```

----

## **Java Program to find sum of array elements?**

```java
public class DeleteElementAtIndex {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5};
        int indexToDelete = 2;

        System.out.println("Original Array:");
        printArray(array);

        int[] newArray = deleteAtIndex(array, indexToDelete);

        System.out.println("\nArray after deleting element at index " + indexToDelete + ":");
        printArray(newArray);
    }

    public static void printArray(int[] array) {
        for (int num : array) {
            System.out.print(num + " ");
        }
    }

    public static int[] deleteAtIndex(int[] array, int index) {
        if (index < 0 || index >= array.length) {
            // Index is out of range, return the original array
            return array;
        }

        int[] newArray = new int[array.length - 1];
        int newIndex = 0;

        // Copy elements to the new array, except the one at the given index
        for (int i = 0; i < array.length; i++) {
            if (i != index) {
                newArray[newIndex] = array[i];
                newIndex++;
            }
        }

        return newArray;
    }
}
```

----

## **Java Program to print all even numbers in array?**

```java
public class PrintEvenNumbers {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

        System.out.println("Original Array:");
        printArray(array);

        System.out.println("\nEven Numbers in the Array:");
        printEvenNumbers(array);
    }

    public static void printArray(int[] array) {
        for (int num : array) {
            System.out.print(num + " ");
        }
    }

    public static void printEvenNumbers(int[] array) {
        for (int num : array) {
            if (num % 2 == 0) {
                System.out.print(num + " ");
            }
        }
    }
}
```

----

## **Java Program to print all odd numbers in array?**

```java
public class PrintOddNumbers {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

        System.out.println("Original Array:");
        printArray(array);

        System.out.println("\nOdd Numbers in the Array:");
        printOddNumbers(array);
    }

    public static void printArray(int[] array) {
        for (int num : array) {
            System.out.print(num + " ");
        }
    }

    public static void printOddNumbers(int[] array) {
        for (int num : array) {
            if (num % 2 != 0) {
                System.out.print(num + " ");
            }
        }
    }
}
```

----

## **Java program to perform left rotation of array elements by two positions?**

```java
public class LeftRotateArray {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5};

        System.out.println("Original Array:");
        printArray(array);

        int[] rotatedArray = leftRotateByTwo(array);

        System.out.println("\nArray after left rotation by two positions:");
        printArray(rotatedArray);
    }

    public static void printArray(int[] array) {
        for (int num : array) {
            System.out.print(num + " ");
        }
    }

    public static int[] leftRotateByTwo(int[] array) {
        int[] rotatedArray = new int[array.length];

        for (int i = 0; i < array.length - 2; i++) {
            rotatedArray[i] = array[i + 2];
        }

        rotatedArray[array.length - 2] = array[0];
        rotatedArray[array.length - 1] = array[1];

        return rotatedArray;
    }
}
```

----

## **Java program to perform right rotation in array by 2 positions?**

```java
public class RightRotateArray {
    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5};

        System.out.println("Original Array:");
        printArray(array);

        int[] rotatedArray = rightRotateByTwo(array);

        System.out.println("\nArray after right rotation by two positions:");
        printArray(rotatedArray);
    }

    public static void printArray(int[] array) {
        for (int num : array) {
            System.out.print(num + " ");
        }
    }

    public static int[] rightRotateByTwo(int[] array) {
        int[] rotatedArray = new int[array.length];

        rotatedArray[0] = array[array.length - 2];
        rotatedArray[1] = array[array.length - 1];

        for (int i = 2; i < array.length; i++) {
            rotatedArray[i] = array[i - 2];
        }

        return rotatedArray;
    }
}
```

----

## **Java program to find all pairs in array of integers whose sum is equal to given number?**

```java

```

----

## **Java Program to remove duplicate elements form array?**

```java
import java.util.ArrayList;
import java.util.List;

public class FindPairs {
    public static void main(String[] args) {
        int[] array = {2, 4, 5, 7, 8, 9};
        int targetSum = 9;

        List<Pair> pairs = findPairs(array, targetSum);

        System.out.println("Pairs with sum " + targetSum + ":");
        for (Pair pair : pairs) {
            System.out.println(pair.toString());
        }
    }

    public static List<Pair> findPairs(int[] array, int targetSum) {
        List<Pair> pairs = new ArrayList<>();

        for (int i = 0; i < array.length; i++) {
            for (int j = i + 1; j < array.length; j++) {
                if (array[i] + array[j] == targetSum) {
                    pairs.add(new Pair(array[i], array[j]));
                }
            }
        }

        return pairs;
    }

    static class Pair {
        int first;
        int second;

        public Pair(int first, int second) {
            this.first = first;
            this.second = second;
        }

        @Override
        public String toString() {
            return "(" + first + ", " + second + ")";
        }
    }
}
```

----


### https://quescol.com/interview-preparation/core-java-coding-questions

### https://quescol.com/interview-preparation/core-java-pattern-questions

## **Different Types of Pyramid Patterns**

*Half pyramid pattern programquescol*

```java
public class HalfPyramidPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```

----

*Half Pyramid Pattern using **

```java
public class HalfPyramidPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("*");
            }
            System.out.println();
        }
    }
}
```

----

*Right inverted half pyramid program in c quescol*

```c
#include <stdio.h>

int main() {
    int rows = 5;

    for (int i = 1; i <= rows; i++) {
        for (int j = 1; j <= rows - i + 1; j++) {
            printf("* ");
        }
        printf("\n");
    }

    return 0;
}
```

----

*Right Inverted Half Pyramid Pattern*

```java
public class RightInvertedHalfPyramid {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= rows - i + 1; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```

----


*Half pyramid using number in C*

```c
#include <stdio.h>

int main() {
    int rows = 5;

    for (int i = 1; i <= rows; i++) {
        for (int j = 1; j <= i; j++) {
            printf("%d ", j);
        }
        printf("\n");
    }

    return 0;
}
```

----

*Half Pyramid Pattern*

```java
public class HalfPyramidPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```

----

*Inverted half pyramid program quescol*

```java
public class InvertedHalfPyramidPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = rows; i >= 1; i--) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```

----

*Inverted Half Pyramid Pattern*

```java
public class InvertedHalfPyramidPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = rows; i >= 1; i--) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```

----

*Full pyramid pattern program in c using star quescol*

```c
#include <stdio.h>

int main() {
    int rows = 5;
    int space, i, j;

    for (i = 1; i <= rows; i++) {
        for (space = 1; space <= rows - i; space++) {
            printf(" ");
        }
        for (j = 1; j <= 2 * i - 1; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

----

*Full Pyramid Pattern*

```java
public class FullPyramidPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= rows - i; j++) {
                System.out.print(" ");
            }
            for (int k = 1; k <= 2 * i - 1; k++) {
                System.out.print("*");
            }
            System.out.println();
        }
    }
}

```

----

*Inverted half pyramid using number program in c*

```c
#include <stdio.h>

int main() {
    int rows = 5;

    for (int i = rows; i >= 1; i--) {
        for (int j = 1; j <= i; j++) {
            printf("%d ", j);
        }
        printf("\n");
    }

    return 0;
}
```

----

*Inverted Half Pyramid Pattern*

```java
public class InvertedHalfPyramidPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = rows; i >= 1; i--) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```

----


*Right half pyramid program quescol*

```java
public class RightHalfPyramidPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```

----

*Right Half Pyramid Pattern*

```java
public class RightHalfPyramidPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= rows - i; j++) {
                System.out.print("  ");
            }
            for (int k = 1; k <= i; k++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```

----


*Inverted full pyramid pattern program in c using star*

```c
#include <stdio.h>

int main() {
    int rows = 5;

    for (int i = rows; i >= 1; i--) {
        for (int j = 1; j <= rows - i; j++) {
            printf("  ");
        }
        for (int k = 1; k <= 2 * i - 1; k++) {
            printf("* ");
        }
        printf("\n");
    }

    return 0;
}
```

----

*Inverted Full Pyramid Pattern*

```java
public class InvertedFullPyramidPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = rows; i >= 1; i--) {
            for (int j = 1; j <= rows - i; j++) {
                System.out.print("  ");
            }
            for (int k = 1; k <= 2 * i - 1; k++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```

----

*Full pyramid using number program in c*

```c
#include <stdio.h>

int main() {
    int rows = 5;
    int number = 1;

    for (int i = 1; i <= rows; i++) {
        for (int j = 1; j <= rows - i; j++) {
            printf("  ");
        }
        for (int k = 1; k <= i; k++) {
            printf("%d ", number++);
        }
        printf("\n");
    }

    return 0;
}
```

----

*Full Pyramid Pattern*

```java
public class FullPyramidPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= rows - i; j++) {
                System.out.print(" ");
            }
            for (int k = 1; k <= 2 * i - 1; k++) {
                System.out.print("*");
            }
            System.out.println();
        }
    }
}
```

----


## **Different Types of Diamond Patterns**

*Solid right half diamond pattern program in C*

```c
#include <stdio.h>

int main() {
    int rows = 5;

    for (int i = 1; i <= rows; i++) {
        for (int j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }
    for (int i = rows - 1; i >= 1; i--) {
        for (int j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

----

*Right Half Diamond Pattern*

```java
public class RightHalfDiamondPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("*");
            }
            System.out.println();
        }
        for (int i = rows - 1; i >= 1; i--) {
            for (int j = 1; j <= i; j++) {
                System.out.print("*");
            }
            System.out.println();
        }
    }
}
```

----


*solid left half diamond pattern program in c*

```c
#include <stdio.h>

int main() {
    int rows = 5;

    for (int i = 1; i <= rows; i++) {
        for (int j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }
    for (int i = rows - 1; i >= 1; i--) {
        for (int j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

----

*Left Half Diamond Pattern*

```java
public class LeftHalfDiamondPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("*");
            }
            System.out.println();
        }
        for (int i = rows - 1; i >= 1; i--) {
            for (int j = 1; j <= i; j++) {
                System.out.print("*");
            }
            System.out.println();
        }
    }
}
```

----

*Solid diamond using star program in c*

```c
#include <stdio.h>

int main() {
    int rows = 5;
    int i, j, k;

    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= rows - i; j++) {
            printf(" ");
        }
        for (k = 1; k <= 2 * i - 1; k++) {
            printf("*");
        }
        printf("\n");
    }

    for (i = rows - 1; i >= 1; i--) {
        for (j = 1; j <= rows - i; j++) {
            printf(" ");
        }
        for (k = 1; k <= 2 * i - 1; k++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

----

*Full Diamond Pattern*

```java
public class FullDiamondPattern {
    public static void main(String[] args) {
        int rows = 5;

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= rows - i; j++) {
                System.out.print(" ");
            }
            for (int k = 1; k <= 2 * i - 1; k++) {
                System.out.print("*");
            }
            System.out.println();
        }

        for (int i = rows - 1; i >= 1; i--) {
            for (int j = 1; j <= rows - i; j++) {
                System.out.print(" ");
            }
            for (int k = 1; k <= 2 * i - 1; k++) {
                System.out.print("*");
            }
            System.out.println();
        }
    }
}
```

----

*Pascal triangle pattern program in c*

```c
#include <stdio.h>

int main() {
    int rows, coefficient = 1;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (int i = 0; i < rows; i++) {
        for (int space = 1; space <= rows - i; space++) {
            printf("  ");
        }

        for (int j = 0; j <= i; j++) {
            if (j == 0 || i == 0) {
                coefficient = 1;
            } else {
                coefficient = coefficient * (i - j + 1) / j;
            }
            printf("%4d", coefficient);
        }

        printf("\n");
    }

    return 0;
}
```

----

*Pascal’s Traingle*

```java
import java.util.Scanner;

public class PascalTriangle {
    public static void main(String[] args) {
        int rows, coefficient = 1;

        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of rows: ");
        rows = scanner.nextInt();

        for (int i = 0; i < rows; i++) {
            for (int space = 1; space <= rows - i; space++) {
                System.out.print("  ");
            }

            for (int j = 0; j <= i; j++) {
                if (j == 0 || i == 0) {
                    coefficient = 1;
                } else {
                    coefficient = coefficient * (i - j + 1) / j;
                }
                System.out.printf("%4d", coefficient);
            }

            System.out.println();
        }

        scanner.close();
    }
}
```

----

*Floyd triangle pattern program in c*

```c
#include <stdio.h>

int main() {
    int rows, number = 1;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (int i = 1; i <= rows; i++) {
        for (int j = 1; j <= i; j++) {
            printf("%d ", number);
            number++;
        }
        printf("\n");
    }

    return 0;
}
```

----

*Print Floyd's Triangle*

```java
import java.util.Scanner;

public class FloydTriangle {
    public static void main(String[] args) {
        int rows, number = 1;

        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of rows: ");
        rows = scanner.nextInt();

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print(number + " ");
                number++;
            }
            System.out.println();
        }

        scanner.close();
    }
}
```

----

## **Different Types of Rhombus Patterns**

*Solid rhombus right inclined pattern program in c*

```c
#include <stdio.h>

int main() {
    int rows, i, j;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= rows - i; j++) {
            printf(" ");
        }
        for (j = 1; j <= rows; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

----

*Solid Rhombus Right Inclined*

```java
import java.util.Scanner;

public class SolidRhombusRightInclined {
    public static void main(String[] args) {
        int rows;

        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of rows: ");
        rows = scanner.nextInt();

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= rows - i; j++) {
                System.out.print(" ");
            }
            for (int j = 1; j <= rows; j++) {
                System.out.print("*");
            }
            System.out.println();
        }

        scanner.close();
    }
}
```

----

*Solid rhombus left inclined pattern program in C*

```c
import java.util.Scanner;

public class SolidRhombusRightInclined {
    public static void main(String[] args) {
        int rows;

        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of rows: ");
        rows = scanner.nextInt();

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= rows - i; j++) {
                System.out.print(" ");
            }
            for (int j = 1; j <= rows; j++) {
                System.out.print("*");
            }
            System.out.println();
        }

        scanner.close();
    }
}
```

----

*Solid Rhombus Left Inclined*

```java
import java.util.Scanner;

public class SolidRhombusLeftInclined {
    public static void main(String[] args) {
        int rows;

        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of rows: ");
        rows = scanner.nextInt();

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i - 1; j++) {
                System.out.print(" ");
            }
            for (int j = 1; j <= rows; j++) {
                System.out.print("*");
            }
            System.out.println();
        }

        scanner.close();
    }
}
```

----

## **Different Types of Rectangle Patterns**

*Solid rectangle pattern program in C*

```c
#include <stdio.h>

int main() {
    int rows, columns, i, j;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);
    printf("Enter the number of columns: ");
    scanf("%d", &columns);

    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= columns; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

----

*Solid Rectangle*

```java
import java.util.Scanner;

public class SolidRectanglePattern {
    public static void main(String[] args) {
        int rows, columns;

        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of rows: ");
        rows = scanner.nextInt();
        System.out.print("Enter the number of columns: ");
        columns = scanner.nextInt();

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= columns; j++) {
                System.out.print("*");
            }
            System.out.println();
        }

        scanner.close();
    }
}
```

----

*Hollow rectangle pattern program in C*

```c
#include <stdio.h>

int main() {
    int rows, columns, i, j;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);
    printf("Enter the number of columns: ");
    scanf("%d", &columns);

    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= columns; j++) {
            if (i == 1 || i == rows || j == 1 || j == columns) {
                printf("*");
            } else {
                printf(" ");
            }
        }
        printf("\n");
    }

    return 0;
}
```

----

*Hollow Rectangle*

```java
import java.util.Scanner;

public class HollowRectanglePattern {
    public static void main(String[] args) {
        int rows, columns;

        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of rows: ");
        rows = scanner.nextInt();
        System.out.print("Enter the number of columns: ");
        columns = scanner.nextInt();

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= columns; j++) {
                if (i == 1 || i == rows || j == 1 || j == columns) {
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }

        scanner.close();
    }
}
```

----

## **Different Types of Patterns Using Star And Hyphen**

*Star hyphen combination pattern program in c*

```c
#include <stdio.h>

int main() {
    int rows, i, j;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= i; j++) {
            if (j % 2 == 0) {
                printf("-");
            } else {
                printf("*");
            }
        }
        printf("\n");
    }

    return 0;
}
```

----

*Star hyphen combination pattern 1*

```java
import java.util.Scanner;

public class StarHyphenPattern {
    public static void main(String[] args) {
        int rows;

        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of rows: ");
        rows = scanner.nextInt();

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                if (j % 2 == 0) {
                    System.out.print("-");
                } else {
                    System.out.print("*");
                }
            }
            System.out.println();
        }

        scanner.close();
    }
}
```

----

*Star hyphen combination 3 pattern program in C*

```c
#include <stdio.h>

int main() {
    int rows, i, j;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= i; j++) {
            if (j % 2 == 0) {
                printf("-");
            } else {
                printf("*");
            }
        }
        printf("\n");
    }

    for (i = rows - 1; i >= 1; i--) {
        for (j = 1; j <= i; j++) {
            if (j % 2 == 0) {
                printf("-");
            } else {
                printf("*");
            }
        }
        printf("\n");
    }

    return 0;
}
```

----

*Triangle Using Star Hyphen*

```java
import java.util.Scanner;

public class TrianglePattern {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of rows: ");
        int rows = scanner.nextInt();

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= rows - i; j++) {
                System.out.print("-");
            }
            for (int j = 1; j <= i; j++) {
                System.out.print("*");
                if (j < i) {
                    System.out.print("-");
                }
            }
            System.out.println();
        }

        scanner.close();
    }
}
```

----

*Star hyphen combination pattern program in c*

```c
#include <stdio.h>

int main() {
    int rows, i, j;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= i; j++) {
            if (j % 2 == 0) {
                printf("-");
            } else {
                printf("*");
            }
        }
        printf("\n");
    }

    return 0;
}
```

----

*Star hyphen combination pattern 2*

```java
import java.util.Scanner;

public class StarHyphenPattern {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of rows: ");
        int rows = scanner.nextInt();

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                if (j % 2 == 0) {
                    System.out.print("-");
                } else {
                    System.out.print("*");
                }
            }
            System.out.println();
        }

        scanner.close();
    }
}
```

----

*Inverted Triangle Using Star Hyphen pattern program in C*

```c
#include <stdio.h>

int main() {
    int rows, i, j;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (i = rows; i >= 1; i--) {
        for (j = 1; j <= rows - i; j++) {
            printf("-");
        }
        for (j = 1; j <= 2 * i - 1; j++) {
            if (j % 2 == 0) {
                printf("-");
            } else {
                printf("*");
            }
        }
        printf("\n");
    }

    return 0;
}
```

----

*Inverted Triangle Using Star Hyphen*

```java
#include <stdio.h>

int main() {
    int rows, i, j;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (i = rows; i >= 1; i--) {
        for (j = 1; j <= rows - i; j++) {
            printf("-");
        }
        for (j = 1; j <= 2 * i - 1; j++) {
            if (j % 2 == 0) {
                printf("-");
            } else {
                printf("*");
            }
        }
        printf("\n");
    }

    return 0;
}
```

----

*Star hyphen combination full pattern program in c*

```c
#include <stdio.h>

int main() {
    int rows, i, j;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    // Upper half of the pattern
    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= i; j++) {
            if (j % 2 == 0) {
                printf("-");
            } else {
                printf("*");
            }
        }
        printf("\n");
    }

    // Lower half of the pattern
    for (i = rows - 1; i >= 1; i--) {
        for (j = 1; j <= i; j++) {
            if (j % 2 == 0) {
                printf("-");
            } else {
                printf("*");
            }
        }
        printf("\n");
    }

    return 0;
}
```

----

*Diamond Using Star Hyphen*

```java
import java.util.Scanner;

public class DiamondPattern {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of rows: ");
        int rows = scanner.nextInt();

        // Upper half of the diamond
        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= rows - i; j++) {
                System.out.print("-");
            }
            for (int j = 1; j <= 2 * i - 1; j++) {
                System.out.print("*");
            }
            System.out.println();
        }

        // Lower half of the diamond
        for (int i = rows - 1; i >= 1; i--) {
            for (int j = 1; j <= rows - i; j++) {
                System.out.print("-");
            }
            for (int j = 1; j <= 2 * i - 1; j++) {
                System.out.print("*");
            }
            System.out.println();
        }

        scanner.close();
    }
}
```

----

### https://quescol.com/interview-preparation/core-java-pattern-questions

### https://quescol.com/interview-preparation/java-interview-question-experienced
### https://quescol.com/interview-preparation/java-interview-question-experienced

### https://quescol.com/interview-preparation/spring-boot-interview-questions

----

## **What is Java Spring Boot?**

Java Spring Boot is an open-source tool that makes it easier to use Java-based frameworks to create microservices and web apps.
For any definition of Spring Boot, the conversation has to start with Java—one of the most popular and widely used development
languages and computing platforms for app development. Developers all over the world start their coding journey learning Java.
Flexible and user-friendly, Java is a developer favorite for a variety of apps—everything from social media, web, and gaming
apps to networking and enterprise applications.

----

## **Explain the Spring Boot key components?**

There are four important key components of spring-boot are
- Spring Boot auto-configuration.
- Spring Boot CLI.
- Spring Boot starter POMs.
- Spring Boot Actuators.

There are two more Spring Boot components
- Spring initializr: To quick start new Spring Boot projects
- Spring Boot IDEs: We have multiple Spring Boot IDEs for example : Eclipse IDE, IntelliJ IDEA, Spring STS Suite etc

Now we will discuss these Spring Boot four components one by one in detail:

*Spring Boot AutoConfigurator*

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

*Spring Boot CLI*

Spring Boot CLI also known as Spring Boot Command Line Interface. It is a Spring Boot tool that allow to run and test Spring Boot applications using command prompt.

When we run Spring Boot applications using CLI, it internally uses Spring Boot Starter and Spring Boot AutoConfigurate components to resolve all dependencies and execute the application.

We can run even Spring Web Applications with simple Spring Boot CLI Commands.

Spring Boot CLI basically run the Groovy scripts. It allows you to quickly develop Spring Framework applications. Groovy scripts is very similar to Java but without boilerplate code.

*Spring Boot Actuator*

Spring Boot Actuator is also a very important Component of the Spring Boot. It helps to monitor the sprint boot applications health , understand traffics, knowing the state of the database, operational information about the running application like metrics, info, dump, env. Spring Boot Actuator also Provides production-grade tools without having to actually implement these features ourselves.

The Three main features of Spring Boot Actuator are

Endpoints
Metrics
Audit
Whenever we run  the Spring Boot Web Application, Spring Boot Actuator provides hostname as “localhost” and default port number as “8080”. We can access this application using “https://localhost:8080/” end point.

----

## **Tell some List of Sprint Boot Actuator EndPoints**

Some of Spring Boot Actuator End Point are:

*auditevents*: This endpoint Exposes the audit events information for the current application.
*beans*: Displays the list of all the Spring beans of application.
*health*: Display the health information of spring boot application.
*caches*: Exposes the all available caches.
*env*: Exposes the  all properties from Spring’s ConfigurableEnvironment.
*metrics*: It Shows the ‘metrics’ information for the current application.

There are some more Spring Actuator endpoints are loggers, mappings, sessions, shutdown, flyway, conditions, etc

----

## **Tell us some benefits of Spring Boot over Spring?**

Ans: Spring boot framework is the extension of spring framework to help developers to start coding with low configuration. It eliminates the boilerplate configurations required for setting up a Spring application. 

Spring Boot comes with multiple starter dependencies for different Spring modules. 

*Some of the most commonly used dependencies are:*
- spring-boot-starter-web
- spring-boot-starter-data-jpa
- spring-boot-starter-security
- spring-boot-starter-test
- spring-boot-starter-thymeleaf
- spring-boot-starter-actuator

*Below are the features provided by spring boot but spring doesn't:*
- Starter POM
- Auto Configuration
- Component Scanning
- Embedded server
- InMemory DB
- Actuators
- Version Management

----

## **What is the starter dependency of the Spring boot module?**

Some of Spring Boot Starter Dependencies are

Spring Boot Starter web:

Important features of spring-boot-starter-web are It is compatible for web development and Provides Auto configuration. This spring-boot-starter-web dependency pulls all dependencies which is used in the Spring Boot web development.

Below is the code to add Spring Boot Starter web in Spring Boot project using POM.xml.

```xml
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```

Spring Boot Starter Actuator:

This dependency is used to monitor and manage the Spring Boot application. Below is the code to add Spring Boot Starter Actuator in Spring Boot project using POM.xml.

```xml
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-actuator</artifactId>
</dependency> 
```

Spring Boot Starter Security:

This dependency is used in Spring Boot application to add the Security in Spring Boot Application. Below is the code to add Spring Boot Starter Security in Spring Boot project using POM.xml.

```xml
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-security</artifactId>
</dependency> 
```

Spring Boot Starter ThymeLeaf:

Spring Boot Starter ThymeLeaf Dependency  is used to create a web application. It provides a good support for serving a XHTML/HTML5 in web applications. Below is the code to add Spring Boot Starter ThymeLeaf in Spring Boot project using POM.xml.

```xml
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-thymeleaf</artifactId>
</dependency> 
```

Spring Boot Starter Test:

This dependency is used in Spring Boot Application to write the Unit Test cases of Java methods. Below is the code to add Spring Boot Starter Test in Spring Boot project using POM.xml.

```xml
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-test</artifactId>
</dependency>
```

----

## **What is Spring Boot dependency management?**

Spring Boot dependency management system manages dependencies and configuration automatically. We need not to specify the version of the dependencies in our configuration file. Spring Boot automatically upgrades all dependencies added in configuration file when we update the Spring Boot version.

----

## **How does Spring Boot works Internally?**

When we Create Spring Boot Application we add the starter Dependencies in it. This Starter Dependencies automatically configures Spring Boot application based on the dependencies you have added to the project. We add `@EnableAutoConfiguration` annotation for the configuration. Suppose if you have not configured any database connection, Spring Boot auto-configures an in-memory database. The entry point of the spring boot application is the class contains @SpringBootApplication annotation and the main method. `@ComponentScan` annotation scans all the components included in the Spring Boot Application automatically.

----

## **Explain Auto Configuration in Spring Boot?**

Spring Boot Auto Configuration , configures Spring application based on the dependencies we have added in the project. For Autoconfiguration we will add `@EnableAutoConfiguration` annotation or @SpringBootApplication annotation in main class file. This annotation will automatically automatically configure Spring Boot application.

Lets see the below example for better understanding.

```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.EnableAutoConfiguration;
@EnableAutoConfiguration
public class SpringBootApplicationDemo {
   public static void main(String[] args) {
      SpringApplication.run(SpringBootApplicationDemo.class, args);
   }
}
```

*Spring Boot Application*

Class that  contains  @SpringBootApplication annotation denotes the entry point of the Spring Boot Application. This class should have the main method to run the Spring Boot application. @SpringBootApplication annotation includes Auto- Configuration, Component Scan, and Spring Boot Configuration.

If we add `@SpringBootApplication` annotation in java class, we need not to add any other annotation like `@EnableAutoConfiguration`, `@ComponentScan` and `@SpringBootConfiguration`.

We can say SpringBootApplication  = EnableAutoConfiguration + ComponentScan + SpringBootConfiguration.

Below example show how we can use SpringBootApplication annotations.

```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class SpringBootApplicationDemo {
   public static void main(String[] args) {
      SpringApplication.run(SpringBootApplicationDemo.class, args);
   }
}
```

*Component Scan*

In Spring Boot application `@ComponentScan` annotation scan all your components that is added in your project. This annotation scans all the beans and package declarations when the application initializes.

Without writing any explicit code, Spring will Scan our application for classes annotated with `@Component`, Instantiate them and inject any specified dependencies into them and Inject them wherever needed.

Below is the example of using component scan

```java
import org.springframework.boot.SpringApplication;
import org.springframework.context.annotation.ComponentScan;

@ComponentScan
public class SpringBootApplicationDemo {
   public static void main(String[] args) {
      SpringApplication.run(SpringBootApplicationDemo.class, args);
   }
}
```

----

## **How does a spring boot application get started?**

Ans:

Spring Boot application Looks for the class having @SpringBootApplication annotation with main method. This method serves as an entry point, which invokes the SpringApplication.run method to start the application.

@SpringBootApplication 
public class SpringBootApplicationDemo{    
       public static void main(String[] args) {        
             SpringApplication.run(SpringBootApplicationDemo.class); 
       } 
}

----

## **Tell some commonly used Spring Boot CLI commands?**

Some commonly used Spring Boot CLI Commands Are:

-run, -test, -install, -uninstall, -grap, -jar, -war, –init, -shell, -help etc

----

## **Tell Some Basic Annotations used in Spring Boot?**

The Spring Boot annotations reside in its org.springframework.boot.autoconfigure package and its sub-packages.

Some Common and Important Spring Boot Annotations are:

`@EnableAutoConfiguration` – It makes Spring Boot look for auto-configuration beans on its classpath and automatically apply them.

`@SpringBootApplication` – This annotation is used to denote the main class of a Boot Application. This annotation combines @Configuration, @EnableAutoConfiguration, and @ComponentScan annotations with their default attributes.

Some More annotations of Spring Boot are:

For Application Basic Setup

- @SpringBootApplication

- @ComponentScan

- @Configuration

- @EnableAutoConfiguration

For Request Response

- @GetMapping

- @PostMapping

- @RequestMapping

For Component Types

- @Repository

- @Service

- @Component

- @Controller

----

## **What is Spring Boot dependency management?**

Spring Boot manages dependencies and configuration automatically. We don’t need to mention the version of the dependencies in our configuration. We can say Dependency Management as it is a way to manage the dependencies efficiently in one place. When we update the Spring Boot version Spring Boot upgrades all dependencies automatically.

----

## **How you can change the port of embedded Tomcat server in Spring Boot?**

There are two ways to change the default port of server in Spring Boot

1). Using application.properties file

server.port = 8081

In the application.properties file just change the default value of port to value what you wanted to be. Here we have given 8081 as a new port value.

2). Using application.yaml file

Server:

   Port:8081

Also you can change the port value from application.yaml by changing the default value of port to value what you wanted to be. Here we have also given 8081 as a new port value.

----

## **How you can change the tomcat server to any other Server in Spring Boot?**

To Replace the embedded tomcat server in Spring Boot first we have to exclude the default server from the pom.xml. And to  add new server we will add the new dependency.

For example:

To exclude tomcat from starter dependency add below code in pom.xml

```xml
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

<!-- And to include new server add as a dependency. Below is the example to add jetty server. -->

<dependency>  
  <groupId>org.springframework.boot</groupId>  
  <artifactId>spring-boot-starter-jetty</artifactId>
</dependency>
```

----

## **What is @RestController annotation in Sprint boot?**

@RestController  annotation is a combination of @Controller and @ResponseBody annotation. It is used to make restful web services and also it converts the response to JSON or XML. This annotation is used at the class level and it allows class to handle the requests made by the client.

----

## **What is the difference between @Controller and @RestController?**

With @controller annotation class is responsible for preparing a model Map with data to be displayed by the view But @RestController annotation class is responsible  for creating Restful controllers.
@controller only behave as controller, we need to add @responsebody annotation with method to return value and writes it to the HTTP response. But @RestController annotation is a combination of @controller and @responsebody which by default converts return as HTTP Response.
@Controller is used to mark classes as Spring MVC Controller whereas @RestController annotation mark class as RESTful Web services.
In @Controller, we need to use @ResponseBody on every handler method but in @RestController we don’t need to use @ResponseBody on every handler method.
@Controller annotation added in Spring 2.0 version whereas @RestController annotation added in Spring 4.0 version.

----

## **What is the difference between RequestMapping and GetMapping?**

RequestMapping annotation is used with GET, POST, PUT, and other request methods. getMapping is an extension of RequestMapping which helps you to improve on clarity of requests.
@RequestMapping annotation is used on a class level but the @GetMapping is used on method-level

----

## **What is Actuator in Spring Boot?**

Ans: An actuator in Spring boot is a feature  that helps you to monitor and manage your application when you push it to production. These actuators include auditing, health, CPU usage, HTTP hits, metric gathering, and many more that are automatically applied to your application.

----

## **What is the process to enable Actuator in Spring boot application?**

To enable the spring actuator feature, we need to add the dependency of “spring-boot-starter-actuator” in pom.xml.

Below is the xml snippet that can be added 

```xml
<dependency>
    <groupId> org.springframework.boot</groupId>
    <artifactId> spring-boot-starter-actuator </artifactId>
</dependency>
```

----

## **Tell some endpoint actuator-provide to monitor the Spring boot application?**

Actuators provide below pre-defined endpoints to monitor our application:
- Health
- Info
- Beans
- Mappings
- Configprops
- Httptrace
- Heapdump
- Threaddump
- Shutdown

----

## **What is the use of Profiles in spring boot?**

To Complete the development process of an application  or we can say during  the development of any application, we deal with multiple
environments such as dev, test and Prod. Sometime we need specific configuration at each environment level. Suppose we are using an
embedded H2 database for dev but for prod, we might have proprietary Oracle.

A profile is a set of configuration settings. Spring Boot allows to define profile specific property files in the form of
application-{profile}.properties. It automatically loads the properties in an application.properties file for all profiles,
and the ones in profile-specific property files only for the specified profile. 

----

## **What is dependency Injection in Spring Boot?**

The process of injecting dependent objects into target class is called dependency injection. Suppose our one class is dependent on the another class object. In that case we will provide the other class object to our class. This process is known as dependency injections.

There are multiple ways to inject the dependencies.

Setter Injection: The IOC container will inject the dependent bean object into the target bean object by calling the setter method.
Constructor Injection: Here IOC container will pass the dependent object via constructor of the class.

```java
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
```

----

## **What is an IOC container?**

IoC Container is a framework for implementing automatic dependency injection. It manages object creation and its life-time and also injects dependencies into the class.

----

## **Tell the steps how you will create spring boot project using Spring Initializer?**

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

## **Tell some difference between @RequestParam vs @PathVariable Annotations?**

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

----

## **Tell something about Spring @GetMapping, @PostMapping, @PutMapping, @DeleteMapping and @PatchMapping?**

@GetMapping – It is a shortcut for @RequestMapping(method = RequestMethod.GET). It is used to get single or all values from the database in Spring Application.

@PostMapping – It is a shortcut for @RequestMapping(method = RequestMethod.POST). Method that has @PostMapping annotation is responsible to Create single or multiple entries in the database. It is used to create single or multiple value in the database in Spring Application.

@PutMapping – It is a shortcut for @RequestMapping(method = RequestMethod.PUT). Method that has @PutMapping annotation is responsible to update the data in the database.

@PatchMapping – It is a shortcut for @RequestMapping(method = RequestMethod.PATCH)

@PatchMapping  annotation is used when we want to apply a partial update on the database.

@DeleteMapping – It is a shortcut for @RequestMapping(method =RequestMethod.DELETE). It is used to Delete single or multiple value from the database in the Spring Application.

----

## **What is Thymeleaf in Spring Boot?**

Thymeleaf is a server-side Java-based template engine. It is used for both web and standalone environments. It is capable of processing HTML, XML, JavaScript, CSS and even plain text. 

----

## **Tell some embedded containers supported by Spring Boot?**

There are three embedded containers supported by Spring Boot are :

Tomcat (used by default)
Undertow
Jetty

----

## **Are exit () and return statements same in function definition?**

No, both are different as we used exit() to immediately exit from the program, where as return is used to return the control of programs execution from the called function to calling function.

----

## **When is the “void” keyword used in a function?**

When we declare the function we have to decide whether we want some return value from the function or not, if we only want to print some value or statements on the screen we use void on the left side of function name otherwise we place the data type of the value on the left side of function name.

----

## **Differentiate between call by value and call by reference?**

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

## **Explain rand() function in c. Write a program in c to generate a random number?**

The rand() function in c is used to generate a random number.

### https://quescol.com/interview-preparation/spring-boot-interview-questions

### https://javarevisited.blogspot.com/2015/10/133-java-interview-questions-answers-from-last-5-years.html#axzz80dfcO0nd


## **Can we make array volatile in Java?**

This is one of the tricky Java multi-threading questions you will see in senior Java developer Interview. Yes, you can make an array volatile in Java but only the reference which is pointing to an array, not the whole array. What I mean, if one thread changes the reference variable to points to another array, that will provide a volatile guarantee, but if multiple threads are changing individual array elements they won't be having happens before guarantee provided by the volatile modifier.

----

## **Can volatile make a non-atomic operation to atomic?**

This another good question I love to ask on volatile, mostly as a follow-up of the previous question. This question is also not easy to answer because volatile is not about atomicity, but there are cases where you can use a volatile variable to make the operation atomic.

One example I have seen is having a long field in your class. If you know that a long field is accessed by more than one thread e.g. a counter, a price field or anything, you better make it volatile. Why? because reading to a long variable is not atomic in Java and done in two steps, If one thread is writing or updating long value, it's possible for another thread to see half value (fist 32-bit). While reading/writing a volatile long or double (64 bit) is atomic.

----

## **What are practical uses of volatile modifier?**

One of the practical use of the volatile variable is to make reading double and long atomic. Both double and long are 64-bit wide and they are read in two parts, first 32-bit first time and next 32-bit second time, which is non-atomic but volatile double and long read is atomic in Java. Another use of the volatile variable is to provide a memory barrier, just like it is used in Disrupter framework. Basically, Java Memory model inserts a write barrier after you write to a volatile variable and a read barrier before you read it. Which means, if you write to volatile field then it's guaranteed that any thread accessing that variable will see the value you wrote and anything you did before doing that right into the thread is guaranteed to have happened and any updated data values will also be visible to all threads, because the memory barrier flushed all other writes to the cache.

----

## **What guarantee volatile variable provides?**

volatile variables provide the guarantee about ordering and visibility e.g. volatile assignment cannot be re-ordered with other statements but in the absence of any synchronization instruction compiler, JVM or JIT are free to reorder statements for better performance. volatile also provides the happens-before guarantee which ensures changes made in one thread is visible to others. In some cases volatile also provide atomicity e.g. reading 64-bit data types like long and double are not atomic but read of volatile double or long is atomic.

----

## **Which one would be easy to write? synchronization code for 10 threads or 2 threads?**

In terms of writing code, both will be of same complexity because synchronization code is independent of a number of threads. Choice of synchronization though depends upon a number of threads because the number of thread present more contention, so you go for advanced synchronization technique e.g. lock stripping, which requires more complex code and expertise.

----

## **How do you call wait() method? using if block or loop? Why?**

wait() method should always be called in loop because it's possible that until thread gets CPU to start running again the condition might not hold, so it's always better to check condition in loop before proceeding. Here is the standard idiom of using wait and notify method in Java:

```java
// The standard idiom for using the wait method
synchronized (obj) {
   while (condition does not hold)
      obj.wait(); // (Releases lock, and reacquires on wakeup)
      ... // Perform action appropriate to condition
}
```

See Effective Java Item 69 to learn more about why wait method should call in the loop.

----

## **What is false sharing in the context of multi-threading?**

false sharing is one of the well-known performance issues on multi-core systems, where each process has its local cache. false sharing occurs when threads on different processor modify variables that reside on same cache line as shown in the following image:

Java Interview questions for experienced programmers

False sharing is very hard to detect because the thread may be accessing completely different global variables that happen to be relatively close together in memory. Like many concurrency issues, the primary way to avoid false sharing is careful code review and aligning your data structure with the size of a cache line.


----

## **What is busy spin? Why should you use it?**

Busy spin is one of the technique to wait for events without releasing CPU. It's often done to avoid losing data in CPU cached which is lost if the thread is paused and resumed in some other core. So, if you are working on low latency system where your order processing thread currently doesn't have any order, instead of sleeping or calling wait(), you can just loop and then again check the queue for new messages. It's only beneficial if you need to wait for a very small amount of time e.g. in micro seconds or nano seconds. LMAX Disrupter framework, a high-performance inter-thread messaging library has a BusySpinWaitStrategy which is based on this concept and uses a busy spin loop for EventProcessors waiting on the barrier.

----

## **How do you take thread dump in Java?**

You can take a thread dump of Java application in Linux by using kill -3 PID, where PID is the process id of Java process. In Windows, you can press Ctrl + Break. This will instruct JVM to print thread dump in standard out or err and it could go to console or log file depending upon your application configuration. If you have used Tomcat then when

----

## **is Swing thread-safe?**

No, Swing is not thread-safe. You cannot update Swing components e.g. JTable, JList or JPanel from any thread, in fact, they must be updated from GUI or AWT thread. That's why swings provide invokeAndWait() and invokeLater() method to request GUI update from any other threads. This methods put update request in AWT threads queue and can wait till update or return immediately for an asynchronous update. You can also check the detailed answer to learn more.

----

## **What is a thread local variable in Java?**

Thread-local variables are variables confined to a thread, its like thread's own copy which is not shared between multiple threads. Java provides a ThreadLocal class to support thread-local variables. It's one of the many ways to achieve thread-safety. Though be careful while using thread local variable in manged environment e.g. with web servers where worker thread out lives any application variable. Any thread local variable which is not removed once its work is done can potentially cause a memory leak in Java application.

----

## **Write wait-notify code for producer-consumer problem?**

Please see the answer for a code example. Just remember to call wait() and notify() method from synchronized block and test waiting for condition on the loop instead of if block.

----

## **Write code for thread-safe Singleton in Java?**

Please see the answer for a code example and step by step guide to creating thread-safe singleton class in Java. When we say thread-safe, which means Singleton should remain singleton even if initialization occurs in the case of multiple threads. Using Java enum as Singleton class is one of the easiest ways to create a thread-safe singleton in Java.

----

## **The difference between sleep and wait in Java?**

Though both are used to pause currently running thread, sleep() is actually meant for short pause because it doesn't release lock, while wait() is meant for conditional wait and that's why it release lock which can then be acquired by another thread to change the condition on which it is waiting.

----

## **What is an immutable object? How do you create an Immutable object in Java?**

Immutable objects are those whose state cannot be changed once created. Any modification will result in a new object e.g. String, Integer, and other wrapper class. Please see the answer for step by step guide to creating Immutable class in Java.

----

## **Can we create an Immutable object, which contains a mutable object?**

Yes, its possible to create an Immutable object which may contain a mutable object, you just need to be a little bit careful not to share the reference of the mutable component, instead, you should return a copy of it if you have to. Most common example is an Object which contain the reference of java.util.Date object.

----

## **Date types and Basic Java Interview Questions**

----

## **What is the right data type to represent a price in Java?**

BigDecimal if memory is not a concern and Performance is not critical, otherwise double with predefined precision.

----

## **How do you convert bytes to String?**

you can convert bytes to the string using string constructor which accepts byte[], just make sure that right character encoding otherwise platform's default character encoding will be used which may or may not be same.

----

## **How do you convert bytes to long in Java?**
This questions if for you to answer :-)

----

## **Can we cast an int value into byte variable? what will happen if the value of int is larger than byte?**

Yes, we can cast but int is 32 bit long in java while byte is 8 bit long in java so when you cast an int to byte higher 24 bits are lost and a byte can only hold a value from -128 to 128.

----

## **There are two classes B extends A and C extends B, Can we cast B into C e.g. C = (C) B**

----

## **Which class contains clone method? Cloneable or Object?**

java.lang.Cloneable is marker interface and doesn't contain any method clone method is defined in the object class. It is also knowing that clone() is a native method means it's implemented in C or C++ or any other native language.

----

## **Is ++ operator is thread-safe in Java?**

 No it's not a thread safe operator because its involve multiple instructions like reading a value, incriminating it and storing it back into memory which can be overlapped between multiple threads.

----

## **Difference between a = a + b and a += b ?**

The += operator implicitly cast the result of addition into the type of variable used to hold the result. When you add two integral variable e.g. variable of type byte, short, or int then they are first promoted to int and them addition happens. If result of addition is more than maximum value of a then a + b will give compile time error but a += b will be ok as shown below
byte a = 127;
byte b = 127;
b = a + b; // error : cannot convert from int to byte
b += a; // ok

----

## **Can I store a double value in a long variable without casting?**

No, you cannot store a double value into a long variable without casting because the range of double is more  that long and you we need to type cast. It's not dificult to answer this question but many develoepr get it wrong due to confusion on which one is bigger between double and long in Java.

----

## **What will this return 3*0.1 == 0.3? true or false?**

This is one of the really tricky questions. Out of 100, only 5 developers answered this question and only of them have explained the concept correctly. The short answer is false because some floating point numbers can not be represented exactly.

----

## **Which one will take more memory, an int or Integer?**

An Integer object will take more memory an Integer is the an object and it  store meta data overhead about the object and int is primitive type so its takes less space.

----

## **Why is String Immutable in Java?**

One of my favorite Java interview question. The String is Immutable in java because java designer thought that string will be heavily used and making it immutable allow some optimization easy sharing same String object between multiple clients. See the link for the more detailed answer. This is a great question for Java programmers with less experience as it gives them food for thought, to think about how things works in Java, what Jave designers might have thought when they created String class etc.

----

## **Can we use String in the switch case?**

Yes from Java 7 onward we can use String in switch case but it is just syntactic sugar. Internally string hash code is used for the switch. See the detaiedl answer for more explanation and discussion.

----

## **What is constructor chaining in Java?**

When you call one constructor from other than it's known as constructor chaining in Java. This happens when you have multiple, overloaded constructor in the class.

----

## **JVM Internals and Garbage Collection Interview Questions**

----

In last a couple of years I have seen increased focus on JVM internal and Garbage collection tuning, monitoring Java appliation, dealing with Java performance issues on various Java interviews. This is actually become the prime topic for interviewing any experienced Java developer for senior position e.g. technical lead, VP or team lead. If you feel you are short of experience and knowledge in this area then you should read atleast one book mentioned in my list of Java Performance books. I vote goes to Java Performance, The Definitive guide by Scott.

----

## **What is the size of int in 64-bit JVM?**

The size of an int variable is constant in Java, it's always 32-bit irrespective of platform. Which means the size of primitive int is same in both 32-bit and 64-bit Java virtual machine.

----

## **The difference between Serial and Parallel Garbage Collector?**

Even though both the serial and parallel collectors cause a stop-the-world pause during Garbage collection. The main difference between them is that a serial collector is a default copying collector which uses only one GC thread for garbage collection while a parallel collector uses multiple GC threads for garbage collection.

----

## **What is the size of an int variable in 32-bit and 64-bit JVM?**

The size of int is same in both 32-bit and 64-bit JVM, it's always 32 bits or 4 bytes.

----

## **A difference between WeakReference and SoftReference in Java?**

Though both WeakReference and SoftReference helps garbage collector and memory efficient, WeakReference becomes eligible for garbage collection as soon as last strong reference is lost but SoftReference even thought it can not prevent GC, it can delay it until JVM absolutely need memory.

----

## **How do WeakHashMap works?**

WeakHashMap works like a normal HashMap but uses WeakReference for keys, which means if the key object doesn't have any reference then both key/value mapping will become eligible for garbage collection.

----

## **What is -XX:+UseCompressedOops JVM option? Why use it?**

When you go migrate your Java application from 32-bit to 64-bit JVM, the heap requirement suddenly increases, almost double, due to increasing size of ordinary object pointer from 32 bit to 64 bit. This also adversely affect how much data you can keep in CPU cache, which is much smaller than memory. Since main motivation for moving to 64-bit JVM is to specify large heap size, you can save some memory by using compressed OOP. By using -XX:+UseCompressedOops, JVM uses 32-bit OOP instead of 64-bit OOP.

----

## **How do you find if JVM is 32-bit or 64-bit from Java Program?**

You can find that by checking some system properties like sun.arch.data.model or os.arch


----

## **What is the maximum heap size of 32-bit and 64-bit JVM?**

Theoretically, the maximum heap memory you can assign to a 32-bit JVM is 2^32 which is 4GB but practically the limit is much smaller. It also varies between operating systems e.g. form 1.5GB in Windows to almost 3GB in Solaris. 64-bit JVM allows you to specify larger heap size, theoretically 2^64 which is quite large but practically you can specify heap space up to 100GBs. There are even JVM e.g. Azul where heap space of 1000 gigs is also possible.

----

## **What is the difference between JRE, JDK, JVM and JIT?**

JRE stands for Java run-time and it's required to run Java application. JDK stands for Java development kit and provides tools to develop Java program e.g. Java compiler. It also contains JRE. The JVM stands for Java virtual machine and it's the process responsible for running Java application. The JIT stands for Just In Time compilation and helps to boost the performance of Java application by converting Java byte code into native code when the crossed certain threshold i.e. mainly hot code is converted into native code.

----

## **Java Interview Questions for 3 years experience**

----

## **Explain Java Heap space and Garbage collection?**
When a Java process is started using java command, memory is allocated to it. Part of this memory is used to create heap space, which is used to allocate memory to objects whenever they are created in the program. Garbage collection is the process inside JVM which reclaims memory from dead objects for future allocation.

----

## **Can you guarantee the garbage collection process?**

No, you cannot guarantee the garbage collection, though you can make a request using System.gc() or Runtime.gc() method.

----

## **How do you find memory usage from Java program? How much percent of the heap is used?**

You can use memory related methods from java.lang.Runtime class to get the free memory, total memory and maximum heap memory in Java.  By using these methods, you can find out how many percents of the heap is used and how much heap space is remaining. Runtime.freeMemory() return amount of free memory in bytes, Runtime.totalMemory() returns total memory in bytes and Runtime.maxMemory() returns maximum memory in bytes.

----

## **What is the difference between stack and heap in Java?**

Stack and heap are different memory areas in the JVM and they are used for different purposes. The stack is used to hold method frames and local variables while objects are always allocated memory from the heap. The stack is usually much smaller than heap memory and also didn't shared between multiple threads, but heap is shared among all threads in JVM.

----

## ***What's the difference between "a == b" and "a.equals(b)"?**

The a = b does object reference matching if both a and b are an object and only return true if both are pointing to the same object in the heap space, on the other hand, a.equals(b) is used for logical mapping and its expected from an object to override this method to provide logical equality. For example, String class overrides this equals() method so that you can compare two Strings, which are the different object but contains same letters.

----


## **What is a.hashCode() used for? How is it related to a.equals(b)?**

hashCode() method returns an int hash value corresponding to an object. It's used in hash based collection classes e.g Hashtable, HashMap, LinkedHashMap and so on. It's very tightly related to equals() method. According to Java specification, two objects which are equal to each other using equals() method must have same hash code.

----

## **Difference between final, finalize and finally?**

The final is a modifier which you can apply to variable, methods and classes. If you make a variable final it means its value cannot be changed once initialized. finalize is a method, which is called just before an object is a garbage collected, giving it last chance to resurrect itself, but the call to finalize is not guaranteed. finally is a keyword which is used in exception handling along with try and catch. the finally block is always executed irrespective of whether an exception is thrown from try block or not.

----

## **What is a compile time constant in Java? What is the risk of using it?**

public static final variables are also known as a compile time constant, the public is optional there. They are replaced with actual values at compile time because compiler know their value up-front and also knows that it cannot be changed during run-time. One of the problem with this is that if you happened to use a public static final variable from some in-house or third party library and their value changed later than your client will still be using old value even after you deploy a new version of JARs. To avoid that, make sure you compile your program when you upgrade dependency JAR files.

----

## **The difference between List, Set, Map, and Queue in Java?**

The list is an ordered collection which allows duplicate. It also has an implementation which provides constant time index based access, but that is not guaranteed by List interface. Set is unordered collection which

----

## **Difference between poll() and remove() method?**

Both poll() and remove() take out the object from the Queue but if poll() fails then it returns null but if remove fails it throws Exception.

----

## **The difference between LinkedHashMap and PriorityQueue in Java?**

PriorityQueue guarantees that lowest or highest priority element always remain at the head of the queue, but LinkedHashMap maintains the order on which elements are inserted. When you iterate over a PriorityQueue, iterator doesn't guarantee any order but iterator of LinkedHashMap does guarantee the order on which elements are inserted.

----

## **Difference between ArrayList and LinkedList in Java?**

The obvious difference between them is that ArrrayList is backed by array data structure, supprots random access and LinkedList is backed by linked list data structure and doesn't supprot random access. Accessing an element with the index is O(1) in ArrayList but its O(n) in LinkedList. See the answer for more detailed discussion.

----

## **What is a couple of ways that you could sort a collection?**

You can either use the Sorted collection like TreeSet or TreeMap or you can sort using the ordered collection like a list and using Collections.sort() method.

----

## **How do you print Array in Java?**

You can print an array by using the Arrays.toString() and Arrays.deepToString() method. Since array doesn't implement toString() by itself, just passing an array to System.out.println() will not print its contents but Arrays.toString() will print each element.

----

## **LinkedList in Java is doubly or singly linked list?**

It's a doubly linked list, you can check the code in JDK. In Eclipse, you can use the shortcut, Ctrl + T to directly open this class in Editor.

----

## **Which kind of tree is used to implement TreeMap in Java?**

A Red Black tree is used to implement TreeMap in Java.

----

## **What is the difference between Hashtable and HashMap?**

There are many differences between these two classes, some of them are following:
a) Hashtable is a legacy class and present from JDK 1, HashMap was added later.
b) Hashtable is synchronized and slower but HashMap is not synchronized and faster.
c) Hashtable doesn't allow null keys but HashMap allows one null key.
See the answer for more differences between HashMap and Hashtable in Java.

----

## **How HashSet works internally in Java?**

HashSet is internally implemented using an HashMap. Since a Map needs key and value, a default value is used for all keys. Similar to HashMap, HashSet doesn't allow duplicate keys and only one null key, I mean you can only store one null object in HashSet.

----

## **Write code to remove elements from ArrayList while iterating?**

 Key here is to check whether candidate uses ArrayList's remove() or Iterator's remove(). Here is the sample code which uses right way o remove elements from ArrayList while looping over and avoids ConcurrentModificationException.

----

## **Can I write my own container class and use it in the for-each loop?**

Yes, you can write your own container class. You need to implement the Iterable interface if you want to loop over advanced for loop in Java, though. If you implement Collection then you by default get that property.

----

## **What is default size of ArrayList and HashMap in Java?**

As of Java 7 now, default size of ArrayList is 10 and default capacity of HashMap is 16, it must be power of 2. Here is code snippet from ArrayList  and HashMap class :

```java
// from ArrayList.java JDK 1.7
private static final int DEFAULT_CAPACITY = 10;  

//from HashMap.java JDK 7
static final int DEFAULT_INITIAL_CAPACITY = 1 << 4; // aka 16
```

----

## **Is it possible for two unequal objects to have the same hashcode?**

Yes, two unequal objects can have same hashcode that's why collision happen in a hashmap.
the equal hashcode contract only says that two equal objects must have the same hashcode it doesn't say anything about the unequal object.

----

## **Can two equal object have the different hash code?**

No, thats not possible according to hash code contract.

----

## **Can we use random numbers in the hashcode() method?**

No, because hashcode of an object should be always same. See the answer to learning more about things to remember while overriding hashCode() method in Java.

----


## **What is the difference between Comparator and Comparable in Java?**

The Comparable interface is used to define the  natural order of object while Comparator is used to define custom order. Comparable can be always one, but we can have multiple comparators to define customized order for objects.

----

## **Why you need to override hashcode, when you override equals in Java?**

Because equals have code contract mandates to override equals and hashcode together .since many container class like HashMap or HashSet depends on hashcode and equals contract.

----

## **In my Java program, I have three sockets? How many threads I will need to handle that**

To handle three sockets in a Java program, you typically need three separate threads, one for each socket. Each thread will be responsible for handling the communication and processing associated with its corresponding socket.

Here's a simple example illustrating the usage of multiple threads to handle three sockets:

```java
import java.io.IOException;
import java.net.ServerSocket;
import java.net.Socket;

public class SocketHandlerExample {
    public static void main(String[] args) throws IOException {
        int port1 = 1234;
        int port2 = 5678;
        int port3 = 9999;

        // Create threads for each socket
        Thread thread1 = new SocketHandlerThread(port1);
        Thread thread2 = new SocketHandlerThread(port2);
        Thread thread3 = new SocketHandlerThread(port3);

        // Start the threads
        thread1.start();
        thread2.start();
        thread3.start();
    }

    static class SocketHandlerThread extends Thread {
        private final int port;

        SocketHandlerThread(int port) {
            this.port = port;
        }

        @Override
        public void run() {
            try {
                ServerSocket serverSocket = new ServerSocket(port);
                System.out.println("Listening on port " + port);

                while (true) {
                    Socket clientSocket = serverSocket.accept();
                    // Handle the client socket communication and processing here
                    // You can create a separate class or method to encapsulate the logic
                }
            } catch (IOException e) {
                e.printStackTrace();
            }
        }
    }
}
```

In this example, we create three threads (SocketHandlerThread) to handle three separate sockets. Each thread listens on a specific port using a ServerSocket and enters a loop to accept client connections (Socket).

Inside the loop, you can handle the communication and processing for each client socket according to your program's requirements. You can create a separate class or method to encapsulate the logic for handling the socket operations.

By starting the three threads, each one will handle the incoming client connections independently and concurrently.

Note that this is a basic example to illustrate the concept of handling multiple sockets with multiple threads. In a real-world scenario, you might need to consider additional factors like thread synchronization, thread pool management, error handling, and scalability, depending on the complexity and specific requirements of your program.

----

## **How do you create ByteBuffer in Java?**

In Java, you can create a ByteBuffer using the ByteBuffer.allocate() method or the ByteBuffer.wrap() method. Here's how you can use each method:

Using ByteBuffer.allocate():

```java
int bufferSize = 1024; // Specify the desired buffer size in bytes
ByteBuffer buffer = ByteBuffer.allocate(bufferSize);
```

This method creates a new ByteBuffer with the specified capacity. The buffer is initially filled with zeros.

Using ByteBuffer.wrap():

```java
byte[] byteArray = { 1, 2, 3, 4, 5 }; // Provide the byte array
ByteBuffer buffer = ByteBuffer.wrap(byteArray);
```

This method wraps an existing byte array into a ByteBuffer. Any changes made to the buffer will reflect in the underlying byte array.

Once you have created a ByteBuffer, you can use its various methods to read from or write to the buffer, manipulate its position and limit, and perform other operations.

It's worth noting that there are also other methods available for creating a ByteBuffer with different characteristics, such as ByteBuffer.allocateDirect() for creating a direct buffer that uses native memory or ByteBuffer.allocate(int capacity) to create a buffer with a specified capacity. The choice of which method to use depends on your specific requirements and use case.

----

## **How do you write and read from ByteBuffer in Java?**

```java
import java.nio.ByteBuffer;

public class ByteBufferExample {
    public static void main(String[] args) {
        int intValue = 42;
        double doubleValue = 3.14;

        // Create a ByteBuffer with a specific capacity
        ByteBuffer buffer = ByteBuffer.allocate(12);

        // Writing data to the ByteBuffer
        buffer.putInt(intValue);
        buffer.putDouble(doubleValue);

        // Resetting the position to prepare for reading
        buffer.flip();

        // Reading data from the ByteBuffer
        int readIntValue = buffer.getInt();
        double readDoubleValue = buffer.getDouble();

        // Output the read values
        System.out.println("Read int value: " + readIntValue);
        System.out.println("Read double value: " + readDoubleValue);
    }
}
```

----

## **Is Java BIG endian or LITTLE endian?**

Java is a language that is platform-independent and does not specify a particular endianness. The endianness (whether big-endian or little-endian) is determined by the underlying hardware architecture and the implementation of the Java Virtual Machine (JVM) on that platform.

Most modern processors and architectures, including x86 and x86-64, use the little-endian byte order. However, some other architectures, such as certain ARM processors and network protocols like IPv6, use big-endian byte order.

In Java, you can use the ByteOrder class from the java.nio package to explicitly specify the byte order when working with byte buffers. The default byte order used by Java's ByteBuffer is the native byte order of the platform.

For example, to create a ByteBuffer with big-endian byte order, you can use the order() method as follows:

```java
import java.nio.ByteBuffer;
import java.nio.ByteOrder;

public class ByteBufferEndianExample {
    public static void main(String[] args) {
        short value = 42;

        ByteBuffer buffer = ByteBuffer.allocate(2);
        buffer.order(ByteOrder.BIG_ENDIAN);

        buffer.putShort(value);

        buffer.flip();

        short readValue = buffer.getShort();

        System.out.println("Read value: " + readValue);
    }
}
```

In this example, the order() method is used to set the byte order of the ByteBuffer to big-endian explicitly before writing and reading the short value.

----

## **What is the byte order of ByteBuffer?**

The byte order of a ByteBuffer in Java is initially set to the native byte order of the underlying platform. The native byte order refers to the byte order used by the hardware architecture on which the Java Virtual Machine (JVM) is running.

You can determine the byte order of a ByteBuffer by using the order() method from the java.nio.ByteBuffer class. It returns a ByteOrder enum representing the current byte order of the buffer.

Here's an example:

```java
import java.nio.ByteBuffer;
import java.nio.ByteOrder;

public class ByteBufferByteOrderExample {
    public static void main(String[] args) {
        ByteBuffer buffer = ByteBuffer.allocate(4);

        ByteOrder byteOrder = buffer.order();

        System.out.println("Byte order: " + byteOrder);
    }
}
```

When you run this code, it will print the byte order of the ByteBuffer. The output will be either BIG_ENDIAN or LITTLE_ENDIAN, depending on the native byte order of your platform.

You can also explicitly set the byte order of a ByteBuffer using the order() method. For example, you can use buffer.order(ByteOrder.BIG_ENDIAN) or buffer.order(ByteOrder.LITTLE_ENDIAN) to set the byte order to a specific value regardless of the native byte order.

----

## **The difference between direct buffer and non-direct buffer in Java?**

In Java, the ByteBuffer class provides two types of buffers: direct buffers and non-direct (or heap) buffers. The main difference between these two types is how the underlying memory is allocated and accessed.

Direct Buffer:

A direct buffer is allocated outside of the JVM heap, typically in native memory.
It is created using the ByteBuffer.allocateDirect() method.
Direct buffers are intended for scenarios where data needs to be efficiently transferred between Java and native code or I/O operations.
Direct buffers can be more efficient for certain I/O operations, as they can be directly read from or written to by native I/O operations without the need for additional copying.
However, the memory allocation and deallocation of direct buffers are typically more expensive compared to non-direct buffers.
Direct buffers are generally recommended for large data transfers, such as network communication or disk I/O operations.
Non-Direct (Heap) Buffer:

A non-direct buffer is allocated within the JVM heap using the ByteBuffer.allocate() method.
Non-direct buffers are the default type of buffer created by ByteBuffer.allocate() and are suitable for most general-purpose scenarios.
They have a slightly higher memory allocation and deallocation overhead compared to direct buffers.
Non-direct buffers are managed by the Java garbage collector, which simplifies memory management.
They are typically used for various data processing tasks, such as in-memory computations or file processing, where the buffer's content is accessed and manipulated within the Java application itself.
It's important to note that the choice between direct and non-direct buffers depends on the specific requirements of your application. If you're working with large amounts of data or performing I/O operations that benefit from direct memory access, using direct buffers may provide performance advantages. However, for most general-purpose use cases, non-direct buffers are suitable and easier to work with.

----

## **What is the memory mapped buffer in Java?**

In Java, a memory-mapped buffer is a ByteBuffer that is associated with a region of memory mapped to a file or other data source. It allows you to directly read from or write to the mapped file as if you were accessing the buffer in memory, without explicit I/O operations.

The memory mapping technique provides a way to efficiently handle large files or data sources by leveraging the underlying operating system's virtual memory management. Instead of reading or writing data in smaller chunks, you can map a file into memory and access it as a contiguous block.

To create a memory-mapped buffer in Java, you can use the java.nio.channels.FileChannel class and its map() method. Here's an example:

```java
import java.io.IOException;
import java.io.RandomAccessFile;
import java.nio.MappedByteBuffer;
import java.nio.channels.FileChannel;

public class MemoryMappedBufferExample {
    public static void main(String[] args) {
        try (RandomAccessFile file = new RandomAccessFile("data.txt", "rw")) {
            FileChannel channel = file.getChannel();
            long fileSize = channel.size();

            // Map the entire file into memory
            MappedByteBuffer buffer = channel.map(FileChannel.MapMode.READ_WRITE, 0, fileSize);

            // Access the buffer as if it were in memory
            // Read or write data directly to the buffer

            // Remember to clean up resources
            buffer.clear();
            channel.close();
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

----

## **What is TCP NO DELAY socket option?**

The TCP_NODELAY socket option is used in TCP (Transmission Control Protocol) to disable the Nagle's algorithm.

The Nagle's algorithm is a technique used to improve network efficiency by reducing the number of small TCP packets that are sent over the network. By default, TCP uses the Nagle's algorithm, which buffers small amounts of outgoing data and delays sending until a sufficient amount of data is accumulated or a TCP acknowledgment (ACK) is received.

However, in some scenarios, such as real-time applications or situations where low latency is crucial, the Nagle's algorithm can introduce unwanted delays. In such cases, you can set the TCP_NODELAY socket option to disable the algorithm and send data immediately without waiting for additional data or ACKs.

When TCP_NODELAY is enabled (set to true), it indicates that the TCP stack should not buffer small amounts of data and should send each packet as soon as possible. This can result in smaller, more frequent TCP packets being sent, but it can reduce latency for applications where responsiveness is important.

In Java, you can enable or disable the TCP_NODELAY socket option using the setTcpNoDelay() method provided by the Socket class or the ServerSocket class. Here's an example:

```java
import java.net.Socket;
import java.io.IOException;

public class TcpNoDelayExample {
    public static void main(String[] args) {
        try {
            Socket socket = new Socket("example.com", 8080);

            // Enable TCP_NODELAY option
            socket.setTcpNoDelay(true);

            // Use the socket for communication

            socket.close();
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

In this example, we create a Socket and enable the TCP_NODELAY option by calling setTcpNoDelay(true) on the socket object. After enabling the option, the socket can be used for communication, and the data will be sent immediately without additional buffering.

It's important to note that enabling TCP_NODELAY can increase network overhead due to the smaller packet sizes, so it should be used judiciously in situations where low latency is a priority.

----

## **What is the difference between TCP and UDP protocol?**

TCP (Transmission Control Protocol) and UDP (User Datagram Protocol) are two widely used transport layer protocols in computer networks. Here are the key differences between them:

Connection-Oriented vs Connectionless:

TCP is a connection-oriented protocol. It establishes a reliable and ordered connection between the sender and receiver before data transmission. It guarantees the delivery of data packets in the order they were sent and handles retransmission of lost packets.
UDP is a connectionless protocol. It does not establish a dedicated connection between sender and receiver. Each UDP packet is independent and can be sent to the recipient without prior setup. It does not guarantee delivery or order of packets.
Reliability:

TCP provides reliable transmission of data. It uses acknowledgments and retransmissions to ensure that all data packets are received correctly.
UDP does not guarantee reliable delivery. It does not have built-in mechanisms for acknowledgment or retransmission. If a UDP packet is lost or corrupted during transmission, it will not be automatically retransmitted.
Ordering:

TCP guarantees the ordering of data packets. It ensures that the packets are delivered in the same order they were sent.
UDP does not guarantee the ordering of packets. The packets may arrive at the receiver in a different order than they were sent.
Flow Control and Congestion Control:

TCP implements flow control and congestion control mechanisms to regulate the rate of data transmission and prevent network congestion.
UDP does not have built-in flow control or congestion control mechanisms. It allows the application to send packets at its own rate, which can potentially lead to network congestion.
Header Overhead:

TCP has a larger header size compared to UDP. TCP headers contain additional information for establishing and maintaining connections, sequencing packets, and handling reliability.
UDP has a smaller header size compared to TCP. UDP headers contain minimal information, providing a lightweight overhead.
Usage:

TCP is commonly used for applications that require reliable and ordered data delivery, such as web browsing, email, file transfer, and database communication.
UDP is suitable for applications that prioritize low latency and real-time communication, such as video streaming, voice over IP (VoIP), online gaming, and DNS (Domain Name System) queries.
Choosing between TCP and UDP depends on the specific requirements of the application. TCP is preferred when reliability and ordered delivery are crucial, while UDP is suitable for scenarios where low latency and real-time communication are more important, even at the expense of reliability.

----

## **The difference between ByteBuffer and StringBuffer in Java?**

ByteBuffer:

The ByteBuffer class is part of the java.nio package and is used for handling binary data. It provides a way to manage a fixed-size buffer of bytes.
ByteBuffer is primarily used for I/O operations, such as reading from or writing to channels, sockets, or files.
It offers methods for reading and writing various data types in binary format, such as integers, floats, and characters.
ByteBuffer is commonly used in scenarios where direct manipulation of binary data is required, such as network communication, serialization, and file handling.
StringBuffer:

The StringBuffer class is part of the java.lang package and is used for manipulating character strings.
StringBuffer is designed to be mutable, meaning you can modify its contents without creating a new object.
It provides methods for appending, deleting, inserting, and modifying strings.

StringBuffer is thread-safe, meaning it can be safely used in multithreaded environments without external synchronization.
StringBuffer is commonly used when you need to build or modify strings dynamically, such as constructing long strings or modifying existing strings in a thread-safe manner.
In summary, ByteBuffer is used for handling binary data and is often used in I/O operations, while StringBuffer is used for manipulating character strings and is commonly used when you need to dynamically build or modify strings.

----

## **Java Best Practices Interview question**

Contains best practices from different parts of Java programming e.g. Collections, String, IO, Multi-threading, Error and Exception handling, design patterns etc. This section is mostly for experience Java developer, technical lead,  AVP, team lead and coders who are responsible for products. If you want to create quality products you must know and follow the best practices.

----

## **What best practices you follow while writing multi-threaded code in Java?**

Here are couple of best practices which I follow while writing concurrent code in Java:
a) Always name your thread, this will help in debugging.
b) minimize the scope of synchronization, instead of making whole method synchronized, only critical section should be synchronized.
c) prefer volatile over synchronized if you can can.
e) use higher level concurrency utilities instead of waitn() and notify for inter thread communication e.g. BlockingQueue, CountDownLatch and Semeaphore.
e) Prefer concurrent collection over synchronized collection in Java. They provide better scalability.

----

## **Tell me few best practices you apply while using Collections in Java?**

Here are couple of best practices I follow while using Collectionc classes from Java:
a) Always use the right collection e.g. if you need non-synchronized list then use ArrayList and not Vector.
b) Prefer concurrent collection over synchronized collection because they are more scalable.
c) Always use interface to a represent and access a collection e.g. use List to store ArrayList, Map to store HashMap and so on.
d) Use iterator to loop over collection.
e) Always use generics with collection.

----

## **Can you tell us at least 5 best practice you use while using threads in Java?**

This is similar to the previous question and you can use the answer given there. Particularly with thread, you should:
a) name your thread
b) keep your task and thread separate, use Runnable or Callable with thread pool executor.
c) use thread pool
d) use volatile to indicate compiler about ordering, visibility, and atomicity.
e) avoid thread local variable because incorrect use of ThreadLocal class in Java can create a memory leak.
Look there are many best practices and I give extra points to the developer which bring something new, something even I don't know. I make sure to ask this question to Java developers of 8 to 10 years of experience just to gauge his hands on experience and knowledge.

----

## **Name 5 IO best practices?**

IO is very important for performance of your Java application. Ideally you should avoid IO in critical path of your application. Here are couple of Java IO best practices you can follow:
a) Use buffered IO classes instead of reading individual bytes and char.
b) Use classes from NIO and NIO2
c) Always close streams in finally block or use try-with-resource statements.
d) use memory mapped file for faster IO.
If a Java candidate doesn't know about IO and NIO, especially if he has at least 2 to 4 years of experience, he needs some reading.

----

## **Name 5 JDBC best practices your follow?**

Another good Java best practices for experienced Java developer of 7 to 8 years experience. Why it's important? because they are the ones which set the trend in the code and educate junior developers. There are many best practices and you can name as per your confort and conviniece. Here are some of the more common ones:
a) use batch statement for inserting and updating data.
b) use PreparedStatement to avoid SQL exception and better performance.
c) use database connection pool
d) access resultset using column name instead of column indexes.
e) Don't generate dynamic SQL by concatenating String with user input.

----

## **Name couple of method overloading best practices in Java?**

Here are some best practices you can follow while overloading a method in Java to avoid confusion with auto-boxing:
a) Don't overload method where one accepts int and other accepts Integer.
b) Don't overload method where number of argument is same and only order of argument is different.
c) Use varargs after overloaded methods has more than 5 arguments.

----

## **Does SimpleDateFormat is safe to use in the multi-threaded program?**

No, unfortunately, DateFormat and all its implementations including SimpleDateFormat is not thread-safe, hence should not be used in the multi-threaded program until external thread-safety measures are applied e.g. confining SimpleDateFormat object into a ThreadLocal variable. If you don't do that, you will get an incorrect result while parsing or formatting dates in Java. Though, for all practical date time purpose, I highly recommend joda-time library.

----

## **How do you format a date in Java? e.g. in the ddMMyyyy format?**

You can either use SimpleDateFormat class or joda-time library to format date in Java. DateFormat class allows you to format date on many popular formats. Please see the answer for code samples to format date into different formats e.g. dd-MM-yyyy or ddMMyyyy.

----

## **How do you show timezone in formatted date in Java?**

```java
import java.text.SimpleDateFormat;
import java.util.Date;
import java.util.TimeZone;

public class TimeZoneExample {
    public static void main(String[] args) {
        Date date = new Date();
        SimpleDateFormat sdf = new SimpleDateFormat("yyyy-MM-dd HH:mm:ss z");
        sdf.setTimeZone(TimeZone.getTimeZone("America/New_York")); // Set the desired timezone
        String formattedDate = sdf.format(date);
        System.out.println("Formatted Date with Timezone: " + formattedDate);
    }
}
```

----

## **The difference between java.util.Date and java.sql.Date in Java?**

In Java, java.util.Date and java.sql.Date are two different classes that represent dates and times but have different purposes and are used in different contexts.

java.util.Date: This class represents a specific instant in time, including both the date and time components. It is part of the core Java library and can be used for general-purpose date and time operations. However, it has some limitations and is not recommended for new code.

java.sql.Date: This class is a subclass of java.util.Date and is specifically designed to work with databases in the context of Java Database Connectivity (JDBC). It represents only the date component (year, month, and day) and does not store the time information. It is used to interact with date columns in relational databases.

The key differences between java.util.Date and java.sql.Date are:

Representation: java.util.Date represents both the date and time components, while java.sql.Date represents only the date component.

Time information: java.util.Date includes the time information, such as hours, minutes, and seconds, along with the date. java.sql.Date does not store the time information and is set to midnight (00:00:00) in the default time zone.

Usage: java.util.Date is a general-purpose class for working with dates and times in Java. It can be used in various contexts outside of databases. java.sql.Date is specifically designed for working with databases using JDBC and is used for interacting with date columns in relational databases.

When working with databases, it is recommended to use the appropriate date and time classes provided by the JDBC API, such as java.sql.Date, java.sql.Time, and java.sql.Timestamp, for better compatibility and consistency with database operations. For general-purpose date and time operations, it is recommended to use the newer date and time classes introduced in Java 8, such as java.time.LocalDate, java.time.LocalTime, and java.time.LocalDateTime, which provide more flexibility and improved functionality.

----

## **How to you calculate the difference between two dates in Java?**

```java
import java.time.LocalDate;
import java.time.temporal.ChronoUnit;

public class DateDifferenceExample {
    public static void main(String[] args) {
        LocalDate date1 = LocalDate.of(2023, 1, 1);
        LocalDate date2 = LocalDate.now();

        long daysDiff = ChronoUnit.DAYS.between(date1, date2);
        System.out.println("Difference in days: " + daysDiff);

        long monthsDiff = ChronoUnit.MONTHS.between(date1, date2);
        System.out.println("Difference in months: " + monthsDiff);

        long yearsDiff = ChronoUnit.YEARS.between(date1, date2);
        System.out.println("Difference in years: " + yearsDiff);
    }
}
```

----

## **How do you convert a String(YYYYMMDD) to date in Java?**

```java
import java.text.ParseException;
import java.text.SimpleDateFormat;
import java.util.Date;

public class StringToDateExample {
    public static void main(String[] args) {
        String dateString = "20230516";
        SimpleDateFormat sdf = new SimpleDateFormat("yyyyMMdd");
        
        try {
            Date date = sdf.parse(dateString);
            System.out.println("Parsed Date: " + date);
        } catch (ParseException e) {
            System.out.println("Error parsing the date: " + e.getMessage());
        }
    }
}
```

----

## **How do you test static method?**

You can use PowerMock library to test static methods in Java.

To test a static method in Java, you can follow these steps:

Create a test class: Create a separate test class to contain your test methods. This class should be in the same package as the class containing the static method you want to test.

Write test methods: In your test class, write one or more test methods to verify the behavior of the static method. Each test method should be annotated with the @Test annotation from a testing framework like JUnit.

Call the static method: Inside each test method, call the static method you want to test, providing appropriate arguments.

Verify the results: Use assertions or other verification techniques to check if the static method produces the expected results. You can use assertions provided by testing frameworks like JUnit's assertEquals() or Hamcrest's assertThat().

Run the tests: Run your test class using a testing framework like JUnit. The testing framework will execute the test methods and report any failures or errors.

Here's an example using JUnit 4:

```java
import org.junit.Test;
import static org.junit.Assert.assertEquals;

public class MyStaticClassTest {

    @Test
    public void testStaticMethod() {
        // Call the static method
        int result = MyStaticClass.myStaticMethod(10, 5);
        
        // Verify the result
        assertEquals(15, result);
    }
}
```

----

## **How to do you test a method for an exception using JUnit?**


To test a method for an expected exception using JUnit, you can use the @Test annotation along with the expected attribute or the assertThrows() method. Here's how you can do it:

In this example, the @Test annotation is used with the expected attribute set to the expected exception class (MyException in this case). The test method testMethod() is executed, and it is expected that the MyClass.myMethod() will throw a MyException. If the exception is thrown during the execution of the method, the test will pass. If the exception is not thrown or a different exception is thrown, the test will fail.

```java
import org.junit.Test;

public class MyClassTest {

    @Test(expected = MyException.class)
    public void testMethod() throws MyException {
        // Call the method that is expected to throw an exception
        MyClass.myMethod();
    }
}
```

----

## **Which unit testing libraries you have used for testing Java programs?**

JUnit: JUnit is one of the most widely used unit testing frameworks for Java. It provides annotations, assertions, and test runners to write and execute tests effectively. JUnit has versions for both Java 4 (JUnit 4) and Java 5+ (JUnit 5).

TestNG: TestNG is another popular testing framework for Java. It offers additional features compared to JUnit, such as flexible test configuration, support for parameterized tests, and better reporting capabilities.

Mockito: Mockito is a mocking framework that allows you to create mock objects for testing. It works well in conjunction with JUnit and TestNG and helps in isolating and testing specific parts of your code.

PowerMock: PowerMock is an extension of Mockito and EasyMock frameworks. It enables you to mock static methods, final classes, and other difficult-to-test code constructs, providing more flexibility in unit testing.

AssertJ: AssertJ is a fluent assertion library that provides a rich set of assertion methods for making assertions in your tests. It offers a more readable and expressive syntax compared to the standard assertions available in JUnit or TestNG.

Hamcrest: Hamcrest is a library for writing matcher objects and performing more flexible assertions in your tests. It provides a large set of matchers that allow you to create custom assertions and make your tests more descriptive.

----

## **What is the difference between @Before and @BeforeClass annotation?**

In JUnit, the @Before and @BeforeClass annotations are used to mark methods that should be executed before each test method and before the test class, respectively. The main difference between them is when they are executed.

The @Before annotation is used to mark a method that should be executed before each test method. This is typically used to set up any necessary resources or objects that will be used by the test methods. The method annotated with @Before is executed once before each test method.

On the other hand, the @BeforeClass annotation is used to mark a method that should be executed before the first test method in the test class. This method is executed only once, and typically used to set up any static objects or resources that will be used by all test methods in the test class.

To summarize, @Before is executed before each test method, whereas @BeforeClass is executed only once before the first test method in the test class. It's important to note that methods annotated with @BeforeClass must be static, while methods annotated with @Before do not have to be static.

----

To check if a String contains only numeric digits in Java, you can use regular expressions or loop through the characters of the String. Here are examples of both approaches:

Using Regular Expressions:

## **How to check if a String contains only numeric digits?**

```java
public static boolean containsOnlyDigits(String str) {
    return str.matches("\\d+");
}
```

In this example, the matches() method is used with the regular expression \\d+. The \\d represents a digit and the + indicates one or more occurrences. The method will return true if the String contains only numeric digits and false otherwise.

```java
public static boolean containsOnlyDigits(String str) {
    for (char c : str.toCharArray()) {
        if (!Character.isDigit(c)) {
            return false;
        }
    }
    return true;
}
```

In this example, the toCharArray() method is used to convert the String into an array of characters. Then, each character is checked using the Character.isDigit() method to determine if it is a digit. If any character is found to not be a digit, the method returns false. If all characters are digits, the method returns true.

You can use either approach based on your preference and requirements. Regular expressions provide a concise way to check for digit patterns, while the loop approach gives you more flexibility for custom checks if needed.

----

## **How to write LRU cache in Java using Generics?**

To implement an LRU (Least Recently Used) cache in Java using generics, you can create a class that combines a LinkedHashMap and a maximum size limit. Here's an example:

java

```java
import java.util.LinkedHashMap;
import java.util.Map;

public class LRUCache<K, V> {

    private LinkedHashMap<K, V> cache;
    private int maxSize;

    public LRUCache(int maxSize) {
        this.maxSize = maxSize;
        this.cache = new LinkedHashMap<>(maxSize, 0.75f, true) {
            protected boolean removeEldestEntry(Map.Entry eldest) {
                return size() > maxSize;
            }
        };
    }

    public synchronized V get(K key) {
        return cache.get(key);
    }

    public synchronized void put(K key, V value) {
        cache.put(key, value);
    }

    public synchronized void clear() {
        cache.clear();
    }

    public synchronized int size() {
        return cache.size();
    }
}
```

In this example, the LRUCache class is defined with type parameters K for the key and V for the value. The cache is implemented using a LinkedHashMap, which maintains the insertion order of the elements. The removeEldestEntry method is overridden to limit the cache size by removing the least recently used entry when the cache reaches the maximum size.

The get method retrieves the value associated with a given key from the cache. The put method inserts a key-value pair into the cache. The clear method clears the cache, and the size method returns the current size of the cache.

You can use the LRUCache class with any data types by providing appropriate key and value types when creating an instance of the class. For example:

```java
LRUCache<String, Integer> cache = new LRUCache<>(10);
cache.put("key1", 100);
int value = cache.get("key1");  // Retrieves the value 100
```

By using generics, the LRUCache class provides flexibility in defining the key and value types according to your specific use case.

----

## **Write a Java program to convert bytes to long?**

```java
import java.nio.ByteBuffer;

public class ByteToLongExample {
    public static void main(String[] args) {
        byte[] bytes = {0x12, 0x34, 0x56, 0x78, 0x9A, 0xBC, 0xDE, 0xF0};
        
        long value = bytesToLong(bytes);
        
        System.out.println("Converted Long value: " + value);
    }
    
    public static long bytesToLong(byte[] bytes) {
        ByteBuffer buffer = ByteBuffer.wrap(bytes);
        return buffer.getLong();
    }
}
```

----

## **How to reverse a String in Java without using StringBuffer?**

```java
public class StringReversalExample {
    public static void main(String[] args) {
        String original = "Hello, World!";
        String reversed = reverseString(original);
        System.out.println("Reversed String: " + reversed);
    }
    
    public static String reverseString(String str) {
        char[] characters = str.toCharArray();
        int left = 0;
        int right = characters.length - 1;
        
        while (left < right) {
            // Swap characters at left and right indices
            char temp = characters[left];
            characters[left] = characters[right];
            characters[right] = temp;
            
            // Move indices towards the center
            left++;
            right--;
        }
        
        return new String(characters);
    }
}
```

----

## **How to find the word with the highest frequency from a file in Java?**

```java
import java.io.File;
import java.io.FileNotFoundException;
import java.util.HashMap;
import java.util.Map;
import java.util.Scanner;

public class HighestFrequencyWordExample {
    public static void main(String[] args) {
        File file = new File("input.txt");
        String mostFrequentWord = findMostFrequentWord(file);
        System.out.println("The most frequent word is: " + mostFrequentWord);
    }

    public static String findMostFrequentWord(File file) {
        Map<String, Integer> wordFrequency = new HashMap<>();

        try (Scanner scanner = new Scanner(file)) {
            while (scanner.hasNext()) {
                String word = scanner.next().toLowerCase();
                wordFrequency.put(word, wordFrequency.getOrDefault(word, 0) + 1);
            }
        } catch (FileNotFoundException e) {
            e.printStackTrace();
        }

        String mostFrequentWord = "";
        int highestFrequency = 0;

        for (Map.Entry<String, Integer> entry : wordFrequency.entrySet()) {
            String word = entry.getKey();
            int frequency = entry.getValue();
            if (frequency > highestFrequency) {
                highestFrequency = frequency;
                mostFrequentWord = word;
            }
        }

        return mostFrequentWord;
    }
}
```

----

## **How do you check if two given String are anagrams?**

```java
import java.util.Arrays;

public class AnagramCheckExample {
    public static void main(String[] args) {
        String str1 = "listen";
        String str2 = "silent";

        boolean areAnagrams = checkIfAnagrams(str1, str2);

        if (areAnagrams) {
            System.out.println(str1 + " and " + str2 + " are anagrams.");
        } else {
            System.out.println(str1 + " and " + str2 + " are not anagrams.");
        }
    }

    public static boolean checkIfAnagrams(String str1, String str2) {
        // Remove whitespace and convert to lowercase
        str1 = str1.replaceAll("\\s", "").toLowerCase();
        str2 = str2.replaceAll("\\s", "").toLowerCase();

        // Check if lengths are different
        if (str1.length() != str2.length()) {
            return false;
        }

        // Convert strings to character arrays
        char[] charArray1 = str1.toCharArray();
        char[] charArray2 = str2.toCharArray();

        // Sort character arrays
        Arrays.sort(charArray1);
        Arrays.sort(charArray2);

        // Compare sorted arrays
        return Arrays.equals(charArray1, charArray2);
    }
}
```

----

## **How to print all permutation of a String in Java?**

```java
public class StringPermutationExample {
    public static void main(String[] args) {
        String str = "abc";
        printPermutations(str);
    }

    public static void printPermutations(String str) {
        char[] chars = str.toCharArray();
        printPermutations(chars, 0, chars.length - 1);
    }

    private static void printPermutations(char[] chars, int left, int right) {
        if (left == right) {
            System.out.println(new String(chars));
        } else {
            for (int i = left; i <= right; i++) {
                swap(chars, left, i);
                printPermutations(chars, left + 1, right);
                swap(chars, left, i);
            }
        }
    }

    private static void swap(char[] chars, int i, int j) {
        char temp = chars[i];
        chars[i] = chars[j];
        chars[j] = temp;
    }
}
```

----

## **How do you print duplicate elements from an array in Java?**

```java
public class DuplicateElementsExample {
    public static void main(String[] args) {
        int[] arr = {1, 2, 3, 4, 3, 2, 1, 5, 6, 5};

        System.out.println("Duplicate elements in the array:");

        // Create a set to store unique elements
        Set<Integer> uniqueElements = new HashSet<>();
        
        // Iterate over the array
        for (int i = 0; i < arr.length; i++) {
            // If the element is already present in the set, it's a duplicate
            if (!uniqueElements.add(arr[i])) {
                System.out.println(arr[i]);
            }
        }
    }
}
```

----

## **How to convert String to int in Java?**

To convert a String to an int in Java, you can use the Integer.parseInt() method or the Integer.valueOf() method. Here's an example of both approaches:

Using Integer.parseInt():

```java
String str = "123";
int number = Integer.parseInt(str);
System.out.println("Converted int value: " + number);
```

In this example, the Integer.parseInt() method is used to convert the String "123" to an int value. The converted value is stored in the number variable, which can then be used in further computations or printed.

Using Integer.valueOf():

```java
String str = "123";
Integer number = Integer.valueOf(str);
System.out.println("Converted Integer value: " + number);
```

In this example, the Integer.valueOf() method is used to convert the String "123" to an Integer object. The Integer object is auto-boxed to an int value because of auto-unboxing in Java. The converted value is stored in the number variable, which can be used as an int or an Integer.

Both methods will throw a NumberFormatException if the String cannot be parsed as an int. Therefore, it's important to handle or catch this exception when converting a String to an int to ensure the program doesn't terminate abruptly in case of an invalid input.

----

## **How to swap two integers without using temp variable?**

To swap two integers without using a temporary variable in Java, you can utilize the bitwise XOR operation. Here's an example:

```java
public class IntegerSwapExample {
    public static void main(String[] args) {
        int a = 10;
        int b = 20;
        
        System.out.println("Before swapping:");
        System.out.println("a = " + a);
        System.out.println("b = " + b);
        
        swapIntegers(a, b);
        
        System.out.println("After swapping:");
        System.out.println("a = " + a);
        System.out.println("b = " + b);
    }
    
    public static void swapIntegers(int a, int b) {
        a = a ^ b;
        b = a ^ b;
        a = a ^ b;
    }
}
```

In this example, the swapIntegers() method takes two integers a and b as parameters. It performs the swap using the XOR operation. The XOR operation (^) on two integers flips the bits in the binary representation if they are different, effectively swapping the bits.

When you run this program, it will output the following result:

```java
Before swapping:
a = 10
b = 20
After swapping:
a = 20
b = 10
```

----

## **Java Interview questions from OOP and Design Patterns**

It contains Java Interview questions from SOLID design principles, OOP fundamentals e.g. class, object, interface, Inheritance, Polymorphism, Encapsulation, and Abstraction as well as more advanced concepts like Composition, Aggregation, and Association. It also contains questions from GOF design patterns.

----

## **What is the interface? Why you use it if you cannot write anything concrete on it?** 

The interface is used to define API. It tells about the contract your classes will follow. It also supports abstraction because a client can use interface method to leverage multiple implementations e.g. by using List interface you can take advantage of random access of ArrayList as well as flexible insertion and deletion of LinkedList. The interface doesn't allow you to write code to keep things abstract but from Java 8 you can declare static and default methods inside interface which are concrete.

----

## **The difference between abstract class and interface in Java?**

There are multiple differences between abstract class and interface in Java, but the most important one is Java's restriction on allowing a class to extend just one class but allows it to implement multiple interfaces. An abstract class is good to define default behavior for a family of class, but the interface is good to define Type which is later used to leverage Polymorphism. Please check the answer for a more thorough discussion of this question.

----

## **Which design pattern have you used in your production code? apart from Singleton?**

This is something you can answer from your experience. You can generally say about dependency injection, factory pattern, decorator pattern or observer pattern, whichever you have used. Though be prepared to answer follow-up question based upon the pattern you choose.

----

## **Can you explain Liskov Substitution principle?**

This is one of the toughest questions I have asked in Java interviews. Out of 50 candidates, I have almost asked only 5 have managed to answer it. I am not posting an answer to this question as I like you to do some research, practice and spend some time to understand this confusing principle well.

----

## **What is Law of Demeter violation? Why it matters?**

Believe it or not, Java is all about application programming and structuring code. If  you have good knowledge of common coding best practices, patterns and what not to do than only you can write quality code.  Law of Demeter suggests you "talk to friends and not stranger", hence used to reduce coupling between classes.

----

## **What is Adapter pattern? When to use it?**

Another frequently asked Java design pattern questions. It provides interface conversion. If your client is using some interface but you have something else, you can write an Adapter to bridge them together. This is good for Java software engineer having 2 to 3 years experience because the question is neither difficult nor tricky but requires knowledge of OOP design patterns.


----

## **What is "dependency injection" and "inversion of control"? Why would someone use it?**

"Dependency injection" and "inversion of control" are closely related concepts in software development.

Dependency Injection (DI) is a design pattern that allows objects to depend on interfaces or abstractions rather than concrete implementations. It is a technique where the dependencies of a class are provided from the outside, typically through constructor parameters or setter methods, instead of the class creating or managing its dependencies internally. The main idea behind DI is to decouple classes and promote loose coupling, making code more modular, reusable, and testable.

Inversion of Control (IoC) is a broader concept and refers to the overall architectural pattern where the control flow of a program is inverted or handed over to a framework or container. Instead of a class controlling the creation and management of its dependencies, IoC containers or frameworks take charge of creating and managing object instances. IoC containers handle the instantiation and wiring of objects, resolving dependencies, and managing the overall lifecycle of the objects.

The main benefits of using DI and IoC are:

Loose Coupling: DI promotes loose coupling between classes by removing direct dependencies on concrete implementations. This makes the code more flexible and maintainable.

Testability: With DI, it becomes easier to write unit tests for individual classes. Dependencies can be easily mocked or replaced with test doubles, allowing for isolated testing.

Reusability: By depending on abstractions, classes become more reusable as they can work with different implementations of the same interface.

Modular and Extensible Design: DI and IoC promote modular design by breaking down systems into smaller, independent components. New functionality can be easily added by creating new implementations of existing interfaces and configuring the container to use them.

Separation of Concerns: DI and IoC help in separating the concerns of object creation and object usage. This improves code organization and maintainability.

Overall, DI and IoC are used to achieve better software design, maintainability, testability, and flexibility in large-scale applications. They are commonly used in frameworks like Spring and Java EE to manage dependencies and provide a foundation for building scalable and maintainable applications.

----

## **What is an abstract class? How is it different from an interface? Why would you use it?**

One more classic question from Programming Job interviews, it is as old as chuck Norris. An abstract class is a class which can have state, code and implementation, but an interface is a contract which is totally abstract. Since I have answered it many times, I am only giving you the gist here but you should read the article linked to answer to learn this useful concept in much more detail.

----

## **Which one is better constructor injection or setter dependency injection?**

Each has their own advantage and disadvantage. Constructor injection guaranteed that class will be initialized with all its dependency, but setter injection provides flexibility to set an optional dependency. Setter injection is also more readable if you are using an XML file to describe dependency. Rule of thumb is to use constructor injection for mandatory dependency and use setter injection for optional dependency.


----

## **What is difference between dependency injection and factory design pattern?**

Though both patterns help to take out object creation part from application logic, use of dependency injection results in cleaner code than factory pattern. By using dependency injection, your classes are nothing but POJO which only knows about dependency but doesn't care how they are acquired. In the case of factory pattern, the class also needs to know about factory to acquire dependency. hence, DI results in more testable classes than factory pattern. Please see the answer for a more detailed discussion on this topic.

----

## **Difference between Adapter and Decorator pattern?**

Though the structure of Adapter and Decorator pattern is similar, the difference comes on the intent of each pattern. The adapter pattern is used to bridge the gap between two interfaces, but Decorator pattern is used to add new functionality into the class without the modifying existing code.

----

## **Difference between Adapter and Proxy Pattern?**

Similar to the previous question, the difference between Adapter and Proxy patterns is in their intent. Since both Adapter and Proxy pattern encapsulate the class which actually does the job, hence result in the same structure, but Adapter pattern is used for interface conversion while the Proxy pattern is used to add an extra level of indirection to support distribute, controlled or intelligent access.

----

## **What is Template method pattern?**

Template pattern provides an outline of an algorithm and lets you configure or customize its steps. For examples, you can view a sorting algorithm as a template to sort object. It defines steps for sorting but let you configure how to compare them using Comparable or something similar in another language. The method which outlines the algorithms is also known as template method.

----

## **When do you use Visitor design pattern?**

The visitor pattern is a solution of problem where you need to add operation on a class hierarchy but without touching them. This pattern uses double dispatch to add another level of indirection.

----

## **When do you use Composite design pattern?**

Composite design pattern arranges objects into tree structures to represent part-whole hierarchies. It allows clients treat individual objects and container of objects uniformly. Use Composite pattern when you want to represent part-whole hierarchies of objects.

----

## **The difference between Inheritance and Composition?**

Though both allows code reuse, Composition is more flexible than Inheritance because it allows you to switch to another implementation at run-time. Code written using Composition is also easier to test than code involving inheritance hierarchies.

----

## **Describe overloading and overriding in Java?**

Both overloading and overriding allow you to write two methods of different functionality but with the same name, but overloading is compile time activity while overriding is run-time activity. Though you can overload a method in the same class, but you can only override a method in child classes. Inheritance is necessary for overriding.

----

## **The difference between nested public static class and a top level class in Java?**

You can have more than one nested public static class inside one class, but you can only have one top-level public class in a Java source file and its name must be same as the name of Java source file.

----

## **Difference between Composition, Aggregation and Association in OOP?**

If two objects are related to each other, they are said to be associated with each other. Composition and Aggregation are two forms of association in object-oriented programming. The composition is stronger association than Aggregation. In Composition, one object is OWNER of another object while in Aggregation one object is just USER of another object. If an object A is composed of object B then B doesn't exist if A ceased to exists, but if object A is just an aggregation of object B then B can exists even if A ceased to exist.

----

## **Give me an example of design pattern which is based upon open closed principle?**

This is one of the practical questions I ask experienced Java programmer. I expect them to know about OOP design principles as well as patterns. Open closed design principle asserts that your code should be open for extension but closed for modification. Which means if you want to add new functionality, you can add it easily using the new code but without touching already tried and tested code.  There are several design patterns which are based upon open closed design principle e.g. Strategy pattern if you need a new strategy, just implement the interface and configure, no need to modify core logic. One working example is Collections.sort() method which is based on Strategy pattern and follows the open-closed principle, you don't modify sort() method to sort a new object, what you do is just implement Comparator in your own way.

----

## **Difference between Abstract factory and Prototype design pattern?**

This is the practice question for you, If you are feeling bored just reading and itching to write something, why not write the answer to this question. I would love to see an example the, which should answer where you should use the Abstract factory pattern and where is the Prototype pattern is more suitable.

----

## **When do you use Flyweight pattern?**

This is another popular question from the design pattern. Many Java developers with 4 to 6 years of experience know the definition but failed to give any concrete example. Since many of you might not have used this pattern, it's better to look examples from JDK. You are more likely have used them before and they are easy to remember as well. Now let's see the answer.
Flyweight pattern allows you to share object to support large numbers without actually creating too many objects. In order to use Flyweight pattern, you need to make your object Immutable so that they can be safely shared. String pool and pool of Integer and Long object in JDK are good examples of Flyweight pattern.

Miscellaneous Java Interview Questions
It contains XML Processing in Java Interview question, JDBC Interview question, Regular expressions Interview questions, Java Error and Exception Interview Questions, Serialization,

----

## **The difference between nested static class and top level class?**

One of the fundamental questions from Java basics. I ask this question only to junior Java developers of 1 to 2 years of experience as it's too easy for an experience Java programmers. The answer is simple, a public top level class must have the same name as the name of the source file, there is no such requirement for nested static class. A nested class is always inside a top level class and you need to use the name of the top-level class to refer nested static class e.g. HashMap.Entry is a nested static class, where HashMap is a top level class and Entry is nested static class.

----

## **Can you write a regular expression to check if String is a number?**

If you are taking Java interviews then you should ask at least one question on the regular expression. This clearly differentiates an average programmer with a good programmer. Since one of the traits of a good developer is to know tools, regex is the best tool for searching something in the log file, preparing reports etc. Anyway, answer to this question is, a numeric String can only contain digits i.e. 0 to 9 and + and - sign that too at start of the String, by using this information you can write following regular expression to check if given String is number or not

----

## **The difference between checked and unchecked Exception in Java?**

checked exception is checked by the compiler at compile time. It's mandatory for a method to either handle the checked exception or declare them in their throws clause. These are the ones which are a sub class of Exception but doesn't descend from RuntimeException. The unchecked exception is the descendant of RuntimeException and not checked by the compiler at compile time. This question is now becoming less popular and you would only find this with interviews with small companies, both investment banks and startups are moved on from this question.

----

## **The difference between throw and throws in Java?**

the throw is used to actually throw an instance of java.lang.Throwable class, which means you can throw both Error and Exception using throw keyword e.g.

throw new IllegalArgumentException("size must be multiple of 2")

On the other hand, throws is used as part of method declaration and signals which kind of exceptions are thrown by this method so that its caller can handle them. It's mandatory to declare any unhandled checked exception in throws clause in Java. Like the previous question, this is another frequently asked Java interview question from errors and exception topic but too easy to answer.

----

## **The difference between Serializable and Externalizable in Java?**

This is one of the frequently asked questions from Java Serialization. The interviewer has been asking this question since the day Serialization was introduced in Java, but yet only a few good candidate can answer this question with some confidence and practical knowledge. Serializable interface is used to make Java classes serializable so that they can be transferred over network or their state can be saved on disk, but it leverages default serialization built-in JVM, which is expensive, fragile and not secure. Externalizable allows you to fully control the Serialization process, specify a custom binary format and add more security measure.

----

## **The difference between DOM and SAX parser in Java?**

Another common Java question but from XML parsing topic. It's rather simple to answer and that's why many interviewers prefers to ask this question on the telephonic round. DOM parser loads the whole XML into memory to create a tree based DOM model which helps it quickly locate nodes and make a change in the structure of XML while SAX parser is an event based parser and doesn't load the whole XML into memory. Due to this reason DOM is faster than SAX but require more memory and not suitable to parse large XML files.

----

## **Tell me 3 features introduced on JDK 1.7?**

This is one of the good questions I ask to check whether the candidate is aware of recent development in Java technology space or not. Even though JDK 7 was not a big bang release like JDK 5 or JDK 8, it still has a lot of good feature to count on e.g. try-with-resource statements, which free you from closing streams and resources when you are done with that, Java automatically closes that. Fork-Join pool to implement something like the Map-reduce pattern in Java. Allowing String variable and literal into switch statements. Diamond operator for improved type inference, no need to declare generic type on the right-hand side of variable declaration anymore, results in more readable and succinct code. Another worth noting feature introduced was improved exception handling e.g. allowing you to catch multiple exceptions in the same catch block.

----

## **Tell me 5 features introduced in JDK 1.8?**

This is the follow-up question of the previous one. Java 8 is path breaking release in Java's history, here are the top 5 features from JDK 8 release
Lambda expression, which allows you pass an anonymous function as object.
Stream API, take advantage of multiple cores of modern CPU and allows you to write succinct code.
Date and Time API, finally you have a solid and easy to use date and time library right into JDK
Extension methods, now you can have static and default method into your interface
Repeated annotation, allows you apply the same annotation multiple times on a type

----

## **What is the difference between Maven and ANT in Java?**

Another great question to check the all round knowledge of Java developers. It's easy to answer questions from core Java but when you ask about setting things up, building Java artifacts, many Java software engineer struggles. 

Coming back to the answer of this question, Though both are build tools and used to create Java application build, Maven is much more than that. It provides a standard structure for Java project based upon the "convention over configuration" concept and automatically manages dependencies (JAR files on which your application is dependent) for Java applications. Please see the answer for more differences between the Maven and ANT tools.

That's all guys, lots of Java Interview questions? isn't it? I am sure if you can answer this list of Java questions you can easily crack any core Java or advanced Java interview. Though I have not included questions from Java EE or J2EE topics e.g. Servlet, JSP, JSF, JPA, JMS, EJB, or any other Java EE technology or from major web frameworks like Spring MVC, Struts 2.0, Hibernate, or both SOAP and RESTful web services, it's still useful for Java developers preparing for Java web developer position, because every Java interview starts with questions from fundamentals and JDK API. 

If you think, I have missed any popular Java question here and you think it should be in this list then feel free to suggest me. My goal is to create the best list of Java Interview Questions with the latest and greatest questions from recent interviews.

In case you don't know, I  have also written a book for Java interviews, Grokking the Java Interview, and Grokking the Spring Boot Interview, where I have shared tips, tricks and frequently asked Java questions from different topics. You can read the book to better prepare for your Java interviews. You can also use the code - friends20 to get a 20% discount because you are already my reader. 

----

## **Recommended Books for Java Programmers**

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

Read more: [https://javarevisited.blogspot.com/2015/10/133-java-interview-questions-answers-from-last-5-years.html#ixzz80dhIw3nT](https://javarevisited.blogspot.com/2015/10/133-java-interview-questions-answers-from-last-5-years.html#ixzz80dhIw3nT)

### https://javarevisited.blogspot.com/2015/10/133-java-interview-questions-answers-from-last-5-years.html#axzz80dfcO0nd

### https://javarevisited.blogspot.com/2014/07/top-50-java-multithreading-interview-questions-answers.html#axzz80dfcO0nd

## **What is Thread in Java?**

The thread is an independent path of execution. It's a way to take advantage of multiple CPUs available on a machine. By employing multiple threads you can speed up CPU-bound tasks. For example, if one thread takes 100 milliseconds to do a job, you can use 10 threads to reduce that task into 10 milliseconds. Java provides excellent support for multithreading at the language level, and it's also one of the strong selling points.

----

## **What is the difference between Thread and Process in Java?**

The thread is a subset of Process, in other words, one process can contain multiple threads. Two processes run on different memory spaces, but all threads share the same memory space. Don't confuse this with stack memory, which is different for the different threads and used to store local data to that thread. For more detail see the answer.

What is the difference between Thread and Process in Java?

----

## **How do you implement Thread in Java?**

At the language level, there are two ways to implement Thread in Java. An instance of java.lang.Thread represents a thread but it needs a task to execute, which is an instance of interface java.lang.Runnable. 

Since the Thread class itself implement Runnable, you can override the run() method either by extending the Thread class or just implementing the Runnable interface. For a detailed answer and discussion see this article.

----

## **When to use Runnable vs Thread in Java?**

This is a follow-up to a previous multi-threading interview question. As we know we can implement thread either by extending the Thread class or implementing Runnable interface, the question arises, which one is better and when to use one? This question will be easy to answer if you know that the Java programming language doesn't support multiple inheritances of class, but it allows you to implement multiple interfaces. 

This means it's better to implement Runnable than extend Thread if you also want to extend another class e.g. Canvas or CommandListener. For more points and discussion you can also refer to this post.

----

## **What is the difference between the start() and run() method of the Thread class?**

One of trick Java questions from early days, but still good enough to differentiate between shallow understanding of Java threading model start() method is used to start a newly created thread, while start() internally calls run() method, there is difference calling run() method directly. 

When you invoke run() as a normal method, it's called in the same thread, no new thread is started, which is the case when you call the start() method. Read this answer for a much more detailed discussion.

----

## **What is the difference between Runnable and Callable in Java?**

Both Runnable and Callable represent task which is intended to be executed in a separate thread. Runnable is there from JDK 1.0 while Callable was added on JDK 1.5. The main difference between these two is that Callable's call() method can return value and throw Exception, which was not possible with Runnable's run() method. Callable return Future object, which can hold the result of the computation. See my blog post on the same topic for a more in-depth answer to this question.

----

## **What is the difference between CyclicBarrier and CountDownLatch in Java?**

Though both CyclicBarrier and CountDownLatch wait for a number of threads on one or more events, the main difference between them is that you can not re-use CountDownLatch once the count reaches to zero, but you can reuse the same CyclicBarrier even after the barrier is broken.  See this answer for a few more points and a sample code example.

----

## **What is the Java Memory model?**

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

## **What is a volatile variable in Java?**

volatile is a special modifier, which can only be used with instance variables. In concurrent Java programs, changes made by multiple threads on instance variables are not visible to others in absence of any synchronizers like synchronized keywords or locks. 

Volatile variable guarantees that a write will happen before any subsequent read: as stated: "volatile variable rule" in the previous question. Read this answer to learn more about volatile variables and when to use them.

----

## **What is thread-safety? is Vector a thread-safe class?**

Thread safety is a property of an object or code which guarantees that if executed or used by multiple threads in any manner e.g. read vs writing it will behave as expected. For example, a thread-safe counter object will not miss any count if the same instance of that counter is shared among multiple threads.

Apparently, you can also divide collection classes into two categories, thread-safe and non-thread-safe. Vector is indeed a thread-safe class and it achieves thread-safety by synchronizing methods that modify the state of Vector, on the other hand, its counterpart ArrayList is not thread-safe.

----

## **What is a race condition in Java? Given one example?**

Race conditions are caused by some subtle programming bugs when Java programs are exposed to a concurrent execution environment. As the name suggests, a race condition occurs due to race between multiple threads, if a thread that is supposed to execute first lost the race and is executed second, the behavior of code changes, which surface as non-deterministic bugs. 

This is one of the hardest bugs to find and re-produce because of the random nature of racing between threads. One example of race conditions is out-of-order processing, see this answer for some more examples of race conditions in Java programs.

----

## **How to stop a thread in Java?**

I always said that Java provides rich APIs for everything but ironically Java doesn't provide a sure-shot way of stopping the thread. There were some control methods in JDK 1.0 e.g. stop(), suspend(), and resume() which were deprecated in later releases due to potential deadlock threats, then Java API designers have not made any effort to provide a consistent, thread-safe, and elegant way to stop threads. 

Programmers mainly rely on the fact that thread stops automatically as soon as they finish execution of run() or call() method. To manually stop, programmers either take advantage of volatile boolean variables and check in every iteration if the run method has loops or interrupt threads to abruptly cancel tasks. See this tutorial for a sample code of stopping thread in Java.

----

## **What happens when an Exception occurs in a thread?**

This is one of the good tricky Java questions I have seen in interviews. In simple words, If not caught thread will die, if an uncaught exception handler is registered then it will get a callback. Thread.UncaughtExceptionHandler is an interface, defined as a nested interface for handlers invoked when a Thread abruptly terminates due to an uncaught exception. 

When a thread is about to terminate due to an uncaught exception the Java Virtual Machine will query the thread for its UncaughtExceptionHandler using Thread.getUncaughtExceptionHandler() and will invoke the handler's uncaughtException() method, passing the thread and the exception as arguments.

----

## **How do you share data between two threads in Java?**

You can share data between threads by using shared objects, or concurrent data structures like BlockingQueue. See this tutorial to learn inter-thread communication in Java. It implements the Producer consumer pattern using wait and notify methods, which involves sharing objects between two threads.


Java concurrency questions for experienced programmers

----

## **What is the difference between notify and notifyAll in Java?**

This is another tricky question from core Java interviews since multiple threads can wait on a single monitor lock, Java API designer provides a method to inform only one of them or all of them, once the waiting condition changes, but they provide the half implementation. 

There notify() method doesn't provide any way to choose a particular thread, that's why it's only useful when you know that there is only one thread is waiting. 

On the other hand, notifyAll() sends a notification to all threads and allows them to compete for locks, which ensures that at least one thread will proceed further. See my blog post on a similar topic for a more detailed answer and code example.

----

## **Why wait, notify, and notifyAll are not inside the thread class?**

This is a design-related question, which checks what the candidate thinks about the existing system or does he ever thought of something which is so common but looks inappropriate at first. In order to answer this question, you have to give some reasons why it makes sense for these three methods to be in the Object class, and why not on Thread class. 

One reason which is obvious is that Java provides lock at the object level, not at the thread level. Every object has a lock, which is acquired by a thread. Now if the thread needs to wait for a certain lock it makes sense to call wait() on that object rather than on that thread.

Had wait() method declared on Thread class, it was not clear for which lock thread was waiting. In short, since wait, notify and notifyAll operate at lock level, it makes sense to define it on object class because the lock belongs to object. You can also see this article for a more elaborate answer to this question.

----

## **What is the ThreadLocal variable in Java?**

ThreadLocal variables are a special kind of variable available to Java programmers. Just like instance, the variable is per instance, ThreadLocal variable is per thread. It's a nice way to achieve thread-safety of expensive-to-create objects, for example, you can make SimpleDateFormat thread-safe using ThreadLocal. Since that class is expensive, it's not good to use it in local scope, which requires separate instances on each invocation. 

By providing each thread their own copy, you shoot two birds with one arrow. First, you reduce the number of instances of expensive objects by reusing a fixed number of instances, and Second, you achieve thread safety without paying the cost of synchronization or immutability. 

Another good example of a thread-local variable is ThreadLocalRandom class, which reduces the number of instances of expensive-to-create Random objects in a multi-threading environment. See this answer to learn more about thread-local variables in Java.

----

## **What is FutureTask in Java?**

FutureTask represents a cancellable asynchronous computation in concurrent Java applications. This class provides a base implementation of Future, with methods to start and cancel a computation, query to see if the computation is complete and retrieve the result of the computation. 

The result can only be retrieved when the computation has been completed; the get methods will block if the computation has not yet been completed. A FutureTask object can be used to wrap a Callable or Runnable object. Since FutureTask also implements Runnable, it can be submitted to an Executor for execution.

----

## **What is the difference between the interrupted() and isInterrupted() method in Java?**

The main difference between interrupted() and isInterrupted() is that the former clears the interrupt status while the latter does not. The interrupt mechanism in Java multi-threading is implemented using an internal flag known as the interrupt status. Interrupting a thread by calling Thread.interrupt() sets this flag. 

When interrupted thread checks for an interrupt by invoking the static method Thread.interrupted(), interrupt status is cleared. The non-static isInterrupted() method, which is used by one thread to query the interrupt status of another, does not change the interrupt status flag. 

By convention, any method that exits by throwing an InterruptedException clears interrupt status when it does so. However, it's always possible that interrupt status will immediately be set again, by another thread invoking interrupt

----

## **Why wait and notify methods are called from the synchronized block?**
The main reason for calling the wait and notify method from either synchronized block or method is that it is made mandatory by Java API. If you don't call them from a synchronized context, your code will throw IllegalMonitorStateException. A more subtle reason is to avoid the race condition between wait and notify calls. To learn more about this, check my similarly titled post here.

----

## **Why should you check the condition for waiting in a loop?**

It's possible for a waiting thread to receive false alerts and spurious wake-up calls, if it doesn't check the waiting condition in a loop, it will simply exit even if the condition is not met. As such, when awaiting thread wakes up, it cannot assume that the state it was waiting for is still valid. It may have been valid in the past, but the state may have been changed after the notify() method was called and before the waiting thread woke up. 

That's why it is always better to call the wait() method from a loop, you can even create a template for calling wait and notify in Eclipse. To learn more about this question, I would recommend you to read Effective Java items on thread and synchronization.

----

## **What is the difference between synchronized and concurrent collection in Java?**

Though both synchronized and concurrent collection provides thread-safe collection suitable for multi-threaded and concurrent access, later is more scalable than former. Before Java 1.5, Java programmers only had synchronized collection which becomes a source of contention if multiple threads access them concurrently, which hampers the scalability of the system. 

Java 5 introduced concurrent collections like ConcurrentHashMap, which not only provides thread safety but also improves scalability by using modern techniques like lock stripping and partitioning internal tables. See this answer for more differences between synchronized and concurrent collection in Java.

----

## **What is the difference between Stack and Heap in Java?**

Why does someone this question as part of multi-threading and concurrency? because Stack is a memory area that is closely associated with threads. To answer this question, both stack and heap are specific memories in Java applications. 

Each thread has its own stack, which is used to store local variables, method parameters, and call stack. Variable stored in one Thread's stack is not visible to other. On another hand, the heap is a common memory area that is shared by all threads. 

Objects whether local or at any level is created inside the heap. To improve performance thread tends to cache values from the heap into their stack, which can create problems if that variable is modified by more than one thread, this is where volatile variables come into the picture. volatile suggest threads read the value of variable always from main memory. See this article for learning more about stack and heap in Java to answer this question in greater detail.


Java thread interview questions with answers difficult ones

----

## **What is a thread pool? Why should you thread pool in Java?**

Creating a thread is expensive in terms of time and resources. If you create a thread at the time of request processing it will slow down your response time, also there is only a limited number of threads a process can create. To avoid both of these issues, a spool of threads is created when the application starts up and threads are reused for request processing.

This pool of thread is known as "thread pool" and threads are known as a worker thread. From JDK 1.5 release, Java API provides Executor framework, which allows you to create different types of thread pools e.g. single thread pool, which processes one task at a time, fixed thread pool (a pool of fixed number of threads), or cached thread pool (an expandable thread pool suitable for applications with many short-lived tasks). See this article to learn more about thread pools in Java to prepare a detailed answer to this question.

----

## **Write code to solve Producer Consumer problems in Java?**

Most of the threading problems you solved in the real world are of the category of Producer consumer pattern, where one thread is producing a task and another thread is consuming that. You must know how to do inter-thread communication to solve this problem. At the lowest level, you can use wait and notify to solve this problem, and at a high level, you can leverage Semaphore or BlockingQueue to implement a Producer consumer pattern, as shown in this tutorial.

----

## **How do you avoid deadlock in Java? Write Code?**

Deadlock is a condition in which two threads wait for each other to take action which allows them to move further. It's a serious issue because when it happens your program hangs and doesn't do the task it is intended for. 

In order for the deadlock to happen, the following four conditions must be true:
Mutual Exclusion: At least one resource must be held in a non-shareable mode. Only one process can use the resource at any given instant of time.
Hold and Wait: A process is currently holding, at least, one resource and requesting additional resources which are being held by other processes.
No Pre-emption: The operating system must not de-allocate resources once they have been allocated; they must be released by the holding process voluntarily.
Circular Wait: A process must be waiting for a resource that is being held by another process, which in turn is waiting for the first process to release the resource.

The easiest way to avoid deadlock is to prevent Circular wait, and this can be done by acquiring locks in a particular order and releasing them in reverse order so that a thread can only proceed to acquire a lock if it held the other one. Check this tutorial for the actual code example and detailed discussion on techniques for avoiding deadlock in Java.

deadlock in multithreading Java

----

## **What is the difference between livelock and deadlock in Java?**

This question is an extension of the previous interview question. A livelock is similar to a deadlock, except that the states of the threads or processes involved in the livelock constantly change with regard to one another, without anyone progressing further. 

Livelock is a special case of resource starvation. A real-world example of livelock occurs when two people meet in a narrow corridor, and each tries to be polite by moving aside to let the other pass, but they end up swaying from side to side without making any progress because they both repeatedly move the same way at the same time. In short, the main difference between livelock and deadlock is that in the former state of process change but no progress is made.

----

## **How do you check if a thread holds a lock or not?**

I didn't even know that you can check if a Thread already holds a lock before this question hits me in a telephonic round of Java interviews. There is a method called holdsLock() on java.lang.Thread, it returns true if and only if the current thread holds the monitor lock on the specified object. You can also check this article for a more detailed answer.

----

## **How do you take thread dump in Java?**

There are multiple ways to take a thread dump of the Java process depending upon the operating system. When you take thread dump, JVM dumps the state of all threads in log files or standard error console. In windows, you can use Ctrl + Break key combination to take thread dump, on Linux you can use the kill -3 command for the same. You can also use a tool called jstack for taking thread dump, it operates on process id, which can be found using another tool called jps.

----

## **Which JVM parameter is used to control the stack size of a thread?**

This is the simple one, -Xss parameter is used to control the stack size of Thread in Java. You can see this list of JVM options to learn more about this parameter.

----

## **What is the difference between synchronized and ReentrantLock in Java?**

There were days when the only way to provide mutual exclusion in Java was via synchronized keyword, but it has several shortcomings e.g. you can not extend lock beyond a method or block boundary, you can not give up trying for a lock, etc.

Java 5 solves this problem by providing more sophisticated control via the Lock interface. ReentrantLock is a common implementation of the Lock interface and provides re-entrant mutual exclusion Lock with the same basic behavior and semantics as the implicit monitor lock accessed using synchronized methods and statements, but with extended capabilities. See this article to learn about those capabilities and some more differences between synchronized vs ReentrantLock in Java.

----

## **There are three threads T1, T2, and T3? How do you ensure sequence T1, T2, T3 in Java?**

Sequencing in multi-threading can be achieved by different means but you can simply use the join() method of thread class to start a thread when another one has finished its execution. To ensure three threads execute you need to start the last one first e.g. T3 and then call join methods in reverse order e.g. T3 calls T2. join and T2 calls T1.join, these ways T1 will finish first and T3 will finish last. To learn more about the join method, see this tutorial.

----

## **What does the yield method of the Thread class do?**

The yield method is one way to request the current thread to relinquish CPU so that other threads can get a chance to execute. Yield is a static method and only guarantees that the current thread will relinquish the CPU but doesn't say anything about which other thread will get CPU. It's possible for the same thread to get the CPU back and start its execution again. See this article to learn more about the yield method and to answer this question better.

----

## **What is the concurrency level of ConcurrentHashMap in Java?**

ConcurrentHashMap achieves its scalability and thread-safety by partitioning the actual map into a number of sections. This partitioning is achieved using a concurrency level.

Its optional parameter of ConcurrentHashMap constructor and its default value is 16. The table is internally partitioned to try to permit the indicated number of concurrent updates without contention. To learn more about concurrency level and internal resizing, see my post How ConcurrentHashMap works in Java.

----

## **What is Semaphore in Java?**

Semaphore in Java is a new kind of synchronizer. It's a counting semaphore. Conceptually, a semaphore maintains a set of permits. Each acquire() blocks if necessary until a permit is available and then takes it. Each release() adds a permit, potentially releasing a blocking acquirer. 

However, no actual permit objects are used; the Semaphore just keeps a count of the number available and acts accordingly. Semaphore is used to protect an expensive resource that is available in fixed numbers e.g. database connection in the pool. See this article to learn more about counting Semaphore in Java.

----

## **What happens if you submit a task when the queue of the thread pool is already filled?**

This is another tricky question on my list. Many programmers will think that it will block until a task is cleared but it's true. ThreadPoolExecutor's submit() method throws RejectedExecutionException if the task cannot be scheduled for execution.

----

## **What is the difference between the submit() and execute() method thread pool in Java?**

Both methods are ways to submit a task to thread pools but there is a slight difference between them. execute(Runnable command) is defined in Executor interface and executes given task in future, but more importantly, it does not return anything. Its return type is void. 

On other hand submit() is an overloaded method, it can take either Runnable or Callable task and can return Future object which can hold the pending result of the computation. 

This method is defined on ExecutorService interface, which extends Executor interface, and every other thread pool class e.g. ThreadPoolExecutor or ScheduledThreadPoolExecutor gets these methods. To learn more about thread pools you can check this article.

----

## **What is the blocking method in Java?**

A blocking method is a method that blocks until the task is done, for example, accept() method of ServerSocket blocks until a client is connected. here blocking means control will not return to the caller until the task is finished. On the other hand, there is an asynchronous or non-blocking method that returns even before the task is finished. To learn more about the blocking method see this answer.

----

## **Is Swing thread-safe? What do you mean by Swing thread-safe?**

You can simply this question as No, Swing is not thread-safe, but you have to explain what you mean by that even if the interviewer doesn't ask about it. When we say swing is not thread-safe we usually refer to its component, which can not be modified in multiple threads. 

All updates to GUI components have to be done on the AWT thread, and Swing provides synchronous and asynchronous callback methods to schedule such updates. You can also read my article to learn more about swing and thread safety to better answer this question. Even next two questions are also related to this concept.

----

## **What is the difference between invokeAndWait and invokeLater in Java?**

These are two methods Swing API provides Java developers for updating GUI components from threads other than the Event dispatcher thread. InvokeAndWait() synchronously update GUI component, for example, a progress bar, once progress is made, the bar should also be updated to reflect that change. 

If progress is tracked in a different thread, it has to call invokeAndWait() to schedule an update of that component by the Event dispatcher thread. On another hand, invokeLater() is an asynchronous call to update components. You can also refer to this answer for more points.

----

## **Which method of Swing API is thread-safe in Java?**

This question is again related to swing and thread-safety though components are not thread-safe there is a certain method that can be safely called from multiple threads. I know about repaint(), and revalidate() being thread-safe but there are other methods on different swing components e.g. setText() method of JTextComponent, insert() and append() method of JTextArea class.

----

## **How to create an Immutable object in Java?**

This question might not look related to multi-threading and concurrency, but it is. Immutability helps to simplify already complex concurrent code in Java. Since immutable objects can be shared without any synchronization it's very dear to Java developers. Core value object, which is meant to be shared among threads should be immutable for performance and simplicity. 

Unfortunately, there is no @Immutable annotation in Java, which can make your object immutable, hard work must be done by Java developers. You need to keep basics like initializing state in the constructor, no setter methods, no leaking of reference, keeping a separate copy of the mutable object to create an Immutable object. For step by step guide see my post, how to make an object Immutable in Java. This will give you enough material to answer this question with confidence.

----

## **What is ReadWriteLock in Java?**

In general, the read-write lock is the result of the lock stripping technique to improve the performance of concurrent applications. In Java, ReadWriteLock is an interface that was added in Java 5 release. 

A ReadWriteLock maintains a pair of associated locks, one for read-only operations and one for writing. The read lock may be held simultaneously by multiple reader threads, so long as there are no writers. 

The write lock is exclusive. If you want you can implement this interface with your own set of rules, otherwise you can use ReentrantReadWriteLock, which comes along with JDK and supports a maximum of 65535 recursive write locks and 65535 read locks.

----

## **What is a busy spin in multi-threading?**

Busy spin is a technique that concurrent programmers employ to make a thread wait on certain conditions. Unlike traditional methods e.g. wait(), sleep(), or yield() which all involve relinquishing CPU control, this method does not relinquish CPU, instead, it just runs the empty loop. Why would someone do that? to preserve CPU caches. 

In a multi-core system, it's possible for a paused thread to resume on a different core, which means rebuilding the cache again. To avoid the cost of rebuilding cache, programmers prefer to wait for a much smaller time doing busy spin. You can also see this answer to learn more about this question.

----

## **What is the difference between the volatile and atomic variables in Java?**

This is an interesting question for Java programmers, at first, volatile and atomic variables look very similar, but they are different. A volatile variable provides you happens-before guarantee that a write will happen before any subsequent write, it doesn't guarantee atomicity. 

For example, the count++ operation will not become atomic just by declaring the count variable as volatile.  On the other hand, AtomicInteger class provides an atomic method to perform such compound operation atomically e.g. getAndIncrement() is the atomic replacement of increment operator. It can be used to atomically increment the current value by one. 

Similarly, you have an atomic version for other data types and reference variables as well.

----

## **What happens if a thread throws an Exception inside a synchronized block?**

This is one more tricky question for the average Java programmer if he can bring the fact about whether the lock is released or not is a key indicator of his understanding. 

To answer this question, no matter how you exist synchronized block, either normally by finishing execution or abruptly by throwing an exception, the thread releases the lock it acquired while entering that synchronized block. 

This is actually one of the reasons I like synchronized block over lock interface, which requires explicit attention to release lock, generally, this is achieved by releasing the lock in a finally block.

----

## **What is double-checked locking of Singleton?**

This is one of the very popular questions on Java interviews, and despite its popularity, the chances of candidates answering this question satisfactory is only 50%. Half of the time, they failed to write code for double-checked locking, and half of the time they failed how it was broken and fixed on Java 1.5.

This is actually an old way of creating a thread-safe singleton, which tries to optimize performance by only locking when the Singleton instance is created the first time, but because of complexity and the fact it was broken for JDK 1.4,  I personally don't like it. 

Anyway, even if you do not prefer this approach it's good to know from an interview point of view. Since this question deserves a detailed answer, I have answered in a separate post, you can read my post how double-checked locking on Singleton works to learn more about it.

----

## **How to create thread-safe Singleton in Java?**

This question is actually a follow-up to the previous question. If you say you don't like double-checked locking then the Interviewer is bound to ask about alternative ways of creating a thread-safe Singleton class. 

There is actually man, you can take advantage of class loading and static variable initialization feature of JVM to create an instance of Singleton, or you can leverage powerful enumeration type in Java to create Singleton. I actually preferred that way, you can also read this article to learn more about it and see some sample code.

----

## **List down 3 multi-threading best practices you follow?**

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

## **How do you force to start a thread in Java?**

This question is like how do you force garbage collection in Java, there is no way though you can make a request using System.gc() but it's not guaranteed. On Java multi-threading there is absolutely no way to force start a thread, this is controlled by thread scheduler and Java exposes no API to control thread scheduling. This is still a random bit in Java.

----

## **What is the fork-join framework in Java?**

The fork-join framework, introduced in JDK 7 is a powerful tool available to Java developers to take advantage of multiple processors of modern-day servers. It is designed for work that can be broken into smaller pieces recursively. 

The goal is to use all the available processing power to enhance the performance of your application. One significant advantage of The fork/join framework is that it uses a work-stealing algorithm. Worker threads that run out of things to do can steal tasks from other threads that are still busy. See this article for a much more detailed answer to this question.

----

## **What is the difference between the calling wait() and sleep() method in Java multi-threading?**

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

### https://javarevisited.blogspot.com/2014/07/top-50-java-multithreading-interview-questions-answers.html#axzz80dfcO0nd

### https://javarevisited.blogspot.com/2015/02/50-programmer-phone-interview-questions-answers.html#axzz80dfcO0nd

## **How much time does it take to retrieve an element if stored in HashMap, Binary tree, and a Linked list? how it change if you have millions of records?**

In HashMap it takes O(1) time, in the binary tree it takes O(logN) where N is a number of nodes in the tree and in linked list it takes O(n) time where n is a number of element in the list. Millions of records don't affect the performance if the data structure is working as expected e.g. HashMap has no or relatively less number of collision or binary tree is balanced. If that's not the case then their performance degrades as a number of records grows.

----

## **What is the difference between Overriding and Overloading?**

Overriding is resolved at runtime while overloading is compile time. Also, rules of overriding and overloading are different, for example in Java, method signature of the overloaded method must be different than original method, but in the case of overriding it must be exactly same as an overriding method.

----

## **What is the difference between forking a process and spawning a thread?**

When you fork a process, the new process will run the same code as the parent process but in different memory space, but when you spawn a new thread in existing process, it just creates another independent path of execution but share same memory space.

----

## **What is a critical section?**

A critical section is the part of a code, which is very important and in multi-threading must be exclusively modified by any thread. Semaphore or mutex is used to protect critical section. In Java, you can use synchronized keyword or ReentrantLock to protect a critical section.

----

## **What is the difference between a value type and a reference type?**

A value type is a more optimized type and always immutable e.g. primitive int, long, double and float in Java while a reference type points to an object, which can be mutable or Immutable. You can also say that value type points to a value while reference type points to an object.

----

## **What is heap and stack in a process?**

They are two separate areas of memory in the same process. Talking about Java, the stack is used to store primitive values and reference type to object but actual object is always created in heap. One critical difference between heap and stack is that heap memory is shared by all threads but each thread has their own stack.

----

## **What is revision/version control?**

Version control is software which is used to store code and manage versions of codebase e.g. SVN, CVS, Git, Perforce, and ClearCase. They are very effective while comparing code, reviewing code and creating a build from previous stable version. All professional development use some sort of revision or version control tool, without them, you cannot manage code effectively, especially if 20 developers are working on same code base at the same time. Version control tool plays very important role to keep code base consistent and resolving code conflicts.

----

## **What is a strongly typed programming language?**

In a strongly typed language compiler ensure type correctness, for example, you can not store the number in String or vice-versa. Java is a strongly typed language, that's why you have different data types e.g. int, float, String, char, boolean etc. You can only store compatible values in respective types. 

On the other hand, weakly typed language don't enforce type checking at compile time and they tree values based upon context. Python and Perl are two popular example of weakly typed programming language, where you can store a numeric string in number type.

----

## **Can you describe the difference between valid and well-formed XML?**

A well-formed XML is the one which has root element and all tags are closed properly, attributes are defined properly, their value is also quoted properly. On another hand, a valid XML is the one which can be validated against an XSD file or schema. So it's possible for an XML to be well-formed but not valid because they contain tags which may not be allowed by their schema.

----

## **What is the difference between DOM and SAX parser?**

DOM parser is an in-memory parser so it loads whole XML file in memory and create a DOM tree to parse. SAX parser is an event based parser, so it parses XML document based on the event received e.g. opening tag, closing tag, the start of attribute or end of the attribute. 

Because of their working methodology, DOM parser is not suitable for large XML file as they will take a lot of space in memory and your process may run out of memory, SAX is the one which should be used to parse large files. For small files, DOM is usually much faster than SAX.

----

## **What is the relationship between threads and processes?**

A process can have multiple threads but a thread always belongs to a single process. Two processes cannot share memory space until they are purposefully doing inter-process communication via shared memory but two threads from the same process always share the same memory.

----

## **What is Immutable class mean?**

A class is said to be Immutable if its state cannot be changed once created, for example, String in Java is immutable. Once you create a String say "Java", you cannot change its content. Any modification in this string e.g. converting into upper case,  concatenating with another String will result in the new object. 

An immutable object is very useful for concurrent programming because they can be shared between multiple threads without worrying about synchronization. In fact, the whole model of functional programming is built on top of Immutable objects.

----

## **Why would you ever want to create a mock object?**
A mock object is very useful to test an individual unit in your Software, in fact, stub and mocks a are a powerful tool for creating automated unit tests. Suppose you write a program to display currency conversion rates but you don't have a URL to connect to, now if you want to test your code, you can use mock objects. In Java world, there are a lot of frameworks which can create powerful mock objects for you e.g. Mockito and PowerMock.

----

## **What is SQL injection?**

SQL injection is a security vulnerability which allows an intruder to steal data from the system. Any system which takes input from the user and creates SQL query without validating or sanitizing that input is vulnerable to SQL injection. In such system, an intruder can inject SQL code instead of data to retrieve more than expected data. 

There are many instances on which sensitive information e.g. user id, password, and personal details are stolen by exploiting this vulnerability. In Java, you can avoid SQL injection by using Prepared statement.

----

## **What is the difference between an inner join and a left join in SQL?**

In SQL, there are mainly two types of joins, inner join, and outer join. Again outer joins can be two types right and left outer join. 

The main difference between inner join and left join is that in the case of former only matching records from both tables are selected while in the case of left join, all records from left table are selected in addition to matching records from both tables. 

Always watch out for queries which have "all" in it, they usually require left join like to write SQL query to find all departments and a number of employees on it. If you use inner join to solve this query, you will miss empty departments where no one works.

What is the difference between an inner join and a left join in SQL

----

## **What does the V in MVC stand for, and what does it signify?**

V stands for View in MVC pattern. The view is what user sees  like web pages. This is a very important design pattern of web development which is based upon segregation of concern so that each area can be modified without impacting other areas. 

In Java world, there are lots of open source framework which provides an implementation of MVC pattern like Struts 2 and Spring MVC. 

By the way, M stands the for model and C stands the for controller. Modes are actual business objects like User, Employee, Order; while the controller is used for the routing request to correct processor.

----

## **What is the difference between a class and an object?**

A class is a blueprint on which objects are created. A class has code and behavior but an object has both the state and behavior. You cannot create an object without creating a class to represent its structure. The class is also used to map an object in memory, in Java, JVM does that for you.

----

## **What is loose-coupling?**

Loose coupling is a desirable quality of software, which allows one part of the software to modify without affecting another part of the software. For example, in a loosely coupled software, a change in UI layout should not affect the back-end class structure.

----

## **What is the difference between composition, aggregation, and association?**

Association means two objects are related to each other but can exist without each other, Composition is a form of association where one object is composed of multiple objects, but they only exists together e.g. human body is the composition of organs, individual organs cannot live they only useful in the body. Aggregation is a collection of object e.g. city is an aggregation of citizens.

What is the difference between composition, aggregation, and association?

----

## **What is the difference between an interface and an abstract class?**

This is the most classical question of all programming interviews. An interface is the purest form of abstraction with nothing concrete in place while an abstract class is a combination of some abstraction and concrete things. The difference may vary depending upon language e.g. in Java you can extend multiple interface but you can only extend on the abstract class. For a more comprehensive discussion see the detailed answer.

----

## **What is unit testing?**

Unit testing is a way to test individual unit for their functionality instead of testing whole application. There are a lot of tools to do the unit testing in different programming language e.g. in Java, you can use JUnit or TestNG to write unit tests. It is often run automatically during the build process or in a continuous environment like Jenkins.

----

## **Can you describe three different kinds of testing that might be performed on an application before it goes live?**

unit testing, integration testing and smoke testing. Unit testing is used to test individual units to verify whether they are working as expected, integration testing is done to verify whether individually tested module can work together or not and smoke testing is a way to test whether most common functionality of software is working properly or not like in a flight booking website, you should be able to book, cancel or change flights.

----

## **What is the difference between iteration and recursion?**

Iteration uses a loop to perform the same step again and again while recursion calls the function itself to do the repetitive task. Many times recursion result in a clear and concise solution to a complex problem like tower of Hanoi, reversing a linked list or reversing a String itself. 

One drawback of recursion is depth  since recursion stores intermediate result in the stack you can only go up to a certain depth, after that your program will die with StackOverFlowError, this is why iteration is preferred over recursion in production code.

----

## **What is difference between & and && operator?**

& is a bitwise operator while && is a logical operator. One difference between & and && is that bitwise operator (&) can be applied to both integer and boolean but logical operator (&&) can only be applied to boolean variables. 

When you do a & b then AND operator is applied to each bit of both integer number, while in the case of a && b, the second argument may or may not be evaluated, that's why it is also known as short circuit operator, at least in Java. I like this question and often asked it to junior or developer and college graduates.

----

## **What is the result of 1 XOR 1?**

The answer is zero because XOR returns 1 if two operands are distinct and zero if two operands are same, for example, 0 XOR 0 is also zero, but 0 XOR 1 or 1 XOR 0 is always 1.

----

## **How do you get the last digit of an integer?**

By using modulus operator, number % 10 returns the last digit of the number, for example, 2345%10 will return 5 and 567%10 will return 7.  Similarly, division operator can be used to get rid of the last digit of  a number e.g. 2345/10 will give 234 and 567/10 will return 56. This is an important technique to know and useful to solve problems like number palindrome or reversing numbers.

----

## **What is test-driven development?**

Test driven is one of the popular development methodologies in which tests are written before writing any function code. In fact, test drives the structure of your program. Purists never wrote a single line of application code without writing a test for that. It greatly improve code quality and often attributed as a quality of Rockstar developers.

What is test-driven development?

----

## **What is the Liskov substitution principle?**

Liskov substitution principle is one of the five principle introduced by Uncle Bob as SOLID design principles. It's the 'L' in SOLID. Liskov substitution principle asserts that every subtype should be able to work as the proxy for parent type. 

For example, if a method except object of Parent class then it should work as expected if you pass an object of the Child class. 

Any class which cannot stand in place of its parent violate LSP or Liskov substitution principle. This is actually a tough question to answer and if you do that you end up with creating a good impression on the interviewer's mind.


----

## **What is the Open closed design principle?**

Open closed is another principle from SOLID, which asserts that a system should be open for extension but closed for modification. This means if new functionality is required in a stable system then your tried and tested code should not be touched and new functionality should be provided by adding new classes only. 


----

## **What is the difference between a binary tree and a binary search tree?**

Binary search tree is an ordered binary tree, where the value of all nodes in the left tree are less than or equal to node and values of all nodes in right subtree is greater than or equal to the node (e.g. root). It's an important data structure and can be used to represent a sorted structure.

----

## **Can you give a practical example of a recursive algorithm?**

There are lots of places where recursive algorithm fits e.g. algorithm related to binary and linked list. A couple of examples of a recursive algorithm is reversing String and calculating Fibonacci series. Other examples include reversing linked list, tree traversal, and quick sort algorithm. 

----

## **What is the time complexity of an algorithm?**

Time complexity specifies the ratio of time to the input. It shows how much time an algorithm will take to complete for a given number of input. It's approximated valued but enough to give you an indication that how your algorithm will perform if the number of input is increased from 10 to 10 million?

What is the time complexity of an algorithm?

----

## **What are some important differences between a linked list and an array?**

linked list and array are two of the most important data structure in the programming world. The most significant difference between them is that array stores its element at the contiguous location while linked list stores its data anywhere in memory. 

This gives linked list enormous flexibility to expand itself because memory is always scattered. 

It's always possible that you wouldn't be able to create an array to store 1M integers but can do by using linked list because space is available but not as contiguous chunk. All other differences are the result of this fact.

For example, you can search an element in array with O(1) time if you know the index but searching will take O(n) time in linked list. For more differences see the detailed answer.

----

## **What is a couple of ways to resolve collision in the hash table?**

linear probing, double hashing, and chaining. In linear probing, if the bucket is already occupied then function check next bucket linearly until it finds an empty one, while in chaining, multiple elements are stored in same bucket location.

----

## **What is a regular expression?**

A regular expression is a way to perform pattern matching on text data. It's very powerful tool to find something like some character in a long string e.g. finding if a book contains some word or not. Almost all major programming language supports regular expression but Perl has been renowned for its enormous capability. 

Java also supports Perl-like regular expression using java.util.regex package. 

You can use the regular expression to check if an email is valid or not, if a phone number is valid, or if a zip code is valid, or even an SSN number is valid or not. One of the simplest examples of the regular expression is to check if a String is a number or not.

----

## **What is a stateless system?**

A stateless system is a system which doesn't maintain any internal state. Such system will produce the same output for same input at any point of time. It's always easier to code and optimize a stateless system, so you should always strive for one if possible.

Programming Phone  Interview Questions answers


----

## **Write SQL query to find second highest salary in employee table?**
This is one of the classic questions from SQL interviews, the event it's quite old it is still interesting and has lots of follow-ups you can use to check the depth of candidate's knowledge. You can find second highest salary by using the correlated and non-correlated subquery. 

You can also use keyword's like TOP or LIMIT if you are using SQL Server or MySQL, given Interviewer allows you. The simplest way to find 2nd highest salary is following:

SELECT MAX(Salary) FROM Employee 
WHERE Salary NOT IN (SELECT MAX(Salary) FROM Employee)

This query first finds maximum salary and then exclude that from the list and again finds maximum salary. Obviously second time, it would be second highest salary.


----

## **Can you describe the difference between correlated and non-correlated subquery?**

In correlated sub-query, the inner query depends upon the outer query and executes for each row in the outer query. While non-correlated subquery doesn't depend upon the outer query and can be executed independently. 

Due to this reason, former is slow and later is fast. BTW, correlated subquery has some nice applications, one of them is finding Nth highest salary in Employee table, as seen on previous SQL question as well.


----

## **How do you find if a number is a power of two, without using an arithmetic operator?**

Assume it's a question of using the bitwise operator as soon as you hear restriction about not allowed to use arithmetic operator. If that restriction is not in place then you can easily check if a number is a power of two by using modulus and division operator. By the using bitwise operator, there is a nice trick to do this.  You can use following code to check if a number if power of two or not

```java
public static boolean powerOfTwo(int x) {
        return (x & (x - 1)) == 0;
}

// x & (x-1) is a nice trick to convert right most bit to zero if it's on, I learned from hackers delight book.
```

----

## **How do you find a  running Java process on UNIX?**

You can use the combination of 'ps' and 'grep' command to find any process running on UNIX machine. Suppose your Java process has a name or any text which you can use to match against just use following command.

ps -ef | grep "myJavaApp"

ps -e will list every process i.e. process from all user not just you and  ps -f will give you full details including PID, which will be required if you want to investigate more or would like to kill this process using kill command.

----

## **How do you find large files in UNIX  like more than 1GB?**

You can easily find big files by using the find command because it provides an option to search files based upon their size. Use this if your file system is full and your Java process is crashing with no more space. This command will list all files which are more than 1GB. You can tweak the size easily like to find all files with more than 100 MB just use +100M.

find . - type f -size +1G -print

----

## **What is the shell script?**

A shell script is a set of shell commands with some programming constructs e.g. if and for loop, which allows you to automate some repetitive task. For example, you can write a shell
script to the daily cleanup of logs files,  for backing up data for historical use and for other housekeeping jobs, releases, and monitoring.

Read more: https://javarevisited.blogspot.com/2015/02/50-programmer-phone-interview-questions-answers.html#ixzz80dhW7mB9

### https://javarevisited.blogspot.com/2015/02/50-programmer-phone-interview-questions-answers.html#axzz80dfcO0nd>
