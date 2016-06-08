# ui-ux

### Human Computer Interaction
Chapter 1,2

#### HCI involves the design, implementation and evaluation of interactive systems in the context of the user’s task and work.


* `Interaction` we mean any `communication between a user and computer`, be it direct or indirect.

* This outlines the three major issues of concern: `the people`, `the computers` and the `tasks that are performed`. The system must support the user’s task, which gives us a fourth focus, `usability`: if the system forces the user to adopt an unacceptable mode of work then it is not usable


1. `useful` – accomplish what is required: play music, cook dinner, format a document;
2. `usable` – do it easily and naturally, without danger of error, etc.;
3. `used` – make people want to use it, be attractive, engaging, fun, etc.


* HCI is required to be both a craft and a science in order to be successful.

`Law of size constancy` indicates that our perception of size relies on factors other than the visual angle


Factors
* our `perception of depth`
* `size and height` of the object in our field of view provides a cue to its distance
* `familiarity`: if we expect an object to be of a certain size then we can judge its distance accordingly

We tend to see the center of a page as being a little above the actual center – so if a page is arranged symmetrically around the actual center, we will see it as too low down. In graphic design this is known as the optical center

---

* Information I/O `- Visual, Aubitory, Haptic, Movment`

* Information Stored in Memory `- Sensory, Short-Term, Long-Term`

* Information Processed and Applied `- Reasoning, Problem Solving, Skill, Error`

---

### Memory
##### Three types of memory or memory function:
* `Sensory` Memory
  * `ionic` memory (`sight`)
  * `echoic` memory (`audio`)
  * `haptic` memory (`touch`)
* `Short-Term` Memory or `Working Memory` (attention)
  * scratch-pad
  * Continuouly Overwritten
  * `Chunking information` can increase the short-term memory capacity
  * The successful formation of a `chunk` is known as `closure`
  * `7+-2`
* `Long-Term` Memory (rehersal)

`Recency effect` - recall of the last words presented is better than recall of those in the middle

##### Long-Term Memory Structure
* `Episodic memory` represents our memory of events and experiences in a serial form
* `Semantic memory` is a structured record of facts, concepts and skills that we have acquired
* `Semantic network` is items that are associated to each other in classes, and may inherit attributes from parent classes

---
#### Reasoning
* `Deduction` - top down solution
  * Point first, follow up with evidence
* `Induction` - bottom up solution
  * Start with facts, finish with Point
* `Abduction` - reasons from a fact to the action or state that caused it

* ##### Emotion
  * Our emotional response to situations affects how we perform
  * A problem that may be easy to solve when we are relaxed, will become difficult if we are frustrated or afraid
  * So what are the implications of this for design?
    * It suggests that in situations of stress, people will be less able to cope with complex problem solving or managing difficult interfaces, whereas if people are relaxed they will be more forgiving of limitations in the design

---

#### Iteratory Process - Plan on Change

"You Cant Eat an Elephane All At Once,.. Small Bites"

"Extract Information => Time is Money, So Narrow Down the `What`"

"Think Time, Think, Money => It's Always an `Interview`"

#### `Scope`, `Quality`, `Time/Cost` => Project Management
  * "SQuaT"

  * "Scope creep => When You Diverge/Tangent Out of Scope"

---

##### Project

