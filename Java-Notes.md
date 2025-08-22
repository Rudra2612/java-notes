# ☕ Java Notes

## 1. Introduction
- Java is a **high-level, object-oriented, platform-independent** programming language.
- Code is compiled into **bytecode**, which runs on the **Java Virtual Machine (JVM)**.
- **Write Once, Run Anywhere (WORA)**.

---

## 2. Basics

### Hello World
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
Data Types
Primitive types: int, long, double, float, char, boolean, byte, short

Non-primitive: String, Arrays, Classes, Interfaces

Variables
java
Copy
Edit
int age = 21;
double price = 19.99;
String name = "Rudra";
3. Control Flow
If-Else
java
Copy
Edit
if (age >= 18) {
    System.out.println("Adult");
} else {
    System.out.println("Minor");
}
Loops
java
Copy
Edit
for (int i = 0; i < 5; i++) {
    System.out.println(i);
}

while (age < 25) {
    age++;
}
4. Object-Oriented Programming (OOP)
Class and Object
java
Copy
Edit
class Car {
    String brand;
    int year;

    void drive() {
        System.out.println("Car is driving...");
    }
}

public class Main {
    public static void main(String[] args) {
        Car myCar = new Car();
        myCar.brand = "Toyota";
        myCar.drive();
    }
}
Encapsulation
Achieved using private fields and getter/setter methods.

Inheritance
java
Copy
Edit
class Animal {
    void sound() { System.out.println("Animal makes sound"); }
}

class Dog extends Animal {
    void sound() { System.out.println("Dog barks"); }
}
Polymorphism
Compile-time (Method Overloading)

Runtime (Method Overriding)

Abstraction
Using abstract classes and interfaces.

5. Collections Framework
List
java
Copy
Edit
import java.util.*;

List<String> names = new ArrayList<>();
names.add("Alice");
names.add("Bob");
System.out.println(names);
Set
java
Copy
Edit
Set<Integer> numbers = new HashSet<>();
numbers.add(1);
numbers.add(2);
numbers.add(2); // duplicate ignored
Map
java
Copy
Edit
Map<String, Integer> scores = new HashMap<>();
scores.put("Alice", 90);
scores.put("Bob", 85);
System.out.println(scores.get("Alice"));
6. Exception Handling
java
Copy
Edit
try {
    int result = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Error: " + e.getMessage());
} finally {
    System.out.println("This block always executes");
}
7. Java Features
✅ Platform independent

✅ Object-oriented

✅ Strongly typed

✅ Automatic Garbage Collection

✅ Rich API (Collections, Streams, etc.)
