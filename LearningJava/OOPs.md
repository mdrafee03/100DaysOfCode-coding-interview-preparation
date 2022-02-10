### OOP
Object oriented programing is a method used for designing a program using classes and objects.

### Methods
Methods consists of six components

- Access modifiers: defines access type of the method from where it can be accessed. There are 4 type of access specifiers namely public, protected, private, default.
- Return type: data type of the value returned from the method or void if no return a value
- Method name: name of the method
- Parameter list: comma separated list of the input parameters (consists of data type and name)
- Exception list: exceptions you expect by the method can throw
- Method body: the code need to be executed by the method

### Class
A class is user defined blueprint/prototype from which objects can be created. It consists of the properties or methods that are common to all objects. Class declaration consists of
- Modifiers: A class can have public or default acceess modifiers, not private or protected
- Class name: name of the class
- Superclass(optional): The class can have parent class which is called superclass. It is used with extends keyword. A class can only extends one parent.
- Interfaces(optional): A comma separated list of interfaces implemented by the class, proceded by the implements interface
- Body: properties and methods exist within the scope of the class

### Object
Object is the member of a class. A object consists of the following
- identity: Identity is a characteristics used to uniquely identify the object with a unique id, it is not visible to the external user. It is used internally by the JVM to identify each object uniquely
- State: represents the data/attribute of an object using properties
- Behavior: represents the behavior (functionality) of an object using methods

Notes:
- Object can't be created from abstract classes
- When object is created, the class is said to be instantiated
- All the instances of the class share the states and behavior

### Intializing an object
new operator instantiates a class by allocating memory to it and returning the reference to that memory. It also invokes the class constructor. Class constructors are recognized as it will have same name as class name. All classes have at least one constructor. If a class doesn't explicitly declare any, Java automatically provides no argument constructor called default constructor

### Anonymous objects
Objects are instantiated but not stored in a variable is called anonymous object.

Features:
- used for immediate method calling
- destroyed after method calling

### Naming convension
- class name should be noun in Pascalcase
- Interface should be adjective like Runnable, Serializable etc. in Pascalcase
- Methods should be verb camelcase
- Constants should be all uppercase and words separated by unerscore

### Four Pillars of OOPs
#### Inheritance
It's a mechanism by which one class is allowed to inherit feature from another class. The class whose feates are inherited is known as superclass or base class or parent class. The class inherits from superclass is known as subclass or derived class or extended class or child class. It is used with the keyword extends

Types of inheritance
- Single Inheritance: subclasses inherits from one superclass
- Multtilevel Inheritance: a subclass inherits from one superclass which in turns used a superclass for other classes. Example class A serves as a superclass for class B and again class B serves as a superclass for class C. 
- Hierarchical Inheritance: a subclass serves as a superclass for multiple subclasses. Example: Animal class serves as a superclass for Dog class and Cow class
- Multiple Inheritance: one class can have multiple superclass but java doesn't support multiple inheritance with classes. It can be achieved through interfaces
- Hybrid Inheritance: It is a mix of two or more of the above types of inheritance. As java doens't support multiple inheritance,hybrid inheritance is not supported with classes. It can be achieved through interfaces

Characteristics
- Except object class, every class has single inheritance. In the absence of explicit superclass, Object is the superclass implicitly.
- A superclass can have any number of subclasses but a subclass can have only one superclass
- A subclass inherits all the members. As constructors are not the member, they are not inherited but constructors of the superclass can be invoked from subclass by super keyword
- Private members can't be inherited
- Inherited members can be accessed directly just like other members
- New members can be declared in subclass which aren't in the superclass
- Super class methods can be overrided by the keyword @override

#### Abstraction
Abstraction is the process of hiding implementation details and expose only the necessary details to the user. It is also a process of identifying the essentation characteristics of an object ignoring irrelevant details. Abstraction is achieved by interfaces and abstract

Abstract classes characteristics
- abstract class is declared with the non-access modifier abstract
- only methods and classes is application for abstract, but not variables
- An abstract method is a method that is declared without implementation
- An abstract class may have either/both concrete method and abstract method
- An abstract method must be redefined in the subclass with overriding
- Any class contains abstract methods must be declared with abstract keyword
- An abstract class can't be directly instantiated with new operator
- An abstract class can have no abstract method which allow to create classes that can't be instantiated but can only be inherited
- An abstract class can have static method that can be called independently without an object

Abstract vs final:
Final is used to prevent inheritance whereas abstract classes depend on their child to complete the implementation. In case of methods, final is used to prevent overriding whereas abstract methods need to be overridden in sub-classes.

