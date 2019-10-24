1. As shown in this chapter, write a pseudocode statement that generates a random number in the range of 1 through 100 and assigns it to a variable named rand.

```
set rand = random(1,100)
```

2. The following pseudocode statement calls a function named half, which returns a value that is half that of the argument. (Assume both the result and number variables are Real.) Write pseudocode for the function.
Set result = half(number)

```
Declare Real result,number

Function Real half(Real num)
    return num/2
End Function

```

3. A pseudocode program contains the following function definition:
	Function Integer cube(Integer num)
   Return num * num * num
End Function
Write a statement that passes the value 4 to this function and assigns its return value to the variable result.

```
Set result = cube(4)
```

4. Design a pseudocode function named timesTen that accepts an Integer argument. When the function is called, it should return the value of its argument multiplied times 10.

```
Function Integer timesTen(Integer num)
    return num*10
End function
```

5. Design a pseudocode function named getFirstName that asks the user to enter his or her first name, and returns it.

```
Function String getFirstName()
    Declare String firstName
    Display "Enter first name"
    input firstName
    return firstName
End Function
```

6. Assume that a program has two String variables named str1 and str2. Write a pseudocode statement that assigns an all uppercase version of str1 to the str2 variable.

```
Set str2 = toUpper(str1)
```

Debugging Exercises
The programmer intends for this pseudocode to display three random numbers in the range of 1 through 7. According to the way we’ve been generating random numbers in this book, however, there appears to be an error. Can you find it?
    1. // This program displays three random numbers
    2. // in the range of 1 through 7.
    3. Declare Integer count
    4. 
    5. // Display three random numbers.
    6. For count = 1 To 3
    7.    Display random(7, 1)
End For

```
// This program displays three random numbers
// in the range of 1 through 7.
Declare Integer count, number

//Display 3 random numbers
For count = 1 to 3
    set number = random(1,7)
    Display number
End for

```

Can you find the reason that the following pseudocode function does not return the value indicated in the comments?
    8. // The calcDiscountPrice function accepts an item's price and
    9. // the discount percentage as arguments. It uses those
    10. // values to calculate and return the discounted price.
    11. Function Real calcDiscountPrice(Real price, Real percentage)
    12.    // Calculate the discount.
    13.    Declare Real discount = price * percentage
    14. 
    15.    // Subtract the discount from the price.
    16.    Declare Real discountPrice = price – discount
    17. 
    18.    // Return the discount price.
    19.    Return discount
End Function

```
// The calcDiscountPrice function accepts an item's price and
// the discount percentage as arguments. It uses those
// values to calculate and return the discounted price.


Function Real calcDiscountPrice(Real price, Real percentage)
    // Calculate the discount.
    Declare Real discount = price * percentage

    // Subtract the discount from the price.
    Declare Real discountPrice = price – discount

    // Return the discount price.
    Return discountPrice
```

Can you find the reason that the following pseudocode does not perform as indicated in the comments?
    20. // Find the error in the following pseudocode.
    21. Module main()
    22.     Declare Real value, result
    23. 
    24.     // Get a value from the user.
    25.     Display "Enter a value."
    26.     Input value
    27. 
    28.     // Get 10 percent of the value.
    29.     Call tenPercent(value)
    30. 
    31.     // Display 10 percent of the value.
    32.     Display "10 percent of ", value, " is ", result
    33. End Module
    34. 
    35. // The tenPercent function returns 10 percent
    36. // of the argument passed to the function.
    37. Function Real tenPercent(Real num)
    38.     Return num * 0.1
End Function


```
Can you find the reason that the following pseudocode does not perform as indicated in the comments?
// Find the error in the following pseudocode.
Module main()
     Declare Real value, result
 
     // Get a value from the user.
     Display "Enter a value."
     Input value
 
     // Get 10 percent of the value.
     set result = Call tenPercent(value)
 
     // Display 10 percent of the value.
     Display "10 percent of ", value, " is ", result
 End Module
 
  // The tenPercent function returns 10 percent
 // of the argument passed to the function.
Function Real tenPercent(Real num)
     Return num * 0.1
End Function


The variable result was never assigned a value
```