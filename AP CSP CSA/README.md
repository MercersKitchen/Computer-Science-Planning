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
- Reading and Debugging Program Code
- Objects
- Exceptions
- General Coding
- Recursion
<a href=""></a>

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

Logic Error (same as Intent Error): program compiles and fails to run as programmer intended



Intent Error (same as Logic Error): program compiles and fails to run as programmer intended

Main Method
- Type: public static
- Returns: void
- Controls entire program execution
- Note: all Java programs must have at least one class with a MAIN Method

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

#### Dynamic Binding (Late Binding)
- Closely related to polymorphism, <a href="https://github.com/MercersKitchen/Computer-Science-Planning/tree/master/AP%20CSP%20CSA#polymorphism">click here to jump to Polymorphism</a>
- Overridden method called during runtime (not compile time) depending on instantiated object
- Example:
  - abstract student class has subclasses of Undergrad and GradStudent
  - when Student Object is processed, appropriate computeGrade method invoked depending on subclass

Encapsulation: grouping variables & methods (data & behaviours) within class and hiding these with private-keyword from other classes
- Accessor methods used (getters) and setters
- See "Information Hiding"

Final Variable: user-defined constant using keyword final

Immutable Object: object without mutator methods (changing data of object)
- String Object is immutable by definition
- Copy of String Object, as new-keyword String can be mutated form of existing String Object
- BEWARE: copying data as new-keyword creates memories or replicas of immutable objects as specific times of computation

Information Hiding: declaring instance variables and helper methods private-keyword to prevent access from client classes

Inheritance: mechanism using super and sub classes to influence variables and methods (state and behavior)
- tested with "is-a" relationship

Interface (superclass)
- declared by keyword interface
- collection of related methods (abstract, headers only, or default, AP subset omits default)
- cannot be instantiated
- Example: Flyer
  - isFlying, isBird
  - Implemented by Airplane, Hawk

Keyword: reserved word used for language and compiler

Method Overriding
- In superclass, public method is rewritten in subclass
- Subclass method has same return type and signature (name and parameters)
- Rewritten with different code

Mutator Method: modifies instance variable, prefix "set" (i.e. setRate, setPrice)

Object: single instance of a class (group of variables in constructor)

#### Overloaded Methods: methods with same name but different signatures (headers and parameters), within class or subclass
- Examples
  - `public int product (int n) //returns int n*n`
  - `public int product (int x * int y) //returns int x*y`
  - `public double product (int n, double y) //returns double n*y`

#### Polymorphism
- Closely related to Dynamic Binding, <a href="https://github.com/MercersKitchen/Computer-Science-Planning/tree/master/AP%20CSP%20CSA#dynamic-binding-late-binding">click here to jump to Dynamic Binding</a>
- Mechanism for selecting correct <a href="">overridden method</a>

### Exceptions
- Runtime errors interrupting normal flow and provides useful error message when exception is thrown

Arithmetic Exception: division by zero

Array Index Out of Bounds Exception: programs tries to call index that is illegal (negative or greater-equal to size of array)

Illegal Argument Exception: thrown when data (arguments) do not match formal parameters

Index Out of Bounds Exception: index of array, arrayList, String, etc. is out of range of data

Null Pointer Exception: when a program attempts to access or modify a variable that is currently NULL



### General Coding

Arithmetic Operators: + - * / %
- Floating Point: returns real-number (floating point or decimal)
  - if one number or variable is float or double
  - if one number or variable is cast as float or double
  - Beware Example:
    - 3 / (double) 4  //returns 0.75
    - (double) 3 / 4  //returns 0.0 since integer division is computed first, then real-number cast

Boolean Expression: true or false

Compound Assignment Operator: += -= * = /= %=

Concatenation Operator: +

Decrement Operator: i-- or --i, often used in loops

Enhanced FOR Loop: for-each loop used to read and write arrays

Escape Sequences: mostly used in println and print
- Examples: \n, \t, \", \\,

Formal Parameters: defined in header of method OR defined in function
- Example: public void setPerson (String name, int age)

Increment Operator: i++ or ++i, often used in loops

Integer Division: a/b, returns truncated integer quotient (i.e. 1/3=0)

Logical Operator: AND(&&), NOT(!), OR(||), returns Boolean result

Nested IF equivalent to AND: IF within IF meaning both IF must be TRUE

Nested Loop: counting in multiple variables and patters



### Recursion

Base Case: termination condition
