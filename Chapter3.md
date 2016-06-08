Tuesday, June 7, 2016
### An Object-Oriented Approach to Programming Logic and Design
#### Programming Logic and Design
###### Chapter 3
###### Making Decisions

`Understand the question you are trying to resolve.`

###### * Objectives
  * Evaluate Boolean Expressions to make comparisons
  * Use the relational comparison operators
  * Understand `AND` Logic
  * Understand `OR` Logic
  * Use selection with ranges
  * Understand precedence when combining `AND` and `OR` selections
  * Understand the case structure
  * Use decision tables

Single-Alternative (or unary) selection structure

Dual-Alternative (or binary) selection structure
  * Also called an `if-then-else` structure
  * Boolean expressions
    * represents only on of two states
    * evaluates to either true or false
  * Expressions with relational operators produce Boolean results (true or false, 0 or 1)

  * Six possible ways to compare two values:
    * both are equal `==`
    * First greater than the second `>`
    * first is less than the second `<`
    * first is greater than or equal to second `>=`
    * first is less than or equal to the second `<=`
    * the tow values are not equal `!=` or `<>`

  * Any logical situation can be expressed with only three types of comparisons: `=`,`>` and `<`

  * Rule of thumb: ask the questions most likely to have a positive outcome first
  * Avoid `Not equal` when it results in a double negative
  * Rephrase in the positive
  * Requires that both of two tests evaluate to true
  * Requires a nested decision (nested if)
  * Developing the application
    * The input Data
    * The intended output
    * The mainline logic
  * For nested decisions, decide which to make first
  * An appropriate choice may improve performance
  * Consider expected outcomes to determine the most efficient way to nest the decisions

  * This analysis may not be possible
    * You may not know decision outcome likelihoods
    * The decisions may not be mutually exclusive
  * Rule of Thumb: First ask the question that is less likely to be true
    * Reduces the number of times the second question will need to be asked

  * Logical `AND` operators
    * Allows you to ask two or more questions (Boolean expressions)in a single comparison
  * Correct questions to determine inclusion in a range
  * `OR` decision
    * At least one has to be true for it to proceed
    * if first condition is true, no need to test the second condition

  * Writing OR Decisions for Efficiency
    * Both produce the same output, but vary widely in number of questions asked
    * If first question is true, no need to ask second
    * Rule of thumb:
      * First ask the question that is more likely to be true

  * Logical OR operators
    * Allows you to ask two or more questions (boolean expressions) in a single comparison
    * Only one Boolean expression in an OR selection must be true to produce a result of true
    * Question placed first will be asked first, so consider efficiency

  * Using Selections Within Ranges
    * Range check: compare a variable to a series of values between limits
    * Use the lowest or highest value in each range
    * Adjust the question logic when using highest versus lowest values
    * Should end points of the range be included

  * Common Errors Using Range Checks
    * Avoid dead or unreachable paths
      * Don't check for values that can never occur
      * Requires some prior knowledge of the data

  *  Avoid asking an un-needed question
    * If there is only on possible outcome
    * If previous logic has already determined the answer

  * Understanding Precedence when combining `AND` and `OR` Selections
    * Can combine multiple `AND` and `OR` operators in an expression
    * When multiple conditions must all be true, use multiple expression
    * When only one of the multiple conditions must be true, use multiple `OR`'s
    * When `AND` and `OR` operators are combined in the same statement, `AND` operators are evaluated first
    * Use parentheses to correct logic and force evaluations to occur in the order desired
    * Mixing `AND` and `OR` operators makes logic more complicated
    * Can avoid mixing `AND` and `OR` decisions by nesting `if` statements

  * Understanding the Case structure
    * Used to provide a series of alternatives based on the value of a single variable
    * Replaces a series of chained `if-else` statements
    * May make the code easier to read

######  * Using Decision Tables
    * Managing multiple possible outcomes to multiple decisions can be difficult
    * Decision table: four-part problem-analysis tool
      * Conditions
      * Possible combinations of Boolean values for each condition
      * Possible actions based on conditions
      * Specific actions that correspond to each boolean value of each condition (rules)

  * Developing the application
    * The Data

  * To create a decision table
    * List all possible conditions
    * Determine the possible boolean value combinations for each conditions
    * # combinations = 2 (number of conditions)
    * Add rows to list possible outcome actions
    * choose one required outcome for each combination
