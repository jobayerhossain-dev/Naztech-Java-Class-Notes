# Day 15 - 10 Oct - Exception Handling start


Exception handling is an important concept in Java that allows you to gracefully handle runtime errors, also known as exceptions, in your java code. It ensures that your program doesn't crash when an unexpected error occurs and provides a mechanism to recover from these errors. Let's dive into the details of exception handling in Java with examples.

### Definition

In Java, exceptions are objects that represent unexpected events or errors that can occur during program execution. These events can be caused by various reasons, such as invalid user input, file not found, or division by zero.
Exceptions are divided into two main categories:

- Checked Exceptions (Compile time Exceptions) and
- Unchecked Exceptions (Runtime Exceptions)

The `try-catch` statement is used for exception handling in Java.

### The `try-catch` Block

To handle exceptions, you use a `try-catch` block. The code that might throw an exception goes inside the `try` block, and you catch and handle the exception in the `catch` block. Here is a basic example of `try-catch` block:

```java
try {
    // Code that may throw an exception
} catch (ExceptionType e) {
    // Handle the exception
}
```

### Details About Types of Exceptions

#### Checked Exceptions (Compiler Time Exception)

Checked exceptions are exceptions that are checked at compile time. This means the compiler ensures that you handle these exceptions either by catching them or declaring that your method throws them. Common examples include `IOException`, `FileNotFoundException`, and `SQLException`. Here is an example of Checked Exception in Java:

```java
import java.io.BufferedReader;
import java.io.FileReader;
import java.io.IOException;

public class CheckedExceptionExample {
    public static void main(String[] args) {
        try {
            BufferedReader reader = new BufferedReader(new FileReader("file.txt"));
            String line = reader.readLine();
            System.out.println(line);
            reader.close();
        } catch (IOException e) {
            System.out.println("An error occurred: " + e.getMessage());
        }
    }
}
```

#### Unchecked Exceptions (Runtime Exceptions)

Unchecked exceptions are exceptions that are not checked at compile time, and you are not required to catch or declare them. Common examples include `NullPointerException`, `ArithmeticException`, and `ArrayIndexOutOfBoundsException`. Here is an example of Unchecked Exception in Java:

```java
public class UncheckedExceptionExample {
    public static void main(String[] args) {
        int[] numbers = {1,2,3};
        int result = numbers[5]; // ArrayIndexOutOfBoundsException
        System.out.println(result);
    }
}
```
