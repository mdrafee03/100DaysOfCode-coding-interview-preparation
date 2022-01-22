### Input
There are two ways to take input from the user or the file
- BufferedReader Class
- Scanner Class

### Buffered Reader
It's a class that used to read sequence of characters. 
InputStreamReader() is a function that converts the input stream of bytes into a stream of characters which is used as a argument of bufferedReader. It needs to throw IOException.

### Scanner
It is an advanced version of BufferedReader that can read formatted input. It contains predefined functions to read string, integer, Character and other data types as well.

next() function returns the next token/word in the input as a string and next().charAt(0) function returns the first character in that string.

hasNextXYZ() function checks if the type of the input is type XYZ. For example. hasNextInt() checks if the input is integer.

### BufferedReader Vs Scanner
- BufferedReader is syncronous but Scanner asyncronous. BufferedReader should be used for multiple threads
- BufferedReader is faster than Scanner

### System.out.println
It is used to print an argument that passed to it. It is upgraded version of print(). It prints any argument to it and adds a new line to the output. It allows the users to print different types of data.
We can use DecimalFormat for format decimal numbers, SimpleDateFormt to format dates
