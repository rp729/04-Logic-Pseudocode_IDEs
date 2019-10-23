# CHOOSE THREE PROMPTS (Plus mandatory ones if assigned)
## Kilometer Converter

Design a modular program that asks the user to enter a distance in kilometers, and then converts that distance to miles. The conversion formula is as follows:

![image](https://user-images.githubusercontent.com/47218880/67329523-99b2e300-f4e0-11e9-8a30-3f31fbd76ae1.png)

```
Start //Module main
    //Declaration
    Declare Real kilometers
    Declare Real miles
    Constant MILES_TO_KILO = 0.6214
Stop

MilesToKilo()
    Display "Enter number of kilometers."
    input kilometers
    miles = kilometers * MILES_TO_KILOS
    Output kilometers," is equalt to ",miles
return
```
## Sales Tax Program Refactoring (Mandatory)

See program below,  the Sales Tax program. This program calculates and displays the county and state sales tax on a purchase. Refactor it so the subtasks are in modules.
```
Start //Module main
    // Variable declarations
    Declare Real purchase, stateTax, countyTax, totalTax, totalSale
    // Constants for the state and county tax rates
    Constant Real STATE_TAX_RATE = 0.04
    Constant Real COUNTY_TAX_RATE = 0.02
Stop

// Get the amount of the purchase.
AmountOfPurchase()
    Display "Enter the amount of the purchase."
    Input purchase

// Calculate the state sales tax.
SalesTaxCalc()
    Set stateTax = purchase * STATE_TAX_RATE

// Calculate the county sales tax.
Set countyTax = purchase * COUNTY_TAX_RATE

// Calculate the total tax.
TotalTaxCalc()
    Set totalTax = stateTax + countyTax

// Calculate the total of the sale.
TotalSale()
    Set totalSale = purchase + totalTax

// Display information about the sale.
DataDisplay()
    Display "Purchase Amount: $", purchase
    Display "State Tax: ", stateTax
    Display "County Tax: ", countyTax
    Display "Total Tax: ", totalTax
    Display "Sale total: ", totalSale
```
 



## How Much Insurance?

Many financial experts advise that property owners should insure their homes or buildings for at least 80 percent of the amount it would cost to replace the structure. Design a modular program that asks the user to enter the replacement cost of a building and then displays the minimum amount of insurance he or she should buy for the property.

```
Start //Module Main
    Declare Real propertyValue
    Declare Real insuranceAmount
    Constant Real INSURANCE_PERCENT = 0.8
Stop

MinInsuranceAmount()
    Display "Enter your property value."
    input propertyValue
    insuranceAmount = propertyValue * INSURANCE_PERCENT
    output insuranceAmount
Return
```

## Automobile Costs

Design a modular program that asks the user to enter the monthly costs for the following expenses incurred from operating his or her automobile: loan payment, insurance, gas, oil, tires, and maintenance. The program should then display the total monthly cost of these expenses, and the total annual cost of these expenses.

```
Start //Module main
    Declare Real loanPayment, insurance, gas, oil, tires, maintenance, monthlyCost, annualCost
Stop

userInput()
    //Retrieve user data
    Display "Enter your loan payment amount."
    input loanPayment
    Display "Enter your insurance amount."
    input insurance
    Display "Enter your monthly gas amount."
    input gas
    Display "Enter monthly amount for your oil maintenance."
    input oil
    Display "Enter monthly amount for tire maintenance."
    input tire
    Display "Enter monthly amount for general maintenance."
    input maintenance
return

//Calculate monthly cost
monthlyCostCalc()
    monthlyCost = loanPayment+insurance+gas+oil+tire+maintenance
Return

//Calculate annual cost
annualCostCalc()
    annualCost = monthlyCost * 12
Return

//Final Result
finalResult()
    output "Your monthly expensis is equal to ", monthlyCost, " and your annual expense is equal to ", annualCost
Return
```

## Property Tax

A county collects property taxes on the assessment value of property, which is 60 percent of the property’s actual value. For example, if an acre of land is valued at $10,000, its assessment value is $6,000. The property tax is then 64¢ for each $100 of the assessment value. The tax for the acre assessed at $6,000 will be $38.40. Design a modular program that asks for the actual value of a piece of property and displays the assessment value and property tax

## Stadium Seating

There are three seating categories at a stadium. For a softball game, Class A seats cost $15, Class B seats cost $12, and Class C seats cost $9. Design a modular program that asks how many tickets for each class of seats were sold, and then displays the amount of income generated from ticket sales.

## Paint Job Estimator

A painting company has determined that for every 115 square feet of wall space, one gallon of paint and eight hours of labor will be required. The company charges $20.00 per hour for labor. Design a modular program that asks the user to enter the square feet of wall space to be painted and the price of the paint per gallon. The program should display the following data:
```
The number of gallons of paint required

The hours of labor required

The cost of the paint

The labor charges

The total cost of the paint job
```
## Monthly Sales Tax

A retail company must file a monthly sales tax report listing the total sales for the month, and the amount of state and county sales tax collected. The state sales tax rate is 4 percent and the county sales tax rate is 2 percent. Design a modular program that asks the user to enter the total sales for the month. From this figure, the application should calculate and display the following:
```
The amount of county sales tax

The amount of state sales tax

The total sales tax (county plus state)

In the pseudocode, represent the county tax rate (0.02) and the state tax rate (0.04) as named constants.
```
## Hot Dog Cookout Calculator

Assume that hot dogs come in packages of 10, and hot dog buns come in packages of 8. Design a modular program that calculates the number of packages of hot dogs and the number of packages of hot dog buns needed for a cookout, with the minimum amount of leftovers. The program should ask the user for the number of people attending the cookout, and the number of hot dogs each person will be given. The program should display the following:
```
The minimum number of packages of hot dogs required

The minimum number of packages of buns required

The number of hot dogs that will be left over

The number of buns that will be left over