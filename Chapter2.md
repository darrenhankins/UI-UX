Monday, June 6, 2016
### An Object-Oriented Approach to Programming Logic and Design
#### Programming Logic and Design
###### Chapter 2
###### Understanding Structure

Objectives
* The 3 Structures
* `sequence`, `selection`, and `loop`
* Each structure has on entry and one exit points
* Structures attach to others only at entry or exit points

* Spaghetti Code - all over the place, no logic and design
  * difficult to read and maintain
  * convoluted logic usually is hard to

* Structure: basic unit of programming logic
* `Sequence`, `selection`, `loop`
  * can be combined by stacking and Nesting
  * one way in, one way out

* Sequence Structure
  * Ask a question, then takes on of two possible courses of action based on the answer

* Dual-alternative if: contains two alternatives
* Single-alternative if: contains on operations

* Loop Structure
  * repeats a set of actions based on the answer to a question
  * also called repetition or Iteration
  * question is asked first in the most common form of Loop
  * `do` will run at least once, checked at end of code (post test loop)
  * `while` may not run, checked at beginning of code (pre test loop)

* All logic problems can be solved using only these three structures
* Structures can be combines in a infinite number of ways
* Stacking: attaching structures end-to-end

* Any individual task or step in a structure can be replaced by a structures
* Nesting: Placing one structure within another
* Indent the nested structure
* Block: group of statements that execute as a block of code

* Priming read (or priming input):
  * Read the first input data record
  * outside the loop that reads the rest of the records
  * Helps Keep the program structured
* Analyze a flowchart for structure on step at a time

* Priming read sets up the process so the loop can be structured
* To analyze a flowchart's structure, try writing pseudocode for it

* case, do-while, do-until structure
* case structure:
  * Decisions with more than two alternatives
  * Tests a variable against a series of values and takes action based on a match

* `do-while` and `do-until` loops
  * question is asked at the end of the loop structure
  * runs at least once
