Wednesday, June 8, 2016
### An Object-Oriented Approach to Programming Logic and Design
#### Programming Logic and Design
###### Lesson 1
###### Understanding Programming

* Algorithms
  * Logical Methods for solving problems
  * A `flowchart` is a graphical representation of an algorithm
    * 5 symbols
        * start (round-corner-square)
        * process (square)
        * input/output (skew)
        * decision making (diamond)
        * flow (arrow)


* Decision Table
  * Useful for large numbers of conditions
  * compact and readable format


* Introducing C# (c-sharp)
  * Microsoft .NET Framework
    * An Execution Environment
    * Reusable Class Libraries
    * Language Compilers


  * The C# Programming Language
    * Part of the .NET Framework
    * High-Level Language (readable code)
    * Program needs to be compiled before they can be executed
    * Case sensitive

###### `Note: Pick one language to master`


  * Structure of a C# Program
    ```csharp
    using System; // library
    namespace Lesson1
    {
      class Program
      {
        static void Main(string[] args)
        {
          Console.WriteLine("hello, world!");
        }
      }
    }

    ```


  * Common elements
    * `Data types` - int, char, float
    * `Variables` - provides temp storage
    * `Constants` - data fields that cannot be modified
    * `Arrays` - collection of items accessed by a unique index
      * `int[] numbers ={1,2,3};`
      * zero start count
    * `Operators` - symbols that specify which operation to perform on operands before returning a result (sub, add, div, mult)
    * `Methods` - code block containing a series of statements. Method can receive input via arguments and can return a value to the caller

`Note: Difference between a function and procedure. A function returns a value`


  * Decision Structures
    * The `if` statements
    * The `if-else` statements
    * The `switch` statement (`case` statement) avoids lengthy if-else nesting

  * `if`
  * `if-else` statement allows your program to perform one action if the Boolean expression evaluates to true and a different action if the Boolean expression evaluates to false
  * `switch` statement allows multi-way branching. In many cases, using a switch statement can simplify a complete combination of if-else statements

  ```csharp
  string firstName = "Darren";
  string lastName = "Hankins";

  Console.WriteLine("First Name: {0} Last Name: {1}", firstName, lastName);

  // {0} and {1} are placeholders

  ```
  ```csharp
  switch (opr)
  {
      case '+':
        result = op1 + op2;
        break;

      case '-':
        result = op1 - op2;
        break;

      default:
        Console.WriteLine("Result = {0}", result);
        return;

  }
  ```

* Repetition Structures
  * The `while` Loop - repeatedly executes a block of statements until a specified Boolean expression evaluates to false
  * the `do-while` Loop - repeatedly executes a block of statements
  * the `for` Loop - combines 3 elements of iteration - the initialization expression, the termination condition expression, and the counting expression - a more readable code
  * the `foreach` Loop - enhanced version of the for loop for iterating through collections such as arrays and lists (objects)
  * recursion - causes a method (function) to call itself in order to compute a result


* Exception Handling
  * an unexpected error condition that occurs during program execution
  * When the exception occurs, the runtime creates an exception object and `throws` it
  * Unless you `catch` the exception, the program execution will terminate
  * Exceptions are an `object` of the `System.Exception` class or on of its derived classes
    * Example: `DivideByZeroException` exception object is thrown when the program attempts to divide by zero
    * Example: `FileNotFoundException` exception object is throws when the program cannot find a given file
  * Place the code that throws the exceptions inside a `try` block
  * Place the code that handles an exception inside a `catch` block
  * You can have more than one `catch` blocks for each `try` block. Each `catch` block handles a specific exception type
  * A `try` block must have at least a `catch` block or a `finally` block associated with it


  `Note: NULL value is "unknown" null != null`


* The `finally` block
  * The finally block is used in association with the try block
  * The finally block is always executed regardless of whether an exception is thrown
  * The finally block is often used to write clean-up code


`Note: "catch" provides the feedback to user, "Exception" is always the last "catch" in your "catch" items, a default`


```csharp
try
{
  sr = File.OpenText(@"c:\data.txt");
  Console.WriteLine(sr.ReadToEnd());
}

catch (SomeOtherExecption fnfe)
{
  Console.WriteLine(fnfe.Message);
}
// `Exception` catch is always last
// This is the `catch all` catch
catch (Exception ex)
{
  Console.WriteLine(ex.Message);
}

finally
{
  if (sr != null)
  {
    sr.Close(0;)
  }
}

```


* VisualStudio (MS) - app development environment
* SharePoint (MS) - develop project management software
