# Day 06 - 05 Sep - Control Flow Statement

Control flow statements in Java are constructs that determine the order in which the instructions within a program are executed. They allow you to control the flow of your program's logic based on conditions and loops. Java provides three types of control flow statements:

- Conditional Statements or Decision Making Statements
  - if statements
    - if statement (Simple if)
    - if-else statement
    - if-else-if statement
    - Nested if-statement
  - switch statement
- Loop Statements
  - for loop
  - while loop
  - do while loop
  - for-each loop
- Jump Statements
  - break statement
  - continue statement

### Conditional Statements

As the name suggests, conditional or decision-making statements decide which statement to execute and when. conditional statements evaluate the **Boolean** expression and control the program flow depending upon the result of the condition provided. There are two types of conditional statements in Java, i.e., If statement and switch statement.

#### If Statements

##### `if` Statement

The `if` statement is used to execute a block of code if a specified condition is true. Here is the basic structure of `if` statement:

```
if (condition) {
    // executes when condition is true
}
```

Example:

```java
public class CheckAdult {
  public static void main(String[] args) {
    int age = 25;
    if (x >= 18) {
      System.out.println("You are adult.");
    }
  }
}
```

##### `if`-`else` Statement

The if-else statement is an extension to the if-statement, which uses another block of code, i.e., else block. The else block is executed if the condition of the if-block is evaluated as false. Here is the basic structure of `if else` statement:

```
if(condition) {
    // executes when condition is true
}
else{
    // executes when condition is false
}
```

Example:

```java
public class CheckAdultOrMinor {
  public static void main(String[] args) {
    int age = 25;
    if (x >= 18) {
      System.out.println("You are adult");
    } else {
        System.out.println("You are minor");
    }
  }
}
```

##### `if`-`else if` Statement

The if-else-if statement contains the if-statement followed by multiple else-if statements. In other words, we can say that it is the chain of if-else statements that create a decision tree where the program may enter in the block of code where the condition is true. We can also define an else statement at the end of the chain. Here is the basic structure of `if`-`else if` statement:

```
if (condition 1) {
  // executes when condition 1 is true
} else if (condition 2) {
  // executes when condition 2 is true
} else {
  // executes when all the conditions are false
}
```

Example:

```java
public class CheckOneTwoOrThree {
   public static void main(String args[]) {
      int x = 3;

      if (x == 1) {
         System.out.print("Value of x is 1");
      } else if (x == 2) {
         System.out.print("Value of x is 2");
      } else if (x == 3) {
         System.out.print("Value of x is 3");
      } else {
         System.out.print("This is else statement");
      }
   }
}
```

##### Nested if-statement

In nested if-statements, the `if` statement can contain a `if` or `if`-`else` statement inside another if or `if`-`else` statement. Here is the basic structure of nested if-statement:

```
if (condition 1) {
  //executes when condition 1 is true
  if (condition 2) {
    //executes when condition 2 is true
  } else {
    //executes when condition 2 is false
  }
} else {
    //executes when condition 1 is false
}
```

Example:

```java
public class NestedIfExample {
  public static void main(String[] args) {
    String address = "Delhi, India";

    if (address.endsWith("India")) {
      if (address.contains("Meerut")) {
        System.out.println("Your city is Meerut");
      } else if (address.contains("Noida")) {
        System.out.println("Your city is Noida");
      } else {
        System.out.println(address.split(",")[0]);
      }
    } else {
      System.out.println("You are not living in India");
    }
  }
}
```

#### `switch` Statement

The `switch` statement allows you to select one of many code blocks to be executed, based on the value of an expression. Here is the basic structure of `switch` statement:

    ```
    switch (expression){
        case value1:
            // Code for value1
            break;
        case value2:
            // Code for value2
            break;
        default:
            // Code if no case matches
    }
    ```

    Example:
    ```java
    import java.util.Scanner;

    public class SwitchExample {
        public static void main(String[] args) {
            int number = 1;

            switch (number) {
                case 0:
                    System.out.println("Zero");
                    break;
                case 1:
                    System.out.println("One");
                    break;
                case 2:
                    System.out.println("Two");
                    break;
                default:
                    System.out.println("Not Zero, One or Two");
            }
        }
    }
    ```

