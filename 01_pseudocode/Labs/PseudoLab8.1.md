# Choose Two additional Programming Projects along with the (Mandatory) one. (Three Total) 

##  Payroll Program with Input Validation


Design a payroll program that prompts the user to enter an employee’s hourly pay rate and the number of hours worked. Validate the user’s input so that only pay rates in the range of $7.50 through $18.25 and hours in the range of 0 through 40 are accepted. The program should display the employee’s gross pay.

```
//Declarations
Declare Real hourlyPayRate, hoursWorked

//User input
Display "Enter your hourly pay rate."
input hourlyPayRate
Display "Enter the number of hours worked."
input hoursWorked

//Call on function
Call inputValidation(hourlyPayRate, hoursWorked)

//Input validation
Function String inputValidation(hourlyPayRate,hoursWorked)
	While hourlyPayRate < 7.5 or hourlyPayRate > 18.25
		Display "Your hourly pay rate is invalid. Try again."
		input hourlyPayRate
	End While
	While hoursWorked < 0 or hoursWorked > 40
		Display "Number of hours worked is invalid. Try again"
		input hoursWorked
	End while
	return hourlyPayRate, hoursWorked
End Function
```

## Theater Seating Revenue with Input Validation

A dramatic theater has three seating sections, and it charges the following prices for tickets in each section: section A seats cost $20 each, section B seats cost $15 each, and section C seats cost $10 each. The theater has 300 seats in section A, 500 seats in section B, and 200 seats in section C. Design a program that asks for the number of tickets sold in each section and then displays the amount of income generated from ticket sales. The program should validate the numbers that are entered for each section.

```
//Declarations
Declare Integer sectionA, sectionB, sectionC

//User input
Display "Enter number of tickets sold for section A."
input sectionA
Display "Enter number of tickets sold for section B."
input sectionB
Display "Enter number of tickets sold for section C."
input sectionC

//User input validation
Call inputValidation(sectionA, sectionB, sectionC)

//Display amount of tickets sold
Display F"Section A sold {sectionA} amount of tickets"
Display F"Section B sold {sectionB} amount of tickets"
Display F"Section C sold {sectionC} amount of tickets"

//Calculate total sales
set sectionA = sectionA * 20
Display F"Section A made ${sectionA}"
set sectionB = sectionB * 15
Display F"Section B made ${sectionB}"
set sectionC = sectionC * 10
Display F"Section C made ${sectionC}"
Display "For a grand total of $"{sectionA+sectionB+sectionC}"

//User input validation.
Function inputValidation(sectionA, sectionB, sectionC)
	while sectionA < 0 or sectionA > 300
		Display "Invalid input, Section A has 300 seats."
		input sectionA
	while sectionB < 0 or sectionB > 500
		Display "Invalid input, Section B has 500 seats."
		input sectionB
	while sectionC < 0 or sectionC > 200
		Display "Invalid input, Section C has 200 seats."
		input sectionC
	End while
	return sectionA, sectionB, sectionC
End function	
```

## Fat Gram Calculator

Design a program that asks for the number of fat grams and calories in a food item. Validate the input as follows:

Make sure the number of fat grams and calories is not less than 0.

According to nutritional formulas, the number of calories cannot exceed "fat grams X 9 "

Make sure that the number of calories entered is not greater than "fat grams X 9"

Once correct data has been entered, the program should calculate and display the percentage of calories that come from fat. Use the following formula:

