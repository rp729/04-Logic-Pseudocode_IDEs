# Exercise Workbench
* Design a While loop that lets the user enter a number. The number should be multiplied by 10, and the result stored in a variable named product. The loop should iterate as long as product contains a value less than 100.

```
//Declarations
Declare Integer product, number
Declare Constant Integer MAX_NUM = 10

//Main functin
Main()
   productMultiplier()
Return

//While loop multiplier
productMultiplier()
   set product = 0
   while product < 100
      Display "Enter a number."
      input number
      product += (number * MAX_NUM)
   end while
Return
```

* Design a Do-While loop that asks the user to enter two numbers. The numbers should be added and the sum displayed. The loop should ask the user whether he or she wishes to perform the operation again. If so, the loop should repeat; otherwise it should terminate.

```
//Declarations
Declare Real number1, number2, sum
Declare String keepGoing = "y"

//Main entry point of program
mainFunction()
   doWhileSum()
Return

//Do-While loop to find sum
doWhileSum()
   while keepGoing == "y" or "Y"
      Display "Enter a number."
      input number1
      Display "Enter another number."
      input number2
      set sum = number1 + number2
      outpout "The sum of the numbers you entered is ",sum
      Display "Would you like to continue? (Y to conintue)"
      input keepGoing
   End while
Return
```


* Design a For loop that displays the following set of numbers:

0, 10, 20, 30, 40, 50, . . . , 1000

```
//Declarations
Declare Integer num = 0

//Main Entry Point
main()
   forLoop()
Return

//Loop repeats 101 times to reflect 0-1000
forLoop()
   for number in range(101)
      Display num
      num += 10
   end for
```

* Design a loop that asks the user to enter a number. The loop should iterate 10 times and keep a running total of the numbers entered.

```
//Declerations
Declare Integer number
Declare Integer total = 0

//Main Entry Point
main()
   forLoop10Times()
Return

forLoop10Times()
   for num in range(10)
      Display "Enter a number."
      input number
      total += number
      Output "The total of the number you have entered is ", total
   End for
Return
```

* Design a For loop that calculates the total of the following series of numbers:
![image](https://user-images.githubusercontent.com/47218880/67423054-31740800-f599-11e9-9565-031c1f729e1c.png)

```
//Declarations
Declare Integer denominator = 30
Declare Integer numerator = 1
Declare Real divide, total

//Main Entry Point
main()
   fractionTotal()
Return

//Finds total of fractions but converts to decimal
fractionTotal()
   for number in range(30)
      set divide = numerator/denominator
      total += divide
      denominator -= 1
      numerator += 1
   End for
Return
```

* Design a nested loop that displays 10 rows of # characters. There should be 15 # characters in each row.

```
for i in range(10)
   Display "#############"
End for
```

* Convert the While loop in the following code to a Do-While loop:
```
Declare Integer x = 1
While x > 0
   Display "Enter a number."
   Input x
End While
```

```
Declare Integer x

Do
   //Prompt the user to enter a number
   Display "Enter a number."
   input x

   //Display error message if x > 0
   If x > 0 then
      Display "Sorry, try again"
   End if
While x > 0

//Indicate that x is equal to or less than 0
Display "Number is equal to or less than 0"

```

* Convert the Do-While loop in the following code to a While loop:
```
Declare String sure
Do
  Display "Are you sure you want to quit?"
  Input sure
While sure != "Y" AND sure != "y"
```

```
Declare String sure = "n"

//Ask user if they would like to quit
While sure != "y" or sure !+ "Y"
   Display "Would you like to quit?"
   input sure
End while
```

* Convert the following While loop to a For loop:
```
Declare Integer count = 0
While count < 50
   Display "The count is ", count
   Set count = count + 1
End While
```
```
Declare Integer count = 0

For x in range(50)
   count += 1
End for
```


* Convert the following For loop to a While loop:
```
Declare Integer count
For count = 1 To 50
   Display count
End For
```
```
Declare Integer count = 0

While count < 50
   count += 1
End while
```