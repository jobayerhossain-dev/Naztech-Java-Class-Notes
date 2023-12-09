# Day 07 - 12 Sep - Loop end

## For Loop

In Java, a `for` loop is a control structure that allows you to execute a block of code repeatedly based on a specified condition. It's commonly used when you know in advance how many times you want to repeat a certain task. Let's break down the parts of a for loop:

```
for (initialization; condition; update) {
    // Code to be executed repeatedly
}
```

Here's what each part does:

1. **Initialization:** This is where you initialize a control variable (usually an
   integer) to a starting value. It's executed only once when the loop begins.

2. **Condition:** This is a boolean expression that's checked before each iteration
   of the loop. If the condition is `true`, the loop continues to execute. If it's `false`, the loop terminates.

3. **Update:** This part is responsible for changing the value of the control
   variable after each iteration. It's executed at the end of each iteration, just
   before re-checking the condition.

Now, let's look at an example:

```java
public class WhileLoopExample {
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            System.out.println("Iteration " + i);
        } //for block
    } //main method block
} //class block
```

In this example:

- **Initialization:** `int i = 1` initializes `i` to 1.
- **Condition:** `i <= 5` checks if `i` is less than or equal to 5.
- **Update:** `i++` increments `i` by 1 after each iteration.

The output of this loop will be:

```
Iteration 1
Iteration 2
Iteration 3
Iteration 4
Iteration 5
```

The loop starts with `i` equal to 1. It prints "Iteration 1," increments `i` to 2, and so on until `i` becomes 6, at which point the condition becomes `false`, and the loop terminates.

You can use for loops for a wide range of tasks, such as iterating over arrays, processing data, or performing calculations. They provide precise control over the number of iterations, making them a valuable tool in Java programming.

## While Loop

The while loop in Java is used to repeatedly execute a block of code as long as a specified condition is `true`. Here's the basic structure of a while loop:

```
while (condition) {
    // Code to be executed repeatedly
}
```

### Example Programs

Let's write a simple program that uses a while loop to print numbers from 1 to 5:

```java
public class WhileLoopExample {
    public static void main(String[] args) {
        int i = 1;
        while (i <= 5) {
            System.out.println("Number: " + i);
            i++;
        } //while block
    } //main method block
} //class block
```

In this program:

- `int i = 1` initializes `i` to 1.
- `i <= 5` checks if `i` is less than or equal to 5.
- `System.out.println("Number: " + i);` prints the value of `i`.
- `i++` increments `i` by 1 after each iteration.

This program will output:

```
Number:1
Number:2
Number:3
Number:4
Number:5
```

## Foreach Loop
Lets learn about the "enhanced for loop" or "for-each loop" in Java. This loop is used for iterating over collections like arrays and lists without the need for indices. It's quite beginner-friendly and simplifies iteration. Here's the basic structure of a foreach loop:

```
for (datatype element:collection) {
    // Code to be executed for each element
}
```

- **datatype:** The type of elements in the collection.
- **element:** A variable to represent each element in the collection.
- **collection:** The array or collection you want to iterate over.

### Example Programs
Let's say you have an array of integers and you want to print each element:

```java
public class ForEachLoopExample {
    public static void main(String[] args) {
        int[] numbers = {1, 2, 3, 4, 5};
        for (int num : numbers) {
            System.out.println("Number: " + num);
        } //for each block
    } //main method block
} //class block
```

In this example:
- int ```num``` is used to represent each element in the numbers array.

- ```for (int num : numbers)``` iterates over each element in the array.

- ```System.out.println("Number: " + num)``` prints each element.

The for-each loop is efficient and simplifies the code when you need to iterate over elements in collections, making it a great choice for beginners.