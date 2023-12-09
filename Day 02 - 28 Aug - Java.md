# Day 02 - 28 Aug

## Java Editions

Java was initially developed by Sun Microsystems and released as open source software under the GNU General Public License (GPL). Now java is a product of Oracle Corporation. There are four editions of java are available:

- Standard Edition (SE)
- Micro Edition (ME)
- Enterprise Edition (EE)
- Card Edition (CE, Learn more about it from [wikipedia](https://en.wikipedia.org/wiki/Java_Card))

## Usage of Package in Java

A package can be used for grouping classes and interfaces together that share a common purpose or concern. It contains all related programs.

## Hierarchy of a java program
Package > Class > Interface or Method

## Basic Structure of All Java Program

```java
// Optional package declaration
package com.example.myprogram;

// Import statements (if needed)
import java.util.*;

// Class declaration
public class MyClass {
    // Main method
    public static void main(String[] args) {
    // Program statements
        System.out.println("Hello, naztech!");
    }

    // Other methods (if needed)
    // ...
}
```

> **Note:**
> Java file name must be same as class name, which identify as main class
> In a single java file, main class must be public
> Must have a main method to main class to start executing a program

## 📝Practical
### Program Practice
HelloWorld.java: A program to print "Hello, World"
```java
public class HelloWorld {
	public static void main(String[] args){
		System.out.println("Hello, World");
	}
}
```

UserInput.java: Write a program that take user input to show some output
```java
import java.util.Scanner;

public class UserInput {
	public static void main(String[] args) {
		Scanner myScanner = new Scanner(System.in);
		System.out.print("What is you name?: ");
		
		String name;
		name = myScanner.nextLine();

		// Output: Welcome, {Inputed name}
		System.out.println("Welcome, " + name);
	}
}
```

CommandLineArg.java: Write a program to show some text by windows command prompt.
```java
public class CommandLineArg {
	public static void main(String[] args) {
		System.out.println(args[0] + " " + args[1] + " " + args[2]);
	}
}
```

### Class Test

#### 10 Reserved Words of Java
if, else, try, catch, finally, for, do, while, class, public, protected, private etc.

#### Data Types
- Char - *char*
- String - *String*
- Byte - *byte*
- Boolean - *bool*
- Integer - *int*
- Double - *double*
- Float - *float*
- Short - *short*

#### Access Modifes in Java
- default
- public
- protected
- private

### 5 Valid Variable Names in Java
- name
- name2
- $name
- _name
- full_name