Abstract class vs Interface:
- Abstract class may have abstract and non-abstract methods but interface can have only abstract methods, default and static methods
- Abstract can have final, non-final, static, non-static variables where interface can have only static and final variables
- Abstract class can provide implementation of the interface where interface can't provide implementation of an abstract class
- Interface can extend only another interface where abstract class can extend both another class and implements multiple interfaces
- Members of the interface are public by default where abstract class members can be any access modifiers
- It application requires common methods or fields or access modifiers other than public, go for abstract class
- It a class need multiple inheritance, go with interface with implements keyword
- It it completely spcification of the behavior of a data but no concern about reuse or implementation go with interface

Advantages of Abstraction
1. It reduces the complexity of viewing the things
2. Avoids code duplication and increases reusability
3. Helps to increase the security of an application as only important details are provided

#### Encapsulation
wrapping up of data and code as a signle unit. In encapsulation, the variables will be hidden from other classes and can be accessed only through the methods of their current class

Advantages of Encapsulation:
- Data Hiding: the implementation and data storing process is hidden from the user
- Reusability: Easy to change with new requirements
- Testing: easy to test for unit testing

Encapsulation vs Abstraction: 
- Abstration is a process to gain the info while encapsulation is the process to contain the info
- Abstration is the method of hiding the unwanted info while encapsulation is method to hide the data in a single unit to protect the info from outside
- Abstration is implemeted using abstract class and interface while encapsulation can be implemented by access modifier
- the objects that help to perform abstraction are encapsulated but objects the results encapsulation need not be abstracted

#### Polymorphism
It is the ability of an object to take same action in many ways. Polymorphism is two types namely compile-time polymorphism and runtime polymorsphism. Compile-time polymorshism is achieved by method overloading. Runtime polymorphism is achieved by method overriding. Polymorphism allows the object to decide which form of the method to implement at compile-time or runtime.

**Method Overloading**: Multiple methods with same name but different parameters are called method overloading. Method can be overloaded by change in argument type, number of arguments.

**Method Overriding**: When derived class has implemented one of the member function of it's base class, the base class member function is said to be overridden. Overriden function is resolved at runtime.


### Why Java not a Pure OOP language
There are 7 qualities to be satisfied for a language to be pure object oriented. They are
1. Encapsulation
2. Inheritance
3. Abstraction
4. Polymorphism
5. All predefined types are objects
6. All object defined types are objects
7. All operations performed on objects must be only through methods exposed at the objects

Java supports all except 5 and 7. The reasons are given below

Primitives data type: Java supports primitive data types like int, float, String etc which violates 5th condition that all predefined types are objects.

Static keyword: Static classes can be used without the use of an object which violates 7th condition that all  operations will be performed through object exposed methods

Wrapper class: In wrapper classes, the operation can be performed without objects. example: String s1 = "ABC" + "D"

### Access Modifiers
There are four types of access modifiers

**Default**: when no access modifiers is specified for a class, method or data member it is called default access modifiers. It is only accessible by the same package

**Private**: The private access modifiers are is specified by the keyword private. The methods or data members declared as private are accessible within the class. Classes or interfaces can't be declared as private

**Protected**: The protected access modifiers are specified by the keyword protected. The methods or data members declared as protected are accessible within the same package or the subclasses in different packages. Classes or interfacescan't be declared as protected

**Public**: the public access modifier is specified by the keyword public. Classes, methods or data members declared as pbulic are accessible from everywhere in the program.

N.B: 
- Try to use most restrictive access level that makes sense for a particular member
- Avoid public fields excepts for constants

### Constructor
Constructors are used to initialize variables. The characteristics are
- Constructors must have the same name as the class which is resides
- Constructors don't return any type
- Constructors are called only once at the time of object creation
- Constructors can't be abstract, final, static or synchronized
- Access modifiers canbe used in the constructor
- recursive constructor calling is invalid
- this() is used to call current class default constructor, super is used to call parent constructor

There are two types of constructor
- No-argument constructor: has no parameter known as default constructor, if it is not declared, compiler creates default
- Parameterized Constructor: constructors that has parameters known as parameterized constructor

Constructors can be overloaded i.e it may have multiple constructors to create object in different ways. Compiler differentiates the constructors based on number of parameters, type of the parameters, and order of the parameters

**Copy Constructor**: A copy constructor is a constructor that creates an object using another object of the same class. It is used to deep copy of existing object. It is useful when the class has several fields and we want a deep copy of it.

Copy Constructor vs Clone
- Copy Constructor is easier to implement, no need to implement cloneable interface and handle CloneNotSupportedException
- Copy constructor can assign value to a final field while clone method cannot
- Clone object returns object reference, which needs to typecast to the appropriate type

**Constructor Chaining**: It is a process of peforming operations combining multiple constructor. One constructor call another, then that constructor call another.

**Private Constructor**: Private constructor is used for two major reasons
- Internal Constructor chaining
- Singleton class design Pattern

Singleton class: Only one object can be created from the class is called singleton class. We can't have more than one object of that class
