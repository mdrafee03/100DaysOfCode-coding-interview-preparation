### Control Flow
Control statements are used to control the flow of execution of program based on certain condition.

### If
It is used to decide whether a certian statement or block of statements will be executed or not.

### If-else
If is used to decide another block will be executed or not if the "if" block condition is false

### Nested if
nested if is an if statement inside another if or else statement

### if-else-if ladder
If statements are executed from top to bottom. As soon as one of the conditions controlling the if is true, the statements associated with that if is executed, and the rest of the ladder is bypassed. If none of the conditions is true, the final else statement will be executed.

### Swich case
Swich case executes one statements from multiple ones. It is equivalent to if-else-if ladder statement

Characteristics:
- duplicate case values are not allowed
- the value for a case must be of the same data type as the variable in the switch
- the value for a case must be constant or a literal. Variables are not allowed
- the break statement in swich is used to terminate a statement associated with it. If break is not used, it will continue on the next case
- 
### Jump
There are three jump statements namely continue, break and return. These statements transfer control to the other part of the program.

#### Break
It can terminate the immediate loop, bypassing the conditional expression and any remaining code in the body of the loop. It only break the innnermost loop in nested loop. break can be used with label to break to the specific labelled loop.

#### Continue
Continue statement breaks one iteration and stop executing the remaining code of the body in the loop and continues next iteration of the loop.

#### Return
It is used to explicitly return from a method and bypassing the remaining of the code. It causes transfer control back to the caller of the method

### Loop
Loops facilitates the excution of a set of statements repeatedly while some condition evaluates to true. There are three control flow to execute the loop namely while, for, do while

#### While
It is a control flow which executes code repeatedly based on certain condition is true.

Characteristics:
- It starts with checking of condition. If the condition is true, the loop body statements are executed
- When the condition is false, the loop terminates and it transfer control from the loop the next statement below the loop

#### For
It is used over while when the iteration is fixed. It consumes initialization, condition checking and increment/decrement. 

There is an enhanced version of for loop which is used to iterate through the elements of a collection. It is easier than loop as it doesn't have to increment. It works on the basis of elements and not the index.

#### Do while
It is similar to the while loop except it check for condition after executing the statement

Characteristics:
- It starts with execution of the statements, no checking of condition at first iteration
- After executing the statements, it checks for the condition. If the condition evaluates to true, next iteration of loop starts
- 
