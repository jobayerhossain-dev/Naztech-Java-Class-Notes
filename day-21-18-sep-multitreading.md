# Day 21 - 18 Sep - Multitreading 🚀

[pdf\_links.md](pdf\_links.md "mention")Multitrading is process where device can run multiple task at a time. It can improve device efficiency, capability and time complexity.

for more learn about multitrading. Please, [click here](pdf\_files/Class17.pdf)

```java
package com.example;

public class MultiThreadExample {
    public static void main(String[] args) {
        NumberPrinter thread1 = new NumberPrinter(1);
        NumberPrinter thread2 = new NumberPrinter(6);

        // Start the threads
        thread1.start();
        thread2.start();
    }
}

class NumberPrinter extends Thread {
    private int start;

    public NumberPrinter(int start) {
        this.start = start;
    }

    public void run() {
        for (int i = start; i <= start + 4; i++) {
            System.out.println(Thread.currentThread().getId() + " : " + i);
        }
    }
}
```
