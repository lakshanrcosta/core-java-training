# 🚀 Introduction to Java

## 📌 1. What is Java?
- Java is a **high-level, object-oriented programming language** developed by **Sun Microsystems** (now owned by **Oracle**).
- First released in **1995**, Java is designed to be **platform-independent**, allowing developers to write code once and run it anywhere (**WORA**).
- It is widely used in **web applications, enterprise software, mobile applications (Android), and cloud computing**.

---

## 🔥 2. Key Features of Java
### ✅ **Platform Independence**
- Java uses the **Java Virtual Machine (JVM)**, making it possible to run Java programs on any operating system without modification.

### ✅ **Object-Oriented Programming (OOP)**
- Java follows the OOP paradigm, supporting core concepts like:
  - **Encapsulation** (data hiding)
  - **Inheritance** (code reusability)
  - **Polymorphism** (method overriding and overloading)
  - **Abstraction** (hiding implementation details)

### ✅ **Robust & Secure**
- **Automatic Memory Management**: Java has a **Garbage Collector (GC)** that manages memory allocation and deallocation.
- **Exception Handling**: Built-in mechanisms to handle runtime errors.
- **Security Features**: Java provides a **Security Manager** to define access control policies.

### ✅ **Multi-threading Support**
- Java supports **concurrent execution** of multiple tasks, allowing better resource utilization and improved performance.

### ✅ **Rich API & Standard Libraries**
- Java provides extensive built-in libraries for:
  - **Networking** (`java.net`)
  - **Database Access (JDBC)** (`java.sql`)
  - **Collections Framework** (`java.util`)
  - **File Handling** (`java.io`)

### ✅ **Portability**
- Java programs can run on **Windows, Linux, macOS, and embedded systems** as long as a JVM is installed.

---

## 🏛 3. Java Architecture
Java follows a **three-step execution model**:

### 🔹 **1. Java Compiler (`javac`)**
- Converts Java **source code** (`.java`) into **bytecode** (`.class`).

### 🔹 **2. Java Virtual Machine (JVM)**
- The JVM reads the **bytecode** and converts it into **machine code** specific to the operating system.

### 🔹 **3. Java Runtime Environment (JRE)**
- **JRE = JVM + Standard Java Libraries** → Required to **run** Java applications.

### 🔹 **4. Java Development Kit (JDK)**
- **JDK = JRE + Compiler (`javac`) + Development Tools** → Required to **develop and compile** Java applications.

---

## 📜 4. Java Program Structure
A **basic Java program** follows this structure:

```java
// Example: Hello World program in Java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```