* How Does It Work?
  * Make It Personal (`You`)
  * "`You will` be able to doe this!"
  * Speak to one person
  * Condense
  * Don't talk yourself out of a connection
  * Connect and move on (don't tangent)

* ###### The Pitch
Speak to 4 ( HR - Director - 2 others)
  * Have `notebook` and `paper`
  * Write name and position under horizontally (know who everyone is)
  * Ask them if they have a question "Help me understand...?"
  * "I don't know, but I really like the question. I'd like to `ponder`/`comeback` to that question."
  * "Help me understand what you mean?"
  * "What's right about it?"
    * "I'm gonna make you blieve in it"
    * Assertive
    * Two way Interview
    * Sell and represent yourself

---

#### Interactive Design Basics (Ch 10)

  * Design `intervene` as opposed to `improve`
  * Design Process (what happens)
  * Users
  * Scenarios (stories of the design)
  * Navigation
  * Iteration and Prototypes
    * be careful of unrealistic expectations based on prototypes
    * usually don't show a lot until sign contracts
  * When speaking with client
    * What do you want?
      * I can solve this...

`Design` || Goals => Purpose || Constraints || Trade-offs

`Golden Rules` => Understand Materials || Computers || People || Their Interaction

`Process of Design`
  * What is wanted?
    * Analysis
    * Design
      * Protoype => Analysis
    * Implement/Deploy


    < Come back to this >

#### User Focus

    < more in between here

    come back to this >

  * 4 Golden Rules
      1. Where you are? (bread crumbs)
      2. What you can do?
      3. Where you're going?
      4. What you've done?


  * Basic Principles
    * Ask
    * Think
    * Design

---
Readings 1, 6, 10

---
Thursday, June 2nd

#### Javascript (Lesson 6)

###### Understanding JavaScript and Coding Essentials

* JavaScript provides action in applicacations
* On client side, Interactivity
* Dynamic application
* Expands opportunity to animate content

Alert Boxes
* Test operation of JS programs
* Generally not used in production code
* Ensures information is displayed to the user
* User has to click OK to close box

JS Statements
* Sequence of statements
* Statements seperated by semi-colons

Functions
* Segment of a program defined and performed in isolation from other parts
* A `function` returns a value
* Should do 1 thing and 1 thing only and does it well; well tested
* `Subroutines` are functions that return no value
* `Expression` doesn't perform any code withi the the function
* Source code is only definition of function
* When `function` is executed something useful happens
* Code can be in the `<head>` or seperate file

```html
<script type="text/javascript" src="path/filename.js" ></script>
```


* `Centralized Management` - Code in one place

Variables
* var syntex to define a Variables

Identifiers
* can't use names that JS uses such as`if`
* are names of variables and functions

Libraies
* collection of resources
* function code and Subroutines
* JS library is pre-written in JS

JQuery
* is leading JS library
* other popular libraries Dojo, MooTools, YUI
* can point to a centralized JS library

`getElementById()` method
* using DOM
* returns a ref to first object with specified `id` or `NAME` attribute

Methods
* always associated with and `object`
* uses DOM
* JavaScript functions that belong to an `object`
* `isNaN()` ex. test for "not a number"
* `document.getElementById()` ex. of a `method` with the special document `object`

Events
* `events` are actions that trigger and action to occur
* `event handler` is a optional script to execute that handles input received in a program
* a `callback` a response to an `event`, such as a script execution in response to a mouse click

`onLoad` Event Handler
* belongs to HTML items, it triggers when the owner is complete

```html
<!-- in <head> tag -->
<script>
function init() {
  alert("Page has loaded.");
}
</script>

<body onload="init();">

```

Flawd JS programs are erratic
* they give different results at different times
* Reasons Ex. hasn't completely loaded, launching  program at different times
* fix with `onload`

Showing and Hiding Elemetns
* The `HMTL` display attribute

```js
first_paragraph.style.display = display;

```
```js
oninput = "check_range()";
```

`innerHTML`
* changes the current content of `html`

```js
total_slot.innerHTML = total;
```



###### Book `HTML & CSS: Design and Build Websites`
---

Friday, June 3rd

#### Lesson 7
###### Creating Animation

Animation - changing a display to make it dynamic

Recursion - when a function calls itself
* timing element - javascript uses `setTimeout`

`createElement` method
* display an image when a button is clicked

Canvas element
* `getElementById()`
* `canvas.getContext` - creates canvas object

`XMLHttpRequest` - data transfer API
* allows JS to pass data in the form of text strings between a client and server

`open` method specifies the HTTP method

`xhr.send(data)` sned the data

parsing

---

Monday, June 6, 2016
#### Programming Logic and Design
###### Chapter 1

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

###### Every C# app has to have a `main()` function (or `start`) and `return` (or `end`) or it will not compile

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
