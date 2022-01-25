### Strings
String is an object that represent sequence of char values. It provides lots of method to work with it.
There are two ways to create String object
- By strin literal
- By new keyword

#### String Literal
It can be created by using double quotes. The object will be created in String constant pool. This allows JVM to optimize the initialization of String literal. 

String Constant Pool: JVM checks the String in constant pool when a string is created by string literal. If the string doesn't exist, then a new string instance is created and placed in a pool. If the string exists, then it will not create a new object. Rather it will return the reference to the same instance. The cache which stores these string instances in known as String Constant pool or String pool.

#### String by new keyword
JVM will create new string object in normal (non-pool) heap memory and the literal is placed in the string constant pool. The varialbe will refer to the object in a heap.

It is prefered to use string literal as it allows JVM to optimize memory allocation

### CharSequence Interface
The charSequence interface is used to represent the sequence of characters. String, StringBuffer and StringBuilder classes implement it. we can create strings with these classes as well

Java String is immutable. When we change any string, a new string is created. If mutable string, StringBuffer and StringBuilder is used.

### StringBuffer
It is a peer class of String which provides growing and mutable sequences. It is recommended over StringBuilder class as it is faster in most implementations.

### StringBuilder
It represents a mutable seuence of characters. StringBuilder provides no guarantee of synchronization whereas the StringBuffer does. Instancs of StringBuilder are not safe for use by multiple threads.

### String Vs StringBuffer Vs StringBuilder
- If a string is going to remain constant throughout the program, use String class object because a String object is immutable
- If a string can change and only be accessed from a single thread, using StrinBuilder is enough
- If a string can change and will be accessed from multiple thread, use StringBuffer because StringBuffer is synchronous, so you have thread safety
- If you don't want thread-safety, you can use StringBuilder as it is not synchronized

### Conversion between types of strings
Case 1: From String to StringBuffer and StringBuilder
pass the string to StringBuilder and StringBuffer constroctors

Case 2: From StringBuffer and StringBuilder to String
toString() method is used to convert from StringBuffer and StringBuilder to String

Case 3: From StringBuffer to StringBuilder and vice-versa
First convert StringBuffer or StringBuilder to string and Follow step 1

### String Tokenizer
It is used to break a string into tokens. StringTokenizer object internally maintains a current position  within the string to be tokenized.

### StringJoiner
It is used to construct a sequence of characters separated by a delimiter and optionally starting with supplied prefix and ending with supplied suffix.

### Why String Immutable
In the String constant pool, a String object is likely to have one or more references. If several references point to the same String, it would be bad if one of the references modified that String. That's why String object is immutable. The String class is marked as final, so no one can even override it.

