### Execution Phase
There three execution phase
1. Write - the program is written by programer (.java extension)
2. Compile - the program is compiled by JAVAC which converts the program to the bytecode(.class extension)
3. Run - JVM executes bytecode
### JVM (Java Virtual Machine)
It is responsible for executing the java Program line by line. JVM calls the main method of the Java Program

### JRE (Java Runtime Environment)
It provides an environment to only run(not develop) the java program

### JDK (Java Development Kit)
It provides an environment to develop and run the Java program. It includes development tools and JRE

### Garbage Collector
It recollects all the objects that are not referenced

### Local Variable
The variables declared within a block or method

### Instance Variable
The non-static variables declared within the class but outside of methods. It is created when an object of the class is created and destroyed with object. 

### Static Variable
The variables declared within the class but only have one instance per class irrespective of the number of object created by the class.

## Scope

### Member Variable
These are declared inside the class but outside of methods. 
- These variables can be accessed anywhere in the class
- Access specified with these variables doesn't effect the access inside the class
- Access modifiers defines what variables can be accessed outside the class
    - public variables can be accessed anywhere outside the class
    - private variables can't be accessed outside the class
    - protected variables can be accessed from package and sub class
    - default/no modifiers variables can be accessed only by package