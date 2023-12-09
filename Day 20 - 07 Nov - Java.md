# Day 20 - 07 Nov - Collections Framework

### Objective

By the end of this class, you should be able to:

1. Understand the Java Collections Framework and its importance.
2. Differentiate between various collection types.
3. Demonstrate practical usage of collections.
4. Use common collection methods.

### Introduction

The Java Collections Framework is a fundamental part of Java programming, offering a set of classes and
interfaces for handling and storing objects. It provides a way to work with groups of objects efficiently.
Collections are widely used in Java to simplify data manipulation and organization.

### Java Collections Framework Hierarchy

The Java Collections Framework is organized into various interfaces and classes. Let's discuss some core
components:

1. Collection Interface:
    - The root interface in the collection hierarchy.
    - It does not allow duplicate elements.

2. List Interface:
    - Extends the Collection interface.
    - Allows duplicate elements.
    - Elements are ordered in a specific sequence.
    - Common implementations include ArrayList and LinkedList.

3. Set Interface:
    - Extends the Collection interface.
    - Does not allow duplicate elements.
    - Elements are not guaranteed to be in a specific order.
    - Common implementations include HashSet and TreeSet.

4. Map Interface:
    - Not a part of the Collection hierarchy.
    - Stores key-value pairs.
    - Common implementations include HashMap and TreeMap.

### Common Collection Methods

Understanding how to use collections involves working with common methods like:

- add()
- remove()
- size()
- isEmpty()
- contains()
- iterator()

Practical Usage:

- Storing and managing data, e.g., student records.
- Sorting data.
- Efficient data retrieval and manipulation.
- Implementing data structures like stacks and queues.

The Java Collections Framework includes many classes and interfaces, but some are more commonly
used and considered more important due to their wide range of applications. Here are the most
important classes and interfaces:

### Core Interfaces

**Collection:** The root interface for collections, which has sub interfaces:
**List:** An ordered collection that allows duplicates.
**Set:** Unordered collection that doesn't allow duplicates.
**Queue:** Ordered collection used for task scheduling.

**Map:** An object that maps keys to values. It doesn't directly extend the Collection interface but is essential in the framework.

### Collection Classes

**ArrayList:** A dynamically resizable array-based list.
**LinkedList:** A doubly-linked list.
**HashSet:** An unordered collection of unique elements.
**LinkedHashSet:** A HashSet with predictable iteration order.
**TreeSet:** A sorted set, often implemented as a Red-Black tree.
**PriorityQueue:** A queue with elements ordered based on their natural order or a specified comparator.
**ArrayDeque:** A resizable array-based double-ended queue.

### Map Classes

**HashMap:** A hash table-based, unordered map.
**LinkedHashMap:** A LinkedHashMap that preserves insertion order.
**TreeMap:** A map with sorted keys, often implemented as a Red-Black tree.
**HashTable:** An older, synchronized version of HashMap (not recommended for new code).
**ConcurrentHashMap:** A thread-safe map for concurrent operations.
**WeakHashMap:** A map that allows keys to be garbage collected when not referenced.

### Utility Classes

**Collections:** A utility class for working with collections, including sorting and searching.
**Arrays:** A utility class for working with arrays, including sorting and searching. These classes and interfaces provide the foundation for working with various data structures in Java, allowing you to store, manipulate, and retrieve data efficiently. The choice of which class to use depends on your specific use case and requirements. The Java Collections Framework is an essential part of Java development. It simplifies the handling of data structures and makes your code more efficient. Understanding its core components and methods is crucial for any Java developer.

## 🛠️Practical

Practice is key to mastering the Java Collections Framework. Have fun exploring and experimenting with
different collection types!
//
Java programs that demonstrate the usage of the Java Collections Framework.

### Program 1: Using ArrayList to Store Student Names
```java
import java.util.ArrayList;

public class StudentList {
  public static void main(String[] args) {
    ArrayList < String > studentNames = new ArrayList < > ();

    // Adding student names to the list
    studentNames.add("Alice");
    studentNames.add("Bob");
    studentNames.add("Charlie");

    // Displaying the list of student names
    System.out.println("Student Names:");
    for (String name: studentNames) {
      System.out.println(name);
    }
  }
}
```

In this program, we use an ArrayList to store a list of student names. We add student names to the list
and then display them.

### Program 2: Using HashSet to Remove Duplicates

```java
import java.util.HashSet;

public class RemoveDuplicates {
  public static void main(String[] args) {
    String[] colors = {
      "Red",
      "Blue",
      "Green",
      "Red",
      "Yellow",
      "Blue"
    };
    
    HashSet < String > uniqueColors = new HashSet < > ();
    
    for (String color: colors) {
      uniqueColors.add(color);
    }

    System.out.println("Unique Colors:");
    for (String color: uniqueColors) {
      System.out.println(color);
    }
  }
}
```

In this program, we use a HashSet to remove duplicate elements from an array of colors. It ensures that only unique colors are displayed. These programs showcase practical applications of the Java Collections Framework with ArrayList, HashSet, and HashMap, which are commonly used collection classes.

## 📝 Home Work

1. Create an ArrayList of integers and demonstrate basic operations such as adding, removing, and
searching for elements.

2. Research and prepare a brief presentation on one specific implementation class of a Java
collection interface.
