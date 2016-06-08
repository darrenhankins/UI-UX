Monday, June 6, 2016
### An Object-Oriented Approach to Programming Logic and Design
#### Programming Logic and Design
###### Chapter 1
###### The overview of computers and logic

Instantiate the instance of a class

###### Objects
* Think object
  * Become the object, ask the question, what can I do?


* Objects Class (book)
  * Specialized Class (ie book, e-book, audiobook)

  1. Attributes (properties)
  2. Functions (behaviors)

---
######  * What objects for the project (keep them singular)

###### * Brewery object
    * name
    * location
    * name
    * established

###### * Beer object
    * Brewery
    * name
    * type of beer
    * color
    * origin
    * likes

###### * Customer object
    * name
    * email
---

###### Objectives

* understand computer components and operations
* Describe the steps involved in the programming Process
* describe the data hierarchy
* Understand how to use flowchart symbols and pseudocode statements
* Use and name variables
* Use a sentinel or dummy value
* Use a connector symbol

###### Hardware - equipment for devices

###### Software - instructions for the computer

  * input (keyboard, voice, gestures, etc)
  * processing
  * output (display, audio, vibration, light, print)
  * storage (persistent storage)

  * input devices
  * processing
  * CPU central processing unit

  * output devices
  * Programming languages
  * Syntax
  * Machine languages
  * compiler or interpreter

  * Free of syntax errors to execute
  * Logic must be correct to function correctly

  * Internal - RAM, volatile
  * External storage - persistent

  * Six Programming Phases
    1. Understand the problem
    2. plan the Logic
    3. Code the Programming
    4. Use software to translate the program to chine languages
    5. Test the program
    6. Deploy the program into production

  * Understanding the problem
    * may be the most difficult Phases
    * Users may not be able to articulate their needs well
    * User needs may be changing frequently
    * Programmers may have to learn the user's functional job tasks
    * Failure to understand the problem is the major cause of most project failures

###### Change Management Process
  * part of the contract
  * important part of the Iteration process


  * Planning the logic
    * steps the program will take
    * use flowcharts and pseudocode
      * Flowchart: a pictorial representation of the logical steps
      * Pseudocode: english-like representation of the logic
    * Walk through the logic before coding by `desk-checking` the logic

  * Coding the program
    * Select the programming languages
    * Write the instructions

  * Using software to translate the program into machine language:
    * Programmers write instructions in English-like high-level languages
    * Compilers or interpreters change the programs into low-level machine language that con be executed
    * Syntax errors are show my the interpreter

  * Testing the program
    * Execute it with sample data and check results
    * Identify logic errors and correct them
    * Choose text data carefully to exercise all branches of the logic

  * Putting the program into production
    * Do this after testing is complete and all know errors have been corrected
    * May require coordination with other related activities or software

#### * Understanding the Data hierarchy

  * Data hierarchy: ordering of data types by size
    * Character: single symbol (letter, number, special symbol)
    * Field: group of characters forming a single dat items
    * Record: a group of related fields
    * File: a group of related records
    * Database: collection of related files, called tables, that serve the information needs of the organization

###### Every C# app has to have a `main()` function (or `start`) and `return` (or `end` or `stop`) or it will not compile

* Input symbol

* Flow lines:
  * connect the steps
  * show the sequence of statements
  * have arrows to show the direction

* Terminal symbol (start/stop symbols)
  * shows the start and end points of the statements
  * lozenge shape

* back pointing arrows show statements that will be repeated

###### Using and Naming Variables
* C# is case sensitive
* Variable: a memory location whose contents can vary; also called an `identifier`

* Each programming language has it own rules for naming identifiers, including
  * Legal characters
  * Maximum length
  * Use of of upper or lower case

* Variable name must be a single work, but can be formed from several words
  * Examples: rate, `interestRate` (camel case naming convention), `interest_rate`, `InterestRate` (pascal or class name starts with capital letter)

  * Choose meaningful names for variables
    * Improves the readability and maintainability of code

  * Infinite Loop: sequence of statements that repeats forever with no escape
  * Avoid infinite loops by testing for a predetermined value that means "stop processing"
  * Decision: testinga value
  * Flowchart `decision symbol`: a `diamond`
  * Sentinel value (or dummy value)
    * doesn not represent real data
    * signal to stop
    * can be used with input from files or from Users
  * End-of-file (EOF) marker:
    * code stored in the file that marks the end of the data
    * Usually used instead do sentinel value for file input
* Flowchart connector symbol:
  * marks a logic transfer to another location in the flowchart
  * Transfer location can be on the sam page or on another page
  * On-page symbol: a circle with a number or letter to identify a new page
* Assignment statement:
  * assigns a value to the variables
  * variable must appear on the left side, value on the right side of the assignment operator
  * right side may be an expressions what will be evaluation before storing the value in the variables
* Assignment operator: the equal signal
* variable:
  * Memory location: has an address and a value
  * Value (contents) is used for variables
* Two types of data
  * text
  * numeric
* Numeric data is sorted by numeric variables
* Text data stored by string, text, or character variables
* Constraints
* Data types
  * `Integer`: whole numbers only
  * `Floating-point`: fractional numeric values with decimal points
  * Character or `string` data is represented as characters "X"
* Higher level languages were developed to allow English-like instructions
* Older programs were "monolithic" and ran from the beginning to the end
* Newer programs contain modules that can stand on there own

* Two types of programming (both are re-usable)
  * Procedural programming: procedures programmers create
  * Object-oriented programing (loosely coupled solution)
