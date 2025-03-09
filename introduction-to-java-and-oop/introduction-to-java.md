# Introduction to Java

## 1. What is Java?
- Java is a **high-level, object-oriented programming language** developed by **Sun Microsystems** (now owned by **Oracle**).
- It was released in **1995** and is designed to be **platform-independent** using the **Java Virtual Machine (JVM)**.

## 2. Key Features of Java
- **Platform Independence**: Write once, run anywhere (WORA) using the JVM.
- **Object-Oriented**: Supports principles like **encapsulation, inheritance, and polymorphism**.
- **Robust & Secure**: Features automatic memory management (Garbage Collection) and security mechanisms.
- **Multi-threading**: Supports concurrent execution for better performance.
- **Rich API**: Provides built-in libraries for various functionalities (e.g., networking, database access, GUI development).
- **Portable**: Java programs can run on any system with a JVM.

## 3. Java Architecture
- **Java Compiler (javac)**: Converts Java source code (`.java`) into **bytecode** (`.class`).
- **Java Virtual Machine (JVM)**: Executes the bytecode on different operating systems.
- **Java Runtime Environment (JRE)**: Contains JVM and necessary libraries to run Java applications.
- **Java Development Kit (JDK)**: Includes JRE, compiler, and development tools.

## 4. Java Program Structure
A basic Java program consists of:
```java
// Example: Hello World program in Java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
