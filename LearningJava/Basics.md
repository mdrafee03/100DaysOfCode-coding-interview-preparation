### Description
Java was developed by James Goslin in the year 1991.

### Execution Phase
There three execution phase
1. Write - the program is written by programer (.java extension)
2. Compile - the program is compiled by JAVAC which converts the program to the bytecode(.class extension) which can be run any platform by interpreter
3. Run - JVM is an interpreter which executes bytecode

### JVM (Java Virtual Machine)
It is responsible for executing the java Program line by line. JVM calls the main method of the Java Program

### JRE (Java Runtime Environment)
It provides an environment to only run(not develop) the java program

### JDK (Java Development Kit)
It provides an environment to develop and run the Java program. It includes development tools and JRE

### Garbage Collector
It recollects all the objects that are not referenced

### Features
- Platform Independent
- Object Oriented
- Simple, not included pointers, operator overloading, multiple inheritence, explicit memory allocation
- Support Multithreading
- Uses JIT which compiles code on-demand basics

### JIT - Just In Time Compiler
It is essential part of JRE which is responsible for performance optimization at run time. JIT compiler interact with JVM at run time and compile suitable bytecode sequence into machine code. While using JIT compiler, the hardware execute the native code. The greater is the degree of optimization done, the more time a JIT compiler spends in execution stage.

### Byte Code
Byte code is an intermediate code between source code and machine code. It is the result of compilation by JVM and it is translated into machine code to run it.

### Machine Code
It is a set of instructions that is processed by the CPU. 

### Notes
- Every application must contain a main method which is the entry point of the application
- By convention, the name of the main class(a class that contains the main method) should match the name of the file that holds the program.
- Every Java program must have a class definition that matches the filename (class name and file name should be same).


### Primitive and Non-Primitive Data Types
Primitive data types are the predefined data types. They specify the size and type of standard values. There are 8 primitive data types namely byte, short, int, long, double, float, boolean, char. When a variable is stored, it is stored in the stack. When a variable is copied, changes made to copied variable will not reflect changes in the original variable.

Non-primitive or reference data types are the user-defined data types that refer to any particular object. When a variable is created, the variable will be stored in the stack and the refered object will be stored in the heap. When a variable is copied, changes made to any variable will reflect the change in both the variables because they both refer to the same object in the heap. Examples are string, array, class etc.


### Local Variable
The variables declared within a block or method. These variables are created when the block is entered and destroyed after exiting from the block.

### Instance Variable
The non-static variables declared within the class but outside of methods. It is created when an object of the class is created and destroyed with object and it can be accessed only by created objects.

### Static Variable
The variables declared within the class but only have one instance per class irrespective of the number of object created by the class.

## Scope
Scope of a variable is the part of the program where the variable is accessible.

### Member Variable
These are declared inside the class but outside of methods. 
- These variables can be accessed anywhere in the class
- Access specified with these variables doesn't effect the access inside the class
- Access modifiers defines what variables can be accessed outside the class
    - public variables can be accessed anywhere outside the class
    - private variables can't be accessed outside the class
    - protected variables can be accessed from package and sub class
    - default/no modifiers variables can be accessed only by package

### Local Variables
Variables declared inside a method is called local variables and it is only accessible inside the method

### Loop Variables
A variable declared inside a pair of brackets {} in a method is called loop variables. They can be accessible only within the loop

Note: The name of the variable of inner and outer loop must be different

### Wrapper Class
A wrapper class is a class whose object contains primitive data types. They are needed to convert primitive data types into objects so that arguments passed to a method can be modified.

### Autoboxing
Automatic conversion of primitive types to the object of their corresponding Wrapper classes is known as autoboxing. Example: conversion of int to Integer

### Unboxing
Reverse of autoboxing i.e conversion of object of a wrapper class to the primitive type. Example conversion of Integer to int.
