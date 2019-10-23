# CHOOSE THREE PROMPTS (unless mandatory ones are assigned)

# Roman Numerals

Design a program that prompts the user to enter a number within the range of 1 through 10. The program should display the Roman numeral version of that number. If the number is outside the range of 1 through 10, the program should display an error message.




# Areas of Rectangles

The area of a rectangle is the rectangle’s length times its width. Design a program that asks for the length and width of two rectangles. The program should tell the user which rectangle has the greater area, or whether the areas are the same.

```
//Start of main function
Declare integer width, length, rectangle1, rectangle2

//Calculate area of Rectangle 1
rectangleArea1()
    Display "Enter length of rectangle 1."
    input length
    Display "Enter width of rectangle 1."
    input width
    set rectangle1 = length * width
Return

//Calculate area of Rectangle 2
rectangleArea2()
    Display "Enter length of rectangle 2."
    input length
    Display "Enter width of rectangle 2."
    input width
    set rectangle2 = length * width
Return

//Calculate larger rectanglelargerRectangle()
    if rectangle 1 > rectangle 2 then
        Output "Rectangle 1 has a greater area than rectangle 2"
    else if rectangle2 > rectangle 1 then
        Output "Rectangle 2 has a greater area than rectangle 1"
    else
        Output "Both rectangles have the same area."
    end if
Return
```

# Mass and Weight

Scientists measure an object’s mass in kilograms and its weight in Newtons. If you know the amount of mass of an object, you can calculate its weight, in Newtons, with the following formula:

![image](https://user-images.githubusercontent.com/47218880/67404289-c6b2d480-f578-11e9-80c0-9bfa15de3df7.png)

Design a program that asks the user to enter an object’s mass, and then calculates its weight. If the object weighs more than 1,000 Newtons, display a message indicating that it is too heavy. If the object weighs less than 10 Newtons, display a message indicating that it is too light.

```
//Variable declarations
Declare Real mass, weight
Constant Real MASS_TO_WEIGHT = 9.8

//Mass to weight module
massToWeight()
    Display "Enter the mass of the object in Newtons".
    input mass
    if mass > 1000 then
        Display "Mass is too heavy!"
    else if mass < 10 then
        Display "Mass is too light!"
    else
        set weight = mass * MASS_TO_WEIGHT
        output "The weight of the mass you entered is ", weight 
    end if
Return
```

# Magic Dates

The date June 10, 1960, is special because when it is written in the following format, the month times the day equals the year:

![image](https://user-images.githubusercontent.com/47218880/67404336-d92d0e00-f578-11e9-9801-6742f67d71fe.png)

Design a program that asks the user to enter a month (in numeric form), a day, and a two-digit year. The program should then determine whether the month times the day equals the year. If so, it should display a message saying the date is magic. Otherwise, it should display a message saying the date is not magic.

```
//Start of program
Declare string primaryColor1, primaryColor2

//User input module
userInput()
    Display "Enter a primary color."
    input primaryColor1
    Display "Enter another primary color."
    input primaryColor2
Return

Color mix module
colorMix()
    //Purple mix
    if primaryColor1 == "red" and primaryColor2 == "blue" then
        Display "When you mix red and blue, you get purple."
    else if primaryColor1 == "blue" and primaryColor2 == "red" then
        Display "When you mix red and blue, you get purple."

    //Orange mix
    else if primaryColor1 == "red" and primaryColor2 == "yellow" then
        Display "When you mix red and yellow, you get orange."
    else if primaryColor1 == "yellow" and primaryColor2 == "red" then
        Display "When you mix red and yellow, you get orange."

    //Green mix
    else if primaryColor1 == "blue" and primaryColor2 == "yellow" then
        Display "When you mix blue and yellow, you get green."
    else if primaryColor1 == "yellow" and primaryColor2 == "blue" then
        Display "When you mix blue and yellow, you get green."

    //No mix
    else if primaryColor1 == primaryColor2 then
        Display "There is no mix since both colors are ", primaryColor1
    
    //Error Message
    else
        Diplay "ERROR, you must enter a primary color (red, yellow, or blue)"
    end if
Return

```

# Color Mixer

The colors red, blue, and yellow are known as the primary colors because they cannot be made by mixing other colors. When you mix two primary colors, you get a secondary color, as shown here:
```
When you mix red and blue, you get purple.

When you mix red and yellow, you get orange.

When you mix blue and yellow, you get green.
```
Design a program that prompts the user to enter the names of two primary colors to mix. If the user enters anything other than “red,” “blue,” or “yellow,” the program should display an error message. Otherwise, the program should display the name of the secondary color that results.

# Book Club Points

Serendipity Booksellers has a book club that awards points to its customers based on the number of books purchased each month. The points are awarded as follows:
```
If a customer purchases 0 books, he or she earns 0 points.

If a customer purchases 1 book, he or she earns 5 points.

If a customer purchases 2 books, he or she earns 15 points.

If a customer purchases 3 books, he or she earns 30 points.

If a customer purchases 4 or more books, he or she earns 60 points.
```

Design a program that asks the user to enter the number of books that he or she has purchased this month and displays the number of points awarded.

# Software Sales

A software company sells a package that retails for $99. Quantity discounts are given according to the following table:

![image](https://user-images.githubusercontent.com/47218880/67404439-04aff880-f579-11e9-8496-6a778d4ce7d1.png)

Design a program that asks the user to enter the number of packages purchased. The program should then display the amount of the discount (if any) and the total amount of the purchase after the discount.

# Change for a Dollar Game

Design a change-counting game that gets the user to enter the number of coins required to make exactly one dollar. The program should ask the user to enter the number of pennies, nickels, dimes, and quarters. If the total value of the coins entered is equal to one dollar, the program should congratulate the user for winning the game. Otherwise, the program should display a message indicating whether the amount entered was more than or less than one dollar.

# Shipping Charges

The Fast Freight Shipping Company charges the following rates:
![image](https://user-images.githubusercontent.com/47218880/67404533-26a97b00-f579-11e9-8944-5cfaa2dc2729.png)
Design a program that asks the user to enter the weight of a package and then displays the shipping charges.

# Time Calculator

Design a program that asks the user to enter a number of seconds, and works as follows:

* There are 60 seconds in a minute. If the number of seconds entered by the user is greater than or equal to 60, the program should display the number of minutes in that many seconds.

* There are 3,600 seconds in an hour. If the number of seconds entered by the user is greater than or equal to 3,600, the program should display the number of hours in that many seconds.

* There are 86,400 seconds in a day. If the number of seconds entered by the user is greater than or equal to 86,400, the program should display the number of days in that many seconds.

# Leap Year Detector

Design a program that asks the user to enter a year, and then displays a message indicating whether that year is a leap year or not. Use the following logic to develop your algorithm:

* If the year is evenly divisible by 100 and is also evenly divisible by 400, then it is a leap year. For example, 2000 is a leap year but 2010 is not.

* If the year is not evenly divisible by 100, but it is evenly divisible by 4, it is a leap year. For example, 2008 is a leap year but 2009 is not.
