# Writing a Simple Java Program

Writing a Java program involves understanding the fundamental structure and syntax of the language. Java programs typically consist of classes and methods, with execution starting from a special method called `main`. In this section, we will explore the key components of a basic Java program and how they work together.

## A Basic Java Program Example

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

---

## Explanation of Keywords

### `public`
- This is an **access modifier** that allows the method or class to be accessible from anywhere in the program.
- When a method is `public`, it can be called from outside its defining class.

### `static`
- The `static` keyword means that the method belongs to the **class** rather than an instance of the class.
- This allows `main` to be called without creating an object of the class.

### `void`
- The `void` keyword indicates that the method **does not return a value**.
- In the `main` method, `void` ensures that no value is returned after execution.

### `main`
- The `main` method is the **entry point** of every Java application.
- It must always be `public static void` and accept a `String[]` parameter.
- JVM starts executing the program from this method.

### `String[] args`
- `args` is an **array of command-line arguments** passed to the program.

#### Example:
```sh
java HelloWorld arg1 arg2
```
---

## Scope in Java

Scope refers to the **visibility and accessibility** of variables, methods, and classes. There are four types of scopes in Java:

---

### 1. Class Scope (Global Scope)
- Variables declared **inside a class but outside methods** are available to all methods in that class.

#### Example:
```java
class Example {
    int globalVar = 10; // Class-level variable

    void print() {
        System.out.println(globalVar);
    }
}
```

---

### 2. Method Scope (Local Scope)

- Variables declared **inside a method** are accessible **only within that method**.

#### Example:
```java
class Example {
    void show() {
        int localVar = 5; // Only available in this method
        System.out.println(localVar);
    }
}
```

---

### 3. Block Scope

- Variables declared inside **blocks `{}`** (such as loops or `if` statements) are only accessible inside those blocks.

#### Example:
```java
class Example {
    void check() {
        if (true) {
            int blockVar = 20; // Only accessible in this block
            System.out.println(blockVar);
        }
        // System.out.println(blockVar); // ERROR: blockVar is out of scope
    }
}
```

---

### 4. Loop Scope

- Variables declared **inside loops** are only accessible **within the loop**.

#### Example:
```java
class Example {
    void loop() {
        for (int i = 0; i < 5; i++) {
            System.out.println(i);
        }
        // System.out.println(i); // ERROR: i is not accessible here
    }
}
```

---

## Execution Priorities in Java

Execution priorities determine the **order** in which Java statements, methods, and blocks execute.

### 1. Method Call Execution
- Java executes methods **in the order they are called**.

#### Example:
```java
class Example {
    public static void main(String[] args) {
        method1();
        method2();
    }
    
    static void method1() {
        System.out.println("Method 1 executed");
    }
    
    static void method2() {
        System.out.println("Method 2 executed");
    }
}
```

`Output`
```sh
Method 1 executed
Method 2 executed
```

---


### 2. Static Block Execution
- **Static blocks** execute **before** the `main` method when the class is loaded.

#### Example:
```java
class Example {
    static {
        System.out.println("Static block executed first");
    }
    
    public static void main(String[] args) {
        System.out.println("Main method executed");
    }
}
```

`Output`

```sh
Static block executed first
Main method executed
```

---

### 3. Instance Block Execution
- **Instance blocks** execute **when an object is created**, **before** the constructor.

#### Example:
```java
class Example {
    {
        System.out.println("Instance block executed");
    }

    Example() {
        System.out.println("Constructor executed");
    }

    public static void main(String[] args) {
        new Example();
    }
}
```

`Output`

```sh
Instance block executed
Constructor executed
```

---


### 4. Loop Scope

- Variables declared **inside loops** are only accessible **within the loop**.

#### Example:
```java
class Example {
    void loop() {
        for (int i = 0; i < 5; i++) {
            System.out.println(i);
        }
        // System.out.println(i); // ERROR: i is not accessible here
    }
}
```

