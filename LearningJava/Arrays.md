### Arrays
- All arrays are dynamically allocated
- The size of an array must be specified by int, short, not long
- The direct superclass of an array type is Object
- Every array type implements the interface Cloneable and Serializable
- It can contain primitives and object reference of a class
- Actual values of primitive data types are stored in contigous memory locations- 

### Creating Array
Array has two components namely type and name. type determines what type of data the array will hold. When an array is declared, only a reference of an array is created, but no memory allocated for it
Example int[] intArray or int intArray[] 

### Instantiating Array
In order to allocate memory to array, instantiation of an array is required by new keyword. The type and number of elements must be specified to allocate memory
Example: int[] intArray = new int[20]

N.B: The elements in the array allocated by new automatically be initialized to zero (for numeric types), false (for boolean), or null (for reference types)

### Array Literal
If the size and variables of the array is known beforehand, array literals can be used
Example: int[] intArray = {1, 2, 3}

### Accessing Array
Each element in the array can be accessed by its index and loop
Example: for(int i=0; i<arr.length; i++) System.out.println(arr[i]);

### Arrays of objects
array of object is similar as primitives except each array element is instantiated using the construcctor of that object

Example: Student[] arr = new Student[2];
arr[1] = new Student("sdfs");

### Accessing out of bound index
JVM throws ArrayIndexOutOfBoundsException to indicate that the array has been accessed with illegal index (either negative or greater than or equal to the size of an array


### Multidimensional Arrays
In arrays of arrays, each array elements holds the reference of other arrays

### Cloning of arrays
When a clone operation is performed in single dimensional array, "deep copy" is performed with the new array containing copies of the original array's element, not the reference. When changing the cloned array, original array will not be changed.

When cloning is performed in multi dimensional array, "shallow copy" is performed. It means that the new array containing the reference of the original array elements.

### Array class
The arrays class provides static methods to dynamically create and access arays. Fro example: binarySearch, sort etc.

### 2D array
When initialize a 2D array, specifying first dimension is required but second dimension is optional as we can initialize different columns for rows.

### Jagged array
An 2D array such that member arrays can be of different size i.e 2D array but a variable number of columns in each row. Example: arr[0] = new int[2], arr[1] = new int[4]

### Final Array
It means the array variable which is reference to an object can't be changed to refer anything else but the members of array can be modified

### Reflection Array class
It provides static methods to create and access array dynamically. It's a final class which means it can't be instantiated or changed. It is different from Util array which is used to manipulating array.