![image](https://user-images.githubusercontent.com/47218880/67504468-0ba93a80-f64f-11e9-85d0-f080ac66a64a.png)

Some nutritionists classify a food as “low fat” if less than 30 percent of its calories come from fat. If the results of this formula are less than 0.3, the program should display a message indicating the food is low in fat.

```
//Declarations
Declare Integer fatGrams, calories, calPercent
Declare Constant Integer FAT_TO_CAL = 9

//Ask for user input
Display "Enter number of grams of fat."
input fatGrams
Display "Enter number of calories."
input calories

//Validate user input
Call inputValidation(fatGrams, calories)

//Calculate percentage of calories from fat
set calPercent = (fatGrams * FAT_TO_CAL)/calories
If calPercent < 0.3 then
	Display "low fat"
Else
	Display "Not low fat"

//User input validation function
Function String inputValidation(fatGrams, calories)
	While fatGrams < 0
		Display "Grams of fat cannot be a negative number."
		input fatGrams
	While calories < 0 and > fatGrams * FAT_TO_CAL
		Display "Invalid number of calories"
		input fatGrams
	End while
	return fatGrams, calories
```

## Speeding Violation Calculator

Design a program that calculates and displays the number of miles per hour over the speed limit that a speeding driver was doing. The program should ask for the speed limit and the driver’s speed. Validate the input as follows:

The speed limit should be at least 20, but not greater than 70.

The driver’s speed should be at least the value entered for the speed limit ­(otherwise the driver was not speeding).
Once correct data has been entered, the program should calculate and display the number of miles per hour over the speed limit that the driver was doing.

```
//Declarations
Declare Integer speedLimit, driverSpeed, speedOver

//Prompt for user input
Display "Enter the speed limit."
input speedLimit
Display "Enter the speed of the driver."
input driverSpeed

//Check input validation
Call inputValidation(speedLimit, driverSpeed)

//Calculate the number of MPH over the driver was going
set speedOver = driverSpeed - speedLimit
Display F"The driver was driving {speedOver} MPH over the speed limit."

//User input validation function
Function String inputValidation(speedLimit,driverSpeed)
	While speedLimit < 20 or > 70
		Display "Invalid speed limit"
		input speedLimit
	While driverSpeed <= speedLimit
		Display "Driver was not speeding. Try again."
		input driverSpeed
	End while
	return speedLimit, driverSpeed
```

# Rock, Paper, Scissors Modification (MANDATORY)

In a previous Programming Exercise option you were asked to design a program that plays the Rock, Paper, Scissors game. In the program, the user enters one of the three strings—"rock", "paper", or "scissors"—at the keyboard. Add input validation (with a case-insensitive comparison) to make sure the user enters one of those strings only.
(If you didnt design one, here is a version of that game program to work with) 

### Program "Rock,Paper,Scissors"

```
// main module
Module main()
// Local variables
Declare Integer computer, player

// Get computer number
Set computer = Rand(1, 3)

// Get player number
Call getNumber(player)

// Show winner
Call showWinner(computer, player)

End Module


// The getNumber module gets an integer
Module getNumber(Integer Ref inputAnswer)
		Display “Enter 1 for rock, 2 for paper, 3 for scissors:  “
		Input inputAnswer
		Call inputValidation(inputAnswer)
		return inputAnswer
End Module


// The showWinner module shows if number is a prime
Module showWinner(Integer computer, player)
Declare Integer which

Display “Computer chose “, whichChoice(computer)
If computer == player Then
	Display “Player made same choice.  Play again.”
Else
Set which = whoWon(computer, player)
If which == 1 Then
		Display “Computer wins.”
Else
If which == 2 Then
			Display “Player wins.”
		Else
			Display “No winner.”
		End If
End If
End If

End Module

// The whichChoice function displays choice 
Function String whichChoice (Integer number)

If number == 1 Then
	Return “rock”
Else
If number == 2 Then
		Return “paper”
	Else
		Return “scissors
	End If

End Function

// The whoWon function selects winner 
Function Integer whoWon(computer, player)
// 1 = rock, 2 = paper, 3 = scissors
// rock smashes scissors
// scissors cuts paper
// paper wraps rock

	// both choose same no winner
If computer == player then
		Return 0
	End If

	// test computer chose rock
	If computer == 1 then
		If player == 2 then
			Return 2  // paper wraps rock
		End If
Else
		If player == 3 then
			Return 1  // rock smashes scissors
		End If
End If

	// test computer chose paper
	If computer == 2 then
		If player == 1 then
			Return 1  // paper wraps rock
		End If
Else
		If player == 3 then
			Return 2  // scissors cuts paper
		End If
End If

	// test computer chose scissors
	If computer == 3 then
		If player == 1 then
			Return 2  // rock smashes scissors 
		End If
Else
		If player == 2 then
			Return 1  // scissors cuts paper
		End If
End If

	Return 0

End Function


//User Input Validation
Module inputValidation(Integer inputAnswer)
	While inputAnswer != 1 and inputAnswer != 2 and inputAnswer != 3
		Display "Input is invlaid. Try again."
		input inputAnswer
	End while
	return inputAnswer
End function
```