### Loop Statements

In programming, sometimes we need to execute the block of code repeatedly while some condition evaluates to true. However, loop statements are used to execute the set of instructions in a repeated order. The execution of the set of instructions depends upon a particular condition.

In Java, we have three types of loops that execute similarly. However, there are differences in their syntax and condition checking time.

1. for loop
2. while loop
3. do-while loop and
4. foreach loop, which is an enhanced for loop to traverse the data structures like array or collection.

Let's understand the loop statements one by one.

#### For Loop

In Java, for loop is similar to C and C++. It enables us to initialize the loop variable, check the condition, and increment/decrement in a single line of code. We use the for loop only when we exactly know the number of times, we want to execute the block of code. Here is the basic structure of `for` loop statement:

```
for (initialization, condition, increment/decrement) {
  // block of statements
}
```

Example:

```java
public class CalculateFirstTenIntegers {
    public static void main(String[] args) {
        int sum = 0;
        for (int j = 1; j <= 10; j++) {
            sum = sum + j;
        }
        System.out.println("The sum of first 10 natural numbers is " + sum);
    }
}
```

#### While Loop

The while loop is also used to iterate over the number of statements multiple times. However, if we don't know the number of iterations in advance, it is recommended to use a while loop. Unlike for loop, the initialization and increment/decrement doesn't take place inside the loop statement in while loop.

It is also known as the entry-controlled loop since the condition is checked at the start of the loop. If the condition is true, then the loop body will be executed; otherwise, the statements after the loop will be executed. The structure of the `while` loop is given below:

```
while (condition) {
  //looping statements
}
```

Example:

```java
public class CalculateFirstTenEvenNumbers {
    public static void main(String[] args) {
        int i = 0;
        System.out.println("Printing the list of first 10 even numbers \n");
        while (i <= 10) {
            System.out.println(i);
            i = i + 2;
        }
    }
}
```

#### Do While Loop

The do-while loop checks the condition at the end of the loop after executing the loop statements. When the number of iteration is not known and we have to execute the loop at least once, we can use do-while loop.

It is also known as the exit-controlled loop since the condition is not checked in advance. The structure of the do-while loop is given below:

```
do {
    //statements
} while (condition);
```

Example:

```java
public class PrintFirstTenEvenNumbers {
    public static void main(String[] args) {
        int i = 0;
        System.out.println("Printing the list of first 10 even numbers \n");
        do {
            System.out.println(i);
            i = i + 2;
        } while (i <= 10);
    }
}
```

### Jump Statements

Jump statements are used to transfer the control of the program to the specific statements. In other words, jump statements transfer the execution control to the other part of the program. There are two types of jump statements in Java, i.e., ```break``` and ```continue```.

#### ```break``` Statement

As the name suggests, the ```break``` statement is used to break the current flow of the program and transfer the control to the next statement outside a loop or ```switch``` statement. However, it breaks only the inner loop in the case of the nested loop.

The ```break``` statement cannot be used independently in the Java program, i.e., it can only be written inside the loop or ```switch``` statement.

Consider the following example in which we have used the ```break``` statement with the for loop.

```java
public class SkipIfFoundSix {
    public static void main(String[] args) {
        for (int i = 0; i <= 10; i++) {
            System.out.println(i);
            if (i == 6) {
                break;
            }
        }
    }
}
```

#### ```continue``` Statement

Unlike ```break``` statement, the ```continue``` statement doesn't break the loop, whereas, it skips the specific part of the loop and jumps to the next iteration of the loop immediately.

Consider the following example to understand the functioning of the continue statement in Java.

```java
public class SkipIfFoundFour {
    public static void main(String[] args) {
        for (int i = 0; i <= 10; i++) {
          if (i == 4) {
              continue;
          }
          System.out.println(i);
        }
    }
}
```