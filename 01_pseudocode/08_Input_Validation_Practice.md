# Input Validation Exercise Workbench

Design an algorithm that prompts the user to enter a positive nonzero number and validates the input.

```
//Declaration
Declare Real nonZero

//Prompt User to Enter Number
Display "Enter a positive nonzero number"
input nonZero

//Call on function for input validation
Call inputValidation(nonZero)

//Input validation function
Function String inputValidation(Real userInput)
   if userInput > 0 then
      Return 
   Else
      While userInput <= 0
         Display userInput," is not a positive nonzero number"
         input userInput
End Function
```

Design an algorithm that prompts the user to enter a number in the range of 1 through 100 and validates the input.

```
//Declaration
Declare Real num

//Prompt User to Enter Number
Display "Enter a number between 1 and 100."
input num

//Call on function for input validation
Call inputValidation(num)

//Input validation function
Function String inputValidation(Real userInput)
   if userInput >= 1 and userInput <= 100 then
      Return userInput,"is a valid number"
   Else
      Return userInput," is not a valid number."
End Function
```

Design an algorithm that prompts the user to enter “yes” or “no” and validates the input. (Use a case-insensitive comparison.)

```
//Declaration
Declare string yes = 'yes'
Declare string no = 'no'
Declare string response

//Call on function for input validation
Call inputValidation(response)

//Where the magic happens
Function String inputValidation(response)
   Display "Please type yes or no"
   input response
   if response == toLower(yes) or response == toLower(no) then
      return "Valid response given."
   else
      return "Invalid response given."
```

Design an algorithm that prompts the user to enter a number that is greater than 99 and validates the input.

```
//Declaration
Declare Real greaterThan99

//Prompt User to Enter Number
Display "Enter a positive nonzero number"
input nonZero

//Call on function for input validation
Call inputValidation(nonZero)

//Input validation function
Function String inputValidation(Real userInput)
   if userInput > 0 then
      Return userInput,"is a positive number"
   Else
      Return userInput," is not a positive nonzero"
End Function
```

Design an algorithm that prompts the user to enter a secret word. The secret word should be at least 8 characters long. Validate the input.

# Debugging Exercises

Why does the following pseudocode not perform as indicated in the comments?
```
// This program asks the user to enter a value
// between 1 and 10 and validates the input.
Declare Integer value

// Get a value from the user.
Display "Enter a value between 1 and 10."
Input value

// Make sure the value is between 1 and 10.
While value < 1 AND value > 10
   Display "ERROR: The value must be between 1 and 10."
   Display "Enter a value between 1 and 10."
   Input value
End While
```
Why does the following pseudocode not perform as indicated in the comments?
```
// This program gets a dollar amount from the user
// and validates the input.
Declare Real amount

// Get the amount from the user.
Display "Enter a dollar amount"
Input amount

// Make sure the amount is not less than zero. If it is,
// get a new amount from the user.
While amount < 0
   Display "ERROR: The dollar amount cannot be less than 0."
   Display "Enter a dollar amount."
End While
```
The following pseudocode works, but it performs a case-sensitive validation of the user’s input. How could the algorithm be improved so the user does not have to pay attention to capitalization when entering a name?
```
// This program asks the user to enter a string
// and validates the input.
Declare String choice

// Get the user's response.
Display "Cast your vote for Chess Team Captain."
Display "Would you like to nominate Lisa or Tim?"
Input choice

// Validate the input.
While choice != "Lisa" AND choice != "Tim"
   Display "Please enter Lisa or Tim."
   Display "Cast your vote for Chess Team Captain."
   Display "Would you like to nominate Lisa or Tim?"
   Input response
End While
```