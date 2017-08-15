# Java Presentation

A brief presentaton on Java detailing a definition, origin statement,
description, advantages, and disadvantages of the program. Instructions for
downloading the latest version of the Java Development Kit, and a brief
demonstrative code-along will also be provided.

## Prerequisites

- Basic knowledge of programming languages such as javascript, C++, etc.

## Objectives

By the end of this, developers should be able to:

- Provide a basic defintion of Java along with details about the language.
- List 2 Pros and 2 Cons of Java.
- Explain what a JVM is and why it is important.
- Create a Java file in Atom.
- Compile a Java file through the terminal.
- Successfully run Java contained in a file through the terminal.
- Find ways to make me look amazing during this presentation.

## Preparation

1. Fork and clone this repository. [FAQ](https://github.com/ga-wdi-boston/meta/wiki/ForkAndClone)
2. Create a new branch, `demo`, for your work.
3. Checkout to the `demo` branch.

## Installation

1. Navigate to the [Java SE development kit download site](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) and follow the instructions provided to install JDK on your computer

## What is Java

- Class-based, object-oriented Programming language (OOP).
- Derived for C and C++ shares similar syntax.
- Created for the purpose of network programming and and the distributed
  environment of the internet.
- Widely used, very popular.
- Predominant language used in Android mobile platform (NO.1 in the world).

## Pros and Cons of Java

### Pros

1. `Portability`
* Java excels in portability, meaning it can run on multiple operating systems
  with little to no porting work necessary.
* Source code is compiled into bytecode (computer object code, or code that has
  been compiled for use by a processor).
* Bytecode is processed by the Java Virtual Machine program and converted into
  instruction that the computer processor using it will understand.
* The JVM takes the place of the operating system meaning source code needs to
  only be compiled once and can run on any platform.
2. `Robust code`
* Java objects do not reference external data or other known objects.
* This protects data storage in other apps or OS preventing them from crashing
  or terminating.
* JVM also performs checks on each object to ensure integrity.
3. `Scalability`
* Java and the JVM is scalable while maintaining performance and reliability.
* JVM now has dynamic code analysis meaning code is analyzed while it running.
* Twitter moved from Ruby-on-Rails to the JVM for scalability.

### Cons

1. `Security`
* Java plugins in browsers created vulnerabilities that hackers exploited in
  2013 with attacks spanning from Microsoft, to Apple, to Facebook
1. `Competition`
* Languages like Javascript, Python and PHP rival Java
3. `Verbose code`
  * A major drawback of Java is how verbose the code is. Other languages can often
    times achieve the same goal with half the code.

## Basic Syntax

* Classes are UpperCamelCase, while methods and instances are lowerCamelCase
* Variables are declared by writing its type and name
* semicolons are still a thing
* ex)
 ```java
 int num = 10;
 ```
* Java applications must have entry point defined by declaring a method called main
* This allows the application to be run
* The syntax for declaring main method is
  ```java
  public static void main(String[] args)
  ```
* The standard edition of Java 8 that was recently released, now allows for
* the use of lambda expressions also known anonymous functions or funtion literals.
* Public is kinda like scope declaration and means that the method can be used by
  any other class or object (essentially giving it global scope).
* [This](img/modifier_example.png) is a picture showing the different modifies
  and relative access that other objects under the specified motifier.
* Public classes must be declared within a file with the same name.
* `Static` means that you can run this method without creating an instance of the class
* `Void` means the method doesn’t return a value.
* `Main` is the name of the method.
* `System` is a pre-defined class provided by Java with methods and variables attached to it.
* `Out` is a static variable within `System` that is the equivilent to (stdout) is javascript.
* `Println` is a method of `out` that is used to print a line similar to console.log or print.

## Code along

1. While in the repo from the terminal, run `javac -version`.
You should see something that looks like [this](https://www.dropbox.com/s/yj5d180qguhc4rt/Screenshot%202017-08-14%2023.54.54.png?dl=0)
2. Next create a new file `(touch)` and calle it `MyFirstJavaCode.java`
3. Now we are gonna write some code in the file. Begin by defining a class.
   ```java
   public class HelloWorld {

   }
   ```
4. Next lets use the main method to print "Hello World" on the terminal.
   ```java
   public static void main(String[] args)
 {

    System.out.println("Hello World.");

 }

 }
 ```
 5. Now from the command line, type `javac <fileName>.java` this will compile
    the file so that we can run it.  You should see a .class file created in atom.
 6. Now lets run the file `java <fileName>.java`
 7. Uh-Oh problemas... No me gusta! What happened?!?!
 8. Luckily we have a nice error handler that tells us exactly what went wrong.
 9. Lets correct the mistake and run the file again.
 10. Success!!! Congradulations you have taken your first step into Java.

## Resources used for this presentation

http://whatis.techtarget.com/definition/bytecode
http://www.theserverside.com/definition/Java
https://en.wikipedia.org/wiki/Java_(programming_language)
http://searchstorage.techtarget.com/definition/portability
http://whatis.techtarget.com/definition/object-code
http://www.infoworld.com/article/2687995/java/4-reasons-to-stick-with-java.html
https://www.quora.com/What-does-the-main-method-do-in-Java
https://en.wikipedia.org/wiki/Java_syntax#Identifier
http://docs.oracle.com/javase/tutorial/java/javaOO/accesscontrol.html
http://www.learnjavaonline.org/en/Hello%2C_World%21
