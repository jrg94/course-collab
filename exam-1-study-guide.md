# Exam 1 Collaborative Study Guide

The following document was created for and by the students of Jeremy
Grifski's section of CSE 2221 in Autumn 2021. 

## Resources

As a class, we brainstormed the following lists of resources.

**Slides**

- [Java Overview Powerpoint](http://web.cse.ohio-state.edu/software/2221/web-sw1/extras/slides/02.Java-Overview.pdf)
- [Output, Strings, Input Powerpoint](http://web.cse.ohio-state.edu/software/2221/web-sw1/extras/slides/03.Output-Strings-Input.pdf)
- [Variables, Types, and Values Powerpoint](http://web.cse.ohio-state.edu/software/2221/web-sw1/extras/slides/04.Variables-Types-Values.pdf)
- [Operators, Expressions, Statements Control Flows Slides](http://web.cse.ohio-state.edu/software/2221/web-sw1/extras/slides/05.Operators-Expressions-Statements-Control-Flow.pdf)
- [Static Methods Powerpoint](http://web.cse.ohio-state.edu/software/2221/web-sw1/extras/slides/06.Static-Methods.pdf)
- [While Loops Slides](http://web.cse.ohio-state.edu/software/2221/web-sw1/extras/slides/06a.While-Loops.pdf)
- [Parameter Passing](http://web.cse.ohio-state.edu/software/2221/web-sw1/extras/slides/07.Parameter-Passing.pdf)

**Readings**

- [Java For Everyone - Chapter 1: Introduction](https://library.ohio-state.edu/record=b9159294~S8)
- Textbook Java for Everyone Chapter 2: Fundamental Data Types
- Java for Everyone - Chapter 3: Decisions
- Java for Everyone - Chapter 4: Loops
- Textbook Java for Everyone Chapter 6: Arrays and Array Lists

**Homeworks**

- [Static Methods](http://web.cse.ohio-state.edu/software/2221/web-sw1/assignments/homeworks/methods.html)

**Labs**

- Monte Carlo Lab
- Hailstone Lab

**APIs**

- [SimpleReader API](http://web.cse.ohio-state.edu/software/common/doc/components/simplereader/package-summary.html)
- [SimpleWriter API](http://web.cse.ohio-state.edu/software/common/doc/components/simplewriter/package-summary.html)

**Misc**

- [Oracle Java Documentation](https://docs.oracle.com/javase/8/docs/api/overview-summary.html)
- https://www.w3schools.com/java/java_variables.asp
- https://www.freecodecamp.org/news/data-types-in-java/
- https://www.w3schools.com/java/.java_data_types.asp
- Java Tutorials: Home Page > Learning the Java Language > Language Basics > Operators
- Java Tutorials: Home Page > Learning the Java Language > Language Basics > Expressions, Statements, and Blocks
- Java Tutorials: Home Page > Learning the Java Language > Language Basics > Control Flow Statements

## Frequently Asked Questions

As a class, we brainstormed the following list of frequently asked questions.

**How is Java executed?**

Java is executed on the JVM

**What is the JVM?**

The JVM is a virtual computer that runs on an operating system (its own computer that runs on the computer)

**What is an algorithm?**

A series of steps that a computer follows to complete a problem

**What are the benefits of the JVM?**

- Portability (allows same program to be run on different machines)
- Safety
- Easy to read

**What kind of programming language is Java?**

General purpose, imperative, object-oriented.

**What are the two types of errors?**

- Run-time
- Compile-time

**How to do output?**

```java
import components.simplewriter.SimpleWriter; // (and 1L)
SimpleWriter out = new SimpleWriter1L();
out.println(“”);
out.close();
```

**How to do input?**

```java
import components.simplereader.SimpleReader; // (and 1L)
SimpleReader in = new SimpleReader1L();
variable = in.nextDatatype();
in.close();
```

**What is a variable?**

A variable is the name of a “location” that “stores” a value of a particular type.

**What are the primitive types?**

- byte: stores whole numbers from -128 to 127
- short: stores whole numbers from -32,768 to 32,767
- int: stores whole numbers from -2,147,483,648 to 2,147,483,647
- long: stores whole numbers from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807
- float: stores fractional numbers. Sufficient for storing 6 to 7 decimal digits
- double: stores fractional numbers. Sufficient for storing 15 decimal digits
- boolean: stores true or false values
- char: stores a single character/letter or ASCII values

**What is a literal?**

A literal is a data value that is literally in a program. An example of this would 
be that “false” would be a literal in regards to a Boolean. 

**What is a constant?**

A Constant is a variable whose value is initialized and never changed. This is
implemented within code by inserting a “final” before you initialize the variable.

**What is the difference between a program variable and a mathematical variable?**

A Program Variable has a particular value at any one point during program execution,
and that value may be subject to change. A Mathematical Variable stands for an 
arbitrary but fixed value.

**What is the difference between a primitive type and a reference type?**

Primitives are a data type that only specify the size and type of a variable, 
and nothing else. Non-Primitive Types, or Reference Types are types that can 
be created by the programmer and can perform multiple call methods and can be 
null. Primitives start with lowercase while Reference types start with uppercase.

**What are examples of reference types in Java?**

String, Arrays, Classes, Interface, etc.

**What is the first index in an array?**

0

**What are some properties of arrays?**

- Size of arrays can’t be changed once declared.
- Arrays can contain arrays
- Arrays can store primitive types or objects
- Easy and fast to access every element in an array

**How can we declare an array literal?**

```java
int[]  arr = {0, 1, 2, 3, 4};
```

**How can we iterate over an array?**

```java
for (double element: values) {…}
```

**What is an operator? What mathematical functions can be used in Java?**

An operator is symbol (or combination of a couple symbols) that is used with 
variables and value to simplify how you write certain program expressions.

**What is an expression? Where do they appear?**

A “syntactically well formed and meaningful fragment” (roughly analogous to a 
word in natural language. Examples include the following:

- i
- j+7
- “Hello” + “World!”
- keyboardIn.nextLine()		
- n==0;
- new SimpleWriter1L()

**What is a statement?**

A “smallest complete unit of execution” — which can be a complete unit of 
manipulation, terminated by semicolon ‘ ; ’.

**What is the difference between an expression and a statement?**

A statement can contain expressions. The expression is some procedure of 
calculation but a statement is a complete unit in a program. 

**How can statements vary from each other?**

TBD

**What is the appropriate way to compare strings?**

Best Practice: do not use == or != with strings. Use “equals” method.

**What is the best way to compare doubles?**

Best Practice: do not check doubles for equality

**What are the most common operators?**

| string | boolean | char            | int             | double |
| ------ | ------- | --------------- | --------------- | ------ |
|        | !       |                 | ++ --           |        |
| +      | \|\|    |                 | + -             | + -    |
|        | &&      |                 | * / %           | * /    |
|        | == !=   | < > <= >= == != | < > <= >= == != | < >    |

**What is control flow?**

Change the flow of execution by adding conditional statements such as 
if/if-else/switch and/or loops.

**What are if statements?**

Executes certain sections of code only if the particular test evaluates to 
true or false.

**What is a while loop?**

Executes a body of code for as long as the condition statement is true.

**What is a for loop?**

A loop used when a body of code needs to be executed for a known number of times.

**What is object-oriented programming?**

A programming which is based on “objects”, like a combination of data and code.

**What does the ‘static’ modifier do in a static method?**

TBD

**Where should you use a static method?**

A static method should be used where object information does not matter. If a method will always give the same outputs for given input parameters, it should be a static method.

**What is the difference between a public and private method?**

TBD

**How do variables created within methods interact with the rest of the code (outside the method)?**

TBD
