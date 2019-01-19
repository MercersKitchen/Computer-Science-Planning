# Advanced Placement Computer Science Curriculum

---

Courses Available, unique to AP
- CSE2950: CSE Intermediate Practicum
- CSE3950: CSE Advanced Practicum

Starting with ABE Curriculum Map Documents, additional information is added specific to
- CSP Curriculum
- CSA Curriculum

CSP Curriculum:
- Digital Portfolio Section (CSP-D)
- Exam Section (CSP-E)

CSA Curriculum, Exam-based (CSA)

---

## Advanced Placement Specific Vocabulary

Table of Contents
- Java Docs
- Objects
- Exceptions

### JavaDoc

@param
- Specifies what the parameter does
- Example: @param par what this parameter does
- Outputs two lines:
  - "Parameters"
  - par - what this parameter does

@return
- Specifies what the method returns (when not void)
- Example: @return what this method returns
- Outputs two lines:
  - "Returns"
  - what this method returns

### Reading and Debugging Program Code

Assertion: precise statement about a program at any given time
- Example: what a program "has done" to that point
- Example: println and print provide evidence of line execution, variables provide computational thinking steps

Average Case of an Algorithm: runtime average as a central tendency value

Best Case of an Algorithm: least amount of successful runtime

Bottom-up vs. Top-Down Development
- Bottom-up Development: writing and testing simplest classes, or prototyping simple algorithm pieces
- Top-Down Development: starting with overall summary of whole program, or case studies (paper & pencil, GUI, pseudocode)

### Objects
Abstract Class
- Superclass
- Declared with keyword *abstract*
- May or may not have abstract methods

Abstract Method
- appears in abstract class or interface as placeholder
- no implementation code, only header
- implementation changes depending on inheritance

Accessor Method: "getter"
- Accesses class without altering object
- Publically facing method accessing private variable

Behaviour of Object: given by methods or groups of named code, void or returning

Class
- Blueprint of implementing objects
- State of object maintained by instance variables
- Behaviors of object described by methods

Client Program for a Class: accesses public methods

Compile-time error: during compilation of program before execution starts
- Examples:
  - undeclared variable
  - invoking method for instance object that does not have access
  - using incorrect parameter type

Composition Relationship between Classes: "has-a"
- Example: store has a item
- Note: if two classes have a composition relationship, one class contains and instance variable whose type is the other class

Constructor
- Used to create an object, block of code
- Always same name as class
- Different than method: no return type, cannot be invoked by direct method call
- Similar to method: can be overloaded

Driver Class
- Class with MAIN Method
- Used to prototype classes as they are developed

### Exceptions

Arithmetic Exception: runtime error thrown during division by zero

Array Index Out of Bounds Exception: runtime error thrown when programs tries to call index that is illegal (negative or greater-equal to size of array)

### General Coding

Arithmetic Operators: + - * / %

Boolean Expression: true or false

Compound Assignment Operator: += -= * = /= %=

Concatenation Operator: +

Decrement Operator: i-- or --i
- often used in loops


### Recursion

Base Case: termination condition
