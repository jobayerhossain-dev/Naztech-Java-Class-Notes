# Day 16 - 11 Oct - Exception Handling end

## Throwing Exceptions

You can throw exceptions manually using the `throw` keyword. This is useful for creating custom exceptions or re throwing exceptions in your code.

Here is a java code example of throwing a custom exception:

```java
public class CustomExceptionExample {
    public static void main(String[] args) {
        try {
            throw new CustomException("This is a custom exception.");
        }
        catch (CustomException e) {
            System.out.println("Caught custom exception: " + e.getMessage());
        }
    }
}

class CustomException extends Exception {
    public CustomException(String message) {
        super(message);
    }
}
```

## Using `throws` Keyword Example

Temporary Example:

```java
public class ThrowsExample {
  static void checkAge(int age) throws ArithmeticException {
    if (age < 18) {
      throw new ArithmeticException("Access denied - You must be at least 18 years old.");
    }
    else {
      System.out.println("Access granted - You are old enough!");
    }
  }

  public static void main(String[] args) {
    checkAge(15); // Set age to 15 (which is below 18...)
  }
}
```
