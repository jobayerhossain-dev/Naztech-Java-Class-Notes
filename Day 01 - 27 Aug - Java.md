# Day 01 - 27 Aug - Basic start

## Course Overview

Course overview was given in this lecture, is available in [README.md](./README.md#course-overview).

## Resources

Some learning resources are suggested in this lecture, is available in [README.md](./README.md#resources)

## What is Java?

Java is a popular object-oriented programming language, created in 1995. Now, it is owned by Oracle, originally developed by Sun Microsystems. More than 3 billion devices run with Java. It allows developers to write code that can run on various platforms. It is a popular choice for building applications ranging from web and mobile to enterprise software.

### Java is Used For

- Mobile Applications (specially Android apps)
- Desktop Applications
- Web Applications
- Web Servers and Application Servers
- Games
- Database connection and much more.

### Features of Java

1. Platform independence (Write Once, Run Anywhere)
2. Object-oriented programming
3. Strongly typed language
4. Automatic memory management (Garbage Collection)
5. Rich standard library
6. Multithreading and concurrency support
7. Exception handling
8. Security features (sandboxing)
9. Dynamic class loading
10. Robustness and error-checking at compile and runtime.
11. Information processed like bytecode.
12. Contain its all previous version.

### Why Use Java?

- Works on different platforms
- Most popular
- Large demand in the current job market
- Easy to learn and simple to use
- Open source and free
- Secured, fast and powerful
- Huge community support
- It is an OOP language which gives a clear structure to program and allows code to be reused, lowering development costs.
- Close to C++ and C# and makes easy to switch from other programming languages.

### Basic Structure of a Java Program

```java
class <Class Name> {
    public static void main(String[] args) {
        /* Write your code here */
    }
}
```

### Example

Code for printing `Hello, naztech` using Java in default package:

```java
class MainProgram {
    public static void main(String[] args) {
        System.out.println("Hello, naztech");
    }
}
```

> _Note: Write any class, package, variable or defining any others identifiers, always should be followed by naming all convention of that programming language. According to convention of java, class name should be title case, package should be lower case and and variable should be camel case._

### Hiererchical View of JVM, JRE, JDK

![Hiererchical View of JVM, JRE, JDK](./images/day01/diagram.jpg "Hiererchical View of JVM, JRE, JDK")

**JVM (Java Virtual Machine):** JVM is the runtime engine that executes Java bytecode, ensuring platform independence. It interprets or compiles bytecode into native machine code for execution, handling memory and threads.

**JRE (Java Runtime Environment):** JRE includes the JVM, libraries, and other runtime components required to run Java applications. It's sufficient for running Java programs but doesn't include development tools.

**JDK (Java Development Kit):** JDK is a comprehensive package containing the JRE, development tools, and libraries necessary for creating Java applications. It includes a compiler, debugger, and other utilities for coding, testing, and deploying Java programs. JDK is essential for both development and running Java applications.

### Syntax and Semantics

Syntax = Structure and format of code.
Semantics = Meaning and behavior of code.

### Identifiers

All java classes, variables must be identified with unique names. These unique names are called identifiers. It is recommended to use "descriptive names" for creating "understandable and maintainable" code.

### Reserved words or keywords in Java

There are about 54 reserved words in Java. [Click here](https://www.w3schools.com/java/java_ref_keywords.asp) for details.

### Key Features of Java

Key features of the Java programming language:

1. **Platform Independence:** Java is designed to be platform-independent, meaning that a Java program can run on any operating system with a compatible Java Virtual Machine (JVM).
2. **Object-Oriented:** Java follows the object-oriented programming (OOP) paradigm, allowing developers to model real-world entities as objects and create reusable and modular code.
3. **Simple and Easy to Learn:** Java has a clean and straightforward syntax, making it relatively easy for beginners to grasp the language's concepts.
4. **Automatic Memory Management:** Java manages memory automatically through its built-in garbage collection system, reducing the chances of memory leaks and providing memory efficiency.
5. **Strongly Typed:** Java enforces strong type-checking during both "compile-time and runtime", enhancing program reliability and reducing errors.
6. **Platform-Independent Libraries:** Java comes with a vast standard library that provides pre-built classes and methods for various tasks, saving developers time and effort.
7. **Multithreading:** Java supports multithreading, enabling the creation of programs that can execute multiple tasks concurrently, improving efficiency and responsiveness.
8. **Exception Handling:** Java has a robust exception handling mechanism that helps manage and recover from runtime errors, ensuring stable and predictable program behavior.
9. **Security:** Java has built-in security features, including a security manager and sandbox environment, making it suitable for developing secure applications, especially in web and network environments.
10. **Rich API:** Java offers a wide range of APIs (Application Programming Interfaces) for tasks such as I/O, networking, databases, GUI development, and more.
11. **Distributed Computing:** Java supports network programming and communication through its rich libraries, making it ideal for building distributed and networked applications.
12. **Dynamic Loading:** Java allows classes to be loaded dynamically, which facilitates more flexible and adaptable program structures.
13. **Open Source Community:** Java has a vibrant open-source community that contributes to the development of various libraries, frameworks, and tools.
14. **Portability:** Java's "Write Once, Run Anywhere" philosophy ensures that code written in Java can be compiled once and executed on multiple platforms without modification.
15. **Continuous Evolution:** Java continues to evolve with regular updates and new features, ensuring that it remains relevant and competitive in the modern programming landscape.

## 🛠️Practical

### How to Install Spring Tools

- Go to >> [https://spring.io/tools](https://spring.io/tools).
- Go to >> ```Spring Tools 4 for Eclipse``` section.
- Choose ```4.19.1 - Windows x86_64``` to download or other option based on your OS.
- Extracting Spring Tools
- Run 'Hello World' using Spring Tools

Note: If you have any further confusion, follow some youtube video or read some blog post.

## 📝 Home Work

1. Learn history of JAVA.
2. Write a JAVA program "Hello World" in notepad and execute with command line.
