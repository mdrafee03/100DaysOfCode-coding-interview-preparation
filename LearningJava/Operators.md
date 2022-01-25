### Arithmetic Operators
This is used perform arithmertic operations on the primitive data types. These operators are
- Addition(+): add two operands
- Substraction(-): substract second operand from the first operand
- Multiplication(*): multiply two operands
- Division(/): divide first operand with the second operand
- Modulus(%): divide the first operand with the second operand and the remainder is returned

### Unary Operators
It needs one operand to perform the operation. The operators are described below

Unary Minus(-): used to convert negative value to a positive value
NOT(!): reverses the logical state of an operand i.e. true to false or vice versa
Increment(++): increment the value of an integer. Two types
  - Post-increment: used to execute the statement first, then increment
  - Pre-increment: used to increment first, then execute the statement

Decrement(--): decrement the value of an integer. Two types
  - Post-decrement: used to execute the statement first, then decrement
  - Pre-decrement: used to decrement first, then execute the statement

Bitwise Complement: It converted the operand into binary number and inverts all the bits.
Example: The operand 5 is represented in binary as one 0101. Then all the bits will be inverted. The result will be 1010 = 10

### Assignment Operators
These operators are used to assign values to another variable. The right side oprand must be same data type of the left side. These are two types
- Siimple Assignment operator: =
- Compound Assignment operator: simple assignment operator is mixed with arithmetic operator +, -, *, /, % makes compund operator

+=: It adds the current value of the left side with the right side and the result is stored in the left side.
-=: It substracts right side value from current value of the left side and the result is stored the left side
*=: It multiplies right side value with the the current value of the left side and the result is stored in the left side
/=: It divides the current value of the left side with the value of the right side and the result is stored in the left side
%= It divides the current value of the left side with the value of the right side and the remainder is stored in the left side

### Relational Operators
It is used to check relations between two operands. The return data type is boolean.

Equal to(==): It is used to check whether the two operand are equal or not. It returns true if equal, else false
Not eual to (!=): It is opposite of equal to. It returns true if not equal, else false
Greater than (>): It is used to check whether the first operand is greater than the second operand or not. If the left operand is greater than the right operand, it returns true, else false
Less than (<): It is opposite of Grater than. It returns true left operand is less than right operand, else false
Greater than or equal to : It checks whether the left operand is greater than or equal to the right operand. It returns true if left operand is greater than or equal to the right operand, else false
Less than or equal to: It checks whether the left operand is less than or equal to the right operand.

### Logical Operators
These operators are used to perform logical "AND", "OR" and "NOT" operation. It is used to combine multiple condition or complement the the evaluation of any condition. The second condition will be evaluated if the first condition is evaluated to false

Logical AND Operator (&&): It returns true if both the conditions are evaluated to true. If any condition is false, the result will be false
Logical OR Operator (||): It returns true if any of the conditions are evaluated to true. If none of the condition is true, it is evaluated to false
Logical NOT Operator (!): It is an unary operator and it returns true if the condition is evaluated to false, true if condition is evaluated to false

### Ternary Operator
It take three operands to perform. It is one liner replacement for if-else-if ladder statement

### Bitwise Operators
It is used to perform manipulation of individual bits of a number. They are

Bitwise OR(|): It returns bit by bit OR of input values. If either of the bit is 1, it gives 1, else 0
Example: 5  | 7 -> binary represention will 0101 | 0111. The result will be 0111 -> 7

Bitwise AND(&): It is return bit by bit AND of input values. If both bits are 1, it returns 1, else 0
Example 5 & 7 -> Binary representation will be 0101 & 0111. The result will be 0101 -> 5

Bitwise XOR(^): It returns bit by bit xor of input values. If corresponding bits are different, it returns 1, else 0
Example 5 ^ 7 -> Binary representation will be 0101 ^ 0111. The result will be 0010 -> 2

Bitwise Complement(~): It is an unary operator. It returns one's complement represention of the input values. If returns inverted value of the individual bits
~5 -> Binary representation will be 0101. The result will be 1010.

### Shift Operators
It is used to shift bit patterns right or left. The types of the shift operator is given below

Signed Left shift (<<): It moves all the bits by a given number of bits to the left. The leftmost bits will be lost.
Example 3 << 2 -> Binary representation of 3 is 0011. If we move this to left by 2 bits. The result will be 1100 -> 12

Signed Right Shift (>>): It moves all bits by bit by a given number of bits to the right. The rightmost bits will be lost
Example 12 >> 2 -> Binary representation of 12 is 1100. If we move it to the right by 2 bits. The result will be 0011 -> 3

Unsigned Right Shift (>>>): It moves the bits of the integer a given number of bits to the right. The sign operator is filled with 0s.
-8 >>> 2 -> Binary Representation of 8 -> 1000
filling up the sing operator with 0's it becomes 0000 0000 0000 0000 0000 0000 0000 1000
2's complement of the its positive number becomes
1111 1111 1111 1111 1111 1111 1111 1000
then move it with 2 digits it becomes
0011 1111 1111 1111 1111 1111 1111 1110
The result will be 1073741822

